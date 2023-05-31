---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 시간대 간 작업
description: 방법을 이해하는 것이 도움이 될 수 있습니다 [!DNL Adobe Workfront] 시간대를 사용하여 이메일과 같은 다른 영역의 오브젝트 및 시간에 대한 시간 필드를 계산합니다.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# 시간대 간 작업

방법을 이해하는 것이 도움이 될 수 있습니다 [!DNL Adobe Workfront] 시간대를 사용하여 다음을 계산합니다.

* 오브젝트의 시간 필드
* 기타 시간 [!DNL Workfront] 영역(예: 자동화된 Workfront 이메일)

## 의 시간대 [!DNL Workfront]

다음에 표시되는 횟수 [!DNL Workfront] 조직의 시간대 구성을 기반으로 합니다. [!DNL Workfront] 인스턴스 및 사용자 프로필용. 이 두 시간대가 다르면 서로 다른 영역 및 기능에서 사용하는 기능에서 시간 불일치가 표시될 수 있습니다 [!DNL Workfront].

>[!NOTE]
>
>오브젝트에 첨부된 사용자 정의 양식에서 계산된 사용자 정의 필드의 날짜 및 시간 문은 조직의 인스턴스 및 사용자 프로필에 대해 설정된 시간대 구성이 아니라 UTC(협정 세계시)에 의해 계산되고 저장됩니다. 사용자 정의 양식의 계산은 각 사용자의 개별 시간대를 기반으로 하여 생성되고 표시됩니다.

