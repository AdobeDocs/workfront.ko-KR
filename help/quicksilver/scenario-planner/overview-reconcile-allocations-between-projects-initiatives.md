---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 프로젝트와 이니셔티브 간 리소스 할당 조정 개요
description: 프로젝트와 이니셔티브 간 리소스 할당 조정 개요
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 프로젝트와 이니셔티브 간 리소스 할당 조정 개요

>[!IMPORTANT]
>
>프로젝트에 대한 이니셔티브 정보를 볼 수 있도록 [!DNL Adobe Workfront Scenario Planner]에 대한 추가 라이선스를 구입해야 합니다. [!DNL Workfront Scenario Planner]을(를) 얻는 방법에 대한 자세한 내용은 [시나리오 플래너를 사용하는 데 필요한 액세스](../scenario-planner/access-needed-to-use-sp.md) 를 참조하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

프로젝트와 이니셔티브를 연결하여 전략적 계획과 실제 작업이 동기화되도록 할 수 있습니다. [!DNL Scenario Planner]에서 전략적 계획과 이니셔티브의 개요를 설명하고 프로젝트의 실제 작업을 계획할 때 프로젝트와 이니셔티브 모두에 대한 리소스가 일치하는지 확인할 수 있으므로 이를 과다 할당하거나 과소 활용하지 않습니다.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 프로젝트에 연결된 이니셔티브가 있는 [!DNL Scenario Planner]의 플랜입니다.
* 이니셔티브에 대한 필수 작업 역할 할당입니다.
* 계획된 시간이 있고 다음 중 하나에 할당된 프로젝트의 작업 또는 문제입니다.

   * 작업 역할
   * 작업 역할과 연계된 사용자

## 프로젝트 및 이니셔티브 연결

>[!NOTE]
>
>조직에서 [!DNL Workfront Scenario Planner]에 대한 추가 라이선스를 구입한 경우에만 이니셔티브를 만들고 프로젝트에 연결할 수 있습니다.

다음 중 하나를 수행하여 프로젝트와 이니셔티브를 연결할 수 있습니다.

* 프로젝트를 새 이니셔티브로 플랜에 가져오기

  자세한 내용은 [플랜에 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)를 참조하십시오.

* 프로젝트에 대한 Publish 이니셔티브

  자세한 내용은 [ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)에서 이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기 를 참조하십시오.

두 프로세스는 프로젝트와 해당 이니셔티브 간에 연결을 만듭니다. 연결한 후 리소스 할당을 비교하고 일치하는지 확인하여 관리할 수 있습니다.

## 연결된 프로젝트 및 이니셔티브의 리소스 조정에 대한 고려 사항

>[!NOTE]
>
>조직에서 [!DNL Workfront Scenario Planner]에 대한 추가 라이선스를 구입한 경우에만 이니셔티브를 보고, 프로젝트에 연결하고, 프로젝트에 대한 리소스 할당을 볼 수 있습니다.

* 프로젝트의 작업 항목에 사용자, 팀 및 작업 역할을 할당하고 이니셔티브에 작업 역할을 할당할 수 있습니다. 따라서 프로젝트와 이니셔티브 간의 작업 역할만 조정할 수 있습니다.

  >[!TIP]
  >
  >프로젝트의 사용자 시간을 이니셔티브에 대한 역할 할당과 대사하려면 사용자를 작업 역할과 연결해야 합니다.

* 프로젝트의 다음 영역에서 연결된 프로젝트에 대한 이니셔티브 작업 역할 할당을 볼 수 있습니다.

   * 프로젝트의 [!UICONTROL 프로젝트 세부 정보] 영역에 있는 [!DNL Scenario Planner] 섹션. 자세한 내용은 다음 문서를 참조하십시오.

      * [ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)에서 이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기
      * [프로젝트 [!UICONTROL 개요] 영역의 정보 관리](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >[!UICONTROL 프로젝트 세부 정보]의 [!DNL Scenario Planner] 섹션에서 프로젝트 및 이니셔티브의 작업 역할 정보를 나란히 볼 수 없습니다.

   * 다음 영역의 [!UICONTROL 역할 할당] 패널:

      * 프로젝트의 [!UICONTROL 업무 균형자]

        [!UICONTROL 업무 균형자]에서 이니셔티브와 연결된 프로젝트 간 역할 할당을 보고 조정하는 방법에 대한 자세한 내용은 [업무 균형자에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시[!UICONTROL 를 참조하십시오]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL 작업] 섹션

        [!UICONTROL 작업] 섹션에서 이니셔티브와 연결된 프로젝트 간 역할 할당을 조정하는 방법에 대한 자세한 내용은 [작업 목록에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시](../scenario-planner/show-role-allocation-task-list-nwe.md)를 참조하십시오.

     >[!TIP]
     >
     >[!UICONTROL 역할 할당] 패널에서 프로젝트와 이니셔티브의 작업 역할 정보를 나란히 볼 수 있습니다.

* 연결된 이니셔티브에서 프로젝트에 대한 작업 역할 할당을 볼 수 없습니다. 자세한 내용은 [플랜에 프로젝트 가져오기 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)를 참조하십시오.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
