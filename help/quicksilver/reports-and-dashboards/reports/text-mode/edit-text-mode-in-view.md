---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드를 사용하여 보기 편집
description: '참고: 다음 문서에서 섹션을 추가합니다. /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** 또한 텍스트 모드 개요 문서에서 이 영역 초안 작성'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# 텍스트 모드를 사용하여 보기 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 더 복잡한 보기를 만들 수 있도록 텍스트 모드를 사용하여 목록 또는 보고서에서 보기를 편집할 수 있습니다.

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
   <td> <p>보고서에서 보기를 편집할 수 있도록 보고서에 대한 권한 관리</p> <p>보기에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
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

## 보기에서 텍스트 모드 편집

텍스트 모드를 사용하여 보기를 편집하는 것은 보고서 및 목록과 동일합니다. 보고서나 목록에서 보기에 액세스하는 것은 다릅니다.

>[!TIP]
>
>표준 모드에서 가능한 많은 보기를 만든 다음 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

뷰 빌드에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

보고서 만들기에 대한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 보기에 액세스하려면 보고서로 이동한 다음 **보고서 작업** > **편집** > **열(보기)** 탭.
   1. 목록에서 보기에 액세스하려면 목록 및 **보기** 드롭다운 메뉴에서 수정할 보기를 마우스로 가리킨 다음 **편집** 아이콘 ![](assets/edit-icon.png).

      뷰 빌더가 열립니다.

1. 보기에서 열을 선택합니다.

   또는

   을(를) 선택합니다 **열(보기)** report builder 탭에서 열을 선택합니다.

   >[!TIP]
   >
   >텍스트 모드를 사용하여 뷰를 편집하려면 한 번에 하나의 열을 편집해야 합니다.

