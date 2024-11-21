---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 시간대 간 작업
description: ' [!DNL Adobe Workfront] 이(가) 시간대를 사용하여 오브젝트와 이메일과 같은 다른 영역의 시간을 계산하는 방법을 이해하는 것이 도움이 될 수 있습니다.'
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# 시간대 간 작업

<!-- Audited: 2/2024 -->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

[!DNL Adobe Workfront]에서 시간대를 사용하여 다음을 계산하는 방법을 이해하는 것이 도움이 될 수 있습니다.

* 오브젝트의 시간 필드
* 자동화된 Workfront 이메일과 같은 다른 [!DNL Workfront] 영역의 시간

>[!WARNING]
>
>제공되는 목록에서 정확한 시간대를 찾을 수 없는 경우 가장 가까운 시간대를 찾아 인스턴스에 대해 업데이트합니다.
>
>또한 유사한 시간대가 사용자의 시간대와 완벽하게 일치하지 않을 수 있다는 점을 고려하십시오.
>
>예를 들어, 일부 국가나 지역에서는 일광 절약 시간제를 준수할 수 있지만, 해당 국가에서는 그렇지 않을 수 있습니다. 필요한 경우 이러한 변경 사항에 따라 시스템의 시간대를 조정해야 할 수 있습니다.


## [!DNL Workfront]의 시간대

[!DNL Workfront]에 표시되는 시간은 조직의 [!DNL Workfront] 인스턴스 및 사용자 프로필에 대한 표준 시간대 구성을 기반으로 합니다. 이 두 시간대가 서로 다르면 [!DNL Workfront]에서 사용하는 다른 영역 및 기능에서 시간 불일치가 표시될 수 있습니다.

>[!NOTE]
>
>오브젝트에 첨부된 사용자 정의 양식에서 계산된 사용자 정의 필드의 날짜 및 시간 문은 조직의 인스턴스 및 사용자 프로필에 대해 설정된 시간대 구성이 아니라 UTC(협정 세계시)에 의해 계산되고 저장됩니다. 사용자 정의 양식의 계산은 각 사용자의 개별 시간대를 기반으로 하여 생성되고 표시됩니다.

