---
title: 기존 양식 빌더로 계산된 데이터를 사용자 정의 양식에 추가
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 정의 양식에서 계산을 생성하는 계산된 사용자 정의 필드를 작성할 수 있습니다. 이를 위해 사용자 지정 필드, 계산된 사용자 지정 데이터 필드 및 기본 제공 Workfront 필드일 수 있는 데이터 표현식과 기존 필드의 이름을 사용하는 문을 만듭니다. 이 명령문은 사용자가 입력하는 데이터를 계산하고 새 계산된 사용자 정의 필드에 결과를 표시합니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: 02b025f228b6e2abc58dbc30f88c055c7850b803
workflow-type: tm+mt
source-wordcount: '2895'
ht-degree: 0%

---

# 기존 양식 빌더로 계산된 데이터를 사용자 정의 양식에 추가

<!--Audited: 01/2024-->

{{form-designer-default}}

사용자 정의 양식에서 사용자 정의 양식을 오브젝트에 첨부할 때 기존 데이터를 사용하는 계산된 사용자 정의 필드를 추가하여 새 데이터를 생성할 수 있습니다.

이를 위해 사용자 지정 필드, 계산된 사용자 지정 데이터 필드 및 기본 제공 Adobe Workfront 필드일 수 있는 데이터 표현식과 기존 필드의 이름을 사용하는 문을 만듭니다.

이 명령문은 사용자가 입력하는 데이터를 계산하고 새 계산된 사용자 정의 필드에 결과를 표시합니다.

계산된 사용자 정의 필드에는 다음이 포함될 수 있습니다.

* 단일 기본 제공 필드에 대한 간단한 참조입니다.

  >[!INFO]
  >
  > **예:** 프로젝트 및 작업에서 생성된 수입을 계산하기 위해 기본 제공 필드 실제 수입을 포함하는 계산된 사용자 정의 필드를 만들 수 있습니다. 누군가 사용자 정의 양식을 프로젝트 또는 작업에 첨부하면 프로젝트 또는 작업의 수익이 필드에 표시됩니다.

* 하나 이상의 필드를 참조하는 표현식입니다. 사용자 정의 필드, 기타 계산된 사용자 정의 필드 및 기본 제공 필드일 수 있습니다.

  >[!INFO]
  >
  >**예:** 프로젝트 및 태스크에서 생성된 이익을 계산하기 위해 매출에서 비용을 빼는 수학 표현식이 포함된 Profit이라는 계산된 사용자 정의 필드를 생성할 수 있습니다.
  >
  >이를 위해 내장된 Workfront 필드 실제 비용 및 실제 수익과 함께 수학 표현식 SUB(빼기)를 사용할 수 있습니다.
  >
  >아래 단계에서 이 예제를 수행하는 방법을 확인할 수 있습니다.

조직의 사용자 정의 양식을 만들고 연결할 수 있는 필드 유형을 이해하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>현재: 플랜</p>
   또는
   <p>새로운 기능: 표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </p> </td> 
  </tr>  
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 수준 구성을 확인하려면 Workfront 관리자에게 문의하십시오. 액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## 사용자 정의 양식에 계산된 필드 추가 {#add-a-calculated-field-to-a-custom-form}

기본 제공 Workfront 필드와 계산된 사용자 정의 필드의 표현식에서 이미 만든 사용자 정의 필드를 모두 사용할 수 있습니다.

>[!IMPORTANT]
>
>계산된 사용자 정의 필드를 만들기 전에 계산에 필요한 데이터가 Workfront에 있는지 확인할 수 있도록 포함하려는 기존 필드를 식별하십시오.

1. 에 설명된 대로 사용자 정의 양식을 만들거나 편집하기 시작합니다. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 다음에서 **필드 추가** 탭을 클릭하고 **계산됨**.

   오른쪽의 표시 영역에서 필드에 12345라는 입력 값이 표시됩니다. 사용자 정의 양식을 만들거나 편집하는 동안 필드가 계산된 사용자 정의 필드임을 알려주는 표시기입니다. 양식이 오브젝트에 첨부되고 사용자가 양식을 작성하는 경우 필드에 계산 결과가 표시되고 12345 값이 표시되지 않습니다.

