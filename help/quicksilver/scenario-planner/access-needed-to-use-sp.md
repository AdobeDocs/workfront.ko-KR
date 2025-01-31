---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너를 사용하는 데 필요한 액세스
description: 시나리오 플래너에는 Adobe Workfront과 별도의 라이센스 및 추가 액세스 권한이 필요합니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# [!DNL Scenario Planner]을(를) 사용하기 위해 필요한 액세스 권한

<!--Audited: 04/2024-->

[!DNL Scenario Planner]에 추가 라이선스 요구 사항이 있습니다. [!DNL Workfront Scenario Planner]에 대한 자세한 내용은 [개요 [!DNL Scenario Planner] 개요](../scenario-planner/scenario-planner-overview.md)를 참조하세요.

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

올바른 액세스 또는 권한이 없으면 [!DNL  Adobe Workfront]의 [!UICONTROL 시나리오] 영역을 보거나 조직의 계획 또는 이니셔티브를 관리하지 못할 수 있습니다. 계획 및 이니셔티브의 관리에는 계획 및 이니셔티브 생성, 편집 및 삭제가 포함됩니다.

## [!DNL Adobe Workfront Scenario Planner]을(를) 보고 사용하는 데 필요한 액세스 권한

[!DNL Workfront Scenario Planner]에 액세스하려면 다음 조건을 모두 충족하는지 확인해야 합니다.

1. 조직에는 아래에 설명된 Workfront 플랜 중 하나가 있어야 합니다.

   새 Workfront 플랜을 사용하는지 아니면 현재 플랜을 사용하는지에 따라 조직에 다음 중 하나가 있어야 합니다.

   * 새 플랜의 경우 조직에 [!UICONTROL Ultimate] [!DNL Workfront] 플랜이 있어야 합니다. 시나리오 플래너는 [!UICONTROL Ultimate] 계획에만 포함되어 있습니다.

   * 현재 Workfront 플랜의 경우 귀사는 다음 두 가지 플랜을 모두 보유해야 합니다.

      * 조직은 [!DNL Workfront] [!UICONTROL 비즈니스] 또는 [!DNL Workfront] 이상의 플랜을 구매해야 합니다.

      * 조직에서 [!DNL Workfront] 라이선스 외에 [!DNL Workfront Scenario Planner] 라이선스를 구입해야 합니다. [!DNL Workfront Scenario Planner] 라이선스에 대한 자세한 내용은 [!DNL Workfront] 계정 담당자에게 문의하세요.

1. 아래에 설명된 Workfront 라이센스 중 하나가 있어야 합니다.

   새 라이선스를 사용하는지 아니면 현재 라이선스를 사용하는지에 따라 [!DNL Workfront] 관리자는 다음 유형의 라이선스를 사용자에게 할당해야 합니다.

   * 새 라이센스의 경우:
      * [!UICONTROL 표준]
      * [!UICONTROL 밝게]

   * 현재 라이센스의 경우:

      * [!UICONTROL 계획]
      * [!UICONTROL 작업]
      * [!UICONTROL 검토]

   >[!NOTE]
   > 
   >* 새 라이선스를 사용할 때 [!UICONTROL 기여자] 또는 [!UICONTROL 외부] 라이선스 유형을 가진 사용자는 [!DNL Scenario Planner]에 액세스할 수 없습니다.
   >
   >* 현재 라이선스를 사용할 때 요청 또는 외부 라이선스 유형을 가진 사용자는 시나리오 플래너에 액세스할 수 없습니다.

1. [!DNL Workfront] 관리자가 액세스 수준의 [!DNL Scenario Planner]에 대한 [!UICONTROL 보기] 또는 [!UICONTROL 편집] 액세스 권한을 부여해야 합니다.

   [!DNL Workfront Scenario Planner]에 대한 액세스 권한 부여에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

1. (선택 사항 및 권장) 계획 및 이니셔티브에 대한 재무 정보를 보거나 업데이트하려면 [!DNL Workfront] 관리자가 액세스 수준의 [!UICONTROL 재무 데이터]에 대한 액세스 권한도 부여해야 합니다. 액세스 수준의 재무 데이터 부여에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

1. (선택 사항) 본인이 만들지 않은 플랜에 액세스해야 하는 경우 플랜 작성자는 해당 플랜에 액세스할 수 있는 올바른 권한을 부여해야 합니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 이 문서의 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션을 참조하십시오.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## 계획 및 이니셔티브 보기에 필요한 액세스

