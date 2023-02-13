---
title: 사용자 지정 양식에 계산된 데이터 추가
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 지정 양식에서 계산을 생성하는 계산된 사용자 지정 필드를 작성할 수 있습니다. 이를 위해 사용자 지정 필드, 계산된 사용자 지정 데이터 필드 및 기본 제공 Workfront 필드일 수 있는 데이터 표현식 및 기존 필드의 이름을 사용하는 문을 만듭니다. 이 문은 사용자가 입력하는 데이터를 계산하고 새 계산된 사용자 지정 필드에 결과를 표시합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e24a0408049e7eb2e7cb97833e7f41ea66e8131b
workflow-type: tm+mt
source-wordcount: '2563'
ht-degree: 0%

---

# 사용자 지정 양식에 계산된 데이터 추가

사용자 지정 양식에서는 사용자 지정 양식이 개체에 첨부된 경우 기존 데이터를 사용하여 새 데이터를 생성하는 계산된 사용자 지정 필드를 추가할 수 있습니다.

계산된 사용자 지정 필드에는 다음을 포함할 수 있습니다.

* 단일 기본 제공 필드에 대한 간단한 참조.

   >[!INFO]
   >
   > **예:** 프로젝트 및 작업에서 생성된 매출을 계산하기 위해 기본 제공 필드 실제 매출이 포함된 계산된 사용자 지정 필드를 만들 수 있습니다. 사용자가 사용자 지정 양식을 프로젝트 또는 작업에 첨부하면 프로젝트 또는 작업의 매출이 필드에 표시됩니다.

* 하나 이상의 필드를 참조하는 식입니다. 사용자 지정 필드, 다른 계산된 사용자 지정 필드 및 기본 제공 필드일 수 있습니다.

   >[!INFO]
   >
   >**예:** 프로젝트 및 태스크에 의해 생성된 수익을 계산하기 위해 수익에서 비용을 빼는 수학 표현식을 포함하는 수익이라는 계산된 사용자 정의 필드를 생성할 수 있습니다.
   >
   >이를 위해 내장된 Workfront 필드 실제 비용 및 실제 매출과 함께 수학 표현식 SUB(빼기)를 사용할 수 있습니다.
   >
   >아래 단계에서는 이 예제를 어떻게 수행할 수 있는지 확인할 수 있습니다.

