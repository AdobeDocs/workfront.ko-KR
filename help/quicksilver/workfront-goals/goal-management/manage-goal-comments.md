---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 주석 관리
description: Adobe Workfront 목표에서 볼 수 있는 모든 목표에 주석을 추가할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 0d53b8651da3602e6f3233597680eede55f847a1
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표 주석 관리

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 환경에서만 사용할 수 있습니다.</span>

Adobe Workfront 목표에서 볼 수 있는 모든 목표에 주석을 추가할 수 있습니다.

<!--drafted for P&P:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 목표에 대한 추가 라이센스를 구매해야 합니다. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>목표에 대한 액세스 권한 보기 이상</p> <p><b>메모</b><p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 보기 이상</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 업데이트 섹션을 찾습니다

목표 페이지의 업데이트 섹션에서 목표에 주석을 추가할 수 있습니다.

사용자 또는 다른 사용자가 이 영역에 추가한 댓글에 답글을 달거나 좋아할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리에서
그러면 목표 목록이 열립니다.
1. 주석을 추가할 목표를 찾은 다음 해당 이름을 클릭하여 목표 페이지를 엽니다.
1. 클릭  **업데이트** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **댓글** 업데이트 영역의 왼쪽 위 모서리에 있는 탭입니다.
1. 에 댓글 입력 시작 **새 댓글** 상자.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Updates 섹션을 벗어나서 의견 입력을 완료하고 댓글을 제출하면 로그오프한 후 다시 로그온해도 초안 모드로 페이지의 주석이 유지됩니다. 초안 주석은 입력하는 사용자만 볼 수 있습니다.

1. (선택 사항)에서 **사람 또는 팀에 태그 지정** 영역에서 이 댓글에 포함할 사용자 또는 팀의 이름 또는 전자 메일을 입력한 다음 목록에 표시될 때 선택합니다.
1. <span class="preview">(선택 사항) 주석을 편집하려면 **자세히** 메뉴 ![](assets/more-icon.png) 좋아요 아이콘 오른쪽에 있는 를 클릭한 다음 **편집**. </span>
1. <span class="preview">주석에서 정보를 편집하거나 태그가 지정된 사용자를 모두 제거합니다. </span>

   <span class="preview">댓글을 제출한 후 15분 이내에 편집을 수행할 수 있습니다. 설명이 업데이트될 때 표시되는 날짜 스탬프 왼쪽에 &quot;편집됨&quot; 표시기가 추가됩니다.</span>

   <span class="preview">![](assets/edited-tag-on-comment-unified-commenting.png)</span>

   >[!TIP]
   >
   >   <span class="preview">원본 업데이트를 제출할 때만 사용자에게 업데이트를 알리는 이메일이 생성됩니다. 업데이트를 편집한 후에는 이메일이 생성되지 않습니다.</span>

1. 클릭 **제출**.

   <!--drafted for 23.2 beta release: 
      >[!TIP]
      >
      >   <span class="preview">If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. </span>
      >
      ><span class="preview">The "New" indicator displays only when both the user that entered a new update as well as the user who is currently entering an update are using the new commenting experience.</span>
      >
      >![](assets/real-time-new-red-indicator-unified-commenting.png)-->

1. (선택 사항) **회신** 기존 주석에 응답하려면 위의 5~9단계를 수행합니다. <!--insure this stays accurate-->
1. (선택 사항) **좋아요** 아이콘![](assets/like-icon.png) 다른 사람이 추가한 설명을 좋아합니다. 아이콘이 좋아요 수로 업데이트됩니다.
1. (선택 사항) 업데이트에 리치 텍스트 서식을 추가하려면 입력할 때 리치 텍스트 도구 모음의 모든 속성을 사용합니다. 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (선택 사항) **시스템 활동** 탭에서 시스템에서 로그된 업데이트를 볼 수 있습니다. 목표가 업데이트되면 Workfront에서는 해당 업데이트에 대한 메모를 생성하여 시스템 활동 탭에 표시합니다. 또한 Workfront은 결과, 활동 또는 프로젝트가 목표에 추가되거나 업데이트될 때 시스템 업데이트를 기록합니다. <!--ensure the casing on the tab has not changed-->

<!--BELOW IS OLD, ATIIM/ WORKFRONT GOALS INFORMATION ABOUT COMMENTS: 

