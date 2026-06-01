---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect에 연결 설정
description: Workfront Data Connect를 사용하면 비즈니스 인텔리전스 도구를 통해 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: d7577da92b7efda5cba26104efac124f75a271c5
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 1%

---

# Workfront Data Connect에 연결 설정

Workfront Data Connect를 사용하면 비즈니스 인텔리전스 도구를 통해 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.

Data Connect 데이터 레이크를 외부 제품과 연결하려면 먼저 [Snowflake에 대한 판독기 계정 또는 연결 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)에 설명된 대로 연결을 만들어야 합니다. 그런 다음 아래 [IP를 허용 목록에 추가하다에 추가](#add-ips-to-the-allowlist)에서 설명한 대로 필요한 IP를 허용 목록에 추가하다에 추가해야 합니다.

대부분의 제품에서 연결을 설정하려면 데이터 레이크에 대한 다음 정보가 필요합니다.

| 필드 이름 | 값 |
|---------------|-------------|
| 서버 | `https://` 부분이 없는 연결의 URL(Workfront*의 **데이터 연결** 페이지에 있음) |
| 포트 | `443` |
| 데이터베이스 | `WORKFRONT` |
| 웨어하우스 | `READER_WH` |
| 스키마 | `WF` |
| 역할 | `READER_ROLE` |
| 사용자 이름 | 연결을 만들 때 선택한 사용자 이름(Workfront*의 **데이터 연결** 페이지에 있음) |
| 암호 | 첫 번째 Snowflake 로그인 시 선택한 암호* |

*연결이 포함된 **Data Connect** 페이지를 찾을 수 있는 위치에 대한 자세한 내용은 [Snowflake에 대한 Reader 계정 또는 연결 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)를 참조하십시오.

>[!IMPORTANT]
>
>한 항목이 IP 허용 목록에 추가되면 다른 모든 IP 주소는 더 이상 허용되지 않습니다. 시각화 도구를 사용하기 전에 시각화 도구의 작성 및 읽기 경험에 필요한 모든 IP 주소를 입력해야 합니다. 그렇지 않은 경우 잘못된 자격 증명에 대한 오류가 발생할 수 있습니다.
>
>허용 목록에 추가하다에 IP 주소가 포함되어 있지 않지만 BI 도구에 연결하는 데 여전히 문제가 있는 경우 BI 도구에 대한 프록시 서버 구성을 확인하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 허용 목록에 추가하다에 IP 추가

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 연결**&#x200B;을 클릭합니다.

1. **허용된 IP** 탭을 클릭한 다음 **IP 주소를 허용 목록에 추가** 단추를 클릭합니다.

1. **IP 주소 설명**&#x200B;에 IP 주소 이름을 입력하고 **IP 주소**&#x200B;에서 사용할 도구의 IP 주소(또는 CIDR 블록)를 입력한 다음 **IP를 허용 목록에 추가**&#x200B;를 클릭합니다.

   ![IP 주소 추가](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Microsoft Power BI에 대한 Azure IP 범위 찾기

Data Connect에 대한 Microsoft Power BI 트래픽은 단일 고정 주소에서 가져오지 않습니다. Microsoft은 IP 범위를 큰 JSON 파일의 CIDR 블록으로 게시합니다. 이 섹션에서는 실제로 사용하는 영역에 대한 블록을 찾는 방법에 대해 설명합니다.

### Azure IP 범위 및 서비스 태그에 대한 공식 Microsoft 소스

Microsoft은 [Azure IP 범위 및 서비스 태그 - 공개 클라우드 다운로드 페이지](https://www.microsoft.com/en-us/download/details.aspx?id=56519)에 목록을 게시합니다. 현재 JSON 파일을 다운로드합니다(파일 이름은 일반적으로 `ServiceTags_Public_YYYYMMDD.json`과(와) 유사함). Microsoft에서 이 파일을 업데이트할 때 또는 연결 문제가 변경되면 Microsoft을 새로 고칩니다.

>[!NOTE]
>
>JSON 파일은 매우 크며, 종종 100,000줄이 훨씬 넘습니다. 그것은 예상되었습니다. 필요한 섹션은 작으므로 전체 파일을 직접 읽을 필요가 없습니다.

### Power BI과 Power Query Online 비교

트래픽이 Microsoft에서 서비스 태그 목록에서 별도의 Power BI 서비스로 처리하는 파워 쿼리 구성 요소에서 실제로 나올 때 고객이 &quot;Azure&quot;를 보고하는 경우가 있습니다.

| 사용자가 다음을 수행하는 경우... | JSON에서 이 서비스 태그를 찾습니다. |
|----------------|---------------------------------------|
| Power BI 서비스, Azure에서 호스팅되는 데이터 세트 또는 클라우드 컨텍스트의 게이트웨이 사용 | `PowerBI`(전역 또는 지역 항목(예: `PowerBI.EastUS`) |
| 파워 쿼리 온라인, 클라우드 데이터 흐름 및 유사한 경험 사용 | `PowerQueryOnline`(전역 또는 지역 항목(예: `PowerQueryOnline.EastUS`) |

조직에서 두 경험을 모두 사용하는 경우 동일한 영역에 대해 `PowerBI`과(와) `PowerQueryOnline` 모두에서 CIDR 블록을 추가하십시오. 하나만 추가하는 경우 일부 사용자는 계속 차단되고 다른 사용자는 성공할 수 있습니다.

### 전역 집계가 아닌 지역 태그 선택

JSON 파일에는 여러 영역을 집계하고 수백 개의 CIDR 블록과 `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` 등의 더 작은 여러 영역 항목을 포함할 수 있는 `PowerBI`(및 `PowerQueryOnline`)에 대한 단일 모든 영역 항목이 포함되어 있습니다. 각 지역 객체에는 해당 지역에 대한 접두어만 나열되며, 일반적으로 최대 수십 개의 줄이 나열됩니다. 모든 Azure 지역을 허용하기 위한 문서화된 요구 사항이 없는 한 글로벌 항목을 추가하지 않는 것이 좋습니다. 대부분의 Data Connect 고객의 경우 지역별 항목이 올바른 기본값입니다. Power BI 테넌트와 사용자가 실제로 실행하는 지역과 중복을 위한 작은 버퍼(예: 회사에서 사용하는 2차 재해 복구 지역)를 추가합니다.

### 지역 선택

파일에 있는 Microsoft의 지역 이름은 `EastUS`, `WestEurope`, `GermanyWestCentral` 등으로 보입니다. 종종 일치하지만 사무실이 아닌 Power BI 용량 및 사용자가 호스팅되는 지역을 사용합니다.

| 시나리오 | 먼저 추가할 항목 |
|----------|-------------------|
| 미국 사용 | 테넌트가 사용하는 미국 지역으로 시작합니다(예: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). Microsoft 관리자가 다중 지역 호스팅을 확인하지 않는 한 모든 미국 지역이 필요하지 않습니다. |
| 유럽 연합 또는 영국 사용 | 테넌트가 사용하는 영역으로 시작합니다(예: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). 사용자가 추가 Microsoft 지역을 포괄하는 경우에만 더 추가합니다. |
| 아시아 태평양 사용 | Power BI 또는 Azure 관리자가 확인한 지역을 추가합니다(예: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| 여러 지역 | 각 서비스(`PowerBI` 및 `PowerQueryOnline`(둘 다 사용 중인 경우)에 대해 두 지역 태그 집합(예: EU 및 US)을 모두 추가합니다. |
| 알 수 없는 영역 | Microsoft 리소스를 호스팅하는 Power BI 지역을 Azure 365 또는 Power BI 관리자에게 문의하거나 Power BI 관리자 테넌트 설정을 검토하십시오. 테스트를 위해 차단을 빨리 해제해야 하는 경우 알려진 영역 쌍(예: `EastUS` 및 `WestUS`) 하나를 추가하고 모니터링한 다음 확인되면 목록의 범위를 좁힙니다. |

### IP 범위를 찾아 허용 목록에 추가하다에 추가합니다.

Microsoft에서 IP 범위를 수집하고 Workfront 허용 목록에 추가하다에 추가하려면 다음을 수행합니다.

1. [Azure IP 범위 및 서비스 태그 - 공용 클라우드 다운로드 페이지](https://www.microsoft.com/en-us/download/details.aspx?id=56519)를 열고 서비스 태그 JSON 파일을 다운로드한 다음 로컬에 저장합니다(예: `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Visual Studio 코드와 같이 큰 JSON을 잘 처리하는 모든 편집기에서 파일을 엽니다.

1. 편집기의 찾기 기능(Windows의 경우 `Ctrl+F`, macOS의 경우 `Cmd+F`)을 사용하여 `"name"` 필드가 `PowerBI.EastUS` 또는 `PowerQueryOnline.WestEurope`과(와) 같은 서비스 태그와 같은 JSON 개체를 찾습니다. 유용한 검색:

   * `"name": "PowerBI.WestUS"` — 미국 서부 Power BI으로 이동합니다.
   * `"name": "PowerQueryOnline.WestUS"` — 미국 서부 파워 쿼리 온라인으로 이동.
   * `PowerBI.` — 모든 Power BI 지역 태그를 나열한 다음 지역 이름으로 세분화합니다.

1. 일치하는 각 개체에서 이름이 `addressPrefixes`인 배열을 찾습니다. 해당 배열의 각 문자열은 CIDR 블록(예: `20.59.79.96/27` 또는 IPv6 접두사)입니다. 이 값은 Workfront에 추가할 값입니다.

1. 이 문서의 [허용 목록에 추가하다에 IP 추가](#add-ips-to-the-allowlist)에 설명된 대로 각 CIDR을 Workfront Add에 추가합니다. 환경이 규칙을 캐시하는 경우 몇 분 동안 정책 전달을 허용합니다.

1. Power BI 또는 Power Query Online에서 Data Connect에 대해 작은 테스트 쿼리를 실행하여 연결을 확인합니다. 실패할 경우 대략적인 시간을 캡처하고 네트워크 팀에 누락된 범위와의 정렬을 거부할지 여부를 문의하십시오. `PowerBI`만 추가되었을 때 `PowerQueryOnline`이(가) 누락되었는지 다시 확인하십시오. 일반적인 간격입니다.

예를 들어 Microsoft 관리자가 Power BI 워크로드가 미국 서부, 미국 서부 2 및 미국 서부 3을 사용하고 사용자가 Power BI 및 Power Query Online을 모두 사용한다고 확인한 경우 6개의 개체 `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` 및 각각에 대해 일치하는 `PowerQueryOnline.<Region>`을(를) 연 다음 6개 모두에서 `addressPrefixes`을(를) 복사합니다.

### JSON 구조 참조

각 서비스 태그 블록은 개념적으로 다음과 같습니다. 실제 파일에는 더 많은 메타데이터가 포함됩니다.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

`addressPrefixes` 배열에 Workfront에 추가할 CIDR 블록이 포함되어 있습니다. 다른 필드는 Azure 네트워킹 시나리오용이며 여기에 적용되지 않습니다.

### 허용 목록 유지

* Microsoft은 시간에 따라 IP 범위를 변경합니다. Microsoft에서 업데이트된 JSON 파일을 게시할 때 특히 연결 문제가 발생한 후에 주기적으로 허용 목록에 추가하다를 새로 고치거나 비교합니다.
* 사용자 환경에서 Snowflake에 IPv6을 지원하고 Microsoft에서 IPv6 접두사를 나열하는 경우 보안 정책에서 IPv6을 허용하는 경우 이를 포함하십시오. 그렇지 않으면 네트워크 팀과 조율하십시오.

## 허용 목록에 추가하다에서 IP 주소 제거

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 연결**&#x200B;을 클릭합니다.

1. **허용된 IP** 탭을 클릭한 다음 제거할 IP 주소의 오른쪽에 있는 휴지통 아이콘 ![삭제 아이콘](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)을 클릭합니다.

1. 표시되는 창에서 확인란에 확인 표시를 한 다음 **삭제**&#x200B;를 클릭합니다.

## 비즈니스 인텔리전스 도구를 사용하여 데이터 공유

다음은 여러 일반적인 비즈니스 인텔리전스 도구입니다. 데이터 레이크에 연결하는 방법에 대해 자세히 알아보려면 설명서 사이트를 방문하십시오.

* 타블로
* Power BI
* 도모
* SAP HANA

## 외부 데이터 웨어하우스에 데이터 저장

아래에 여러 개의 공통 데이터 웨어하우스가 나와 있습니다. 데이터 레이크 연결에 대한 자세한 내용은 해당 문서 사이트를 참조하십시오.

* Databricks
* AWS Redshift
