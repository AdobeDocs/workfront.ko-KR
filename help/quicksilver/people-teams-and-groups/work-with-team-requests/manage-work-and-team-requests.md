---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 작업 및 팀 요청 관리
description: 요청은 보류 중인 작업 또는 문제 할당을 나타냅니다. 개인에게 작업 요청이 이루어지고, 팀에게 팀 요청이 이루어진다.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 작업 및 팀 요청 관리

요청은 보류 중인 작업 또는 문제 할당을 나타냅니다. 개인에게 작업 요청이 이루어지고, 팀에게 팀 요청이 이루어진다.

>[!NOTE]
>
>애자일 팀에는 팀 요청이 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>검토 이상을 통해 요청을 할당하거나 작업하고, 작업 이상을 통해 요청을 재할당합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 팀에 요청 할당 {#assign-a-request-to-a-team}

프로젝트 관리자 및 문제 요청자는 누가 작업을 수행해야 하는지 알 수 없거나 누가 작업을 완료해도 상관없는 경우 팀에 작업을 할당할 수 있습니다.

팀에 할당된 작업은 팀의 사용자가 요청에 대해 작업할 때까지 [!UICONTROL 팀 요청] 탭에 남아 있습니다.

요청이 팀과 팀의 구성원이 아닌 사용자 모두에 할당되면 [!UICONTROL 팀 요청] 탭과 사용자의 작업 요청 영역에 모두 표시됩니다. 팀에 없는 사용자가 작업에 자원하면 팀의 사용자가 자원하여 작업을 수행할 때까지 작업은 [!UICONTROL 팀 요청] 탭에 남아 있습니다.

다음 방법 중 하나로 작업 및 문제에 팀을 할당할 수 있습니다.

* [!UICONTROL 간트 차트]를 통해
* 작업 또는 문제 목록에서(개별적으로 또는 일괄적으로)
* 작업 또는 문제를 만들거나 수정할 때
* 요청에 대한 라우팅 규칙을 통해(문제만)

이 섹션에 설명된 대로 팀 페이지에서 팀에 요청을 수동으로 할당할 수 있습니다.

팀 페이지에서 팀에 요청을 수동으로 할당하려면 다음을 수행합니다.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png)을 클릭한 다음 **[!UICONTROL 작업 요청 보내기]**&#x200B;를 선택합니다.

   ![](assets/edit-team-settings-350x205.png)

1. 열려 있는 상자에 정보를 입력합니다.
1. **[!UICONTROL 요청 보내기]**&#x200B;를 클릭합니다.\
   이제 팀에게 팀 요청 탭에 표시되는 새 작업이 할당됩니다. 이 작업은 현재 프로젝트와 연결되어 있지 않지만 [작업 이동](../../manage-work/tasks/manage-tasks/move-tasks.md)에 설명된 대로 이동할 수 있습니다.

## 요청 재할당 {#reassign-requests}

팀에 할당된 요청을 재할당할 수 있습니다.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL 팀 요청]**&#x200B;을 선택합니다.
1. **[!UICONTROL 다시 할당]** 아이콘을 클릭합니다.

1. 요청을 재할당할 사용자, 그룹 또는 팀의 이름을 입력한 다음 **[!UICONTROL 할당]**&#x200B;을 클릭합니다.\
   요청이 다시 할당되었습니다.
