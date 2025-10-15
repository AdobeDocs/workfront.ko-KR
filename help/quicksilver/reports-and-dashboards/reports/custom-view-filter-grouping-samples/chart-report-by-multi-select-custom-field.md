---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 다중 선택 사용자 정의 필드로 보고서 차트 작성
description: 다중 선택 사용자 지정 필드에서 선택한 선택 사항을 캡처하는 추가 계산된 필드를 생성한 후에만 다중 선택 사용자 지정 필드로 보고서를 차트로 작성할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# 다중 선택 사용자 정의 필드로 보고서 차트 작성

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

다중 선택 사용자 지정 필드를 사용하여 차트를 작성하기 보다는 다중 선택 사용자 지정 필드의 각 옵션에 대해 별도의 필드를 만드는 것이 좋습니다.

다중 선택 사용자 정의 필드의 예는 다음과 같습니다.

* 확인란
* 드롭다운 메뉴 다중 선택

텍스트 모드 사용에 대한 자세한 내용은 문서 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

그러나 다중 선택 필드의 각 옵션에 대해 별도의 필드를 사용할 수 없는 경우 계산된 사용자 정의 필드를 사용하여 다중 선택 필드의 선택 항목을 먼저 그룹화하여 다중 선택 사용자 정의 필드별로 보고서를 차트로 작성할 수 있습니다. 그런 다음 계산된 필드를 기준으로 보고서를 차트로 작성할 수 있습니다.