조직을 위한 사용자 지정 양식 작성 및 이와 연결할 수 있는 필드 유형 이해에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 양식에 계산된 필드 추가 {#add-a-calculated-field-to-a-custom-form}

기본 제공 Workfront 필드와 이미 만든 사용자 지정 필드를 모두 사용할 수 있습니다.

>[!IMPORTANT]
>
>새 계산된 사용자 지정 필드를 만들기 전에 계산에 필요한 데이터가 Workfront에 있는지 확인하기 위해 포함할 기존 필드를 식별합니다.

1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집을 시작합니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 설정 **필드 추가** 탭, **계산된 지표**.

   오른쪽에 있는 표시 영역에 필드가 표시됩니다 *12345*. 사용자 지정 양식을 만들거나 편집하는 동안 필드가 계산된 사용자 지정 필드임을 알려주는 표시일 뿐입니다. 양식이 개체에 첨부된 상태에서 사용자가 양식을 채우는 경우에는 필드에서 계산의 결과가 확인되고, *12345* 표시기.

1. 계산된 필드에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td>필드의 레이블을 입력합니다. 사용자가 사용자 지정 양식을 사용할 때 보게 되는 것입니다. 필드 <b>이름</b>자동으로 채워지는 은 보고서에서 Workfront에 의해 참조됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">지침</td> 
      <td> 기본적으로 필드에 대해 만드는 수식은 여기에 저장됩니다. 텍스트를 추가하여 필드 및 필드의 수식에 대한 추가 정보를 제공할 수 있습니다. 이 기능은 다음 두 가지 방법으로 유용합니다. 
       <ul> 
        <li> <p>공식이 무엇이고 어떻게 작동하는지 알려주는 것입니다. 이 기능은 여러 양식에서 이 계산된 사용자 지정 필드를 사용할 계획인 경우 특히 유용합니다.</p> </li> 
        <li> <p>도구 설명으로 사용자는 필드 위로 마우스를 가져가면 볼 수 있습니다. 도구 설명에 표시할 텍스트를 여기에 추가합니다.</p> <p>해당 사용자가 도구 설명에 있는 수식을 보지 못하게 하려면 해당 수식에 혼동을 줄 수 있습니다. 자세한 내용은 섹션의 테이블 행 "지침에 수식 표시"를 참조하십시오 <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">계산된 사용자 지정 필드에 대한 계산을 작성합니다</a> 참조하십시오.</p> </li> 
       </ul> <p>새 양식에서 동일한 계산된 사용자 지정 필드를 사용하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">포맷</td> 
      <td> <p>필드 결과를 저장할 형식을 지정하여 표시합니다.</p> <p>필드를 수학 계산에 사용하는 경우 항상 <strong>숫자</strong> 또는 <strong>통화</strong> 형식 지정 번호 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</p> 
      <p><b>중요 사항</b>: 형식을 선택하기 전에 새 필드에 올바른 형식을 고려하십시오. 사용자 지정 양식을 저장한 후에는 형식 필드를 편집할 수 없습니다. 또한 잘못된 형식을 선택하면 보고서 및 목록 그룹의 향후 계산 및 집계 값에 영향을 줄 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 계속 [계산된 사용자 지정 필드에 대한 계산을 작성합니다](#build-the-calculation-for-your-calculated-custom-field) 참조하십시오.

## 계산된 사용자 지정 필드에 대한 계산을 작성합니다 {#build-the-calculation-for-your-calculated-custom-field}

1. 섹션에 설명된 대로 계산된 사용자 지정 필드 만들기를 시작합니다 [사용자 지정 양식에 계산된 필드 추가](#add-a-calculated-field-to-a-custom-form) 참조하십시오.

1. 클릭 **최대화** 열다 **계산 편집기** 계산을 빌드합니다.

   >[!INFO]
   >
   >**예:** 이 문서 소개 의 예를 사용하여 프로젝트 및 작업에 대해 사용자 정의 양식에 Profit이라는 계산된 사용자 정의 필드를 생성할 수 있습니다. 이 필드에는 실제 매출과 실제 원가 간의 차이를 표시하는 계산이 포함될 수 있습니다.
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >이 예제에서는 `SUB` 는 표현식이고 참조된 필드는 다음과 같습니다 `actualRevenue` 및 `actualCost`.

   계산은 일반적으로 표현식으로 시작되고, 사용자 지정 양식이 개체에 첨부된 경우 참조할 필드가 포함된 괄호가 옵니다. 사용 가능한 표현식에 대한 자세한 내용은 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   각 필드는 섹션에 설명된 대로 중괄호로 둘러싸야 합니다 [계산된 사용자 지정 필드에 필요한 구문](#syntax-required-in-calculated-custom-fields) 참조하십시오. 필드의 이름을 입력하기 시작하면 시스템이 제안을 하고 하나를 선택하여 계산에 삽입할 수 있습니다.

   계산에서 형식 지정 유형의 텍스트 필드와 설명 텍스트의 두 가지 항목을 제외하고 모든 유형의 사용자 지정 필드를 참조할 수 있습니다. 사용자 지정 필드 유형에 대한 자세한 내용은 [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. 큰 텍스트 상자에서 를 클릭한 다음 **표현식** 및 **필드** 계산 시 사용할 수 있습니다.

   큰 텍스트 상자에 표현식이나 필드 입력을 시작한 다음 표시될 때 선택할 수도 있습니다. 각 항목은 필드의 경우 &quot;F&quot;, 표현식의 경우 &quot;E&quot;로 표시됩니다.

   여는 괄호를 입력하면 닫는 괄호가 자동으로 추가됩니다.

   >[!TIP]
   >
   >다음 중 하나를 수행하여 계산에 도움이 될 수 있습니다.
   > 
   >* 계산의 표현식을 마우스로 가리키면 설명, 사용 방법을 보여주는 예제 및 문서에 있는 추가 정보에 대한 &quot;추가 정보&quot; 링크가 표시됩니다 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* 색상 코딩을 사용하여 추가한 구성 요소를 식별합니다. 표현식은 파란색으로 표시되고 필드는 녹색으로 표시됩니다.
      >  ![](assets/colors-fields-expressions.jpg)
   >* 계산 오류를 찾아 이동할 때 분홍색으로 강조 표시됩니다. 강조 표시된 오류 위로 마우스를 가져가면 해당 원인에 대한 간단한 설명을 표시할 수 있습니다.
      >  ![](assets/error-help.png)
   >* 계산 아래 영역에서 기존 Workfront 개체에서 결과를 미리 봅니다.

   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* 왼쪽에 표시되는 라인 번호를 사용하여 긴 계산에서 표현식을 참조합니다.


1. 클릭 **최소화** 계산된 사용자 지정 필드에 대한 계산 만들기를 완료하면 됩니다.

   >[!NOTE]
   >
   >오른쪽에 있는 표시 영역에 필드가 표시됩니다 *12345.* 사용자 지정 양식을 만들거나 편집하는 동안 필드가 계산된 사용자 지정 필드임을 알려주는 표시일 뿐입니다. 양식이 개체에 첨부된 상태에서 사용자가 양식을 채우는 경우에는 필드에서 계산의 결과가 확인되고, *12345* 표시기.

1. (선택 사항) 다음 옵션 중 하나를 사용하여 계산된 사용자 지정 필드를 추가로 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">논리 추가</td> 
      <td>표시 논리 를 추가하여 양식을 채울 때 이전 다중 선택 필드(드롭다운, 확인란 또는 라디오 단추)에서 사용자가 선택한 하나 이상의 항목을 기준으로 계산된 필드가 표시되는지 여부를 결정할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다</a>. <p>확인란, 라디오 단추 또는 드롭다운 필드가 양식의 계산된 사용자 지정 필드 앞에 적어도 한 개 있는 경우에만 사용할 수 있습니다. </p> <p>계산된 사용자 지정 필드에 논리 건너뛰기 를 사용할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이전 계산 업데이트</td> 
      <td>기존의 계산된 사용자 지정 필드를 편집할 때 이 옵션을 선택하여 사용자 지정 양식을 저장할 때 계산에서 업데이트를 트리거할 수 있습니다. 사용자 지정 양식을 저장할 때만 발생합니다. 옵션을 비활성화한 상태로 돌아갑니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침에 수식 표시</td> 
      <td>사용자 지정 양식을 채우는 사용자가 필드를 마우스로 가리키면 필드의 공식을 표시하도록 하려면 이 옵션을 활성화하십시오. 자세한 내용은 <a href="#instructions" class="MCXref xref">지침</a> 이 테이블의 앞부분</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **완료** 계산된 사용자 지정 필드에서 모든 변경 사항이 완료되면.

   또는 **적용** 사용자 지정 필드를 양식에 계속 추가하려면 아직 변경 내용을 양식에 적용하십시오.

   또는 **저장 + 닫기** 사용자 지정 양식에서 모든 변경 사항이 완료되면.
1. 계산된 사용자 지정 필드가 올바르게 작동하는지 확인하려면 사용자 지정 양식을 개체에 첨부한 다음 계산된 사용자 지정 필드에서 결과를 검토하십시오.

   사용자 지정 양식 첨부에 대한 지침은 [개체에 사용자 지정 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   사용자 지정 양식을 다른 방식으로 계속 빌드하려면 다음 문서 중 하나를 계속 진행할 수 있습니다.

   * [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 계산된 사용자 지정 필드에 필요한 구문

각 필드는 각 필드 이름 주위에 중괄호를 사용하여 아래 설명된 구문을 사용해야 합니다. 필드의 이름을 입력하기 시작하면 시스템이 제안을 하고 하나를 선택하여 계산에 삽입할 수 있습니다. 계산에 데이터를 잘못 입력하면 경고 메시지가 나타납니다. 유효한 필드와 유효한 계산된 식을 포함하도록 계산을 편집하지 않으면 양식을 저장할 수 없습니다.

>[!NOTE]
>
>현재, 사용자 지정 양식이 첨부할 개체에 참조할 필드의 이름을 입력할 때 개체의 상위가 아니라 입력해야 합니다.

### 중괄호로 둘러싸인 필드 이름

* 계산 시 기본 제공 필드를 참조하려면 필드 이름을 중괄호로 묶어야 합니다.

For example: `{actualRevenue}`

필드 이름은 대/소문자를 구분하며, Workfront 시스템에 표시되는 방식과 정확히 같은 계산에 표시되어야 합니다.

* 계산 시 사용자 지정 필드를 참조하려면 필드의 이름을 중괄호로 둘러싸며 앞에 `DE:` 괄호 안에 있어야 합니다.

For example: `{DE:Profit}`

입력 시 선택할 수 있는 모든 사용자 지정 필드가 시스템에 나열됩니다 `DE:`.

* 계산에서 *상위* 사용자 지정 양식이 개체에 첨부된 경우 필드 이름 앞에 상위 개체의 개체 형식, 중괄호로 묶어야 합니다.

   예를 들어, 사용자 지정 양식이 작업에 대해 작동하도록 구성되었으며 양식이 작업에 첨부된 경우 필드가 상위 개체의 실제 수입을 계산하도록 하려면 다음을 표시해야 합니다 `Project` 필드의 개체 유형으로:

   `{project}.{actualRevenue}`

   또는 사용자 지정 필드인 경우:

   `{project}.{DE:profit}`

   에 대한 사용자 지정이 여러 객체 유형에 대해 구성되어 있기 때문에 상위 객체의 객체 유형을 잘 모를 경우 와일드카드 필터 변수를 사용할 수 있습니다 `$$OBJCODE` 를 사용하여 가능한 각 유형에 대해 계산이 작동하도록 할 수 있습니다. 자세한 내용은 [다중 개체 사용자 지정 양식의 계산된 사용자 지정 필드](#calculated-custom-fields-in-multi-object-custom-forms) 참조하십시오.

### 마침표로 항목 구분

계산된 사용자 지정 필드에서 관련 개체를 참조할 때 개체 이름과 속성을 마침표로 구분해야 합니다.

예를 들어 작업 유형 사용자 지정 양식에서 계산된 사용자 지정 필드에 Portfolio 소유자의 이름을 표시하려면 다음을 입력합니다.

`{project}.{porfolio}.{owner}`

이에 따라 다음 내용이 결정됩니다. 사용자 지정 양식(작업)의 개체에서 작업과 관련된 다음 개체(프로젝트)에 액세스할 수 있습니다. 여기에서 프로젝트(포트폴리오)에 연결된 다음 관련 개체에 액세스한 다음 포트폴리오의 다음 관련 개체(소유자)에 액세스할 수 있습니다.

### 사용자 지정 필드 참조용 이름 구문

계산된 사용자 지정 필드에서 다른 사용자 지정 필드를 참조하는 경우 Workfront 사용자 인터페이스에 표시되는 대로 필드의 이름을 입력해야 합니다.

예를 들어, 경영진 스폰서라는 사용자 지정 필드에서 선택한 옵션을 참조하려면 다음을 입력합니다.

`{DE:Executive sponsor}`

>[!NOTE]
>
>typeahead 필드의 구문은 추가해야 하므로 다른 유형의 필드에 대한 구문과 약간 다릅니다 `:name` 끝.
>
>예를 들어, &quot;Executive sponsor&quot;라는 사용자 지정 서체 앞 필드에서 선택한 옵션을 참조하려면 다음을 입력합니다.
>
>`{DE:Executive sponsor:name}`


## 다중 개체 사용자 지정 양식의 계산된 사용자 지정 필드 {#calculated-custom-fields-in-multi-object-custom-forms}

다중 개체 사용자 지정 양식에서 선택한 개체 유형은 양식의 계산된 사용자 지정 필드에서 참조하는 모든 필드와 호환되어야 합니다. 비호환성이 있는 경우 조정을 하라는 메시지가 표시됩니다.

>[!INFO]
>
>**예:**
>
>작업 개체 유형으로 작동하도록 구성된 사용자 정의 양식에서는 In Charge라는 계산된 사용자 정의 필드를 만듭니다. 기본 제공 필드를 참조하도록 구성하면, 양식을 작업에 첨부할 때마다 담당 기본 할당자의 이름을 표시할 수 있습니다.
>
>`{assignedTo}.{name}`
>
>나중에 사용자 지정 양식에 프로젝트 개체 유형을 추가합니다. 경고 메시지는 프로젝트 개체 유형이 계산된 사용자 지정 필드와 호환되지 않음을 알려줍니다.

이 경우 다음 중 하나를 수행할 수 있습니다.

* 사용자 지정 양식에서 호환되지 않는 두 항목(개체 유형 또는 참조된 계산된 사용자 지정 필드) 중 하나를 제거합니다.
* 두 항목을 모두 유지하고 와일드카드 필터 변수를 사용하십시오 `$$OBJCODE` 를 IF 표현식의 조건으로 사용하여 In Charge 필드의 두 가지 다른 버전을 만듭니다. 따라서 양식이 첨부된 객체 유형에 관계없이 필드가 성공적으로 작동할 수 있습니다.

>[!INFO]
>
>**예:** 지정 대상 없음: 프로젝트에 이름 필드가 기본적으로 제공되는 소유자 필드가 있습니다(수동으로 변경하지 않는 한 프로젝트를 생성한 사람의 이름으로 자동으로 입력됨).
>
>따라서 사용자 지정 담당자 필드에서 `$$OBJCODE` 사용자 지정 양식이 프로젝트에 첨부된 경우 소유자 필드를 참조하고 지정 대상: 양식에 작업이 첨부된 경우 이름 필드:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

와 같은 변수에 대한 자세한 정보 `$$OBJCODE,` 참조 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 계산된 사용자 지정 필드의 자동 업데이트

개체의 계산된 사용자 지정 필드는 다음 상황이 발생하면 자동으로 다시 계산됩니다.

* 일별 타임라인 계산과 같이 객체에 대한 항목이 변경됩니다.
* 누군가 개체의 계산된 사용자 지정 필드에서 참조하는 다른 필드를 편집합니다.
* 계산된 표현식이 비어 있고 필드에 값이 있습니다. 이 값은 null로 설정됩니다.

   >[!NOTE]
   >
   ><div>개체에 첨부된 사용자 지정 양식에서는 조직의 인스턴스 및 사용자 프로필에 대해 설정된 시간대 구성이 아니라 계산된 사용자 지정 필드의 날짜 및 시간 문이 UTC(Coordinated Universal Time)로 계산되어 저장됩니다. 사용자 지정 양식의 계산은 각 사용자의 개별 시간대를 기반으로 생성합니다.</div>

