---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 프로젝트 및 이니셔티브 간 리소스 할당 조정 개요
description: 프로젝트 및 이니셔티브 간 리소스 할당 조정 개요
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# 프로젝트 및 이니셔티브 간 리소스 할당 조정 개요

>[!IMPORTANT]
>
>조직은 Adobe Analytics 세트에 대해 추가 라이센스를 구입해야 합니다 [!DNL Adobe Workfront Scenario Planner] 프로젝트에 대한 이니셔티브 정보를 볼 수 있습니다. 를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. [시나리오 플래너를 사용하는 데 필요한 액세스](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

프로젝트를 이니셔티브에 연결하여 전략적 계획과 실제 작업이 동기화되도록 할 수 있습니다. Adobe Analytics Mobile Apps 또는 Analytics Premium에서 [!DNL Scenario Planner] 프로젝트에서 실제 작업을 계획하면 프로젝트와 이니셔티브 모두에서 리소스가 일치하는지 확인할 수 있으므로 리소스를 과다 할당하거나 사용하지 않습니다.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 의 플랜 [!DNL Scenario Planner] 프로젝트에 연결된 이니셔티브로
* 이니셔티브에 필요한 작업 역할 할당입니다.
* 계획 시간이 있고 다음 중 하나에 지정된 프로젝트의 작업 또는 문제:

   * 작업 역할
   * 작업 역할과 연결된 사용자

## 프로젝트 및 이니셔티브 연결

>[!NOTE]
>
>조직에서 다음에 대한 추가 라이센스를 구입한 경우에만 이니셔티브를 생성하고 프로젝트에 연결할 수 있습니다 [!DNL Workfront Scenario Planner].

다음 중 하나를 수행하여 프로젝트를 이니셔티브에 연결할 수 있습니다.

* 새로운 이니셔티브로 프로젝트를 계획에 가져오기

   자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 프로젝트에 이니셔티브 게시

   자세한 내용은 [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

두 프로세스 모두 프로젝트와 해당 이니셔티브 간에 연결을 만듭니다. 연결된 후 비교하고 일치하는지 확인하여 리소스 할당을 관리할 수 있습니다.

## 연결된 프로젝트 및 이니셔티브에서 리소스 조정에 대한 고려 사항

>[!NOTE]
>
>조직에서 프로젝트에 대한 추가 라이선스를 구입한 경우에만 이니셔티브를 보고 프로젝트에 연결하고 프로젝트에서 해당 리소스 할당을 볼 수 있습니다 [!DNL Workfront Scenario Planner].

* 사용자, 팀 및 작업 역할을 프로젝트의 작업 항목에 할당하고, Job 역할을 이니셔티브에 할당할 수 있습니다. 따라서 프로젝트와 이니셔티브 간의 작업 역할만 조정할 수 있습니다.

   >[!TIP]
   >
   >프로젝트에 대한 사용자의 시간을 이니셔티브에 대한 역할 할당과 조정하기 위해서는 사용자를 작업 역할과 연결해야 합니다.

* 프로젝트의 다음 영역에서 연결된 프로젝트에 대한 초기 작업 역할 할당을 볼 수 있습니다.

   * [!DNL Scenario Planner] 섹션 [!UICONTROL 프로젝트 세부 사항] 프로젝트 영역. 자세한 내용은 다음 문서를 참조하십시오.

      * [에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만들 수 있습니다 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [프로젝트의 정보 관리 [!UICONTROL 개요] 영역](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >프로젝트에서 작업 역할 정보를 볼 수 없고, [!DNL Scenario Planner] 섹션 [!UICONTROL 프로젝트 세부 사항].

   * 다음 [!UICONTROL 역할 할당] 패널은 다음 영역에 있습니다.

      * [!DNL Workload Balancer] 프로젝트

         에서 이니셔티브와 연결된 프로젝트 간의 역할 할당을 보고 조정하는 방법에 대한 자세한 정보 [!DNL Workload Balancer]를 참조하십시오. [에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시 [!DNL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL 작업] 섹션

         에서 이니셔티브와 연결된 프로젝트 간의 역할 할당을 조정하는 방법에 대한 자세한 정보 [!UICONTROL 작업] 섹션을 참조하십시오. [작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >프로젝트 및 이니셔티브의 Job 역할 정보를 나란히 볼 수 있습니다 [!UICONTROL 역할 할당] 패널.



* 연결된 이니셔티브에서 프로젝트에 대한 작업 역할 할당을 볼 수 없습니다. 자세한 내용은 [계획 로 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
