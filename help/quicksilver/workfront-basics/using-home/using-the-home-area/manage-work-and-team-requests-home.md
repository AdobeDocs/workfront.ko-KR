---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 홈 영역에서 작업 및 팀 요청 관리
description: 작업 작업 및 문제가 할당되면 내 작업 위젯, 내 작업 위젯 및 내 문제 위젯에 나열됩니다.  작업 항목 및 요청을 보거나, 작업하거나, 제거할 수 있습니다.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---


# [!UICONTROL Home] 영역에서 작업 항목 및 팀 요청 관리

작업 작업 및 문제가 할당되면 내 작업 위젯, 내 작업 위젯 및 내 문제 위젯에 나열됩니다.  작업 항목 및 요청을 보거나, 작업하거나, 제거할 수 있습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td>
   <p>표준</p>
    <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 권한 이상 부여</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 내 작업 위젯에서 작업 항목 보기

내게 할당된 작업 항목이 [!UICONTROL Home]의 내 작업 위젯에 표시됩니다. [!UICONTROL 작업 목록] 위젯의 맨 위에 있는 필터를 사용하여 내 작업 위젯에 표시되는 작업 항목을 구성할 수 있습니다.

작업할 준비가 된 항목 또는 현재 이미 작업 중인 항목을 표시하는 필터를 선택할 수 있습니다.

이 문서에서는 [!UICONTROL Home] 영역의 필터를 사용하여 현재 작업 중이거나 작업을 시작할 것으로 예상되는 항목을 보는 방법에 대해 설명합니다. [!UICONTROL Home] 영역에서 필터를 사용하는 방법에 대한 자세한 내용은 [[!UICONTROL Home] 영역에서 [!UICONTROL worklist]에 항목 표시](/help/quicksilver/workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)를 참조하십시오.

내 작업 위젯에서 작업 항목을 보려면 다음과 같이 하십시오.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 작업** 위젯을 추가합니다.

1. 위젯 작업 목록의 왼쪽 상단 모서리에 있는 **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭합니다.

1. 작업에 대해 다음 옵션 중 하나 또는 모두를 클릭합니다.

   **[!UICONTROL 시작할 준비]:** 시작할 준비가 된 작업과 문제만 표시합니다. 다음 문은 모두 true여야 합니다.

   * 과제와 그 부모에게는 작업을 할 수 없는 전임자나 과업 제한이 없다.
   * 작업 또는 문제의 [!UICONTROL 계획된 시작 일자]가 과거 또는 최대 2주 후입니다.

   **[!UICONTROL 준비 안 됨]**: 아직 시작할 준비가 되지 않은 작업 및 문제만 표시합니다. 다음 문 중 하나가 true여야 합니다.

   * 작업 및 상위 사용자에게 작업을 수행할 수 없는 선행 작업 또는 작업 제한이 있을 수 있습니다.
   * 작업 또는 문제의 [!UICONTROL 계획된 시작 일자]가 향후 2주 이상입니다.

1. **[!UICONTROL 작업]** 또는 [!UICONTROL 문제]에서 [!UICONTROL 작업 중]을 클릭하여 현재 작업 중인 작업 및 문제를 표시합니다.
1. **[!UICONTROL 문제]** 아래의 [!UICONTROL 요청됨]을(를) 클릭하여 귀하로부터 요청된 문제(귀하에게 할당된 문제)를 표시하지만 아직 작업에 동의하지 않았습니다.

## 팀 요청 위젯에서 팀 요청에 액세스

[!UICONTROL Home] 영역의 팀 요청 위젯에서 팀에 직접 할당된 요청에 액세스할 수 있습니다. 팀 요청에 대한 자세한 내용은 [팀 요청 개요](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md)를 참조하십시오.

팀 요청에 액세스하려면:

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **팀 요청** 위젯을 추가합니다.

   위젯은 팀 그룹화 아래에 팀 요청을 표시합니다. **[!UICONTROL 팀 요청]** 위젯은 사용자가 속한 모든 팀에 할당된 모든 요청을 표시하고 표시합니다. 팀 요청 작업에 대한 자세한 내용은 [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)를 참조하십시오.

   ![팀 요청 위젯](assets/team-request-widget.png)

## 내 작업 위젯의 작업 항목 작업

[!UICONTROL 작업 중] 단추를 클릭하면 작업 항목을 제출한 사용자와 작업을 시작할 작업 항목에 할당할 수 있는 다른 사용자에게 표시됩니다.

작업 항목에 대해 작업하려면

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 작업** 위젯을 추가합니다.

1. 위젯의 **[!UICONTROL 작업 목록]** 영역에서 작업할 요청을 선택한 다음 **[!UICONTROL 작업]**&#x200B;을 클릭합니다.
1. 작업 항목 위로 마우스를 가져간 다음 **요약** 아이콘을 클릭하여 작업 항목에 대한 정보를 봅니다.

   ![요약 열기](assets/open-summary-new-home.png)


## 작업 항목 제거

작업 항목을 작업하지 않기로 결정한 경우 목록에서 제거할 수 있습니다.

작업 항목을 제거하려면 다음 작업을 수행하십시오.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 작업** 위젯을 추가합니다.

1. 위젯 작업 목록에서 작업 항목을 마우스로 가리킨 다음 **요약** 아이콘을 클릭하여 작업 항목에 대한 정보를 봅니다.
   ![요약 열기](assets/open-summary-new-home.png)
1. **할당** 섹션에서 이름을 제거합니다.
   ![할당 제거](assets/remove-assignment.png)



<!--
## Reassign a request

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reassign.

1. Click on the **[!UICONTROL Assignments]** widget and remove yourself from the request, then type the name of the user you want to reassign the request to.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or Not Ready state, you can use the **[!UICONTROL Reassign]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![Reassign button](assets/reassign-in-left-panel-350x204.png)

1. If a task's status is changed to [!UICONTROL New] or [!UICONTROL In Progress] after it was completed, you must unassign the user, save the task, then reassign the user in order for the task to reappear in their Home Work List.



## Reply to a request

You can reply to a request to further clarify the request or to propose a new date.

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reply to.
1. Locate the individual who assigned the request to you.

   You can find this information on the [!UICONTROL Updates] tab of the task. Make sure the option to **[!UICONTROL Show System Updates]** is enabled.

1. Click **[!UICONTROL Start new update]** and begin typing your reply.
1. Enter the name of the recipient in the **[!UICONTROL Notify]** box, then click **[!UICONTROL Update]**.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or [!UICONTROL Not Ready] state, you can use the **[!UICONTROL Reply]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![[!UICONTROL Reply button]](assets/reassign-in-left-panel-350x204.png)   

   -->