>[!NOTE]
>
>선택한 항목이 있는 항목은 한 번만 카운트됩니다.
>
>예를 들어, 선택 항목 1과 선택 항목 2가 옵션으로 있는 확인란 사용자 정의 필드가 있고, 양식을 작업에 첨부하는 경우, 선택 항목 1과 선택 항목 2가 모두 있는 작업이 선택 항목 1 또는 선택 항목 2만 선택된 작업이 아닌 별도의 차트 요소에 표시됩니다.
>
>선택 항목 1이 선택된 작업은 선택 항목 1 및 선택 항목 2가 선택된 작업과 동일한 차트 요소에 표시되지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>필터 수정을 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다중 선택 사용자 정의 필드에서 선택한 값을 표시하는 계산된 사용자 정의 필드를 만들어야 합니다. 자세한 내용은 이 문서의 [다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드 작성](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 섹션을 참조하십시오.

## 다중 선택 사용자 정의 필드로 보고서 차트 작성

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

다중 선택 사용자 지정 필드를 참조하여 보고서에서 차트를 작성할 수 없습니다. 대신 계산된 필드를 사용하여 특정 오브젝트 및 그룹에 대한 다중 선택 사용자 정의 필드의 값을 기록하는 계산된 필드를 만들 수 있습니다. 

* [다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 빌드합니다](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [계산된 사용자 정의 필드를 참조하는 차트 작성](#build-a-chart-that-references-a-calculated-custom-field)

### 다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성합니다 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

다중 선택 사용자 지정 필드를 참조하는 계산된 필드를 작성하려면 다음 사전 요구 사항이 있어야 합니다.

* 사용자 정의 양식의 다중 선택 사용자 정의 필드.\
  사용자 정의 양식을 작성하고 사용자 정의 필드를 추가하는 방법에 대한 자세한 내용은 문서 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

* 다중 선택 사용자 정의 필드가 오브젝트에 첨부된 사용자 정의 양식입니다.
* 각 개체에 대한 다중 선택 사용자 정의 필드 값.

다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성하려면 다음을 수행하십시오.

1. 사용자 정의 양식을 만들거나 기존 양식을 편집합니다.

   사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. 사용자 정의 양식과 함께 사용할 개체를 선택합니다.
1. **필드 추가**&#x200B;를 클릭한 다음 **계산됨**&#x200B;을 클릭하여 다중 선택 사용자 지정 필드를 양식에 추가합니다.

1. **레이블** 상자에서 다중 선택 사용자 지정 필드를 참조하도록 새 계산된 필드의 이름을 지정합니다.

   예: &quot;계산된 다중 선택 필드&quot;

1. **계산** 상자에 다음 코드를 입력합니다.

   `{DE:Multi-select Custom Field}`

   이렇게 하면 다중 선택 사용자 정의 필드에서 선택한 항목이 계산된 사용자 정의 필드에 추가됩니다. 예를 들어, 양식이 작업에 첨부되고 다중 선택 사용자 정의 필드에서 선택 항목 1을 선택한 경우 계산된 사용자 정의 필드에 값 &quot;선택 항목 1&quot;이 표시됩니다. 다른 작업에 대해 선택 항목 1과 선택 항목 2를 선택한 경우 계산된 사용자 정의 필드에 &quot;선택 항목 1, 선택 항목 2&quot; 값이 표시됩니다.

1. &quot;다중 선택 사용자 정의 필드&quot;를 Workfront에 나타나는 대로 다중 선택 사용자 정의 필드의 실제 이름으로 바꿉니다.

   ![계산된 다중 선택 사용자 지정 필드](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (선택 사항) 다중 선택 사용자 지정 필드가 이미 이 양식에 있고 이 양식이 개체에 이미 연결되어 있는 경우 **기존 계산에 적용** 옵션을 활성화합니다.

   이렇게 하면 다중 선택 사용자 정의 필드의 값이 객체에 이미 첨부된 양식에 추가될 때 새 계산된 필드가 자동으로 채워집니다.

1. **적용**&#x200B;을 클릭합니다.
1. **저장 후 닫기**&#x200B;를 클릭합니다.

   계산된 사용자 정의 필드가 사용자 정의 양식에 추가되고 양식이 현재 오브젝트에 첨부된 경우 필드는 다중 선택 사용자 정의 필드의 정보로 채워집니다.

### 계산된 사용자 정의 필드를 참조하는 차트 작성 {#build-a-chart-that-references-a-calculated-custom-field}

1. (선택 사항) 차트로 작성할 모든 계산된 필드가 값으로 채워지도록 하려면 보고서의 세부 정보 탭에서 다중 선택 사용자 지정 필드와 계산된 사용자 지정 필드가 모두 있는 사용자 지정 양식을 포함하는 모든 개체를 선택한 다음 **편집**&#x200B;을 클릭합니다.
1. (선택 사항 및 조건부) **사용자 지정 표현식 다시 계산** 필드를 선택한 다음 **변경 내용 저장**&#x200B;을 클릭합니다.\
   ![사용자 지정 표현식 다시 계산](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >이 옵션은 프로젝트 일괄 편집에서 제거되었습니다.  프로젝트 목록 맨 위에 있는 **자세히** 아이콘 ![자세히 아이콘](assets/more-icon-45x33.png)을 클릭한 다음 **식을 다시 계산**&#x200B;하여 프로젝트에 대한 식을 일괄적으로 다시 계산할 수 있습니다.

1. 다중 선택 사용자 정의 필드를 참조하는 계산된 필드에 대한 차트를 추가하려는 보고서로 이동합니다.
1. **보고서 동작**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. <strong>그룹화</strong> 탭을 선택한 다음 <strong>그룹화 추가</strong>를 클릭합니다.
1. 그룹화로 생성한 <strong>계산된 다중 선택 필드</strong>를 추가합니다.
1. <strong>차트</strong> 탭을 선택하고 보고서에 차트를 추가합니다.

   예를들어 **열** 차트를 선택하세요.
   <br>보고서에 차트를 추가하는 방법에 대한 자세한 내용은 문서 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">사용자 지정 보고서 만들기</a>에서 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">보고서에 차트 추가</a> 섹션을 참조하십시오.
1. **아래쪽(X) 축** 필드에서 차트에 표시할 <strong>계산된 다중 선택 필드</strong>를 선택합니다.
1. <strong>저장 및 닫기</strong>를 클릭합니다.

   이 보고서는 차트에 계산된 다중 선택 필드로 그룹화된 결과를 표시합니다.

   ![차트의 다중 선택 필드](assets/chart-multi-select-field-column-chart-example.png)
