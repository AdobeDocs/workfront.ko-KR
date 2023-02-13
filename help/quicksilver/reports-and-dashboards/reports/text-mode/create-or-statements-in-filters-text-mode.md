---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드 필터에서 "OR" 문 만들기
description: 목록 및 보고서에서 필터를 만들 때 여러 구문을 포함할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 텍스트 모드 필터에서 &quot;OR&quot; 문 만들기

목록 및 보고서에서 필터를 만들 때 여러 구문을 포함할 수 있습니다.

필터 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [텍스트 모드를 사용하여 필터 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 텍스트 모드 필터 연산자

표준 필터 인터페이스의 Adobe Workfront 필터 연산자에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront에는 각 필터 문을 연결하는 2개의 필터 연산자가 있습니다.

* **및**: AND 연산자로 2 필터 문을 조인하는 경우 두 필터 문을 동시에 충족하도록 지정합니다.

   기본적으로 필터의 문은 AND 연산자로 연결됩니다.

   텍스트 모드 인터페이스에서 AND 필터를 작성할 때는 AND 연산자를 사용할 필요가 없습니다. 가정한 것입니다.

   **예:** 계획 완료 일자가 오늘이고 완료율이 100%보다 낮은 태스크를 필터링하려면 다음 텍스트 모드 코드를 사용합니다.

   <pre>planningCompletionDate=$$오늘</pre><pre>planningCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **또는**: OR 연산자로 2개의 필터 문을 조인하는 경우 두 문 중 하나를 충족하도록 지정합니다.

   >[!TIP]
   >
   >AND 문을 OR 문으로 변경할 때 보고서의 항목 수가 증가합니다.

   텍스트 모드 인터페이스를 사용하여 OR 필터를 작성할 때는 OR 연산자를 사용해야 합니다.

   **예:** 계획 완료 일자가 오늘 또는 완료율이 100%보다 낮은 태스크를 필터링하려면 다음 텍스트 모드 코드를 사용합니다.

   <pre>planningCompletionDate=$$오늘</pre><pre>planningCompletionDate_Mod=eq</pre><pre>또는:1:percentComplete=100</pre><pre>또는:1:percentComplete_Mod=lt</pre>

## OR 필터의 텍스트 모드 구문

OR 필터의 텍스트 모드 구문은 다음을 포함해야 합니다.

* OR 연산자 뒤에 콜론, 숫자 및 OR 문의 개체를 참조하는 각 필터 라인의 시작 부분에 콜론, 다른 콜론이 옵니다. 여기에는 필터 필드 또는 속성을 참조하는 라인과 필터 수정자를 참조하는 선이 포함됩니다.

   OR 필터를 빌드할 때 다음 패턴을 따르십시오.

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>또는:1:<field name in camel case>=<value></pre><pre>또는:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >OR 연산자는 대/소문자를 구분하며 항상 대문자입니다.

   필터에 여러 개의 OR 문이 있을 수 있습니다. 이 경우 모든 OR 문은 명령문을 적용할 순서대로 번호를 받습니다.

   **예:**  계획 완료 일자가 오늘 또는 완료율이 100%보다 작거나 신규 상태가 있는 태스크를 필터링하려면 다음 텍스트 모드 코드를 사용합니다.

   <pre>planningCompletionDate=$$오늘</pre><pre>planningCompletionDate_Mod=eq</pre><pre>또는:1:status=NEW</pre><pre>또는:1:status_Mod=in</pre><pre>또는:2:percentComplete=100</pre><pre>또는:2:percentComplete_Mod=lt</pre>

* 필터에 참조하는 필드 이름 또는 특성의 이름은 카멜 표기법으로 작성해야 합니다. 카멜 사례에 대한 자세한 내용은 [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* OR 필터의 사용자 지정 필드를 참조하는 경우 DE를 삽입해야 합니다. 또는 수정자 구문과 사용자 지정 필드의 이름 사이에 있는 사용자 지정 필드에 대해 설명합니다. 사용자 지정 필드의 이름은 Workfront 인터페이스에 표시되는 대로 사용자 지정 필드의 이름을 입력해야 합니다.

   **예:** 상태가 신규 또는 완료율이 100%보다 작은 작업 또는 값이 &quot;같음&quot;인 &quot;계정 유형&quot;이라는 사용자 지정 필드를 필터링하려면 다음 텍스트 모드 코드를 사용하십시오.

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>또는:1:percentComplete=100</pre><pre>또는:1:percentComplete_Mod=lt</pre><pre>또는:2:DE:계정 유형=대문자</pre><pre>또는:2:DE:Account Type_Mod=in</pre>
