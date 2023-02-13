---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드를 사용하여 필터 편집
description: '참고: 다음 문서에서 섹션을 추가합니다. /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** 텍스트 모드 개요 문서에서 이 영역 초안 작성'
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# 텍스트 모드를 사용하여 필터 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 더 복잡한 필터를 만들 때 텍스트 모드를 사용하여 목록 또는 보고서에서 필터를 편집할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 보고 요소를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리를 통해 보고서의 필터를 편집합니다</p> <p>필터에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

보고서나 목록에서 텍스트 모드를 사용하기 전에 항상 Workfront 텍스트 모드 구문에 익숙한지 확인하십시오.

자세한 내용은 다음을 참조하십시오.

* [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [사용자 정의 보기, 필터 및 그룹화 샘플](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 필터에서 텍스트 모드 편집

텍스트 모드를 사용하여 필터를 편집하는 것은 보고서 및 목록과 동일합니다. 보고서나 목록에서 보기에 액세스하는 것은 다릅니다.

>[!TIP]
>
>표준 모드에서 가능한 많은 필터를 빌드한 다음 필터를 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

필터 만들기에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

보고서 만들기에 대한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 필터에 액세스하려면 보고서로 이동한 다음 **보고서 작업** > **편집** > **필터** 탭.
   1. 목록에서 필터에 액세스하려면 목록 및 **필터** 드롭다운 메뉴에서 수정할 필터를 마우스로 가리키고 **편집** 아이콘 ![](assets/edit-icon.png).

      필터 빌더가 열립니다.

1. 클릭 **필터 규칙 추가** 필터 조건 추가를 시작하려면 다음을 클릭합니다 **텍스트 모드로 전환** 빌더 오른쪽 위 모서리에서 을(를) 클릭합니다.
1. 텍스트 모드를 사용하여 필터 문을 추가합니다. 각 필터 문에는 다음 줄과 추가 정보가 포함될 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>필터 라인/정보</td> 
      <td>예</td> 
     </tr> 
     <tr> 
      <td> <p>필드 이름 및 Workfront 데이터베이스에 표시되는 값과 같은 값입니다.</p> <p>이 줄은 필수입니다.</p> <p> 데이터베이스에서 개체와 필드가 표시되는 방법에 대한 자세한 내용은 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>진행 중 상태의 작업을 필터링하려면 다음 라인을 사용합니다.</p> <p><code>status=INP</code> </p> <p>팁: 상태에 대해 필터링할 때는 이름이 아닌 상태의 3자로 된 코드를 사용해야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>필드 이름 수정자 및 수정자가 무엇에 해당합니까? 이것은 필터링하고 있는 필드가 충족해야 하는 조건을 나타냅니다.</p> <p>이 줄은 필수입니다.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>필터링하는 작업의 상태가 진행 중 과 같아야 함을 나타내려면 위의 라인 외에 다음 라인을 사용합니다.</p> <p><code>status_Mod=in</code> </p> <p>수정자가 범위인 경우 수정자를 나타내는 두 개의 라인이 있습니다.</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>예: </b></span></span> 
        <p>이 필터는 현재 달에 계획된 완료 날짜가 있고 특정 GUID를 가진 사용자에게 할당된 진행 중인 작업을 찾는 텍스트 모드 필터입니다.</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>텍스트 모드의 필터 수정자 전체 목록에 대해서는 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">필터 및 조건 수정자</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>문 연산자입니다. 기본적으로 각 필터 문은 "AND" 연산자로 연결됩니다. 텍스트 모드 인터페이스에는 표시되지 않습니다. 두 문 사이에 "OR" 연산자를 추가하여 두 조건 중 하나 또는 다른 조건을 충족할 수 있는 객체를 필터링할 것임을 나타낼 수도 있습니다.</p> <p>필터 연산자는 문이 두 개 이상인 필터에만 필요합니다.</p> <p>팁:   
        <ul> 
         <li> <p>"OR"는 대/소문자를 구분하며 항상 대문자로 사용해야 합니다.</p> </li> 
         <li> <p>연산자를 AND에서 OR로 변경하면 목록 항목 수가 늘어날 수 있습니다.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>예: </b></span></span> 
        <p>진행 중 상태나 계획된 완료 일자가 오늘 상태인 태스크를 필터링하려면 다음을 사용합니다. </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>필터에서 정보를 일반화하고 현재 시간이나 로그인한 사용자를 참조할 수 있는 와일드카드입니다.</p> <p>와일드카드는 선택 사항입니다.</p> <p>팁:   <p>필터를 보다 동적으로 만들고 각 사용자 또는 유사한 기간에 대해 동일한 필터를 복제하지 않도록 가능한 경우 와일드카드를 사용하는 것이 좋습니다.</p> <p>필터 와일드카드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">와일드카드 필터 변수</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>예: </b></span></span> 
        <p>현재 로그인한 사용자에게 할당된 작업을 필터링하려면 다음을 사용하십시오.</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. &quot;OR&quot; 연산자로 연결된 필터 문을 추가하려면 다음을 수행합니다.

   1. 새 코드 줄 추가 및 유형 OR:1: 다음에 을 필터링하려는 개체 또는 속성 및 비교할 값이 옵니다. 새로 만들기를 제외한 임의의 상태에 있는 작업을 참조하려면 다음 행을 사용하십시오.

      ```
      OR:1:status=NEW
      ```

   1. 두 번째 줄 및 OR 입력 추가:1: 그 뒤에는 개체, 수정자 및 수정자 코드가 옵니다. 신규를 제외한 모든 태스크 상태를 참조하는 코드 라인의 수정자를 정의하려면 다음 수정자 라인을 사용합니다.

      ```
      OR:1:status_Mod=notin
      ```

      새 문의 각 행에는 &quot;OR:`<number>`:&quot;

      필터에 &quot;OR&quot; 문을 만드는 방법에 대한 자세한 내용은 [텍스트 모드 필터에서 &quot;OR&quot; 문 만들기](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>동일한 필터에 여러 &quot;OR&quot; 문을 사용할 수 있습니다. 새 &quot;OR&quot; 문이 있을 때마다 &quot;OR:&quot; 뒤의 숫자가 증가합니다.
진행 중 상태이거나 로그인한 사용자에게 지정되었거나 오늘 계획 완료 일자가 있는 작업을 필터링하려면 다음을 사용합니다.
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. 클릭 **완료** 변경 사항을 저장하고 보고서 또는 필터를 계속 편집하려면 다음을 수행하십시오.
1. 클릭 **저장 + 닫기** 보고서를 저장하려면 **필터 저장** 필터를 목록에 저장합니다.
