---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: 사용자,예약
navigation-topic: configure-timesheets-and-schedules
title: 일정 개요
description: 스케줄을 사용하여 작업 주를 정의할 수 있습니다. 사용자 또는 프로젝트와 일정을 연결할 수 있습니다. 이렇게 하면 [!DNL Adobe Workfront] 을 클릭하여 타임라인 및 사용자 가용성을 계산합니다. 자세한 내용은 예약 만들기 를 참조하십시오.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 일정 개요

<!-- Audited: 1/2024 -->

스케줄을 사용하여 작업 주를 정의하고 사용자 또는 프로젝트와 스케줄을 연관시킬 수 있습니다. 이렇게 하면 [!DNL Adobe Workfront] 을 클릭하여 타임라인 및 사용자 가용성을 계산합니다. 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Workfront에서 일정을 사용할 때는 다음 사항을 고려하십시오.

* 다음 [!DNL Workfront] 관리자는 일정에 있는 조직의 운영 시간을 식별합니다.

  마찬가지로 그룹 관리자는 자신이 관리하는 그룹이 관리하는 스케줄의 운영 시간을 식별할 수 있습니다. 그룹 관리자에 대한 자세한 내용은 [그룹 관리자](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  예를 들어, 월요일부터 금요일까지, 오전 8시부터 오후 5시까지(점심에는 1시간 휴식) 예약으로 정의할 수 있습니다.

* [!DNL Workfront] 에서는 스케줄을 사용하여 근무일의 시작 및 종료 시점을 결정합니다.

  그렇다고 해서 사용자가에서 작업하거나 작업을 완료할 수 있습니다. [!DNL Workfront] 정상 업무 시간 외. 일반적으로 저녁에 계획된 작업에 집중하기 위해 새 일정이나 일정 예외를 만들 필요는 없습니다.

  마찬가지로, 조직은 근무일에 대해 유연한 도착 시간을 가질 수 있습니다. 오전 8시에 도착하는 사원과 오전 9시에 도착하는 사원이 있을 수 있습니다. 그룹이 유사하거나 동일한 일정을 갖는 경우 각 그룹에 대해 고유한 일정을 생성할 필요는 없습니다. 그러나 그룹의 일정이 크게 다를 경우 사용자는 고유한 일정과 연결되어야 합니다. 사원은 오후 5시에 발령이 완료되어야 하는 경우 출근과 상관없이 업무가 업무일 종료일까지 완료되어야 한다는 것을 이해합니다.

* 조직과 연관된 각 시간대에 대해 별도의 일정을 생성하는 것이 좋습니다.

  각 일정에 특정 시간대를 할당하여 다른 시간대에서 작업하는 사용자에게 작업이 적절하게 예약되도록 할 수 있습니다.

* 다음 [!DNL Workfront] 사용자 또는 프로젝트가 일정과 연결되어 있지 않을 때 타임라인 계산에 기본 일정이 사용됩니다.

  기본 일정은 [!DNL Workfront] 새 일정으로 대체되지 않는 한 시스템 및 을(를) 삭제할 수 없습니다.

* 타임라인을 계산하는 것 외에도 [!DNL Workfront] 은 일정을 사용하여 사용자 가용성을 계산합니다.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] 사용자 또는 프로젝트 일정을 사용하여 리소스 플래너에서 리소스 가용성을 결정합니다. 어떤 일정을 사용할지는 [!DNL Workfront] 에 대해 선택된 관리자 [!UICONTROL 리소스 가용성 계산] 설정. 리소스 관리 설정에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 일정 계층

일정과 연관된 사용자에게 작업이 할당되고 두 번째 일정과 연관된 프로젝트에 있는 경우 타임라인 계산에 적용할 수 있는 일정이 최소 2개 있습니다.

>[!IMPORTANT]
>
>[!DNL Workfront] 은(는) 다음의 경우에만 사용자의 일정을 사용합니다. [!UICONTROL 리소스 가용성 계산] 설정이 로 설정되어 있습니다. [!UICONTROL 사용자의 일정] 다음에서 [!UICONTROL 리소스 관리] 영역 [!UICONTROL 설정]. 다음 방법에 대한 자세한 내용은 [!UICONTROL 리소스 가용성 계산] 설정은 리소스 관리에 사용되는 일정에 영향을 줍니다. [리소스 관리 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

둘 이상의 일정이 있을 때 시스템에서 일정을 사용하는 순서는 다음과 같습니다.

* 사용자가 작업에 할당되면, [!DNL Workfront] 은 작업의 타임라인 계산에 사용자의 일정을 사용합니다. 여기에는 사용자의 개인 시간도 포함됩니다. 프로젝트의 일정이 무시됩니다.

  개인 시간에 대한 자세한 내용은 [개인 휴무 구성](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 작업에 여러 사용자가 할당되고 작업 기간 동안 다른 일정이 있는 경우 [!DNL Workfront] 에서 정의한 대로 다음 일정 중 하나를 사용합니다. [!UICONTROL 프로젝트 환경 설정] 영역 [!UICONTROL 설정]:

   * 기본 피할당자로 지정된 사용자의 일정
   * 프로젝트와 연계된 일정.

     프로젝트 환경 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 작업에 할당된 사용자에게 일정이 없거나 작업이 작업 역할, 팀에만 할당되거나 할당이 해제된 경우 [!DNL Workfront] 에서는 타임라인 계산에 프로젝트 일정을 사용합니다.
* 작업에 할당된 사용자에게 일정이 없거나 작업이 작업 역할, 팀에만 할당되거나 할당이 해제되고 프로젝트에 일정이 없는 경우 [!DNL Workfront] 에서는 타임라인 계산을 위해 기본 일정으로 지정된 시스템의 일정을 사용합니다.

  ![](assets/default-schedule.png)

## 에서 공동 작업 [!DNL Workfront] 시간대 간

사용자가에서 공동 작업을 지원하는 데 일정을 사용하는 방법에 대한 자세한 정보 [!DNL Workfront] 시간대에서 다음을 참조하십시오. [시간대 간 작업](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
