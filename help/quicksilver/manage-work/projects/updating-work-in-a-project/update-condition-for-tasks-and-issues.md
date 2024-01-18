---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 및 문제에 대한 상태 업데이트
description: 작업 또는 문제의 상태는 작업 또는 문제의 진행 상황을 나타내는 플래그입니다. 이는 항목의 현재 개발 단계를 나타내는 작업 항목의 상태와 다릅니다.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# 작업 및 문제에 대한 상태 업데이트

작업 또는 문제의 상태는 작업 또는 문제의 진행 상황을 나타내는 플래그입니다. 이는 항목의 현재 개발 단계를 나타내는 작업 항목의 상태와 다릅니다.

작업 또는 문제의 상태를 자동 또는 수동으로 설정할 수 있습니다.

Adobe Workfront 관리자는에 설명된 대로 환경에 대한 사용자 지정 조건을 만들 수 있습니다. [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## 액세스 요구 사항 {#access-requirements}

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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

새 라이센스의 경우:
<ul><li><p>작업 표준</p></li>
   <li><p>문제에 대한 기여자 이상</p></li></ul>


현재 라이센스의 경우:
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
   <p>작업 및 문제에 대한 권한을 관리하여 조건 업데이트</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 작업 및 문제의 상태 찾기

조건이 작업 또는 문제와 관련된 플래그로 표시됩니다. 레이블 대신 보고서에 표시할 수 있는 숫자와 연결할 수도 있습니다. 조건을 숫자와 연관시키는 방법에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

다음 영역에서 작업 및 문제의 상태를 찾을 수 있습니다.

* 작업 및 문제 업데이트 영역(업데이트 내부)으로, 작업 또는 문제에 할당되었을 때 새 댓글 달기 환경에서는 지원되지 않습니다. 자세한 내용은 [새 댓글 달기 환경](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
* 보기 또는 그룹화에 조건 필드를 표시할 때의 보고서 및 목록입니다.

>[!NOTE]
>
>분개 입력 보고서의 필드 이름 필드에 &quot;조건&quot;이라는 단어가 표시되면 항목의 조건이 갱신되었음을 나타냅니다. 분개 입력 보고서에서 조건 필드를 추적할 때, 신규 및 이전 번호 값에는 해당 이름 대신 조건과 연관된 번호가 표시됩니다. 원래 작업 또는 문제에 대해 조건이 정의되지 않은 경우 나중에 업데이트하면, 업데이트를 캡처하는 저널 항목에 조건 필드의 이전 숫자 값이 -2,147,483,648로 표시됩니다.

## 상태를 업데이트하여 상태 자동 업데이트

작업 또는 문제가 할당되고 **처리 중** , 작업 또는 문제 시작 또는 상태 업데이트. 작업 또는 문제의 상태가 과 연결된 기본 상태로 자동 변경됩니다. **매끄럽게 진행 중**.

사용자 지정 조건을 기본 조건으로 사용하는 방법에 대한 자세한 내용은 문서 를 참조하십시오  [작업 및 문제에 대한 기본값으로 사용자 지정 조건 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) 및 [사용자 지정 조건을 프로젝트의 기본값으로 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

작업 상태 변경에 대한 자세한 내용은 [작업 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

문제 상태 변경에 대한 자세한 내용은 [문제 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

처리 중(Work On It) 단추를 작업 시작 또는 문제 시작 단추로 설정하는 방법에 대한 자세한 내용은 [처리 중 단추를 시작 단추로 바꾸기](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## 수동으로 조건 업데이트

상태를 설정하려면 작업 또는 문제에 할당되거나 작업 또는 문제에 대한 관리 권한이 있어야 합니다.

보기에 조건 필드를 표시할 때 작업 또는 문제 보고서 또는 목록에서 작업 또는 문제의 조건을 수동으로 업데이트할 수 있습니다.


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

작업 또는 문제의 상태를 수동으로 갱신하려면

1. 관리 권한이 있는 작업 또는 문제 목록으로 이동합니다. 다음을 확인합니다. **조건** 필드는 목록의 보기에 표시됩니다.

1. 업데이트 **조건** 기존 조건을 두 번 클릭하고 드롭다운 메뉴에서 새 값을 선택하여 문제 또는 작업 인라인입니다.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >사용자 환경에 맞게 조건을 사용자 정의할 수 있으므로 사용자 환경에서 조건에 대한 세 가지 이상의 옵션을 찾을 수 있습니다. 조건의 이름은 위에 나열된 조건과 다를 수 있습니다. Workfront에서 조건 사용자 지정에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. 누르기 **입력** 키보드에서 을(를) 클릭하거나 조건 필드 외부를 클릭하여 새 작업 또는 문제 조건을 저장합니다.

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
