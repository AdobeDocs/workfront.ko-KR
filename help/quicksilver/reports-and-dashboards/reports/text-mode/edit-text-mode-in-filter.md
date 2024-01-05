---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드를 사용하여 필터 편집
description: 텍스트 모드를 사용하여 목록 또는 보고서에서 필터를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 필터를 만들 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# 텍스트 모드를 사용하여 필터 편집

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

텍스트 모드를 사용하여 목록 또는 보고서에서 필터를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 필터를 만들 수 있습니다.

필터를 만들 때의 추가 텍스트 모드 예제는 섹션 을 참조하십시오 [맞춤형 필터 샘플](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) 이 문서에서 [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
    <p>또는</p>
    <p>현재: 플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기 및 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드 및 달력에 대한 액세스 권한을 편집하여 보고서의 보고 요소를 편집합니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에서 필터를 편집할 보고서에 대한 권한 관리</p> <p>편집할 필터에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

보고서나 목록에서 텍스트 모드 사용을 시작하기 전에 항상 Workfront 텍스트 모드 구문을 잘 알고 있는지 확인하십시오.

자세한 내용은 다음을 참조하십시오.

* [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 필터에서 텍스트 모드 편집

텍스트 모드를 사용하여 필터를 편집하는 것은 보고서와 목록에 대해 동일합니다. 보고서나 목록에서 필터에 액세스하는 방법은 서로 다릅니다.

>[!TIP]
>
>표준 모드에서 가능한 한 많은 필터를 작성한 다음 필터를 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

필터 빌드에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 필터에 액세스하려면 보고서로 이동한 다음 **보고서 작업** > **편집** > **필터** 탭.
   1. 목록에서 필터에 액세스하려면 목록으로 이동한 다음 **필터** 메뉴를 클릭하고 수정할 필터를 마우스로 가리킨 다음 **편집** 아이콘 ![](assets/edit-icon.png).

      필터 빌더가 열립니다.

1. 클릭 **필터 규칙 추가** 필터의 조건을 추가하려면 을 클릭합니다. **텍스트 모드** 또는 **텍스트 모드로 전환** 빌더 오른쪽에 있습니다.
1. 텍스트 모드를 사용하여 필터 문을 추가합니다. 각 필터 문에는 다음 줄과 추가 정보가 포함될 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>필터 라인/정보</b></td> 
      <td><b>예</b></td> 
     </tr> 
     <tr> 
      <td> <p>필드 이름 및 Workfront 데이터베이스에 나타나는 값과 동일합니다.</p> <p>이 라인은 필수입니다.</p> <p> 개체와 필드가 데이터베이스에 표시되는 방법에 대한 자세한 내용은 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>진행 중 상태의 작업을 필터링하려면 다음 줄을 사용하십시오.</p> <p><code>status=INP</code> </p> <p><b>팁</b>

   상태를 필터링할 때는 이름이 아닌 세 글자로 된 상태 코드를 사용해야 합니다.</p> </td>
   </tr> 
     <tr> 
      <td> <p>필드 이름 수정자 및 수정자가 동일한 항목. 필터링 기준 필드가 충족해야 하는 조건을 나타냅니다.</p> <p>이 라인은 필수입니다.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>필터링하는 작업의 상태가 [진행 중]과 같아야 함을 나타내려면 위의 줄 외에 다음 줄을 사용하십시오.</p> <p><code>status_Mod=in</code> </p> <p>수정자가 범위인 경우 수정자를 나타내는 라인이 두 개 있습니다.</p> 
       <div> <span class="autonumber"><span><b>예 </b></span></span> 
        <p>다음 텍스트 모드 필터는 진행 중이며 현재 달 내에 계획된 완료 일자가 있고 특정 GUID를 가진 사용자에게 할당된 작업을 찾습니다.</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>텍스트 모드의 전체 필터 수정자 목록은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">필터 및 조건 수정자</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>문 연산자. 기본적으로 각 필터 문은 "AND" 연산자로 연결됩니다. 텍스트 모드 인터페이스에는 표시되지 않습니다. 두 문 사이에 "OR" 연산자를 추가하여 두 조건 중 하나 또는 다른 조건을 충족할 수 있는 객체를 필터링할 것임을 나타낼 수도 있습니다.</p> <p>필터 연산자는 명령문이 두 개 이상 있는 필터에만 필요합니다.</p> <p>팁:   
        <ul> 
         <li> <p>"OR"은 대소문자를 구분하므로 항상 대문자로 표기해야 합니다.</p> </li> 
         <li> <p>연산자를 AND에서 OR로 변경하면 목록 항목의 수가 늘어날 수 있습니다.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>예 </b></span></span> 
        <p>진행 중 상태이거나 계획된 완료 일자가 오늘인 작업을 필터링하려면 다음을 사용합니다. </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>와일드카드: 필터에 있는 정보를 일반화하고 현재 시간 또는 로그인한 사용자를 참조할 수 있습니다.</p> <p>와일드카드는 선택 사항입니다.</p> <p>팁:   <p>필터를 보다 역동적으로 만들고 각 사용자 또는 유사한 시간대에 대해 동일한 필터를 복제하지 않도록 할 때는 가능하면 와일드카드를 사용하는 것이 좋습니다.</p> <p>필터 와일드카드에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">와일드카드 필터 변수 개요</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>예</b></span></span> 
        <p>현재 로그인한 사용자에게 할당된 작업을 필터링하려면 다음을 사용합니다.</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. &quot;OR&quot; 연산자로 연결된 필터 문을 추가하려면 다음을 수행합니다.

   1. 새 코드 행을 추가하고 OR 입력:1: 뒤에 필터링할 개체 또는 특성과 비교할 값이 옵니다. 신규를 제외한 모든 상태의 작업을 참조하려면 다음 라인을 사용합니다.

      `OR:1:status=NEW`

   1. 두 번째 줄을 추가하고 OR 입력:1: 뒤에 object, modifier 및 modifier 코드가 옵니다. 신규를 제외한 모든 태스크 상태를 참조하는 코드 라인의 수정자를 정의하려면 다음 수정자 라인을 사용합니다.

      `OR:1:status_Mod=notin`

      새 명령문의 각 줄 앞에는 &quot;OR:`<number>`:&quot;.

      필터에서 &quot;OR&quot; 문을 만드는 방법에 대한 자세한 내용은 [텍스트 모드 필터에서 &quot;OR&quot; 문 만들기](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >동일한 필터에 여러 &quot;OR&quot; 문이 있을 수 있습니다. 새 &quot;OR&quot; 문이 있을 때마다 &quot;OR:&quot; 다음의 숫자가 증가합니다.
      >
      >진행 중 상태이거나 로그인한 사용자에게 할당되었거나 오늘 계획된 완료 일자가 있는 작업을 필터링하려면 다음을 사용합니다.
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. 클릭 **텍스트 모드 종료** 또는 **완료** 텍스트 모드 변경 내용을 저장하고 보고서 또는 필터 편집을 계속합니다.
1. 클릭 **저장 + 닫기** 보고서를 저장하거나 **필터 저장** 필터를 목록에 저장합니다.