* [조직의 [!DNL Workfront] 인스턴스](#your-organization-s-workfront-instance)
* [사용자 프로필](#your-user-profile)

### 조직의 [!DNL Workfront] 인스턴스 {#your-organization-s-workfront-instance}

조직의 시간대 [!DNL Workfront] 인스턴스는 일반적으로 본사의 위치에 대해 설정됩니다. 이에 따라 다음이 결정됩니다.

* 다음에 의해 생성된 이메일에 표시된 시간 [!DNL Workfront]
* 새로 추가된 사용자의 시간대(이전) [!DNL Workfront] 관리자는 작업 위치에 따라 시간대를 다르게 구성합니다.)

   이 두 예제에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 프로젝트에 대한 재정의된 청구 요금의 시작 또는 끝. 자세한 내용은 [프로젝트 수준에서 작업 역할 청구 요금 재정의](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### 사용자 프로필 {#your-user-profile}

사용자 프로필의 시간대는 사용자가 근무하는 위치에 맞게 구성해야 합니다. 이에 따라 다음이 결정됩니다.

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 시작 및 종료 시간 등 작업 중인 오브젝트의 시간

   여러 시간대의 사용자가 오브젝트에 할당된 경우 [!DNL Workfront] 는 각 사용자 프로필에 구성된 시간대를 사용하여 관련된 모든 사용자의 개체 시간을 변환합니다.

   **예:** 작업하는 동부 표준시(EST) 영역에서는 오후 4시에 시작하도록 작업을 설정하고 태평양 표준시(PST) 영역에서 작업하는 사용자에게 할당합니다. 해당 사용자의 경우 시작 시간은 오후 1시로 표시됩니다. 오후 4시로 표시하면 3시간 늦게 작업을 시작해요.

   객체 작성자가 할당자의 시간대의 차이를 인지하지 못하고 객체 시간을 설정할 때 필요한 조정을 하지 않거나 할당자가 그러한 차이를 인지하지 못하는 경우 모든 사용자가 객체를 공동 작업하는 동안 타이밍을 올바르게 설정하기 어려울 수 있습니다.

   **예:** 작업에 있는 일부 사용자가 PST 영역에서 작업하는 것을 잊고 EST 오전 9시에 시작하도록 1일 작업을 구성합니다. 시작 시간은 오전 6시입니다. 9시(시간 정오)까지는 작업을 시작하지 않으므로 작업이 시작되고 3시간 늦게 끝납니다.

사용자 프로필에서 표준 시간대 구성에 대한 자세한 내용은 [내 설정 구성](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

다음 방법에 대한 정보: [!DNL Workfront] 관리자(또는 [!UICONTROL 편집] 사용자에 대한 액세스 권한) 사용자 프로필에서 시간대를 구성할 수 있습니다. 다음을 참조하십시오. [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 사용자가 시간대 간에 보다 쉽게 작업할 수 있도록 하는 방법

여러 가지 방법으로 여러 시간대에서 보다 쉽게 작업할 수 있습니다.

* [일정 사용](#use-schedules)
* [사용자 정의 양식에서 계산된 시간 필드 사용](#use-calculated-time-fields-in-a-custom-form)
* [사용자 정의 양식의 날짜 필드 대신 텍스트 필드 사용](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 일정 사용 {#use-schedules}

[!DNL Workfront] 관리자는 조직 내의 각 시간대에 대해 별도의 일정을 만들어 작업이 어디에 있든 모든 사용자에게 적절하게 예약되도록 합니다. 관리자가 일정을 만들면 특정 프로젝트 및 사용자와 연결할 수 있습니다.

* **[!UICONTROL 프로젝트]**: 프로젝트 작성자는 개별 프로젝트에 대한 일정을 선택할 수 있습니다. 피할당자의 시간대에 설정된 작업 시간을 기반으로 프로젝트의 작업 일정을 결정합니다.
* **[!UICONTROL 사용자]**: A [!DNL Workfront] 관리자(또는 [!UICONTROL 편집] 사용자에 대한 액세스)는 사용자 프로필에서 개별 사용자에 대한 일정을 선택할 수 있습니다.

   이 일정은 프로젝트 일정과 다를 수 있습니다. 예를 들어 누군가가 프로젝트에서 작업을 만들고 아직 아무도 할당하지 않은 경우 작업은 프로젝트 일정을 사용합니다. 사용자가 작업에 할당되면 작업은 해당 사용자의 일정을 사용합니다.

   작업에 여러 사용자가 할당된 경우 시스템은 시스템 전체 프로젝트 환경 설정에 구성된 대로 다음 중 하나를 사용합니다.

   * 작업 기본 소유자의 일정에 대한 시간대
   * 프로젝트 일정에 대한 시간대입니다.

   이로 인해 작업 날짜가 변경될 수 있습니다.

   **예:** EST 사용자는 EST 정오 시간인 오전 9시(PST)에 시작하기로 예정된 1일 작업에 할당됩니다. EST 사용자는 당일 근무시간이 2시간만 남아 있으므로 임무 완료 일자는 다음 근무일까지 약 6시간 연장됩니다.

   에 대한 자세한 내용은 [!UICONTROL 프로젝트 환경 설정] 영역 [!UICONTROL 설정], 참조 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   프로젝트 또는 사용자에게 일정을 할당하는 방법에 대한 지침은 [일정 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   일정에 구성된 시간대가 의 분포에 미치는 영향에 대한 자세한 정보 [!UICONTROL 계획된 시간] 다음에서 [!UICONTROL 업무 균형자], 참조 [에서 사용자 할당 관리 [!UICONTROL 업무 균형자]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### 사용자 정의 양식에서 계산된 시간 필드 사용 {#use-calculated-time-fields-in-a-custom-form}

여러 도시의 시간을 표시하는 공항 시계 행과 같이, 사용자 정의 양식에서 일련의 계산된 사용자 정의 필드를 사용하여 조직의 사용자에 대한 현재 시간을 표시할 수 있습니다. 사용자가 근무하는 각 시간대에 대해 시간대의 시간을 계산하는 필드를 만들 수 있습니다.

자세한 내용은 [사용자 정의 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), 섹션 [계산된 날짜 및 시간 사용자 정의 필드](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 이 문서에서 [계산된 데이터 표현식](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### 사용자 정의 양식의 날짜 필드 대신 텍스트 필드 사용 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

원치 않으시면 [!DNL Workfront] 시간대가 다른 사용자용으로 개체에서 를 구성하는 시간을 변환하려면 날짜 필드 대신 개체에 첨부하는 사용자 정의 양식의 텍스트 필드를 사용할 수 있습니다. 이렇게 하면 프로젝트의 모든 사용자에 대해 입력한 시간이 시간에 표시됩니다.

이 작업을 수행하는 경우 작업의 시작 및 종료 시점을 사용자가 결정할 수 있도록 양식의 사용자에게 표준 시간대와 사용자의 시간대의 차이를 계산하도록 알리는 것이 좋습니다. 사용자 정의 양식에 입력하는 지침이나 해당 필드의 도구 설명에 이를 포함할 수 있습니다. 자세한 내용은 [사용자 정의 양식에 사용자 정의 필드 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
