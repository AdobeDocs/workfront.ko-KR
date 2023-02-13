---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 복사
description: Adobe Workfront 목표에서 목표를 복사하여 목표를 만들 수 있습니다. 원래 목표 정보 중 일부는 새 목표에 전달됩니다.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표 복사

Adobe Workfront 목표에서 목표를 복사하여 목표를 만들 수 있습니다. 원래 목표 정보 중 일부는 새 목표에 전달됩니다.

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
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b>

<p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
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

## 목표 복사를 위한 고려 사항

목표를 복사하려면 액세스 수준에서 목표 편집에 액세스할 수 있어야 합니다. 목표에 대한 액세스 권한 부여에 대한 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

기존 목표를 복사하려는 몇 가지 이유는 다음과 같습니다.

* 기간(분기 또는 연도)이 끝날 때 다음 기간 동안 동일한 목표를 다시 만들려는 경우
* 목표를 완수할 수 없는 기간이 끝나고 다른 기간 동안 작업을 수행하려는 경우
* 여러 팀 구성원이 유사한 목표를 가지고 있고 각 팀 구성원에 대해 하나씩 만들어야 하는 경우

>[!TIP]
>
>어떤 상태로든 목표를 복사할 수 있습니다. 목표 상태에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 상태 개요](../../workfront-goals/goal-management/goal-status-overview.md).

목표를 복사할 때에는 다음 사항을 고려하십시오.

* 목표에 대한 모든 정보도 새 목표에 복사됩니다.
* 기존 목표 결과를 복사하도록 선택할 수 있습니다. 결과 이름은 새 목표에 전송되지만, 기존 목표에 대한 결과의 현재 진행 상태는 새 목표에 복사되지 않습니다. 복사된 결과는 기본적으로 동일한 소유자에게 지정됩니다.

   >[!NOTE]
   >
   >Workfront에서 원래 소유자가 삭제되거나 비활성화된 경우 로그인한 사용자에게 새 결과가 할당됩니다.

* 목표를 복사할 때에는 목표 활동을 복사할 수 없습니다.

## 목표 복사

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
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
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. 목표로 이동하고 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **목표 복사**.

   ![](assets/copy-goal-box-unshimmed.png)

1. 복사된 목표에 대해 다음 정보를 업데이트합니다.
   * **목표 이름**: 새 목표의 이름입니다. 복사된 목표의 기본 이름은 &quot;복사본 &lt;original goal=&quot;&quot;>&quot;.
   * **기간**: 목표를 달성하고자 하는 기간입니다. 드롭다운 메뉴에서 기간을 선택합니다

      또는

      선택 **사용자 지정 날짜 활성화** 목표의 사용자 지정 날짜를 지정하려면 **시작** 및 **종료 날짜**. 사용자 지정 날짜 활성화 설정은 기본적으로 비활성화됩니다.

      >[!TIP]
      >
      >   사용자 지정 날짜 사용 을 선택 취소하면 원래 목표의 기간으로 되돌아갑니다.

      * **목표 소유자**: 목표 소유자. 사용자, 팀, 그룹 또는 회사일 수 있습니다. 기본값은 원래 목표의 소유자입니다.
      * **설명**: 목표에 대한 추가 정보입니다.
      * **결과 복사**: 현재 목표의 결과를 복사된 목표로 전송하려면 이 옵션을 선택합니다. 이렇게 하면 원래 결과가 복제되고 복사된 목표에 첨부됩니다. 복사된 목표의 결과에는 원래 목표의 결과와 동일한 소유자, 이름 및 측정값이 있습니다.

         >[!NOTE]
         >
         >* 원본 결과의 진행 상태는 복사된 목표에 전송되지 않습니다.
         >* Workfront에서 원래 소유자가 삭제되거나 비활성화된 경우 로그인한 사용자에게 새 결과가 할당됩니다.


1. 클릭 **목표 복사**.

   원래 목표와 유사한 목표가 생성되며 초안 상태입니다.

   >[!NOTE]
   >
   >원래 목표의 결과를 복사하지 않은 경우, 새 목표를 활성화하고 이를 달성하기 위한 작업을 시작하기 전에 먼저 진행 표시기와 새 목표를 연결해야 합니다.
   >목표를 진행률 표시기와 연결하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.
   >* [Adobe Workfront 목표에 결과 추가](../results-and-activities/add-results-to-goals.md)
   >* [Adobe Workfront 목표의 목표에 활동 추가](../results-and-activities/add-activities-to-goals.md)
   >* [Adobe Workfront 목표에 연결하여 목표 정렬](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >목표 활성화에 대한 자세한 내용은 [목표 활성화](../goal-management/activate-goals.md).

