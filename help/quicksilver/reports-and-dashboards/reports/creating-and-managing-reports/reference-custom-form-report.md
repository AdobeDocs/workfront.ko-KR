---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 보고서에서 사용자 지정 양식 참조
description: 해당 개체의 보기, 필터 및 보고서 그룹에서 개체의 사용자 지정 양식을 참조할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# 보고서에서 사용자 지정 양식 참조

해당 개체의 보기, 필터 및 보고서 그룹에서 개체의 사용자 지정 양식을 참조할 수 있습니다.

보고서에 포함할 사용자 지정 양식의 컨텐츠를 참조하거나 보고서에 포함할 사용자 지정 양식 자체에 대한 정보를 참조할 수 있습니다.

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

보고서에서 사용자 지정 양식을 참조할 수 있으려면 먼저 사용자 지정 양식이 있어야 합니다.

사용자 지정 양식 만들기에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 사용자 지정 양식의 콘텐츠 참조

사용자 지정 양식 내의 필드를 참조할 수 있습니다. 사용자 지정 양식이 개체에 적용되면, 해당 사용자 지정 양식과 연결된 모든 필드를 개체의 다른 필드로 보고서에서 참조할 수 있습니다.

>[!NOTE]
>
>여러 선택 사항이 있는 필드의 경우 숨겨진 옵션을 포함하여 보고서의 필터 및 프롬프트에 모든 옵션을 사용할 수 있습니다.\
>여러 선택 사항이 있는 사용자 지정 필드에서 선택 사항을 숨기는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

보고서를 만들 때 양식의 개체 유형을 필드 소스로 사용하고 사용자 지정 필드의 이름을 필드 이름으로 사용하면 됩니다.

예를 들어 사용자 지정 필드를 포함하는 모든 프로젝트에 사용자 지정 양식이 적용되어 있을 수 있습니다 **컨설턴트**. 컨설턴트인 올리비아 킴이 있는 모든 프로젝트를 나열하는 보고서를 만들려면 **프로젝트** 개체 유형을 필드 소스로 사용하고 **컨설턴트** 를 입력합니다. 필터 한정자를 로 설정합니다. **Equal**&#x200B;그리고 올리비아 김을 입력합니다.

![](assets/qs-consultant-filter-example-350x126.png)

보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 사용자 지정 양식에 대한 참조 정보

개체와 연결된 사용자 지정 양식의 이름 등 사용자 지정 양식에 대한 정보를 참조할 수 있습니다.

요소&#x200B;(보기, 필터 또는 그룹화)에 따라 다음 중 하나를 참조할 수 있습니다.

* 개체에 적용되는 기본 사용자 지정 양식:

   객체의 세부 정보 페이지에 먼저 나타나는 양식입니다.

* 모든 사용자 지정 양식(개체에 두 개 이상의 사용자 지정 양식이 적용되는 경우)

보기, 필터 및 그룹화에서 사용자 지정 양식을 참조할 수 있습니다.

* [보고서 보기에서 사용자 지정 양식 참조(열)](#reference-custom-forms-in-a-report-view-column)
* [보고서 필터에서 사용자 지정 양식 참조](#reference-custom-forms-in-a-report-filter)
* [보고서 그룹에서 사용자 지정 양식 참조](#reference-custom-forms-in-a-report-grouping)

### 보고서 보기에서 사용자 지정 양식 참조(열) {#reference-custom-forms-in-a-report-view-column}

객체와 연관된 모든 사용자 정의 양식을 표시하려면 다음을 수행하십시오.

1. 문서에 설명된 대로 보고서 만들기를 시작합니다 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 설정 **열** 탭에서 참조할 사용자 지정 양식이 적용되는 개체 유형을 확장한 다음 **카테고리 이름**.\
   예를 들어 작업과 연결된 모든 사용자 지정 양식을 표시하려면 **작업** 필드 소스를 찾은 다음 **카테고리 이름** 필드 이름.\
   ![](assets/qs-category-name-column-350x267.png)

개체와 연결된 기본 사용자 지정 양식만 표시하려면 다음을 수행하십시오.

1. 문서에 설명된 대로 보고서 만들기를 시작합니다 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 설정 **열** 탭에서 을 확장합니다. **카테고리** 필드 소스를 찾은 다음 **이름** 필드 이름.\
   ![](assets/qs-category-name-column-2-350x248.png)

### 보고서 필터에서 사용자 지정 양식 참조 {#reference-custom-forms-in-a-report-filter}

개체 유형과 연결된 모든 사용자 지정 양식을 필터링하려면 다음을 수행하십시오.

1. 문서에 설명된 대로 보고서 만들기를 시작합니다 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 설정 **필터** 탭, 확장 **카테고리**&#x200B;를 클릭한 다음 **이름**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. 사용할 조건 구분자를 선택합니다.

   * 비어 있음
   * 비어 있지 않음
   * 포함:
   * 포함하지 않음
   * 같음
   * 같지 않음

   각 한정자에 대한 자세한 내용은 문서를 참조하십시오 [필터 및 조건 수정자](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >을 필터링하는 필드에 여러 선택 사항이 있고 **같지 않음** 또는 **다음을 포함하지 않음** 구분자, 지정한 선택만 포함하는 결과를 필터링합니다. 필드에 지정된 옵션을 포함한 추가 옵션이 포함되어 있으면 해당 결과가 보고서에서 필터링되지 않습니다. 여기에는 동일한 개체에 첨부된 여러 사용자 지정 Forms에 대한 필터링이 포함됩니다.

1. 필터링할 사용자 지정 양식의 이름을 입력한 다음 드롭다운 목록에 표시될 이름을 클릭합니다.
1. (선택 사항) **다른 필터 규칙 추가**&#x200B;를 입력한 다음 2-4단계를 반복하여 추가 필터 규칙을 만듭니다.
1. 클릭 **저장+닫기**.

객체 유형과 연관된 기본 사용자 지정 양식에서만 필터링하려면

1. 문서에 설명된 대로 보고서 만들기를 시작합니다 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 설정 **필터** 탭에서 을 확장합니다. **카테고리** 필드 소스를 찾은 다음 **이름** 필드 이름.\
   ![](assets/qs-category-name-filter-350x437.png)

1. 사용할 조건 구분자를 선택합니다.

   * 비어 있음
   * 비어 있지 않음
   * 포함:
   * 포함하지 않음
   * 같음
   * 같지 않음

   각 한정자에 대한 자세한 내용은 문서를 참조하십시오 [필터 및 조건 수정자](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 필터링할 사용자 지정 양식의 이름을 입력한 다음 드롭다운 목록에 표시될 이름을 클릭합니다.
1. (선택 사항) **다른 필터 규칙 추가**&#x200B;를 입력한 다음 2-4단계를 반복하여 추가 필터 규칙을 만듭니다.
1. 클릭 **저장+닫기**.

### 보고서 그룹에서 사용자 지정 양식 참조 {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>개체와 연결된 기본 사용자 지정 양식으로만 항목을 그룹화할 수 있습니다. 개체와 연결된 모든 양식을 기준으로 항목을 그룹화할 수는 없습니다.

1. 문서에 설명된 대로 보고서 만들기를 시작합니다 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 설정 **그룹화** 탭, 확장 **카테고리**&#x200B;를 클릭한 다음 **이름**.\
   ![](assets/qs-category-name-grouping-350x373.png)