## Add comments to goals in the Check-in section

<div class="preview">

The Check-in section has been removed from the Preview environment. You can update goals by accessing the goal page. For information, see 
[Update goals in the Goal details section in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md). 


</div>

>[!TIP]
>
>You must have access to Edit Goals in your access level to view the Check-in section.

You can add comments to goals in the Check-in section of Workfront Goals, as part of updating your list of goals. For information about updating goals, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

You can also like goal comments that other users have added to mark your approval of them in the Check-in section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   ( Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))

   This opens the Workfront Goals area. 

1. Click the **Check-in** section in the left panel.

   ![](assets/check-in-icon-left.png)

   Goals assigned to you or that have results and activities that are assigned to you display in this area. 

1. (Optional) Click the right-pointing arrow to the left of the goal name to expand the goal, if the goal is not already expanded. 
1. Type your comment in the **Add a comment to this goal (optional)** field, then click **Post**.

   Two most recent comments display by default under each goal.

1. Click **Show all comments** to display all comments on a goal. A number of total comments for the goal also displays. Comments display in the order they were entered, with the most recent first. 
1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

## Add comments to goals in the Pulse section


<div class="preview">

The Pulse section has been removed from the Preview environment. You can update goals by accessing the goal page. For information, see 
[Update goals in the Goal details section in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md). 

</div>

You can add comments to goals in the Pulse section of Workfront Goals, as part of reviewing goals that might affect yours. For information about reviewing goals in the Pulse section, see [Review goals in the Adobe Workfront Goals Pulse section](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goals-in-pulse.md).

You can also like goal comments that other users have added to mark your approval of them in the Pulse section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))

   This opens the Workfront Goals area. 

1. Click the Pulse section in the left panel.

   ![](assets/pulse-icon-left.png)

   All current goals display in this section, regardless of their status.

1. Click **Add a comment**, then type your comment in the **Add a comment to this goal (optional)** field.
1. Click **Post**.

   Three comments display by default under each goal.

1. Click **Show all updates** to display all comments on a goal. A number of total comments for the goal also displays. Comments display in the order they were entered, with the most recent first. 
1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

-->

<!--
Locating goal comments differs depending on what environment you use. 

### Locate goal comments in the Production environment

You can add comments to goals in the following areas of Workfront Goals:

* The Goal Details panel
* The Check-in section 
* The Pulse section

Although the process for adding comments to goals is similar in these areas, there are differences in being able to edit, delete, or react to a comment when using one area versus another. When you enter a comment in any of these areas, the comment is visible in all areas where goal comments display.

>[!NOTE]
>
>You cannot add comments to results and activities.

-->

<!--
## Add comments to goals in the Goal Details panel

Adding comments to goals differs depending on what environment you use.

### Add comments to goals in the Production environment


You can add comments to goals in the Goal Details panel, as part of updating an individual goal.

You can edit or delete a comment that you entered in this area, or you can like comments.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner))
   

   This opens the Workfront Goals area. 

1. Locate the goal you want to add comments to, then click its name to open the Goal Details panel to the right. 
1. Click the **Updates** tab.
1. Type your comment in the **Comment here** field, then click **Post**. 
1. (Optional and conditional) Select the **Comments** option at the top of the list to view your comment at the top of the list. It is enabled by default and comments display here with the most recent comment first. 
1. (Optional) Click **Edit** to edit your comment, then click **Save** to save your changes, or **Cancel** to revert to the original update.

   >[!TIP]
   >
   >* You can only edit comments you entered. 
   >* There is no time limit for how long after you enter a comment you are allowed to edit it.

1. (Optional) Click **Delete** to delete your comment, then click **Yes, Delete** to confirm.

   >[!TIP]
   >
   >* You can only delete comments you entered. 
   >* There is no time limit for how long after you enter a comment you are allowed to delete it.

1. (Optional) Click the **Like icon** ![](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes. 

1. (Optional) Click the number of likes next to a comment and a list with the names of the users who liked the comment displays in the right panel.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this functionality might change)</p>
   

   ![](assets/list-of-likes-users-350x121.png)

1. (Conditional) Click **Back to Updates** to return to the Updates tab of the Goal Details panel, or click the **X icon** in the upper-right corner to close the right panel.

-->