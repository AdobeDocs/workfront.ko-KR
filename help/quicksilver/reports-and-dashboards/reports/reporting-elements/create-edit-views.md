---
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront에서 보기 만들기 또는 편집
description: 보기를 사용하여 화면에 표시할 정보 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서 여러 유형의 보기를 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 4%

---

# Adobe Workfront에서 보기 만들기 또는 편집

<!-- Audited: 11/2024 -->

보기를 사용하여 화면에 표시할 정보 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서 여러 유형의 보기를 사용할 수 있습니다.

이 문서에서는 목록 및 보고서에 대한 표준 보기를 만들고 편집하는 방법에 대해 설명합니다.

자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</strong></td> 
   <td> 
    <p>기여자 이상</p>
    <p>요청 이상</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 만들기</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에서 보기를 만들거나 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 편집 권한 관리</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 보기 만들기 또는 사용자 지정

뷰를 만들거나 사용자 정의하는 프로세스는 표준 뷰, 애자일 뷰 또는 보드 뷰를 만들거나 사용자 정의하는지에 따라 다릅니다.

* [표준 보기 만들기 또는 사용자 지정](#create-or-customize-a-standard-view)
* [애자일 보기 만들기 또는 사용자 지정](#create-or-customize-an-agile-view)

### 표준 보기 만들기 또는 사용자 지정 {#create-or-customize-a-standard-view}

새 표준 뷰를 생성하거나 이전에 생성한 기존 표준 뷰를 사용자 정의할 수 있습니다.

1. 보기를 만들거나 사용자 지정할 목록에서 **보기** 드롭다운 메뉴를 클릭합니다.

1. 새 보기를 만들려면 **+ 새 보기** 단추를 클릭하십시오.
또는
편집할 기존 보기의 오른쪽 마우스에 표시되는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
**보기 사용자 지정** 대화 상자가 표시됩니다.

1. **열 미리 보기** 섹션에서 다음 중 하나를 수행합니다.

   * 열 제목을 클릭한 다음 새 필드를 선택하여 열의 값을 수정합니다.
   * **열 추가**&#x200B;를 클릭하여 열을 추가하고 추가할 열의 이름을 입력한 다음 드롭다운 목록에 나타나면 해당 열을 클릭합니다.
   * 열 제목을 새 위치로 끌어 열 표시 순서를 조정합니다.

   * **열 설정** 영역에서 **이 열을 다음 기준으로 요약**&#x200B;을 클릭하고 열에 데이터를 표시할 방법을 선택하십시오. 이 옵션은 다음 열 유형에 사용할 수 있습니다.
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>날짜 필드</strong></td> 
           <td><ul>
           <li>최대</li>
         <li>최소</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>통화 필드</strong></td> 
           <td><ul>
           <li>계수</li>
         <li>Sum</li>
           <li>평균</li>
         <li>최대</li>
           <li>최소</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>문자열 및 부울 필드</strong></td> 
           <td><ul><li>계수</li></ul>
           <p>참고: 값이 항상 true/false이므로 Workfront에서는 일반적으로 개수별로 부울 필드를 요약하지 않는 것이 좋습니다.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >다음 필드 값을 그룹화할 때 상위 객체(예: 상위 작업)에 다음 예외가 적용됩니다.
     >   
     > * 실제 시간(예: 계획/실제 인건비, 계획/실제 경비, 계획/실제 원가, 계획 시간)을 제외한 모든 숫자 및 통화 필드는 하위 태스크 및 독립형 태스크에 대한 값만 요약합니다. 부모의 과제나 부모의 부모에 대한 가치를 요약하지 않는다.
     > * 실제 시간은 기본 상위 작업과 독립형 작업에 대한 값을 요약합니다. 상위 작업 또는 1차 하위 구성요소 작업의 상위 작업에는 숫자를 요약하지 않습니다.
     > * 숫자 및 통화 값에 대한 사용자 정의 데이터 필드는 상위, 1차 하위 구성요소, 상위 및 독립 실행형 작업과 같은 모든 작업을 요약합니다.
     >
     >보고서에서 그룹화를 사용하는 방법에 대한 자세한 내용은 문서 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.

      * (선택 사항) 열에 대해 다음 정보를 지정하려면 **고급 옵션**&#x200B;을 클릭합니다.

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>사용자 정의 열 레이블</strong></td> 
           <td><p>열에 대한 사용자 지정 레이블을 지정합니다. 이 레이블은 기본 레이블을 대체합니다. 호환성 문제를 방지하려면 UTF-8 문자만 사용하는 것이 좋습니다.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>필드 형식</strong></td> 
           <td>열의 필드에 값을 표시할 형식을 선택합니다.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>대시보드에 있을 때 이 열 표시</strong></td> 
           <td><p>보고서가 다른 보고서와 나란히 표시되는 경우 대시보드에 이 열을 표시하려면 이 옵션을 선택합니다. 이 옵션을 선택하지 않으면 보고서가 나란히 표시되는 대시보드에서 보고서를 볼 때 이 열이 표시되지 않습니다.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>열 규칙</strong></td> 
           <td><p><strong>+ 이 열에 대한 규칙 추가</strong>를 클릭하여 열에 대한 규칙을 정의합니다. 규칙을 추가한 후 해당 규칙과 일치하는 필드가 표시되는 방식에 대한 필드 및 텍스트 스타일을 정의할 수 있습니다. 규칙 정의를 마치면 <strong>규칙 추가</strong>를 클릭합니다.</p></td> 
          </tr> 
         </tbody> 
        </table>

        보고서의 조건부 서식 보기에 대한 자세한 내용은 문서 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)을 참조하십시오.

1. (조건부) **고급 옵션**&#x200B;을 클릭한 경우 **완료**&#x200B;를 클릭합니다.

1. 새 보기를 만들거나 현재 보기를 변경 내용으로 바꾸려면 **보기 저장**&#x200B;을 클릭하세요.\
   또는\
   **새 보기로 저장**&#x200B;을 클릭하여 변경 내용을 새 보기로 저장합니다.

   >[!TIP]
   >
   >기본 제공 Workfront 보기를 사용자 지정할 때 사용할 수 있는 옵션은 **새 보기로 저장**&#x200B;뿐입니다.

   액세스 권한에 따라 보기가 저장되는 방법이 결정됩니다. 원래 뷰를 생성한 경우 변경 사항을 저장할 수 있습니다. 그렇지 않으면 버전을 저장하라는 메시지가 표시됩니다. 보기에 대한 변경 내용은 보기가 공유된 사용자에게 영향을 줍니다.

### 애자일 보기 만들기 또는 사용자 지정 {#create-or-customize-an-agile-view}

보드 보기 라고도 하는 애자일 보기는 프로젝트의 작업 및 문제 목록에 대해서만 표시됩니다.

사전 구성되어 있지만 특정 설정을 수정할 수 있습니다.

애자일 또는 게시판 보기에 대한 자세한 내용은 문서 [애자일 보기에서 프로젝트 관리](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)를 참조하십시오.

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
