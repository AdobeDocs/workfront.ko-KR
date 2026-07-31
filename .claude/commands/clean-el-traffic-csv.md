---
name: clean-el-traffic-csv
description: 페이지 보기 횟수별로 정렬된 Workfront 전용 페이지로의 원시 Experience League/Adobe Analytics 트래픽 CSV 내보내기를 정리합니다. 사용자가 Experience League 페이지 트래픽 CSV("페이지 URL 일반", "고유 방문자 수", "방문 횟수", "페이지 보기 수")를 제공하고 정리하거나, 필터링하거나, 처리할 것을 요청하거나, "문서 추적" / "가장 많이 본 문서" 스프레드시트를 언급한 경우 사용합니다.
source-git-commit: 3c5f28f5656fec574cb1ca9d3853703b6b900fdb
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---


# Experience League 트래픽 CSV 정리

Experience League 페이지 트래픽의 원시 Adobe Analytics 자유 형식 테이블 내보내기를 페이지 보기별로 정렬된 깔끔한 Workfront 전용 중복 제거 CSV로 변환하여 원본 파일을 덮어씁니다.

## 입력 모양

입력은 다음 두 가지 형태 중 하나일 수 있습니다.

1. **원시 내보내기** — 메타데이터 주석 줄(`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"` 등)로 시작한 다음 계층 구조 분류 테이블(예: 개별 URL 행→ `Solution (v2)` → `workfront` → `Page URL Generic (v33)`)이 옵니다. 리터럴 셀 `Page URL Generic (v33)`(또는 유사한 `Page URL Generic ...` 레이블)이 두 번째 열에서 중간에 나타납니다.
2. **이미 정리된 CSV** — 첫 번째 행은 이미 `Page URL Generic (v33),Unique Visitors,Visits,Page Views`과(와) 같은 일반 헤더이며 메타데이터 행 또는 추가 선행 열이 없습니다.

시작하기 전에 어떤 셰이프를 가지고 있는지 검색합니다. 행 1이 셰이프 2와 일치하는 일반 머리글 행인 경우 2단계로 바로 건너뜁니다(날짜 범위를 사용할 수 없으므로 사용자가 날짜 범위를 별도로 제공하지 않는 한 7단계도 건너뜀).

## 워크플로

### 0단계: 날짜 범위를 캡처합니다(모든 항목을 삭제하기 전에 원시 내보내기만).

일치하는 맨 위 `# Date: <range>`(예: `"# Date: Jul 1, 2026 - Jul 31, 2026"`) 근처에서 메타데이터 줄을 찾습니다. `<range>` 기록(예: `Jul 1, 2026 - Jul 31, 2026`) — 7단계에서 나중에 필요합니다. 행을 삭제하기 전에 이 작업을 수행합니다.

### 1단계: 원시 내보내기를 일반 테이블로 줄입니다(원시 내보내기만).

1. `Page URL Generic (...)` 셀을 포함하는 행을 찾습니다(표준 내보내기의 두 번째 열에 있음).
2. 메타데이터 주석 행과 `Solution (v2)` / `workfront` 소계 행을 포함하여 해당 행 위에 있는 모든 행을 삭제합니다.
3. `Page URL Generic` 셀의 왼쪽에 있는 모든 열을 삭제합니다(표준 내보내기에서 이 열은 A 열입니다).
4. 같은 행(현재 머리글 행)에서 `Page URL Generic (...)`의 오른쪽에 있는 숫자 소계 값을 리터럴 헤더로 바꿉니다(`Unique Visitors`, `Visits`, `Page Views`). `Page URL Generic (...)` 셀 자체를 변경하지 마십시오.

결과: 헤더가 `Page URL Generic (v33),Unique Visitors,Visits,Page Views`이고 URL당 하나의 행이 뒤따르는 일반 CSV입니다.

### 2단계: Workfront 행만 유지

