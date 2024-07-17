---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 필터에서 "OR" 문 만들기
description: 목록 및 보고서에서 필터를 만들 때 여러 문을 포함할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# 텍스트 모드 필터에서 &quot;OR&quot; 문 만들기

목록 및 보고서에서 필터를 만들 때 여러 문을 포함할 수 있습니다.

필터 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 텍스트 모드 필터 연산자

표준 필터 인터페이스의 Adobe Workfront 필터 연산자에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.

Workfront에는 각 필터 문을 연결하는 2개의 필터 연산자가 있습니다.

* **AND**: AND 연산자로 2개의 필터 문을 조인할 때 두 필터 문을 동시에 충족하도록 지정할 수 있습니다.

  기본적으로 필터의 문은 AND 연산자로 연결됩니다.

  텍스트 모드 인터페이스에서 AND 필터를 작성할 때는 AND 연산자를 사용할 필요가 없습니다. 이 경우,

  **예:** 계획된 완료 일자가 오늘이고 완료율이 100%보다 낮은 작업을 필터링하려면 다음 텍스트 모드 코드를 사용하십시오.

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OR**: OR 연산자로 2개의 필터 문을 조인할 때 두 문 중 하나를 충족시키려고 함을 나타냅니다.

  >[!TIP]
  >
  >AND 문을 OR 문으로 변경하면 보고서의 항목 수가 증가합니다.

  텍스트 모드 인터페이스를 사용하여 OR 필터를 작성할 때는 OR 연산자를 사용해야 합니다.

  **예:** 계획된 완료 일자가 오늘이거나 완료율이 100%보다 낮은 작업을 필터링하려면 다음 텍스트 모드 코드를 사용하십시오.

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>또는:1:percentComplete=100</pre><pre>또는:1:percentComplete_Mod=lt</pre>

## OR 필터의 텍스트 모드 구문

OR 필터의 텍스트 모드 구문에는 다음 내용이 포함되어야 합니다.

* OR 연산자 뒤에는 콜론, 숫자 및 OR 문의 개체를 참조하는 각 필터 줄의 시작 부분에 다른 콜론이 옵니다. 여기에는 필터 필드 또는 특성을 참조하는 라인과 필터 수정자를 참조하는 라인이 포함됩니다.

  OR 필터를 작성할 때 다음 패턴을 따르십시오.

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>또는:1:<field name in camel case>=<value></pre><pre>또는:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >OR 연산자는 대소문자를 구분하며 항상 대문자입니다.

  필터에 여러 OR 문이 있을 수 있습니다. 이 경우 모든 OR 문은 명령문을 적용할 순서대로 숫자를 받습니다.

  **예:** 계획된 완료 일자가 오늘이거나 완료율이 100%보다 낮거나 상태가 새로움인 작업을 필터링하려면 다음 텍스트 모드 코드를 사용하십시오.

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>또는:1:상태=새로 만들기</pre><pre>OR:1:status_Mod=in</pre><pre>또는:2:percentComplete=100</pre><pre>또는:2:percentComplete_Mod=lt</pre>

* 필터에서 참조하는 필드 이름이나 특성은 카멜 대/소문자로 작성해야 합니다. 낙타 사례에 대한 자세한 내용은 [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)를 참조하십시오.
* OR 필터에서 사용자 지정 필드를 참조할 때 OR 수정자 구문과 사용자 지정 필드의 이름 사이에 DE: 를 삽입해야 합니다. 사용자 정의 필드의 이름이 Workfront 인터페이스에 표시되는 대로 맞춤법을 입력해야 합니다.

  **예:** Status가 New 또는 Percent가 100%보다 낮은 작업 또는 값이 &quot;Equal&quot;인 &quot;Account Type&quot;이라는 사용자 지정 필드를 필터링하려면 다음 텍스트 모드 코드를 사용하십시오.

  <pre>status=신규</pre><pre>status_Mod=in</pre><pre>또는:1:percentComplete=100</pre><pre>또는:1:percentComplete_Mod=lt</pre><pre>OR:2:DE:Account Type=Capital</pre><pre>OR:2:DE:Account Type_Mod=in</pre>
