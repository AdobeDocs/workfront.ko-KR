---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너를 사용하는 데 필요한 액세스
description: 시나리오 플래너는 Adobe Workfront과 별도의 라이센스와 추가 액세스가 필요합니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]

다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. [다음 [!DNL Scenario Planner] 개요](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

올바른 액세스 또는 권한이 없으면 [!UICONTROL 시나리오] 영역[!DNL  Adobe Workfront] 조직에 대한 계획 또는 이니셔티브를 관리하지도 않습니다. 계획 및 이니셔티브 관리에는 계획 생성, 편집 및 삭제 등이 포함됩니다.

>[!IMPORTANT]
>
>액세스 시 [!UICONTROL 시나리오]로 지정하는 경우 생성된 계획만 보고 관리할 수 있습니다. 다른 사용자가 작성한 계획을 보거나 관리하도록 하려면 다음을 수행해야 합니다.
>
>* 다른 사용자에게 플랜에 대한 링크 보내기
>* 다른 사용자와 계획 공유
>
>  계획 공유에 대한 자세한 내용은 [에서 플랜 공유 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>사용자가 비활성화되면 계획에 소유자가 없으므로 이전에 링크와 공유하지 않는 한 액세스할 수 없습니다.

## 을(를) 보고 사용하는 데 필요한 액세스 권한 [!DNL Adobe Workfront Scenario Planner]

에 액세스하려면 먼저 다음 조건이 모두 충족되었는지 확인해야 합니다 [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* 조직이 [!DNL Workfront] [!UICONTROL 비즈니스] 이상 [!DNL Workfront] 계획. 에 대한 정보 [!DNL Workfront] 계획 참조 [Workfront 플랜](http://workfront.com/plans).
* 조직이 [!DNL Workfront Scenario Planner] 라이센스, [!DNL Workfront] 라이센스. 다음 사항에 문의하십시오. [!DNL Workfront] 계정 담당자에게 문의하십시오 [!DNL Workfront Scenario Planner] 라이센스.

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* 사용자 [!DNL Workfront] 관리자는 다음 중 하나의 라이센스를 사용자에게 할당해야 합니다 [!DNL Workfront] 유형:

   * [!UICONTROL 플랜]
   * [!UICONTROL 작업]
   * [!UICONTROL 검토]

   >[!NOTE]
   >
   >을 사용하는 사용자 [!UICONTROL 요청] 또는 [!UICONTROL 외부] 라이선스 유형에 액세스할 수 없습니다. [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* 사용자 [!DNL Workfront] 관리자는 [!UICONTROL 보기] 또는 [!UICONTROL 편집] 액세스 [!DNL Scenario Planner] 액세스 수준에서

   액세스 권한 부여에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* (선택 사항 및 권장) 계획 및 이니셔티브에 대한 재무 정보를 보거나 갱신하려면 [!DNL Workfront] 또한 관리자는 [!UICONTROL 재무 데이터] 액세스 수준에서 액세스 수준에서 재무 데이터 부여에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* 만들지 않은 계획에 액세스해야 하는 경우 계획 작성자가 계획에 액세스할 수 있는 올바른 권한을 제공해야 합니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션에 자세히 설명되어 있습니다.

## 계획 및 이니셔티브를 보는 데 필요한 액세스

귀사에 대한 올바른 라이센스를 획득하는 것 외에도 [!DNL Workfront Scenario Planner], [!DNL Workfront] 또한 관리자가 다음 액세스 및 설정을 할당하여 [!DNL Workfront Scenario Planner] 그리고 이 영역에 있는 정보는 다음과 같습니다.

* 적어도 [!UICONTROL 보기] 액세스 [!DNL Scenario Planner].

   액세스 수준에 대한 자세한 내용은 [!DNL Scenario Planner]를 참조하십시오. [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 적어도 [!UICONTROL 보기] 액세스 [!UICONTROL 재무 데이터] 계획 및 이니셔티브에 대한 재무 정보도 확인해야 하는 경우 재정 정보의 몇 가지 예는 예산, 비용 또는 직무 역할율입니다.

   에 대한 정보 [!UICONTROL 재무 데이터] 액세스 수준 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL 요청자] 및 [!UICONTROL 외부] 사용자에게 [!DNL Scenario Planner].

* 계획에 대한 권한을 봅니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션에 자세히 설명되어 있습니다.

## 계획 및 이니셔티브를 관리하는 데 필요한 액세스

사용자 [!DNL Workfront] 관리자로부터 계획 및 해당 정보를 관리할 수 있도록 다음 액세스 권한을 지정해야 합니다. [!DNL Scenario Planner]:

* A [!UICONTROL 계획] 또는 [!UICONTROL 작업] 액세스 권한이 있는 라이선스 유형 [!DNL Scenario Planner] 액세스 수준에서

   다른 모든 라이선스 유형에는 플랜을 관리할 수 있는 액세스 권한이 없습니다.

   액세스 권한 부여에 대한 정보 [!DNL Scenario Planner] 액세스 수준에서 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL 계획] 라이센스 유형 [!UICONTROL 편집] 액세스 [!UICONTROL 재무 데이터] 액세스 수준에서 계획에 대한 재무 정보도 업데이트해야 합니다.

   편집할 수 있는 재무 정보의 몇 가지 예는 다음과 같습니다 [!UICONTROL 예산], [!UICONTROL 계획된 혜택], 및 [!UICONTROL 고정 비용].

   >[!TIP]
   >
   >전용 [!UICONTROL 계획] 라이센스 보유자가 [!UICONTROL 편집] 액세스 [!UICONTROL 재무 데이터].

   에 대한 정보 [!UICONTROL 재무 데이터] 액세스 수준 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 만들지 않은 계획에 대한 권한을 관리합니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션에 자세히 설명되어 있습니다.

## 계획 및 이니셔티브에 액세스하는 데 필요한 권한

액세스 레벨은 [!DNL Workfront] 사용자가 만들지 않은 계획과 이니셔티브에 대한 가시성을 제공하기 위해 액세스 수준을 올바르게 설정하면서 [!DNL Scenario Planner]를 지정하는 경우, 해당 계획의 작성자가 아닌 경우 보거나 관리할 계획에 대한 올바른 권한이 있어야 합니다.

기본적으로 생성된 계획에만 액세스할 수 있습니다. 다른 사용자가 작성한 계획을 보려면 자신의 계획을 사용자와 공유해야 합니다. 계획 공유에 대한 자세한 내용은 [에서 플랜 공유 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

사용자가 계획을 공유하지 않고 계획에 대한 링크를 공유하는 경우 계획에 대한 권한을 요청할 수 있습니다. 계획에 권한 요청에 대한 자세한 내용은 [에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