* [조직의  [!DNL Workfront] 인스턴스](#your-organization-s-workfront-instance)
* [사용자 프로필](#your-user-profile)

### 조직의 [!DNL Workfront] 인스턴스 {#your-organization-s-workfront-instance}

조직의 [!DNL Workfront] 인스턴스에 대한 시간대는 일반적으로 본사의 위치에 대해 설정됩니다. 이에 따라 다음이 결정됩니다.

* [!DNL Workfront]이(가) 생성한 전자 메일에 표시된 시간
* 새로 추가된 사용자의 시간대([!DNL Workfront] 관리자가 작업 위치에 따라 다른 시간대를 구성하기 전)

  이 두 예제에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.

* 프로젝트에 대한 재정의된 청구 요금의 시작 또는 끝. 자세한 내용은 [프로젝트 수준에서 작업 역할 청구 요금 재정의](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)를 참조하십시오.

### 사용자 프로필 {#your-user-profile}

사용자 프로필의 시간대는 사용자가 근무하는 위치에 맞게 구성해야 합니다. 이에 따라 다음이 결정됩니다.

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 시작 및 종료 시간 등 작업 중인 오브젝트의 시간

  여러 시간대의 사용자가 개체에 할당된 경우 [!DNL Workfront]은(는) 각 사용자 프로필에 구성된 시간대를 사용하여 관련된 모든 사용자의 개체 시간을 변환합니다.

  **예:** 작업하는 동부 표준시(EST) 영역에서 오후 4시에 시작하도록 작업을 설정하고 태평양 표준시(PST) 영역에서 작업하는 사용자에게 할당합니다. 해당 사용자의 경우 시작 시간은 오후 1시로 표시됩니다. 오후 4시로 표시하면 3시간 늦게 작업을 시작해요.

  객체 작성자가 할당자의 시간대의 차이를 인지하지 못하고 객체 시간을 설정할 때 필요한 조정을 하지 않거나 할당자가 그러한 차이를 인지하지 못하는 경우 모든 사용자가 객체를 공동 작업하는 동안 타이밍을 올바르게 설정하기 어려울 수 있습니다.

  **예:** 작업에 있는 일부 사용자가 PST 영역에서 작업하는 것을 잊고 오전 9시에 시작하도록 하루 작업을 구성합니다. 시작 시간은 오전 6시입니다. 9시(시간 정오)까지는 작업을 시작하지 않으므로 작업이 시작되고 3시간 늦게 끝납니다.

사용자 프로필에서 표준 시간대를 구성하는 방법에 대한 자세한 내용은 [내 설정 구성](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)을 참조하십시오.

[!DNL Workfront] 관리자(또는 사용자에 대해 [!UICONTROL 편집] 액세스 권한을 가진 사용자)가 사용자 프로필에서 시간대를 구성하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

## 사용자가 시간대 간에 보다 쉽게 작업할 수 있도록 하는 방법

여러 가지 방법으로 여러 시간대에서 보다 쉽게 작업할 수 있습니다.

* [일정 사용](#use-schedules)
* [사용자 정의 양식에서 계산된 시간 필드 사용](#use-calculated-time-fields-in-a-custom-form)
* [사용자 정의 양식의 날짜 필드 대신 텍스트 필드 사용](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 일정 사용 {#use-schedules}

[!DNL Workfront] 관리자는 조직 내의 각 시간대에 대해 별도의 일정을 만들어 작업이 어디에 있든 모든 사용자에게 맞게 예약되도록 합니다. 관리자가 일정을 만들면 특정 프로젝트 및 사용자와 연결할 수 있습니다.

* **[!UICONTROL 프로젝트]**: 프로젝트 작성자는 개별 프로젝트에 대한 일정을 선택할 수 있습니다. 피할당자의 시간대에 설정된 작업 시간을 기반으로 프로젝트의 작업 일정을 결정합니다.
* **[!UICONTROL 사용자]**: [!DNL Workfront] 관리자(또는 사용자에 대해 [!UICONTROL 편집] 액세스 권한이 있는 사용자)가 사용자 프로필에서 개별 사용자에 대한 일정을 선택할 수 있습니다.

  이 일정은 프로젝트 일정과 다를 수 있습니다. 예를 들어 누군가가 프로젝트에서 작업을 만들고 아직 아무도 할당하지 않은 경우 작업은 프로젝트 일정을 사용합니다. 사용자가 작업에 할당되면 작업은 해당 사용자의 일정을 사용합니다.

  작업에 여러 사용자가 할당된 경우 시스템은 시스템 또는 그룹 전체 프로젝트 환경 설정에 구성된 대로 다음 중 하나를 사용합니다.

   * 작업 기본 소유자의 일정에 대한 시간대
   * 프로젝트 일정에 대한 시간대입니다.

  <div class="preview">

  한 명의 사용자가 작업에 할당되면 시스템은 시스템 또는 그룹 전체 프로젝트 환경 설정에 구성된 대로 다음 중 하나를 사용합니다.

   * 작업 할당자의 일정에 대한 시간대
   * 프로젝트 일정에 대한 시간대입니다.

  </div>

  이로 인해 작업 날짜가 변경될 수 있습니다.

>[!BEGINSHADEBOX]

**예:**
EST 사용자는 EST 정오 시간인 오전 9시(PST)에 시작하기로 예정된 1일 작업에 할당됩니다. EST 사용자는 당일 근무시간이 2시간만 남아 있으므로 임무 완료 일자는 다음 근무일까지 약 6시간 연장됩니다.


>[!ENDSHADEBOX]

[!UICONTROL 설정]의 [!UICONTROL 프로젝트 환경 설정] 영역에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

프로젝트 또는 사용자에게 일정을 할당하는 방법에 대한 지침은 [일정 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

일정에 구성된 시간대가 [!UICONTROL 업무 균형자]에서 [!UICONTROL 계획된 시간]의 분포에 미치는 영향에 대한 자세한 내용은 [업무 균형자에서 [!UICONTROL 사용자 할당 관리]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.


### 사용자 정의 양식에서 계산된 시간 필드 사용 {#use-calculated-time-fields-in-a-custom-form}

여러 도시의 시간을 표시하는 공항 시계 행과 같이, 사용자 정의 양식에서 일련의 계산된 사용자 정의 필드를 사용하여 조직의 사용자에 대한 현재 시간을 표시할 수 있습니다. 사용자가 근무하는 각 시간대에 대해 시간대의 시간을 계산하는 필드를 만들 수 있습니다.

자세한 내용은 [계산된 데이터 표현식 개요](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md) 문서의 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [날짜 및 시간 계산된 사용자 정의 필드](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 섹션을 참조하십시오.

### 사용자 정의 양식의 날짜 필드 대신 텍스트 필드 사용 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

다른 시간대의 사용자를 위해 개체에서 구성한 시간을 [!DNL Workfront]에서 변환하지 않도록 하려면 날짜 필드 대신 개체에 첨부하는 사용자 지정 양식의 텍스트 필드를 사용할 수 있습니다. 이렇게 하면 프로젝트의 모든 사용자에 대해 입력한 시간이 시간에 표시됩니다.

이 작업을 수행하는 경우 작업의 시작 및 종료 시점을 사용자가 결정할 수 있도록 양식의 사용자에게 표준 시간대와 사용자의 시간대의 차이를 계산하도록 알리는 것이 좋습니다. 사용자 정의 양식에 입력하는 지침이나 해당 필드의 도구 설명에 이를 포함할 수 있습니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
