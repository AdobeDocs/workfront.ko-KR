---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 목표 만들기
description: CEO, 관리자 또는 개별 기여자의 경우 Adobe Workfront 목표에 목표를 세워 조직의 전략을 요약하는 목표 및 목표에 맞게 작업을 수행할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# Adobe Workfront 목표에서 목표 만들기

CEO, 관리자 또는 개별 기여자의 경우 Adobe Workfront 목표에 목표를 세워 조직의 전략을 요약하는 목표 및 목표에 맞게 작업을 수행할 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P release: 

You must have the following:

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

다음 항목이 있어야 합니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b><p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 관리</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 목표 작성 지침

Workfront 목표를 시작하기 전에 목표 관리를 위한 우수 사례 권장 사항 및 지침을 읽어 보는 것이 좋습니다. 목표 만들기 및 관리 지침에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../workfront-goals/goal-management/wf-goals-overview.md).

## 목표 만들기

이 문서에서는 Workfront 목표에서 전략적 목표를 만드는 방법을 설명합니다. 비즈니스 사례 목표 생성에 대한 자세한 내용은 [비즈니스 사례 목표 생성](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

다음 방법 중 하나로 전략적 목표를 만들 수 있습니다.

* [처음부터 목표 만들기](#create-a-goal-from-scratch)
* [기존 목표 복사](#copy-an-existing-goal)
* [결과나 활동을 목표로 변환](#convert-a-result-or-activity-to-a-goal)

### 처음부터 목표 만들기 {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) 오른쪽 상단 모서리에서 을(를) 클릭하고 **목표**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   목표 목록이 표시됩니다.
1. 클릭 **새 목표**.

   새 목표 상자가 표시됩니다.

   ![](assets/new-goal-box-unshimmed.png)

1. 다음 필드에 정보를 입력합니다.
   * **목표 이름**: 목표명을 입력합니다. 필수 필드입니다.
   * **기간**: 에서 사전 정의된 분기 또는 연도를 선택합니다 **기간** 드롭다운 필드

      또는

      을(를) 선택합니다 **사용자 지정 날짜 활성화** 옵션을 선택한 다음 **시작** 및 **종료 날짜** 목표를 향해서.

      이전, 현재 및 다음 연도 및 해당 분기는 기간 드롭다운 필드에 사전 정의된 옵션으로 나열됩니다.

      목표 기간 은 목표가 완료될 것으로 예상되는 기간을 가리킵니다.

   * **목표 소유자**: 사용자, 팀, 그룹 또는 조직의 이름을 입력하여 목표 소유자가 누구인지를 나타냅니다. 기본적으로 목표 소유자로 선택됩니다.
   * **설명**: 목표에 대한 추가 정보를 입력합니다.
1. 클릭 **목표 만들기**.

   새 목표는 목표 목록에 나열되며 상태는 입니다 **초안**.

   목표를 활성화하고 작업을 시작하려면 목표 및 진행 표시기를 연결해야 합니다.

   활성화 목표를 준비하려면 다음 중 하나 이상을 수행하십시오.
   * 결과 추가

      결과 추가에 대한 자세한 내용은 [Adobe Workfront 목표에 결과 추가](../results-and-activities/add-results-to-goals.md).
   * 활동 추가

      활동 추가에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../results-and-activities/add-activities-to-goals.md).
   * 다른 목표를 맞추다

      목표 정렬에 대한 자세한 내용은 [Adobe Workfront 목표에 연결하여 목표 정렬](../goal-alignment/align-goals-by-connecting-them.md).


### 기존 목표 복사 {#copy-an-existing-goal}

기존 목표를 복사하여 목표를 만들 수 있습니다.

목표 복사에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 복사](../../workfront-goals/goal-management/copy-goals.md).

### 결과나 활동을 목표로 변환 {#convert-a-result-or-activity-to-a-goal}

기존 목표의 결과나 활동을 목표로 변환하여 목표를 만들 수 있습니다. 새 목표가 원래 목표에 맞춰진다.

결과 및 활동을 목표로 변환하는 방법에 대한 자세한 내용은 [결과 및 활동을 목표로 변환하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

