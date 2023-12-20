---
product-area: reporting
navigation-topic: text-mode-reporting
title: 텍스트 모드를 사용하여 보기 편집
description: '참고: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html에 섹션을 추가합니다*** 또한 텍스트 모드 개요 문서에서 이 영역을 초안합니다.'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 1%

---

# 텍스트 모드를 사용하여 보기 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

텍스트 모드를 사용하여 목록이나 보고서의 보기를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 보기를 만들 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서의 보고 요소를 편집합니다.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서의 보기를 편집할 수 있도록 보고서에 대한 권한 관리</p> <p>보기에 대한 편집 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

보고서나 목록에서 텍스트 모드 사용을 시작하기 전에 항상 Workfront 텍스트 모드 구문을 잘 알고 있는지 확인하십시오.

자세한 내용은 다음을 참조하십시오.

* [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 보기에서 텍스트 모드 편집

텍스트 모드를 사용하여 뷰를 편집하는 것은 보고서와 목록에 대해 동일합니다. 보고서 또는 목록에서 보기에 액세스하는 방법은 다릅니다.

>[!TIP]
>
>표준 모드에서 가능한 한 많은 보기를 작성한 다음 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

빌딩 보기에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 보기에 액세스하려면 보고서로 이동한 다음 를 클릭합니다. **보고서 작업** > **편집** > **열(보기)** 탭.
   1. 목록에서 보기에 액세스하려면 목록으로 이동한 후 **보기** 드롭다운 메뉴를 수정하려는 뷰를 마우스로 가리킨 다음 **편집** 아이콘 ![](assets/edit-icon.png).

      뷰 빌더 가 열립니다.

1. 보기에서 열을 선택합니다.

   또는

   다음 항목 선택 **열(보기)** report builder의 탭에서 열을 선택합니다.

   >[!TIP]
   >
   >텍스트 모드를 사용하여 뷰를 편집하려면 한 번에 한 열씩 편집해야 합니다.

1. 클릭 **텍스트 모드로 전환** 빌더의 오른쪽 상단 모서리에서 을 클릭합니다.

   >[!NOTE]
   >
   >텍스트 모드에서 열을 편집하면 Workfront이 다음을 추가합니다. `textmode=true` 열에 대한 코드 행입니다. 텍스트 모드에서 열이 수정되었음을 나타냅니다.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   다음 표에서는 텍스트 모드 보기의 주요 행에 대해 설명합니다.

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
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>데이터베이스에 나타나는 개체 또는 필드의 이름입니다. 개체와 필드가 데이터베이스에 표시되는 방법에 대한 자세한 내용은 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> <p>다음과 같은 시나리오가 있습니다.</p> 
       <ol> 
        <li value="1"> <p> 표시되는 필드 이름이 단일 명사가 아닌 구문인 경우 <code>valuefield</code>. 예를 들어 작업의 계획된 시작 일자의 경우 코드는 다음과 같습니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>사용자 지정 필드를 표시하려면 <code>valuefield</code> 값은 인터페이스에 표시된 실제 필드 이름입니다. 예를 들어 "추가 정보"라는 사용자 정의 필드의 경우 코드는 다음과 같습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>를 사용하여 뷰의 다른 객체와 관련된 객체를 표시하려면 <code>valuefield</code> 코드 행 개체 이름과 특성은 콜론으로 구분됩니다. </p> <p>예를 들어, Portfolio 소유자의 이름을 표시하는 작업 보기의 열에는 valuefield 행에 대해 다음 값이 있습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>이는 보고서(작업) 객체에서 다음 관련 객체(프로젝트)에 액세스할 수 있음을 나타냅니다. 이 객체에서는 프로젝트(포트폴리오)에서 다음 관련 객체에 액세스한 다음 포트폴리오 소유자(소유자)와 이름(이름)을 차례로 선택할 수 있습니다. </p> </li> 
       </ol> <p>개체가 서로 연결되는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">객체의 상호 의존성 및 계층</a> 위치: <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront의 오브젝트 이해</a>.</p> <p>주: 표준 인터페이스에서 유효하지 않은 텍스트 모드의 필드를 선택하는 경우 열 내의 표준 인터페이스로 다시 전환할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>이 줄은 을 표시하는 데 사용되는 형식을 나타냅니다. <code>valuefield</code>. 다음 <code>valueformat</code> 개체나 필드가 텍스트, 숫자, 백분율 또는 날짜로 표시되는지 여부를 식별합니다.</p> <p>다음을 사용하는 것이 좋습니다. <code>HTML</code> 에 대한 <code>valueformat</code>, 특히 을 사용할 때 <code>valueexpression</code>를 사용하여 정보를 가장 정확하게 표시할 수 있습니다. </p> <p>이 라인의 추가 값에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">텍스트 모드에서 조건부 서식 사용</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>이 줄을 추가하여 바꿀 수 있습니다. <code>valuefield</code>열에 계산된 필드를 표시하려면 을(를) 선택합니다.</p> <p>다음을 동봉해야 합니다. <code>valuefield</code> 에서 사용할 때마다 중괄호로 묶인 개체의 수를 <code>valueexpression</code>.</p> <p>다음과 같은 시나리오가 있습니다. </p> 
       <ol> 
        <li value="1"> <p>위의 대소문자로 열에 필드를 표시하려면 다음을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>다음 <code>valuefield</code> API 탐색기에 나타나는 대로 개체의 철자가 지정됩니다. </p> </li> 
        <li value="2">여러 을(를) 추가하려면 <code>valuefields</code> 그것들을 한데 묶어서, 당신은 그것들을 주기별로 분리해야 한다.</li> 
        <li value="3"> <p>예를 들어 을 사용하여 작업의 기본 피할당자의 이름을 표시하려는 경우 <code>valueexpression</code>, 다음을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>에서 사용자 정의 필드를 사용하려면 <code>valueexpression</code> 줄 필드 이름 앞에 다음 기한까지 와야 합니다. <code>DE:</code> 사용자 정의 필드임을 나타냅니다. 필드 이름의 철자는 인터페이스에 나타나는 대로 입력됩니다. </p> <p>중요: 일부 사용자에 대한 권한이 제한된 사용자 정의 양식 섹션에 배치된 사용자 정의 필드를 사용하는 경우 해당 사용자가 보고서에서 이 계산을 볼 때 valueexpression 계산이 비어 있습니다. 사용자 정의 양식 섹션의 권한 조정에 대한 자세한 내용은 <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 정의 양식 만들기 또는 편집</a></span>.</p> <p>예를 들어 사용자 정의 필드에 "개발자 이름"이라는 레이블이 있고 이 필드를 열의 대소문자로 표시하려는 경우 다음을 사용할 수 있습니다 <code>valueexpression</code> 이를 나타내는 방법:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>타이프 어헤드 유형 사용자 정의 필드를 참조할 때 다음 표현식을 사용하여 "개발자 이름"이라는 레이블이 지정된 필드에서 선택한 개체의 이름을 참조합니다.</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>이 선은 열 이름 위로 마우스를 가져갈 때 도구 설명의 텍스트를 정의합니다. 이 경우 키를 사용하여 설명 텍스트의 이름 값을 번역하는 것입니다. 설명을 수정하려면 이 줄을 다음과 같이 변경하십시오. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>이 줄은 열 레이블을 정의합니다. 이 경우 키를 기반으로 하는 축약값을 사용합니다.</p> <p>열 이름을 수정하려면 이 값을 다음과 같이 변경할 수 있습니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> 에서는 열 이름에 대한 텍스트를 입력할 수 있지만<code>namekey</code> 열 이름을 번역하는 데 사용되는 키를 입력해야 합니다.</p> <p>열 이름을 변경하려면 <code>displayname </code>줄, 없는 경우.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>다음 줄을 추가하여 열의 이름을 변경할 수 있습니다. 이렇게 하면 <code>namekey/name</code> 값:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>이 줄은 열 머리글을 클릭할 때 결과가 정렬되는 방법을 정의합니다. 열이 없으면 보고서 실행 후에는 열을 정렬할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>이 선은 열에 사용되는 픽셀 수를 나타냅니다. 행을 생략하거나 0으로 설정하면 열이 뷰에 나타나지 않습니다.</p> <p>텍스트 모드에서 이 필드를 수동으로 수정할 때 <code>usewidths=true</code> 값을 열에 추가합니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>다음 줄 외에 이 줄을 사용해야 합니다. <code>width=</code> 열 너비를 사용자 지정할 때 사용됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>이 선은 열에 표시된 값을 인라인으로 편집할 수 있는지 여부를 정의합니다. 이 줄이 다음과 같은 경우 <strong>true</strong>, 열의 값은 인라인 편집할 수 있습니다. 이 줄이 다음과 같은 경우 <code>false</code>, 열의 값을 인라인으로 편집할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>열에 표시된 값이 연결된 오브젝트에 연결되게 하려는 경우에만 이 줄을 삽입합니다. 객체의 세부내용 페이지가 열립니다. 이 값은 다음과 일치해야 합니다. <code>valuefield=</code> 줄. 이 항목을 삽입할 때 <code>link.valueformat=</code> 줄. </p> <p> 예를 들어 를 삽입할 수 있습니다 <code>link.valuefield=priority</code> 문제 보기에 문제의 우선 순위가 링크로 표시됩니다. 이 링크를 클릭하면 문제 페이지가 열립니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>을(를) 삽입한 경우에만 이 줄을 삽입합니다. <code>link.valuefield</code> 열에 있는 값에 대한 링크를 추가할 줄. 객체의 세부내용 페이지가 열립니다. 이 값은 다음과 일치해야 합니다. <code>valueformat=</code> 라인 및 표시 형식을 나타냅니다. <code>valuefield</code>. </p> <p>중요: 링크가 포함된 기본 제공 열에서 텍스트 모드를 볼 때 링크를 참조하는 여러 줄이 표시됩니다. 텍스트 모드에서 사용자 지정 열을 만들고 여기에 링크 구문을 추가할 때 이러한 행 중 일부는 더 이상 지원되지 않거나 필요하지 않을 수 있습니다. 연결된 값을 추가할 때 필수 라인은 다음과 같습니다.<code> link.valuefield</code> 및 <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>각 열의 값을 요약하는 방법을 나타냅니다. 다음으로 시작하는 줄이 여러 개 있습니다. <code>aggregator.</code> 열 결과를 요약하는 집계를 말합니다. </p> <p>일반적으로 <code>aggregator.</code> 행은 열 객체의 행과 일치합니다. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>예: </b></span></span> 
        <p>Sum으로 요약된 작업 보고서의 계획된 시간 열은 다음과 같습니다. </p> 
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
        다음 <code>aggregator. </code>행에 다음이 포함될 수 있음: <code>valuefield </code>또는 <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **적용** 변경 내용을 저장하고 보기를 계속 편집하려면 다음을 수행하십시오.
1. 클릭 **저장 + 닫기** 보고서를 저장합니다.

   또는

   클릭 **보기 저장** 를 클릭하여 보기를 목록에 저장합니다.
