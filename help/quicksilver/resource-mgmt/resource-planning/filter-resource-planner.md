---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너에서 정보 필터링
description: '(AL:*이 문서에 대해 반복합니다. 사용자 정의 데이터에 의한 필터링. 기타 개선 사항 주의 사항 있는 특수 문자가 변경될 수 있습니다. 스토리를 따라 언제 변경되는지 알아보십시오. 그것은 원래 베타 3 17.3)에서 왔다'
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '2415'
ht-degree: 0%

---

# 리소스 플래너에서 정보 필터링

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

필터를 사용하면 시스템에 저장된 모든 정보에서 리소스 플래너에 표시되는 정보를 수정할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 사용자 및 리소스 관리에 대한 보기 이상의 액세스 권한 </p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 리소스 플래너 필터 개요

리소스 플래너에 표시되는 정보의 양을 최소화하기 위해 Adobe Workfront에서는 사전 구성된 기준이 있는 기본 필터를 제공합니다. 기본 필터에 대한 자세한 내용은 섹션을 참조하십시오 [리소스 플래너의 기본 필터 개요](#overview-of-the-default-filter-in-the-resource-planner) 이 문서에서.

사용자 지정된 필터를 빌드할 수도 있습니다. 리소스 플래너에서 필터 맞춤화에 대한 자세한 내용은 섹션 을 참조하십시오. [리소스 플래너 필터 만들기](#create-resource-planner-filters) 이 문서에서.

리소스 플래너에서 필터를 사용할 때는 다음 사항을 고려하십시오.

* 사용자가 만든 필터는 사용자만 볼 수 있습니다. 필터를 공유하여 다른 사용자가 사용할 수 있도록 할 수 있습니다.
* Workfront 관리자는 사용자가 만들거나 사용자와 공유하는 필터만 볼 수 있습니다.
* 리소스 플래너에 대해 다른 보기를 선택하면 필터링된 결과가 변경되지 않습니다.\
  리소스 플래너의 보기 변경에 대한 자세한 내용은 의 &quot;프로젝트/역할/사용자 보기&quot; 선택 섹션을 참조하십시오. [리소스 플래너 탐색 개요](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* 필터를 적용해도 프로젝트, 역할 또는 사용자에 대한 리소스 플래너의 할당 및 가용성 데이터는 변경되지 않습니다. 필터는 리소스 플래너에 표시되는 개체 수만 변경합니다.
* 필터링은 리소스 플래너에 동시에 표시되는 모든 오브젝트에 적용됩니다. 예를 들어 특정 사용자에 대해 필터링하면 리소스 플래너는 다음 결과만 표시합니다.

   * 해당 사용자가 리소스 풀(프로젝트 및 역할 보기)의 일부이거나 프로젝트에 대한 할당이 있는 프로젝트(사용자 보기)
   * 해당 프로젝트의 사용자와 연결된 역할\
     사용자가 연결된 프로젝트의 다른 역할 또는 사용자는 표시되지 않습니다.

## 리소스 플래너의 기본 필터 개요 {#overview-of-the-default-filter-in-the-resource-planner}

리소스 플래너를 처음 열면 Workfront에서 기본 필터를 적용합니다. 기본 필터를 편집하여 표시할 항목에 대해서만 필터링할 수 있습니다. 필터 수정에 대한 자세한 내용은 섹션을 참조하십시오 [리소스 플래너에서 필터 편집](#edit-a-filter-in-the-resource-planner) 이 문서에서.

기본 필터를 사용할 때는 다음 사항을 고려하십시오.

* 기본 필터는 다음과 같은 프로젝트에서만 정보를 검색합니다.

   * 현재 월의 첫 번째 일자 이후 발생하는 계획된 완료 일자
   * 현재 날짜로부터 4번째 달의 마지막 날 전에 발생하는 계획된 시작 일자
   * 현재 또는 계획 상태

  >[!IMPORTANT]
  >
  >기본 필터는 리소스 플래너에 표시하기 위해 선택한 기간에 관계없이 현재 월의 첫 번째 날부터 항상 4개월 이내에 발생하는 프로젝트에서 정보를 검색합니다.

* 사용자 보기에서는 시스템의 모든 사용자가 표시되지만 필터링된 프로젝트와 연결된 사용자만 시간 정보를 표시합니다.
* 필터를 저장하지 않고 기본 필터에서 정보를 편집할 수 있습니다.
* 기본 필터의 복사본을 복제 및 편집하고, 기본 필터에서 원하는 기준을 변경한 다음, 새 필터로 저장할 수 있습니다.
* 기본 필터는 삭제하거나 공유할 수 없습니다.

  ![RP_new_default_fitler_criteria__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## 리소스 플래너 필터 만들기 {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

리소스 플래너에서 필터를 만드는 것은 모든 보기에 대해 동일합니다.

필터를 만들기 전에 리소스 플래너에서 올바른 정보를 보기 위한 사전 요구 사항이 준비되었는지 확인하십시오.\
리소스 플래너 작업에 필요한 사전 요구 사항 충족에 대한 자세한 내용은 의 &quot;리소스 플래너에서 작업을 위한 사전 요구 사항&quot; 섹션을 참조하십시오. [리소스 플래너 개요](../../resource-mgmt/resource-planning/get-started-resource-planner.md) 기사.

필터를 만들 때 다음 사항을 고려하십시오.

* 한 번에 필터링할 수 있는 개체 수에는 제한이 없습니다.
* 필터에 추가할 수 있는 필드는 리소스 플래너에 적용하는 보기의 객체에 따라 변경됩니다. 예를 들어 문제 또는 작업 필드는 사용자 보기에만 표시되므로 사용자 보기에서만 필터링할 수 있습니다. 사용자 보기에서 문제 또는 작업에 대한 필터를 작성한 다음 프로젝트 또는 역할 보기에 적용하면 프로젝트 또는 역할 보기에 필드가 없으므로 무시됩니다. 이 경우 필터를 사용할 수 없는 것으로 표시됩니다.

리소스 플래너에서 필터를 만들려면 다음을 수행하십시오.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.

1. 클릭 **리소스 조달**.

   다음 **플래너** 기본적으로 표시됩니다.

   기본적으로 리소스 플래너에 처음 액세스하면 <strong>기본 필터</strong> 이 적용됩니다.<br>기본 필터에 대한 자세한 내용은 <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">리소스 플래너의 기본 필터 개요</a> 이 문서의 섹션.

1. 의 왼쪽 위 모서리에서 을(를) 클릭합니다. **필터** 아이콘.\
   ![filter_icon.png](assets/filter-icon.png)\
   또는\
   확장 **필터** 드롭다운 메뉴 및 클릭 **새 필터 추가**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. 기본 제공 기준을 사용하여 필터를 빌드하려면 다음 필드 중 하나를 지정합니다.

   * **Portfolio**: 리소스 플래너에 포함할 정보가 포함된 포트폴리오의 이름을 입력한 다음 목록에 표시될 때 이름을 클릭합니다.\
     여러 포트폴리오의 정보를 포함하려면 이 프로세스를 반복합니다.

   * **프로젝트 상태**: 프로젝트 상태 드롭다운 메뉴를 확장하고 목록에서 사용할 수 있는 프로젝트 상태를 하나 이상 선택합니다.
   * **팀**: 보려는 프로젝트의 작업에 할당된 사용자와 연결된 하나 또는 여러 팀의 이름을 입력하세요.
   * **작업 역할**: 보려는 프로젝트의 작업에 할당된 사용자와 연결된 하나 또는 여러 작업 역할의 이름을 입력합니다.
   * **풀**: 프로젝트(프로젝트 보기의 경우), 사용자(사용자 보기의 경우) 또는 보려는 프로젝트 및 사용자(역할 보기의 경우) 모두와 연결된 하나 이상의 리소스 풀 이름을 입력합니다.
   * **그룹**: 보려는 사용자(사용자 보기) 또는 프로젝트(프로젝트 및 역할 보기)와 연결된 하나 이상의 그룹 이름을 입력합니다.

1. 클릭 **필터 규칙 추가**&#x200B;을(를) 만든 다음 **항목을 필터링하려면 입력** 상자. 필드를 사용할 수 있는 경우 해당 필드는 연결할 수 있는 각 오브젝트에 대해 채워집니다.

   >[!IMPORTANT]
   >
   >사용자 정의 필드를 참조할 때는 필드 레이블이 아니라 필드 이름을 입력해야 합니다. 필드 레이블은 오브젝트에 첨부된 사용자 정의 양식에 표시됩니다. 레이블과 사용자 정의 필드의 이름 간의 차이에 대한 자세한 내용은  [사용자 정의 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. 목록에 나타날 때 필드 이름을 클릭하여 필터에 추가합니다.\
   목록에 표시되는 필드에 대한 자세한 내용은 [Adobe Workfront 용어 목록](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (선택 사항) 필터에 대한 필터 및 조건 수정자를 선택합니다. 사용 가능한 수정자는에 설명되어 있습니다 [필터 및 조건 수정자](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   사용자 기반 또는 날짜 기반 와일드카드를 사용하여 로그인한 사용자와 관련된 정보를 필터링할 수 있습니다.\
   필터에서 지원되는 와일드카드에 대한 자세한 내용은 [와일드카드 필터 변수 개요](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. 클릭 **저장**&#x200B;필터 규칙을 저장합니다.
1. (선택 사항) **필터 규칙 추가** 다른 객체 또는 필드에 대한 새 규칙을 추가합니다.
1. 클릭 **적용** 필터를 저장하지 않고 적용합니다.

   또는

   클릭 **필터 저장** 필터를 저장합니다.\
   ![RP_Apply_or_Save_buttons_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (조건부) **저장**&#x200B;에서 필터 이름을 지정합니다. **필터 이름** 안에 있는 상자 **필터 저장** 대화 상자. 필수 필드입니다.\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >필터 이름에 특수 문자가 포함된 경우 다음 문자만 사용합니다.
   >
   >* 쉼표
   >* 슬래시
   >* 하이픈
   >* 밑줄

1. **저장**&#x200B;을 클릭합니다.

   이제 리소스 플래너의 결과가 필터 규칙에 포함된 정보에 의해 필터링됩니다.

## 기존 필터 적용

사용자 또는 리소스 플래너에 대한 액세스 권한이 있는 사용자가 필터를 저장하면 리소스 플래너를 사용하는 모든 사용자가 필터를 사용할 수 있습니다.

기존 필터를 적용하려면

1. 리소스 플래너로 이동합니다.
1. 왼쪽 상단 모서리에서 을(를) 확장합니다. **필터** 드롭다운 메뉴.

   이 메뉴에서 사용자가 만든 필터 또는 다른 사용자가 만들어 사용자와 공유한 필터를 볼 수 있습니다.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. 드롭다운 메뉴에서 필터를 선택합니다. 사용자 또는 다른 사용자가 이 메뉴에서 만든 필터를 볼 수 있습니다.\
   필터를 선택하면 리소스 플래너에 표시되는 정보의 양이 자동으로 줄어듭니다.

## 리소스 플래너에서 필터 편집 {#edit-a-filter-in-the-resource-planner}

다음 중 하나를 수행하여 리소스 플래너에서 필터를 편집할 수 있습니다.

* [필터 이름 바꾸기](#rename-a-filter)
* [필터에서 정보 편집](#edit-the-information-in-a-filter)
* [필터 복제](#duplicate-a-filter)

필터를 편집하면 리소스 플래너에 대한 액세스 권한이 있는 시스템의 모든 사용자에 대해 업데이트됩니다.

### 필터 이름 바꾸기 {#rename-a-filter}

필터 조건을 변경하지 않고 필터 이름을 변경할 수 있습니다. 필터가 다른 사용자에게 표시되므로 시스템의 다른 사용자에게 이 변경 사항을 알리는 것이 좋습니다. 이 변경 사항은 리소스 플래너를 볼 수 있는 모든 사람의 필터 목록에 영향을 줍니다.

1. 리소스 플래너로 이동하여 **필터** 드롭다운 메뉴를 사용하여 저장된 필터를 선택합니다.
1. 확장 **필터** 드롭다운 메뉴. 이름을 바꿀 필터를 찾은 다음 필터 이름을 마우스로 가리킵니다.
1. 다음 항목 선택 **필터 이름 바꾸기** 아이콘을 클릭합니다.

   ![](assets/rp-filter-options-edit-350x154.png)

1. 에서 필터의 새 이름을 지정합니다. **필터 이름** 상자.
1. **저장**&#x200B;을 클릭합니다.\
   필터에 포함된 정보는 동일하며 이름이 업데이트됩니다.

### 필터에서 정보 편집 {#edit-the-information-in-a-filter}

이름을 변경하지 않고 필터에 포함하는 정보를 변경할 수 있습니다. 필터가 표시되므로 시스템의 다른 사용자에게 이 변경 사항을 알리는 것이 좋습니다. 이 변경 사항은 리소스 플래너를 볼 수 있는 모든 사람의 필터 목록에 영향을 줍니다.

1. 리소스 플래너로 이동하여 **필터** 왼쪽 위 모서리에 있는 드롭다운 메뉴.
1. 편집할 기존 필터를 선택합니다.
1. 다음을 클릭합니다. **필터** 아이콘.\
   ![filter_icon.png](assets/filter-icon.png)

1. 새 필드를 필터에 추가합니다.\
   필터 빌드에 대한 자세한 내용은 [리소스 플래너 필터 만들기](#create-resource-planner-filters).

1. 필터에 대해 선택한 기존 필드 위로 마우스를 가져간 다음 **편집** 아이콘을 클릭하여 다른 필드를 선택하거나 **삭제** 필드 삭제 아이콘\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (선택 사항) **필터 규칙 추가** 새 필드를 필터에 추가합니다.\
   필터 조건 정의에 대한 자세한 내용은 [리소스 플래너 필터 만들기](#create-resource-planner-filters).

1. 클릭 **적용** 필터를 저장하지 않고 적용합니다.

   또는

   클릭 **저장** 필터를 저장합니다.\
   필터는 동일한 이름으로 저장되지만 새로운 필터링 기준을 사용합니다.

### 필터 복제 {#duplicate-a-filter}

기존 필터를 복제할 수 있습니다. 원본 필터링 기준은 복제된 필터에 동일하게 유지되며 새 필터를 새 이름으로 저장할 수 있습니다.

1. 리소스 플래너로 이동하여 **필터** 왼쪽 위 모서리에 있는 드롭다운 메뉴.
1. 복제할 저장된 필터의 이름 위로 마우스를 가져갑니다.
1. 다음을 클릭합니다. **복제** 아이콘.

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   [중복 필터] 상자가 표시됩니다.

1. 다음에서 **필터 이름** 필드에서 복제된 필터의 새 이름을 지정합니다.\
   새 필터의 기본 이름은 입니다. *`<Original Filter Name>`(복사)*.

1. 클릭 **저장**. 원본 필터와 동일한 기준으로 새 이름이 있는 새 필터가 만들어집니다.

   >[!NOTE]
   >
   >이름이 같고 기준이 동일한 필터 2개가 있을 수 있지만 혼동을 피하기 위해 리소스 플래너에 고유한 필터링 기준과 이름이 있는 필터를 저장하는 것이 좋습니다.

## 필터 삭제

더 이상 필요하지 않은 필터를 삭제할 수 있습니다. 기본 필터는 삭제할 수 없습니다.

기본 필터에 대한 자세한 내용은 [리소스 플래너의 기본 필터 개요](#overview-of-the-default-filter-in-the-resource-planner) 이 문서의 섹션.

필터를 삭제하면 리소스 플래너에 대한 액세스 권한이 있는 모든 Workfront 사용자에 대한 필터가 삭제됩니다. 제거하기 전에 제거할 필터를 리소스 플래너에서 작업 중인 다른 사용자가 더 이상 사용하지 않는지 확인하십시오. 삭제된 필터는 복구할 수 없습니다.

필터를 제거하려면 다음 작업을 수행하십시오.

1. 리소스 플래너로 이동합니다.
1. 확장 **필터** 드롭다운 메뉴.
1. 제거할 필터를 찾아 이름을 마우스로 가리킵니다.
1. 다음 항목 선택 **필터 삭제** 아이콘을 클릭합니다.

   ![](assets/rp-filter-options---delete-350x154.png)

1. 클릭 **삭제** 다음에서 **필터 삭제** 대화 상자.

1. 리소스 플래너에서 필터가 삭제되고 제거됩니다.

## 필터 공유

빌드했거나 다른 사용자와 공유할 수 있는 액세스 권한이 있는 필터를 공유할 수 있습니다. 기본 필터는 공유할 수 없지만 복제하고 복사본을 공유할 수 있습니다.

>[!NOTE]
>
>Workfront 관리자를 비롯한 모든 사용자는 자신이 빌드했거나 자신과 공유된 필터에만 액세스할 수 있습니다. 특정 사용자와 필터를 공유하여 모든 리소스 플래너 사용자가 필터를 사용할 수 있도록 할 수 있습니다.

기본 필터에 대한 자세한 내용은 [리소스 플래너의 기본 필터 개요](#overview-of-the-default-filter-in-the-resource-planner) 이 문서의 섹션.

필터 복제에 대한 자세한 내용은 [필터 복제](#duplicate-a-filter) 이 문서의 섹션.

1. 리소스 플래너로 이동합니다.
1. 확장 **필터** 드롭다운 메뉴.
1. 공유할 필터를 찾아 이름을 마우스로 가리킵니다.
1. 다음 항목 선택 **필터 공유** 아이콘을 클릭합니다.

   ![](assets/rp-filter-options---share-350x154.png)

   필터 액세스 대화 상자가 표시됩니다.

1. (선택 사항) 모든 리소스 플래너 사용자가 필터를 사용할 수 있도록 하려면 **설정** 아이콘을 클릭한 다음 을 선택합니다 **시스템 전체에 표시**.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. 다음에서 **리소스 플래너 필터 액세스 권한 부여 대상:** 확인란을 선택하고 필터를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력합니다.
1. 다음 권한 수준 중에서 선택합니다.

   * 보기
   * 관리

     Workfront의 권한에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (선택 사항) **고급 설정**&#x200B;을(를) 클릭하여 각 수준에 대한 권한을 추가하거나 선택 해제하여 각 수준에 대한 권한을 제거합니다.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. **저장**&#x200B;을 클릭합니다.

   필터는 선택한 엔티티와 공유되며 **나와 공유됨** 영역입니다.

   ![](assets/rp-shared-with-me-area.png)