모든 데이터 행에 대해 URL에 리터럴 하위 문자열 `/workfront/`(양쪽에 슬래시)이 포함되어 있는지 확인합니다. 로케일 접두사는 문제가 되지 않습니다(`/en/`, `/zh-hans/` 등 — 모두 제품 세그먼트가 일치하는 한 유지됩니다).

- URL에 `/workfront/`이(가) 경로 세그먼트로 포함되어 있지 **않음**&#x200B;인 경우 행을 삭제합니다. 이렇게 하면 `workfront-fusion`, `workfront-learn`, `proofhqpapi` 등과 같은 다른 제품이 제거됩니다. `tutorials-workfront`과(와) 같은 하위 문자열은 **not**&#x200B;을(를) 계산합니다. 일치 항목은 정확한 세그먼트 `/workfront/`이어야 합니다.
- 그렇지 않으면 행을 유지합니다.

### 3단계: URL 트리밍

각 나머지 행에 대해 URL에서 `/using`을(를) 찾고 `/using`을(를) 포함하여 `/`의 다음 부분만 삭제합니다.

예: `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

`/using`이(가) Workfront 행의 URL에 없는 경우 해당 URL을 그대로 두고 추측하는 대신 사용자를 위해 플래그를 지정합니다.

### 4단계: 조각/쿼리 접미사 제거

트리밍된 URL에 `#` 또는 `?`이(가) 포함된 경우 해당 문자와 그 뒤에 있는 모든 항목을 삭제하십시오.

예: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### 5단계: 중복 항목 병합

트리밍 후 여러 행이 동일한 URL을 공유할 수 있습니다(예: 동일한 경로로 축소되는 두 개의 서로 다른 로케일 행). URL이 동일한 모든 행을 하나의 행으로 결합하여 `Unique Visitors`, `Visits` 및 `Page Views`을(를) 독립적으로 합합니다.

예: `/home,2,2,3` 및 `/home,5,6,7` → `/home,7,8,10`

### 6단계: 페이지 보기 횟수별로 정렬

`Page Views`개 내림차순(가장 큰 먼저)으로 모든 데이터 행을 정렬합니다. 머리글 행은 정렬된 데이터 위의 맨 위에 고정된 상태를 유지합니다.

### 7단계: 날짜 범위 행 추가(0단계에서 캡처된 경우 원시 내보내기만)

삽입하기 전에 캡처된 날짜 범위(예: `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`)에서 쉼표를 제거하십시오. 원시 범위에는 해당 행에서 CSV 열 구분 기호로 잘못 읽을 수 있는 쉼표가 있습니다.

헤더 행 위쪽의 맨 위에 쉼표로 구분된 날짜 범위만 포함하는 새 행을 삽입합니다.

최종 행 순서: 날짜 범위 행 → 헤더 행→ 정렬된 데이터 행입니다.

### 8단계: 저장

원래 입력 파일을 정리가 완료된 결과로 덮어씁니다.

## 범위를 벗어남

정리된 CSV를 게시 또는 공유(예: Slack에)하는 것은 아직 정의되지 않은 별도의 단계입니다. 이 스킬의 일부로 파일을 첨부하거나 업로드하지 마십시오.

## 구현(원시 내보내기)

원시 내보내기의 경우, 수동으로 행을 편집하는 대신 이 테스트된 PowerShell 스크립트로 단계 0-8을 실행하십시오. 수백 개의 행이 있는 파일의 경우 더 빠르고 오류 발생 가능성이 줄어듭니다. `$path`의 실제 파일 경로를 대체하십시오.

실행하기 전에 파일이 잠겨 있는지(예: Excel에서 열기) 확인합니다. — `Set-Content`이(가) &quot;다른 프로세스에서 사용 중&quot;으로 실패하면 사용자에게 파일을 닫도록 요청한 후 다시 실행합니다.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8
```

이미 정리된 CSV(입력 모양 2)의 경우 헤더 재배치 및 날짜 범위 논리를 건너뜁니다. 기존 헤더/행에서 2-6단계와 8단계를 그대로 실행하기만 하면 됩니다.