귀사에서 [!DNL Workfront Scenario Planner]에 대한 올바른 라이선스를 취득하는 것 외에도 [!DNL Workfront] 관리자가 귀하에게 다음 액세스 및 설정을 할당하여 [!DNL Workfront Scenario Planner] 및 이 영역의 정보를 볼 수 있도록 해야 합니다.

* [!DNL Scenario Planner]에 대한 액세스 권한이 [!UICONTROL 보기]개 이상인 액세스 수준입니다.

  [!DNL Scenario Planner]에 대한 액세스 수준에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

* 플랜 및 이니셔티브에 대한 재무 정보를 확인해야 하는 경우 [!UICONTROL 재무 데이터]에 대한 액세스 권한이 [!UICONTROL 보기]개 이상인 액세스 수준입니다. 재무 정보의 몇 가지 예는 예산, 비용 또는 직무 역할률입니다.

  [!UICONTROL 재무 데이터] 액세스 수준에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

  >[!TIP]
  >
  >[!UICONTROL 요청자] 및 [!UICONTROL 외부] 사용자는 [!DNL Scenario Planner]을(를) 볼 수 있는 액세스 권한이 없습니다.

* 플랜에 대한 권한을 봅니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 이 문서의 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션을 참조하십시오.

## 계획 및 이니셔티브 관리에 필요한 액세스

[!DNL Scenario Planner]에서 계획과 해당 정보를 관리할 수 있도록 [!DNL Workfront] 관리자가 다음 액세스 권한을 귀하에게 할당해야 합니다.

* 액세스 수준의 [!DNL Scenario Planner]에 대한 편집 액세스 권한이 있는 [!UICONTROL 플랜] 또는 [!UICONTROL 작업] 라이선스 유형입니다.

  다른 모든 라이선스 유형에는 플랜 관리에 대한 액세스 권한이 없습니다.

  액세스 수준에서 [!DNL Scenario Planner]에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

* 플랜에 대한 재무 정보도 업데이트해야 하는 경우 액세스 수준의 [!UICONTROL 재무 데이터]에 대한 [!UICONTROL 편집] 액세스 권한을 가진 [!UICONTROL 플랜] 라이선스 유형입니다.

  편집할 수 있는 재무 정보의 일부 예는 [!UICONTROL 예산], [!UICONTROL 계획된 혜택] 및 [!UICONTROL 고정 비용]입니다.

  >[!TIP]
  >
  >[!UICONTROL 플랜] 라이선스 소유자만 [!UICONTROL 재무 데이터]에 대한 [!UICONTROL 편집] 액세스 권한을 갖습니다.

  [!UICONTROL 재무 데이터] 액세스 수준에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

* 만들지 않은 플랜에 대한 권한을 관리합니다. 만들지 않은 계획 및 이니셔티브에 액세스하는 데 필요한 권한에 대한 자세한 내용은 이 문서의 [계획 및 이니셔티브에 액세스하는 데 필요한 권한](#permissions-needed-to-access-plans-and-initiatives) 섹션을 참조하십시오.

## 계획 및 이니셔티브에 액세스하는 데 필요한 권한

액세스 수준은 [!DNL Workfront]의 권한과 함께 작동하여 사용자가 만들지 않은 계획 및 이니셔티브를 볼 수 있도록 합니다. [!DNL Scenario Planner]에 액세스할 수 있는 올바른 액세스 수준을 보유할 뿐만 아니라 해당 계획을 만든 사람이 아니라면 보거나 관리할 계획에 대한 올바른 사용 권한도 보유해야 합니다.

시스템 관리자를 포함한 모든 사용자는 자신이 생성한 플랜에만 액세스할 수 있습니다.

다른 사용자가 만든 플랜을 보려면 다음과 같은 방법으로 해당 플랜을 사용자와 공유해야 합니다.

* 플랜을 공유합니다.

  공유 계획에 대한 자세한 내용은 [다음에서 계획 공유 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)를 참조하십시오.

* 자신이 만든 플랜에 대한 링크 보내기

  사용자가 플랜도 공유하지 않고 플랜에 대한 링크를 공유하는 경우 플랜에 대한 권한을 요청할 수 있습니다. 플랜에 대한 권한 요청에 대한 자세한 내용은 [의 플랜에 대한 액세스 요청 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)을 참조하십시오.

>[!NOTE]
>
>사용자가 비활성화되면 플랜에는 소유자가 없으며 이전에 링크와 공유하지 않는 한 액세스할 수 없습니다.