1. 계산된 필드에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td>필드에 대한 레이블을 입력합니다. 이는 사용자가 사용자 정의 양식을 사용할 때 표시되는 내용입니다. 필드 <b>이름</b>가 자동으로 채워지고 레이블과 일치하는 는 보고서에서 Workfront에 의해 참조됩니다. 필수 필드입니다.</td> 
     </tr>

   <tr> 
   <td role="rowheader">이름</td> 
   <td>기본적으로 필드의 이름은 레이블과 같습니다. 그러나 필드의 이름 을 필드의 레이블 과 다르게 수정할 수 있습니다. 필드 <b>이름</b> 는 보고서에서 Workfront에 의해 참조됩니다. 필수 필드입니다.</td> 
   </tr>

   <tr> 
     <td role="rowheader" id="instructions">지침</td> 
      <td> <p>필드 및 수식에 대한 추가 정보를 제공하는 텍스트를 추가합니다.</p>
      <p>사용자 정의 필드 계산에 사용되는 공식을 여기에 붙여넣을 수도 있습니다. 이 경우 먼저 사용자 정의 필드의 계산을 업데이트한 다음 계산 필드에서 최종 표현식을 복사하여 지침 필드에 붙여넣는 것이 좋습니다. </p>


   이 기능은 다음과 같은 방법으로 유용할 수 있습니다.
   <ul> 
      <li> <p>공식이 무엇인지, 어떻게 작동하는지 다시 알리기 위해 이 기능은 여러 양식에서 이 계산된 사용자 정의 필드를 사용하려는 경우 특히 유용합니다.</p> </li> 
       <li> <p>툴팁으로 사용자는 필드를 마우스로 가리키면 표시됩니다. 도구 설명에 표시할 텍스트를 여기에 추가할 수 있습니다.</p> </li> 
       </ul>
       <p>사용자가 도구 설명에 수식을 볼 수 없도록 하려는 경우, 이러한 수식은 사용자에게 혼동을 줄 수 있으므로 지침 필드에 추가하지 마십시오. 대신 "지침에 수식 표시" 설정을 사용하여 수식을 표시하거나 숨깁니다(이 문서에 설명된 대로). <a href="#build-the-calculation-for-your-calculated-custom-field">계산된 사용자 정의 필드에 대한 계산을 작성합니다</a> 이 문서에서.</p>

   <p>새 양식에서 동일한 계산된 사용자 정의 필드를 사용하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">포맷</td> 
      <td> <p>필드의 결과를 저장 및 표시할 형식입니다.</p> <p>수학 계산에서 필드를 사용할 계획이라면 항상 <strong>숫자</strong> 또는 <strong>통화</strong> 포맷. 숫자 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</p> 
      <p><b>중요 사항</b>: <p>형식을 선택하기 전에 새 필드에 대한 올바른 형식을 고려하십시오. 사용자 정의 양식을 저장한 후에는 형식 필드를 편집할 수 없습니다. 그리고 잘못된 포맷을 선택하면 보고서와 목록 그룹화의 향후 계산 및 집계 값에 영향을 줄 수 있습니다.</p>
      <p><strong>참고:</strong> 통화 형식의 계산된 필드에는 따옴표를 포함하지 않아야 합니다. (예를 들어, "800.00"이 아닌 800.00을 사용합니다.) 따옴표를 사용하면 통화 유형의 언어 서식과 관련된 뉘앙스로 인해 예기치 않은 결과가 발생할 수 있습니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 섹션에 설명된 대로 사용자 정의 필드 정보를 계속 업데이트합니다 [계산된 사용자 정의 필드에 대한 계산을 작성합니다](#build-the-calculation-for-your-calculated-custom-field) 이 문서에서.

## 계산된 사용자 정의 필드에 대한 계산을 작성합니다 {#build-the-calculation-for-your-calculated-custom-field}

1. 섹션에 설명된 대로 계산된 사용자 정의 필드 만들기를 시작합니다. [사용자 정의 양식에 계산된 필드 추가](#add-a-calculated-field-to-a-custom-form) 이 문서에서.

1. 클릭 **최대화** 을(를) 열려면 **계산 편집기** 계산을 빌드합니다.

   >[!INFO]
   >
   >**예:** 이 문서 소개에 있는 예를 사용하여 프로젝트 및 작업에 대한 사용자 정의 양식에서 Profit이라는 계산된 사용자 정의 필드를 만들 수 있습니다. 이 필드에는 실제 수익과 실제 비용의 차이를 표시하는 계산이 포함될 수 있습니다.
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >이 예에서는 `SUB` 는 표현식이며 참조된 필드는 다음과 같습니다. `actualRevenue` 및 `actualCost`.

   일반적으로 계산은 표현식으로 시작하며, 그 뒤에는 사용자 정의 양식을 오브젝트에 첨부할 때 참조할 필드를 포함하는 괄호가 옵니다. 사용할 수 있는 표현식에 대한 자세한 내용은 [계산된 데이터 표현식 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   각 필드는 섹션에 설명된 대로 중괄호로 묶어야 합니다 [계산된 사용자 정의 필드에 필요한 구문](#syntax-required-in-calculated-custom-fields) 이 문서에서. 필드 이름을 입력할 때 시스템에서 제안을 하며 이를 선택하여 계산에 삽입할 수 있습니다.

   >[!NOTE]
   >
   >   계산에서 다음 유형의 필드를 참조할 수 없습니다. 
   >   
   >   * 포맷이 지정된 텍스트 필드
   >   * 설명 텍스트입니다.
   >   
   >   사용자 지정 필드 유형에 대한 자세한 내용은 [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. 계산 편집기 상자의 큰 텍스트 상자를 클릭한 다음 검색 또는 확장을 클릭하고 **표현식** 및 **필드** 텍스트 상자의 오른쪽에 있는 섹션입니다. 이렇게 하면 계산에 추가됩니다.

   큰 텍스트 상자에 식이나 필드를 입력한 다음 표시될 때 선택할 수도 있습니다. 각 항목은 필드에 &quot;F&quot;를 표시하거나 표현식에 &quot;E&quot;를 표시합니다.

   여는 괄호를 입력하면 닫는 괄호가 자동으로 추가됩니다.

   >[!TIP]
   >
   >다음 중 원하는 작업을 수행하여 계산에 도움을 받을 수 있습니다.
   > 
   >* 계산에서 표현식 위로 마우스를 가져가 설명, 사용 방법을 보여주는 예 및 문서의 추가 정보에 대한 &quot;자세히 알아보기&quot; 링크를 확인합니다 [계산된 데이터 표현식 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* 색상 코딩을 사용하여 추가한 구성 요소를 식별합니다. 표현식은 파란색으로 표시되고 필드는 녹색으로 표시됩니다.
   >  ![](assets/colors-fields-expressions.jpg)
   >* 가면서 분홍색으로 강조 표시된 계산 오류를 찾습니다. 강조 표시된 오류 위로 마우스를 가져가 원인에 대한 간단한 설명을 표시할 수 있습니다.
   >  ![](assets/error-help.png)
   >* 다음에서 **기존 오브젝트에서 미리 보기** 계산 아래 영역에서 Workfront 개체의 이름을 입력하고 목록에 표시될 때 선택합니다. 이렇게 하면 양식이 오브젝트에 첨부될 때의 필드 모양을 미리 볼 수 있습니다.
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* 왼쪽에 표시되는 줄 번호를 사용하여 긴 계산에서 참조 표현식입니다.

1. 클릭 **최소화** 계산된 사용자 정의 필드에 대한 계산 생성을 마치면

   >[!NOTE]
   >
   >오른쪽의 표시 영역에서 필드에 12345라는 입력 값이 표시됩니다. 사용자 정의 양식을 만들거나 편집하는 동안 필드가 계산된 사용자 정의 필드임을 알려주는 표시기입니다. 양식이 오브젝트에 첨부되고 사용자가 양식을 작성하는 경우 필드에 계산 결과가 표시되고 12345 값이 표시되지 않습니다.

1. (선택 사항) 다음 옵션 중 하나를 사용하여 계산된 사용자 정의 필드를 추가로 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">논리 추가</td> 
      <td>표시 논리를 추가하여 사용자가 양식을 채울 때 이전 다중 선택 필드(드롭다운, 확인란 또는 라디오 버튼)에서 선택한 하나 이상의 항목에 따라 계산된 필드가 표시되는지 여부를 결정할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가</a>. <p>적어도 하나의 확인란, 라디오 버튼 또는 드롭다운 필드가 양식의 계산된 사용자 지정 필드 앞에 오는 경우에만 사용할 수 있습니다. </p> <p>계산된 사용자 정의 필드에는 건너뛰기 논리를 사용할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이전 계산 업데이트</td> 
      <td>기존 계산된 사용자 정의 필드를 편집할 때 이 옵션을 선택하여 사용자 정의 양식을 저장할 때 계산에서 업데이트를 트리거할 수 있습니다. 이 작업은 사용자 정의 양식을 저장할 때 한 번만 발생합니다. 이렇게 하면 옵션이 비활성화 상태로 돌아갑니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침에 수식 표시</td> 
      <td>사용자 정의 양식을 작성하는 사용자가 필드를 마우스로 가리키면 필드의 공식이 표시되도록 하려면 이 옵션을 활성화한 상태로 두십시오. 자세한 내용은 다음에 대한 정보를 참조하십시오. <a href="#instructions" class="MCXref xref">지침</a> 이 테이블의 앞부분입니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **완료** 계산된 사용자 정의 필드에서 모든 변경이 완료된 경우.

   또는 **적용** 사용자 정의 필드를 양식에 계속 추가하려면 지금까지 변경 사항을 양식에 적용하십시오.

   또는 **저장 + 닫기** 사용자 정의 양식에서 모든 변경 사항이 완료된 경우.
1. 계산된 사용자 정의 필드가 올바르게 작동하는지 확인하려면 사용자 정의 양식을 오브젝트에 첨부한 다음 계산된 사용자 정의 필드에서 결과를 검토합니다.

   사용자 정의 양식을 첨부하는 방법은 [오브젝트에 사용자 정의 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   다른 방법으로 사용자 정의 양식을 계속 빌드하려면 다음 문서 중 하나를 계속 진행할 수 있습니다.

   * [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 계산된 사용자 정의 필드에 필요한 구문

사용자 지정 계산 필드에 사용되는 각 필드는 각 필드 이름 주위에 중괄호를 사용하여 아래에 설명된 구문을 사용해야 합니다. 필드 이름을 입력할 때 시스템에서 제안을 하며 이를 선택하여 계산에 삽입할 수 있습니다. 계산에 데이터를 잘못 입력하면 경고 메시지가 표시됩니다. 유효한 필드와 유효한 계산된 표현식을 포함하도록 계산을 편집하지 않으면 양식을 저장할 수 없습니다.

>[!NOTE]
>
>현재, 시스템은 객체의 상위가 아니라 사용자 정의 양식이 첨부될 객체에 참조할 필드 이름을 입력할 때만 제안을 합니다.

### 필드 이름을 중괄호로 묶습니다.

* 계산에서 기본 제공 필드를 참조하도록 하려면 필드 이름을 중괄호로 묶어야 하며 Workfront 데이터베이스에 나타나는 형식이어야 합니다. Workfront 인터페이스에 표시되는 필드의 이름은 사용할 수 없습니다.

예: `{actualRevenue}`

필드 이름은 대소문자를 구분하며 Workfront 시스템에 표시되므로 카멜 대/소문자 형식으로 표시되어야 합니다.

* 계산에서 사용자 정의 필드를 참조하도록 하려면 필드 이름을 중괄호로 묶고 앞에 를 붙여야 합니다 `DE:` 대괄호 안에 있습니다. 사용자 지정 필드는 대/소문자를 구분하므로 Workfront 인터페이스에 나타나는 대로 형식을 지정해야 합니다.

예: `{DE:Profit}`

입력할 때 선택할 수 있는 모든 사용자 정의 필드가 시스템에 나열됩니다 `DE:`.

* 사용자 정의 양식을 오브젝트에 첨부할 때 부모 오브젝트에서 데이터를 가져오는 필드를 계산에서 참조하려면 필드 이름 앞에 중괄호를 포함한 부모 오브젝트의 오브젝트 유형을 붙여야 합니다.

  예를 들어 사용자 정의 양식이 작업에서 작동하도록 구성되어 있고 양식을 작업에 첨부할 때 필드가 상위 개체의 실제 수입을 계산하도록 하려면 다음을 표시해야 합니다 `project` 을(를) 필드의 오브젝트 유형으로 만들면:

  `{project}.{actualRevenue}`

  또는 사용자 정의 필드인 경우:

  `{project}.{DE:profit}`

  사용자 정의 양식이 여러 객체 유형에 대해 구성되어 있기 때문에 상위 객체의 객체 유형을 잘 모를 경우 와일드카드 필터 변수를 사용할 수 있습니다 `$$OBJCODE` 가능한 각 유형에 대해 계산이 작동하도록 합니다. 자세한 내용은 [다중 오브젝트 사용자 정의 양식의 계산된 사용자 정의 필드](#calculated-custom-fields-in-multi-object-custom-forms) 이 문서에서.

### 마침표로 항목 구분

계산된 사용자 정의 필드에서 관련 객체를 참조할 때는 객체 이름과 속성을 마침표로 구분해야 합니다.

예를 들어 작업 유형 사용자 정의 양식에서 계산된 사용자 정의 필드에 Portfolio 소유자의 이름을 표시하려면 다음을 입력합니다.

`{project}.{porfolio}.{owner}`

이 시스템은 다음 단계(이 순서로)로 정보를 검색합니다.

1. 사용자 정의 양식(작업)의 객체에서
1. 작업의 상위 또는 다른 관련 개체(프로젝트)에 액세스한 다음
1. 프로젝트의 상위 또는 다른 관련 개체(포트폴리오)에 액세스한 다음
1. 포트폴리오(포트폴리오 소유자)에 대한 다음 관련 오브젝트에 액세스합니다.

### 사용자 정의 필드를 참조하기 위한 이름 구문

계산된 사용자 정의 필드에서 다른 사용자 정의 필드를 참조할 때 Workfront 인터페이스에 표시되는 대로 필드 이름을 입력해야 합니다.

예를 들어, 경영 스폰서라는 레이블이 지정된 사용자 정의 필드에서 선택한 옵션을 참조하려면 다음을 입력합니다.

`{DE:Executive sponsor}`

>[!NOTE]
>
>자동 완성 필드의 구문은 를 추가해야 하므로 다른 유형의 필드에 대한 구문과 다릅니다. `:name` 끝에 있습니다.
>
>예를 들어, &quot;경영 스폰서&quot;라는 사용자 정의 타이프 어헤드 필드에서 선택한 옵션을 참조하려면 다음을 입력합니다.
>
>`{DE:Executive sponsor:name}`

## 다중 오브젝트 사용자 정의 양식의 계산된 사용자 정의 필드 {#calculated-custom-fields-in-multi-object-custom-forms}

다중 개체 사용자 정의 양식에서 선택한 개체 유형은 해당 양식의 계산된 사용자 정의 필드에서 참조되는 모든 필드와 호환되어야 합니다.

>[!INFO]
>
>**예:**
>
>Task 개체 유형으로 작동하도록 구성된 사용자 정의 양식에서 In Charge라는 계산된 사용자 정의 필드를 만듭니다. 기본 제공 필드를 참조하도록 구성하여 양식이 작업에 첨부될 때마다 담당 기본 피할당자의 이름을 표시할 수 있습니다.
>
>`{assignedTo}.{name}`
>
>나중에 프로젝트 오브젝트 유형을 사용자 정의 양식에 추가하지만 프로젝트 오브젝트 유형이 계산된 사용자 정의 필드와 호환되지 않습니다.

이 경우 다음 중 하나를 수행할 수 있습니다.

* 사용자 정의 양식에서 호환되지 않는 두 항목 중 하나(오브젝트 유형 또는 참조된 계산된 사용자 정의 필드)를 제거합니다.
* 두 항목을 모두 유지하고 와일드카드 필터 변수 사용 `$$OBJCODE` IF 표현식에서 두 가지 서로 다른 버전의 담당 필드를 만드는 조건으로 사용됩니다. 이렇게 하면 양식이 첨부된 오브젝트 유형에 관계없이 필드가 정상적으로 작동할 수 있습니다.

>[!INFO]
>
>**예:** 프로젝트에는 할당 대상: 이름 필드가 없지만 기본 제공 소유자 필드가 있습니다(누군가 수동으로 이 필드를 변경하지 않는 한, 프로젝트를 만든 사람의 이름으로 자동으로 채워짐).
>
>따라서 사용자 정의 담당 필드에서 `$$OBJCODE` 아래 표시된 대로 사용자 정의 양식을 프로젝트에 첨부할 때 소유자 필드를 참조하고, 양식을 작업에 첨부할 때 할당 대상: 이름 필드를 참조합니다.
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

변수에 대한 자세한 내용은 다음을 참조하십시오 `$$OBJCODE,` 참조 [와일드카드 필터 변수 개요](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 계산된 사용자 정의 필드의 자동 업데이트

다음 상황이 발생하면 오브젝트의 계산된 사용자 정의 필드가 자동으로 다시 계산됩니다.

* 일별 타임라인 계산과 같이 오브젝트에 대한 내용이 변경됩니다.
* 누군가 개체의 계산된 사용자 정의 필드에서 참조하는 다른 필드를 편집합니다.
* 계산된 표현식이 비어 있고 필드에 값이 있습니다. 이 값은 null로 설정됩니다.

  >[!NOTE]
  >
  >오브젝트에 첨부된 사용자 정의 양식에서 계산된 사용자 정의 필드의 날짜 및 시간 문은 조직의 인스턴스 및 사용자 프로필에 대해 설정된 표준 시간대 구성이 아니라 UTC(협정 세계시)에 따라 계산되고 저장됩니다. 하지만 사용자 정의 양식의 계산은 각 사용자의 개별 시간대를 기반으로 하여 표시됩니다.
