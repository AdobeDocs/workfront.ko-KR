---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 다중 선택 사용자 지정 필드로 보고서 차트 지정
description: 다중 선택 사용자 지정 필드로 보고서를 차트할 수 없습니다. 다중 선택 사용자 지정 필드를 참조하는 추가 계산된 필드를 만들어 다중 선택 사용자 지정 필드의 값으로 보고서를 차트화해야 합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 다중 선택 사용자 지정 필드로 보고서 차트 지정

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

다중 선택 사용자 지정 필드로 보고서를 차트할 수 없습니다. 다중 선택 사용자 지정 필드를 참조하는 추가 계산된 필드를 만들어 다중 선택 사용자 지정 필드의 값으로 보고서를 차트화해야 합니다.

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
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다중 선택 사용자 지정 필드에서 선택한 값을 표시하는 계산된 사용자 지정 필드를 만들어야 합니다. 자세한 내용은 [다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성합니다](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 섹션에 자세히 설명되어 있습니다.

## 보고서를 다중 선택 사용자 지정 필드별로 차트 지정

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

다중 선택 사용자 지정 필드를 참조하여 보고서에 차트를 작성할 수 없습니다. 대신, 계산된 필드에 따라 지정된 개체 및 그룹의 다중 선택 사용자 지정 필드 값을 기록하는 계산된 필드를 만들 수 있습니다. 

* [다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성합니다](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [계산된 사용자 지정 필드를 참조하는 차트 작성](#build-a-chart-that-references-a-calculated-custom-field)

### 다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성합니다 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

다중 선택 사용자 지정 필드를 참조하는 계산된 필드를 만들려면 다음 전제 조건이 있어야 합니다.

* 사용자 지정 양식에서 다중 선택 사용자 지정 필드를 작성합니다.\
   사용자 지정 양식 작성 및 사용자 지정 필드 추가에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 개체에 사용자 지정 양식을 첨부합니다.
* 다중 선택 사용자 지정 필드를 각 개체의 값으로 채웁니다.

다중 선택 사용자 지정 필드를 참조하는 계산된 사용자 지정 필드를 작성하려면:

1. 사용자 지정 양식을 만들거나 기존 양식을 편집합니다.\
   사용자 지정 양식 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 사용자 지정 양식에 사용할 개체나 개체를 선택합니다.
1. 클릭&#x200B;**필드 추가**, 그런 다음 **계산된 지표** 다중 선택 사용자 지정 필드를 양식에 추가합니다.

1. 에서 **레이블** 상자에서 새 계산된 필드의 이름을 지정하여 다중 선택 사용자 지정 필드를 참조함을 나타냅니다.\
   예: &quot;계산된 다중 선택 필드.&quot;

1. 에서 **계산** 상자에 다음 코드를 입력합니다.

   ```
   {DE:Multi-select Custom Field}
   ```

1. Workfront에 표시되는 다중 선택 사용자 지정 필드의 실제 이름으로 &quot;Multi-select Custom Field&quot;를 대체합니다.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (선택 사항) 다중 선택 사용자 지정 필드가 이미 이 양식에 있고 이 양식이 이미 개체에 연결되어 있는 경우 **이전 계산 업데이트** 선택 사항입니다.\
   이렇게 하면 새 필드가 이미 객체에 첨부된 양식에 추가되므로 다중 선택 사용자 지정 필드의 값으로 자동으로 채워집니다.

1. 클릭 **완료**.
1. 클릭 **저장 +닫기**.

### 계산된 사용자 지정 필드를 참조하는 차트 작성 {#build-a-chart-that-references-a-calculated-custom-field}

1. (선택 사항) 차트하려는 모든 계산된 필드가 값으로 채워지는지 확인하려면 다중 선택 사용자 지정 필드와 계산된 사용자 지정 필드가 모두 있는 사용자 지정 양식이 포함된 보고서의 모든 개체를 선택한 다음 을 클릭합니다 **편집**.
1. (선택 사항 및 조건부) **사용자 지정 표현식 다시 계산** 필드를 클릭한 다음 **변경 내용 저장**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >이 옵션은 프로젝트를 일괄적으로 편집할 때 제거되었습니다.  을 클릭하여 프로젝트의 표현식을 일괄적으로 다시 계산할 수 있습니다 **자세히** 아이콘 ![](assets/more-icon-45x33.png) 프로젝트 목록의 맨 위에서 **표현식 다시 계산**.


1. 다중 선택 사용자 지정 필드를 참조하는 계산된 필드에 대한 차트를 추가할 보고서로 이동합니다.
1. 클릭 **보고서 작업**, 그런 다음 **편집**.

1. 을(를) 선택합니다 <strong>그룹화</strong> 탭을 클릭한 다음 <strong>그룹화 추가</strong>.
1. 추가<strong>계산된 다중 선택 필드</strong> 그룹으로 만들었습니다.
1. 을(를) 선택합니다 <strong>차트</strong> 탭을 선택하고 보고서에 차트를 추가합니다.<br>보고서에 차트를 추가하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">보고서에 차트 추가</a> 기사 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.
1. 을(를) 선택합니다 <strong>계산된 다중 선택 필드</strong> 차트에 표시할 필드 중 하나로 사용됩니다.
1. 클릭 <strong>저장 + 닫기</strong>.<br>이 보고서는 차트의 계산된 다중 선택 필드별로 그룹화된 결과를 표시합니다.
