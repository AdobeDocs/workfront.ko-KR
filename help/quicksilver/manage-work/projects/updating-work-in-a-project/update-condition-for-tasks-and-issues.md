---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 및 문제에 대한 상태 업데이트
description: 작업 또는 문제의 상태는 작업 또는 문제의 진행 상황을 나타내는 플래그입니다. 이는 항목의 현재 개발 단계를 나타내는 작업 항목의 상태와 다릅니다.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# 작업 및 문제에 대한 상태 업데이트

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

작업 또는 문제의 상태는 작업 또는 문제의 진행 상황을 나타내는 플래그입니다. 이는 항목의 현재 개발 단계를 나타내는 작업 항목의 상태와 다릅니다.

작업 또는 문제의 상태를 자동 또는 수동으로 설정할 수 있습니다.

이 문서에서 참조하는 조건 값은 기본적으로 Workfront에서 사용할 수 있습니다. [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)에 설명된 대로 Adobe Workfront 관리자가 환경에 대한 사용자 지정 조건을 만들 수 있습니다.

## 액세스 요구 사항 {#access-requirements}

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
   신규:
   <ul><li><p>작업 표준</p></li>
   <li><p>문제에 대한 기여자 이상</p></li></ul>
   현재:
   <ul><li><p>작업 이상</p></li>
   <li><p>문제에 대한 요청 이상</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>작업 및 문제에 대한 액세스 편집 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 대한 또는 그 이상의 권한을 보고 해당 조건 보기</p>
   <p>조건 업데이트를 위한 작업 및 문제에 대한 Contribute 권한</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

상태를 수동으로 업데이트할 수 있는 작업 또는 문제를 할당해야 합니다.

## 작업 및 문제의 상태 찾기

조건이 작업 또는 문제와 관련된 플래그로 표시됩니다. 레이블 대신 보고서에 표시할 수 있는 숫자와 연결할 수도 있습니다. 조건을 숫자와 연결하는 방법에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)을 참조하세요.

Workfront의 다음 영역에서 작업 및 문제의 상태를 찾을 수 있습니다.

* Workfront 또는 그룹 관리자가 레이아웃 템플릿에 추가하면 세부 정보 페이지가 표시됩니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

* Workfront 또는 그룹 관리자가 작업 또는 문제를 레이아웃 템플릿에 추가한 후의 헤더. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.

* 요약 패널은 Workfront 또는 그룹 관리자가 레이아웃 템플릿에 추가하면 됩니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 요약 패널 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)을 참조하십시오.

* 보기 또는 그룹화에 조건 필드를 표시할 때의 보고서 및 목록입니다.

  >[!NOTE]
  >
  >분개 입력 보고서의 필드 이름 필드에 &quot;조건&quot;이라는 단어가 표시되면 항목의 조건이 갱신되었음을 나타냅니다. 분개 입력 보고서에서 조건 필드를 추적할 때, 신규 및 이전 번호 값에는 해당 이름 대신 조건과 연관된 번호가 표시됩니다. 원래 작업 또는 문제에 대해 조건이 정의되지 않은 경우 나중에 업데이트하면, 업데이트를 캡처하는 저널 항목에 조건 필드의 이전 숫자 값이 -2,147,483,648로 표시됩니다.

## 상태를 업데이트하여 상태 자동 업데이트

작업 또는 문제가 할당되어 **작업**, 작업 또는 문제 시작 또는 상태 업데이트를 클릭하면 작업 또는 문제의 상태가 **원활하게 진행**&#x200B;과(와) 관련된 기본 상태로 자동 변경됩니다.

사용자 지정 조건을 기본 조건으로 사용하는 방법에 대한 자세한 내용은 문서 [작업 및 문제에 대한 기본값으로 사용자 지정 조건 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) 및 [프로젝트의 기본값으로 사용자 지정 조건 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)을 참조하십시오.

작업 상태 변경에 대한 자세한 내용은 [작업 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md)를 참조하십시오.

문제 상태 변경에 대한 자세한 내용은 [문제 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md)를 참조하십시오.

[처리 중] 단추를 [작업 시작] 또는 [문제 시작] 단추로 설정하는 방법에 대한 자세한 내용은 [처리 중 단추를 [시작] 단추로 바꾸기](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)를 참조하십시오.

## 수동으로 조건 업데이트

상태를 설정하려면 작업 또는 문제에 할당되거나 작업 또는 문제에 대한 관리 권한이 있어야 합니다.

보기에 조건 필드를 표시할 때 작업 또는 문제 보고서 또는 목록에서 작업 또는 문제의 조건을 수동으로 업데이트할 수 있습니다.

>[!NOTE]
>
>시스템 또는 그룹 관리자에게 요약 패널, 작업 또는 문제 헤더 또는 세부 정보 페이지에 조건 필드를 추가하도록 요청할 수 있습니다.
>
>자세한 내용은 다음 문서를 참조하십시오.
>
>* [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [레이아웃 템플릿을 사용하여 요약 패널을 사용자 지정합니다](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Workfront의 다양한 영역에서 작업 및 문제의 상태를 수동으로 업데이트할 수 있습니다. 다음 섹션에서는 작업 및 문제의 상태를 수동으로 업데이트하는 방법에 대해 설명합니다.

### 작업 또는 문제 헤더에서 작업 또는 문제의 상태 업데이트

1. (조건부) Workfront 또는 그룹 관리자가 레이아웃 템플릿의 작업 또는 문제 헤더에 조건 필드를 추가한 경우 헤더에서 **조건** 필드를 클릭하고 다음 옵션 중에서 선택합니다.
   * 매끄럽게 진행 중
   * 일부 우려 사항
   * 주요 장애물

   ![](assets/condition-in-task-header.png)
1. Enter 를 클릭하여 조건을 저장합니다.

### 작업 또는 문제 세부 정보 섹션에서 작업 또는 문제의 상태 업데이트

1. (조건부) Workfront 또는 그룹 관리자가 레이아웃 템플릿에 있는 작업 또는 문제의 세부 정보 섹션에 조건 필드를 추가한 경우 왼쪽 패널에서 **세부 정보**&#x200B;를 클릭한 다음 **작업 조건** 또는 **문제 조건**&#x200B;을 클릭하고 다음 옵션 중에서 선택하십시오.
   * 매끄럽게 진행 중
   * 일부 우려 사항
   * 주요 장애물
1. **변경 내용 저장**&#x200B;을 클릭합니다. 작업 또는 문제의 상태가 업데이트됩니다.

### 보고서 또는 목록에서 작업 또는 문제의 상태 업데이트

1. 관리 권한이 있는 작업 또는 문제 목록으로 이동합니다. **Condition** 필드가 목록의 보기에 표시되는지 확인합니다.

1. 기존 조건을 두 번 클릭하고 드롭다운 메뉴에서 새 값을 선택하여 문제 또는 작업 인라인의 **조건**&#x200B;을(를) 업데이트합니다.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >사용자 환경에 맞게 조건을 사용자 정의할 수 있으므로 사용자 환경에서 조건에 대한 세 가지 이상의 옵션을 찾을 수 있습니다. 조건의 이름은 위에 나열된 조건과 다를 수 있습니다. Workfront에서 조건을 사용자 지정하는 방법에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)을 참조하십시오.


1. 키보드에서 **Enter**&#x200B;를 누르거나 Condition 필드 외부를 클릭하여 새 작업 또는 문제 Condition을 저장합니다.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


