---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너를 사용하는 데 필요한 액세스
description: 시나리오 플래너에는 Adobe Workfront과 별도의 라이센스 및 추가 액세스 권한이 필요합니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# [!DNL Scenario Planner]을(를) 사용하기 위해 필요한 액세스 권한

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

올바른 액세스 또는 권한이 없으면 [!UICONTROL 의 ]시나리오[!DNL  Adobe Workfront] 영역을 보거나 조직의 계획 또는 이니셔티브를 관리하지 못할 수 있습니다. 계획 및 이니셔티브의 관리에는 계획 및 이니셔티브 생성, 편집 및 삭제가 포함됩니다.

## [!DNL Adobe Workfront Scenario Planner]을(를) 보고 사용하는 데 필요한 액세스 권한

[!DNL Workfront Scenario Planner]에 액세스하려면 다음 조건을 모두 충족하는지 확인해야 합니다.

1. 조직에 Workfront Ultimate 패키지가 있어야 합니다.

   시나리오 플래너는 Workfront 워크플로 패키지에 사용할 수 없습니다.

   현재 Workfront을 갱신하고 있으며 시나리오 플래너를 유지하려는 경우 Workfront 계정 담당자에게 문의하십시오.

   신규 고객인 경우 시나리오 플래너를 더 이상 구매할 수 없습니다.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. 다음 Workfront 라이선스 중 하나가 있어야 합니다.

   * [!UICONTROL 밝게] 이상
   * [!UICONTROL 검토자] 이상

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. [!DNL Workfront] 관리자가 액세스 수준의 [!UICONTROL 에 대한 ]보기[!UICONTROL  또는 ]편집[!DNL Scenario Planner] 액세스 권한을 부여해야 합니다.

   [!DNL Workfront Scenario Planner]에 대한 액세스 권한 부여에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

1. (선택 사항 및 권장) 계획 및 이니셔티브에 대한 재무 정보를 보거나 업데이트하려면 [!DNL Workfront] 관리자가 액세스 수준의 [!UICONTROL 재무 데이터]에 대한 액세스 권한도 부여해야 합니다. 액세스 수준의 재무 데이터 부여에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## 계획 및 이니셔티브에 액세스하는 데 필요한 권한

액세스 수준은 [!DNL Workfront]의 권한과 함께 작동하여 사용자가 만들지 않은 계획 및 이니셔티브를 볼 수 있도록 합니다. [!DNL Scenario Planner]에 액세스할 수 있는 올바른 액세스 수준을 가질 수 있을 뿐만 아니라 해당 계획을 만든 사람이 아니라면 보거나 관리할 계획에도 올바른 권한이 있어야 합니다.

시스템 관리자를 포함한 모든 사용자는 자신이 생성한 플랜에만 액세스할 수 있습니다.

다른 사용자가 만든 플랜을 보려면 다음과 같은 방법으로 해당 플랜을 사용자와 공유해야 합니다.

* 플랜을 공유합니다.

  공유 계획에 대한 자세한 내용은 [다음에서 계획 공유 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)를 참조하십시오.

* 자신이 만든 플랜에 대한 링크 보내기

  사용자가 플랜도 공유하지 않고 플랜에 대한 링크를 공유하는 경우 플랜에 대한 권한을 요청할 수 있습니다. 플랜에 대한 권한 요청에 대한 자세한 내용은 [의 플랜에 대한 액세스 요청 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)을 참조하십시오.

>[!NOTE]
>
>사용자가 비활성화되면 플랜에는 소유자가 없으며 이전에 링크와 공유하지 않는 한 액세스할 수 없습니다.