1. 클릭 **텍스트 모드로 전환** 빌더 오른쪽 위 모서리에서 을(를) 클릭합니다.

   >[!NOTE]
   >
   >텍스트 모드에서 열을 편집하면 Workfront에서 `textmode=true` 열에 대한 코드 줄. 이는 열이 텍스트 모드에서 수정되었음을 나타냅니다.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   다음 표에서는 텍스트 모드 보기의 주요 줄에 대해 설명합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>샘플 라인</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>값</strong>=</p> </td> 
      <td> <p>데이터베이스에 표시되는 객체 또는 필드의 이름입니다. 데이터베이스에서 개체와 필드가 표시되는 방법에 대한 자세한 내용은 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> <p>다음 시나리오가 있습니다.</p> 
       <ol> 
        <li value="1"> <p> 표시되는 필드의 이름이 단일 명사가 아닌 구문인 경우, 다음과 같은 경우 다음과 같이 낙타식 대/소문자 구문을 사용해야 합니다 <code>valuefield</code>. 예를 들어 작업의 계획 시작 날짜에 대한 코드는 다음과 같습니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>사용자 지정 필드를 표시하려면 <code>valuefield</code> 값은 인터페이스에 표시되는 필드의 실제 이름입니다. 예를 들어 "추가 정보"라는 사용자 지정 필드의 경우 코드는 다음과 같습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>뷰에서 다른 객체와 관련된 객체를 표시하려면 <code>valuefield</code> 코드 줄 개체 이름과 속성은 콜론()으로 구분됩니다. </p> <p>예를 들어, Portfolio 소유자의 이름을 표시하는 작업 뷰의 열에는 값 필드 라인에 대해 다음 값이 있습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>이것은 보고서(작업)의 객체에서 다음 관련 객체(프로젝트)에 액세스할 수 있음을 나타냅니다. 여기에서 프로젝트(포트폴리오)에서 다음 관련 객체에 액세스한 다음 포트폴리오 소유자(소유자)와 이름(이름)을 액세스할 수 있습니다. </p> </li> 
       </ol> <p>개체가 서로 연결되는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">개체의 상호 종속성 및 계층</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront의 개체 이해</a>.</p> <p>참고: 표준 인터페이스에서 유효하지 않은 텍스트 모드의 필드를 선택하면 열 내의 표준 인터페이스로 다시 전환할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>이 선은 <code>valuefield</code>. 다음 <code>valueformat</code> 개체나 필드가 텍스트, 숫자, 백분율 또는 날짜로 표시되는지 여부를 식별합니다.</p> <p>을 사용하는 것이 좋습니다 <code>HTML</code> 에 대해 <code>valueformat</code>특히 <code>valueexpression</code>를 입력하여 정보를 가장 정확하게 표시할 수 있습니다. </p> <p>이 라인의 추가 값에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">텍스트 모드에서 조건부 서식 사용</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>바꿀 이 줄을 추가할 수 있습니다 <code>valuefield</code>, 열에 계산된 필드를 표시하려면 을 클릭합니다.</p> <p>이(가) <code>valuefield</code> 중괄호로 묶은 개체를 <code>valueexpression</code>.</p> <p>다음 시나리오가 있습니다. </p> 
       <ol> 
        <li value="1"> <p>대소문자를 사용하여 열에 필드를 표시하려면 다음을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>다음 <code>valuefield</code> API 탐색기에 표시될 때 개체의 철자가 지정됩니다. </p> </li> 
        <li value="2">여러 개를 추가하려면 <code>valuefields</code> 그것들을 한데 묶어서 마침표로 구분해야 한다.</li> 
        <li value="3"> <p>예를 들어, <code>valueexpression</code>를 사용하는 경우:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>에서 사용자 지정 필드를 사용하려면 <code>valueexpression</code> 필드 이름 앞에 줄을 와야 합니다. <code>DE:</code> 를 사용하여 사용자 지정 필드임을 나타냅니다. 인터페이스에 표시되는 필드 이름의 철자가 나타납니다. </p> <p>중요 사항: 일부 사용자에 대한 권한이 제한된 사용자 지정 양식 섹션에 배치된 사용자 지정 필드를 사용하는 경우 해당 사용자가 보고서에서 이 계산을 볼 때 값 표현식 계산은 비어 있습니다. 사용자 지정 양식 섹션의 권한 조정에 대한 자세한 내용은 <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a></span>.</p> <p>예를 들어 사용자 지정 필드에 "개발자 이름"이라는 레이블이 있고 이 필드를 열에 있는 대소문자를 표시하려면 다음을 사용할 수 있습니다 <code>valueexpression</code> 다음을 나타냅니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Typeahead 유형 사용자 지정 필드를 참조할 때 다음 표현식을 사용하여 "개발자 이름"이라는 필드에서 선택한 객체의 이름을 참조합니다.</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>description= / description=</strong> </p> </td> 
      <td> <p>이 선은 도구 팁의 텍스트를 마우스로 열 이름을 가리키면 정의합니다. 이 경우 키를 사용하여 설명 텍스트의 이름 값을 변환합니다. 설명을 수정하려면 다음 라인을 읽도록 변경합니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>name 키= / name=</strong> </td> 
      <td> <p>이 선은 열 레이블을 정의합니다. 이 경우 키를 기반으로 단축된 값을 사용합니다.</p> <p>열 이름을 수정하려면 이 값을 다음으로 변경할 수 있습니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> 열 이름의 텍스트를 입력할 수 있는 반면<code>namekey</code> 열 이름을 번역하는 데 사용되는 키를 입력해야 합니다.</p> <p>열 이름을 변경하려면 <code>displayname </code>없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>다음 줄을 추가하여 열을 일시 중단하는 열 이름을 변경할 수 있습니다 <code>namekey/name</code> 값:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>이 선은 열 헤더를 클릭할 때 결과가 정렬되는 방법을 정의합니다. 표시되지 않으면 보고서를 실행한 후 열을 정렬할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>이 행은 열에 사용되는 픽셀 수를 나타냅니다. 행을 생략하거나 0(영)으로 설정하면 뷰에 열이 표시되지 않습니다.</p> <p>텍스트 모드에서 이 필드를 수동으로 수정하는 경우 <code>usewidths=true</code> 값을 열에 추가합니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidthes=true</strong> </td> 
      <td> <p>이 줄과 <code>width=</code> 열 너비를 사용자 지정할 때 행 </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>이 선은 열에 표시된 값이 인라인 편집 가능 인지 여부를 정의합니다. 이 줄이 다음과 같은 경우 <strong>true</strong>: 열의 값은 인라인 편집 가능합니다. 이 줄이 다음과 같은 경우 <code>false</code>: 열의 값은 인라인 편집 가능하지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valufield=</strong> </td> 
      <td> <p>열에 표시된 값이 연결된 객체에 연결되도록 하려는 경우에만 이 행을 삽입합니다. 그러면 개체의 세부 정보 페이지가 열립니다. 이 값은 <code>valuefield=</code> 줄. 이 항목을 삽입할 때는 <code>link.valueformat=</code> 줄. </p> <p> 예를 들어 <code>link.valuefield=priority</code> 문제 보기에서 문제의 우선순위 는 링크로 표시됩니다. 이 링크를 클릭하면 문제 페이지가 열립니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>삽입한 경우에만 이 줄을 삽입합니다. <code>link.valuefield</code> 열의 값에 대한 링크를 추가하는 행. 그러면 개체의 세부 정보 페이지가 열립니다. 이 값은 <code>valueformat=</code> 라인 및 는 <code>valuefield</code>. </p> <p>중요 사항: 링크도 포함된 기본 제공 열에서 텍스트 모드를 볼 때 링크를 참조하는 많은 줄이 표시됩니다. 텍스트 모드에서 사용자 지정 열을 만들고 링크 문을 추가할 때 이러한 행 중 일부가 더 이상 지원되지 않거나 필요하지 않을 수 있습니다. 연결된 값을 추가할 때 필수입니다<code> link.valuefield</code> 및 <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregation.function=</strong> </td> 
      <td> <p>이것은 각 열의 값을 요약하는 방식을 나타냅니다. 다음으로 시작하는 줄이 여러 개 있습니다 <code>aggregator.</code> 그리고 모두 열의 결과를 요약하는 누적 합계를 말합니다. </p> <p>일반적인 규칙으로서, <code>aggregator.</code> 선은 열 객체의 선과 일치합니다. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>예: </b></span></span> 
        <p>Sum으로 요약된 작업 보고서의 계획 시간 열은 다음과 같을 수 있습니다. </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=compound</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        다음 <code>aggregator. </code>행에는 다음이 포함될 수 있습니다 <code>valuefield </code>또는 <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **적용** 변경 사항을 저장하고 보기를 계속 편집하려면 다음을 수행하십시오.
1. 클릭 **저장 + 닫기** 보고서를 저장합니다.

   또는

   클릭 **보기 저장** 를 클릭하여 목록에 보기를 저장합니다.
