---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user,schedule
navigation-topic: configure-timesheets-and-schedules
title: 예약 개요
description: 일정을 사용하여 작업 주를 정의할 수 있습니다. 일정을 사용자 또는 프로젝트와 연결할 수 있습니다. 이렇게 하면 [!DNL Adobe Workfront] 타임라인과 사용자 가용성을 계산하기 위해 자세한 내용은 예약 만들기를 참조하십시오.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 예약 개요

일정을 사용하여 작업 주를 정의하고 일정을 사용자 또는 프로젝트와 연결할 수 있습니다. 이렇게 하면 [!DNL Adobe Workfront] 타임라인과 사용자 가용성을 계산하기 위해 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Workfront에서 일정을 사용할 때는 다음 사항을 고려하십시오.

* 다음 [!DNL Workfront] 관리자는 스케줄에서 조직의 작업 시간을 식별합니다.

   마찬가지로, 그룹 관리자는 관리 그룹이 관리하는 스케줄의 작동 시간을 식별할 수 있습니다.

   그룹 관리자에 대한 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   예를 들어 일정을 다음과 같이 정의할 수 있습니다. 월요일부터 금요일까지, 오전 8시부터 오후 5시까지, 점심 식사 시간 1시간이 있습니다.

* [!DNL Workfront] 스케줄을 사용하여 작업일이 시작되고 종료되는 시점을 결정합니다.

   이로 인해 사용자가 의 작업 또는 작업을 완료하지 못합니다 [!DNL Workfront] 정상적인 업무 시간 외에 일반적으로 저녁에 계획된 일에 초점을 맞추기 위해 새로운 일정이나 일정 예외를 만들 필요는 없습니다.

   마찬가지로, 조직에서는 근무일에 대해 유연한 도착 시간을 가질 수 있습니다. 오전 8시에 도착하는 직원 집합과 오전 9시에 도착하는 다른 세트가 있을 수 있습니다. 그룹이 유사하거나 동일한 일정을 갖는 경우에는 각 그룹에 대해 고유한 일정을 만들 필요가 없습니다. 하지만 그룹이 너무 다른 일정을 가지고 있다면, 해당 사용자는 고유한 예약과 연결되어 있어야 합니다. 직원은 오후 5시에 완료해야 하는 발령인지 파악합니다. 즉, 업무 개시 시간과 상관없이 업무 종료 전까지 작업이 완료되어야 합니다.

* 조직과 연관된 각 시간대에 대해 별도의 일정을 만드는 것이 좋습니다.

   각 예약에 대해 특정 시간대를 할당하여 작업량이 다른 시간대에 근무하는 사용자에게 적절하게 예약되도록 할 수 있습니다.

* 다음 [!DNL Workfront] 사용자 또는 프로젝트가 일정과 연결되어 있지 않을 때 타임라인 계산에서 기본 일정이 사용됩니다.

   기본 예약은 [!DNL Workfront] 시스템을 삭제할 수 없습니다.

* 타임라인을 계산하는 것 외에도 [!DNL Workfront] 일정을 사용하여 사용자 가용성을 계산합니다.

   >[!IMPORTANT]
   >
   >[!DNL Workfront] 사용자나 프로젝트 스케줄을 사용하여 자원 계획자의 자원 가용성을 결정합니다. 어떤 일정이 사용되는지는 [!DNL Workfront] 에 대해 선택된 관리자 [!UICONTROL 다음을 사용하여 리소스 가용성 계산] 설정 리소스 관리 설정에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 일정 계층

작업이 예약과 연관된 사용자에게 할당되고 두 번째 예약과 연관된 프로젝트에 상주하는 경우 타임라인 계산에 적용할 수 있는 일정이 2개 이상 있습니다.

>[!IMPORTANT]
>
>[!DNL Workfront] 는 [!UICONTROL 다음을 사용하여 리소스 가용성 계산] 설정이 [!UICONTROL 사용자 일정] 에서 [!UICONTROL 리소스 관리] 영역 [!UICONTROL 설정]. 자세한 내용은 [!UICONTROL 다음을 사용하여 리소스 가용성 계산] 리소스 관리에 사용되는 예약에 영향을 주는 설정 [리소스 관리 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

두 개 이상의 일정이 있을 때 시스템에서 일정을 사용하는 순서는 다음과 같습니다.

* 사용자가 작업에 할당되면 [!DNL Workfront] 작업 타임라인을 계산하기 위해 사용자의 일정을 사용합니다. 사용자의 개인 시간도 포함됩니다. 프로젝트 일정이 무시됩니다.

   개인 시간에 대한 자세한 내용은 [에서 개인 시간 초과 구성 [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 여러 사용자가 작업에 할당되고 사용자가 작업의 기간 동안 일정이 서로 다른 경우 [!DNL Workfront] 에서는 [!UICONTROL 프로젝트 환경 설정] 영역 [!UICONTROL 설정]:

   * 기본 할당자로 지정된 사용자의 일정
   * 프로젝트와 연결된 일정입니다.

      프로젝트 환경 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 작업에 지정된 사용자에게 일정이 없거나 작업이 작업 역할, 팀 또는 할당되지 않은 경우에만 할당되는 경우 [!DNL Workfront] 프로젝트 일정을 타임라인 계산에 사용합니다.
* 작업에 지정된 사용자에게 일정이 없거나 작업이 작업 역할, 팀 또는 할당되지 않은 경우에만 할당되며 프로젝트에 일정이 없는 경우 [!DNL Workfront] 타임라인 계산을 위해 기본 예약으로 지정된 시스템의 일정을 사용합니다.

   ![](assets/default-schedule.png)

## 의 공동 작업 [!DNL Workfront] 표준 시간대

사용자가 공동 작업할 수 있도록 스케줄을 사용하는 방법에 대한 자세한 내용은 [!DNL Workfront] 표준 시간대 간에 [시간대 작업](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
