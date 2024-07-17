---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 칸반 보드의 스토리에 플래그 사용
description: ' [!DNL Kanban] 보드에서 플래그는 스토리가 다음 상태로 이동할 준비가 되었을 때를 시각적으로 표시합니다. 이를 통해 Kanban 팀은 상태 간에 스토리를 이동할 때 "푸시" 접근 방식이 아닌 "풀" 접근 방식을 사용할 수 있습니다.'
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# [!UICONTROL Kanban] 보드의 스토리에 플래그 사용

[!DNL Kanban] 보드에서 플래그는 스토리가 다음 상태로 이동할 준비가 된 시기를 시각적으로 표시합니다. 이를 통해 [!UICONTROL Kanban] 팀이 여러 상태에서 스토리를 이동할 때 &quot;푸시&quot; 접근 방식이 아닌 &quot;풀&quot; 접근 방식을 사용할 수 있습니다.

**예:** &quot;가져오기&quot; 방법을 사용하는 팀의 다음 예를 생각해 보십시오. 팀의 그래픽 디자이너인 Olivia는 작업을 마친 다음 스토리 플래그를 &quot;[!UICONTROL 가져올 준비]&quot;로 설정합니다. 이 깃발은 그 팀의 카피라이터 Tony에게 그 이야기가 그가 다음 상태로 옮겨갈 준비가 되었다는 시각적인 표시를 제공합니다. 그런 다음 토니는 작업을 시작할 준비가 되면 다음 상태로 이야기를 옮깁니다.

스토리에 플래그를 사용할 때는 다음 사항을 고려하십시오.

* 플래그는 상태가 아니라 다른 팀원이 다음 상태로 스토리를 이동할 준비가 되었음을 나타내는 시각적 표시입니다.
* [!UICONTROL 백로그] 열 또는 [!UICONTROL 완료] 열(또는 열의 상태가 [!UICONTROL 완료]와 동일한 열)에 있는 스토리 카드에 플래그가 표시되지 않습니다.

  스토리 상태에 대한 자세한 내용은 [Kanban 보드에서 스토리에 플래그 사용](#updating-the-status-of-stories-and-subtasks)을 참조하세요.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## [!UICONTROL Kanban] 보드의 스토리에 플래그 사용

스토리의 플래그를 변경하려면 다음과 같이 하십시오.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 [!UICONTROL Kanban] 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 스토리의 플래그를 변경할 [!UICONTROL Kanban] 보드로 이동합니다.
1. 스토리 타일을 확장하여 플래그를 봅니다.\
   기본적으로 각 스토리에 대해 **[!UICONTROL 트랙에서]**(으)로 설정됩니다.\
   ![칸반 카드](assets/agile-storycard-kanban-2021-350x308.png)

1. 현재 플래그를 클릭한 다음 다음 플래그 옵션 중에서 선택합니다.

   * **[!UICONTROL 트랙에서]:** 스토리가 적절한 상태이므로 지금은 아무 작업도 수행할 필요가 없습니다.\

     칸반 보드의 각 스토리에 대한 기본 플래그입니다.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL 차단됨]:** 스토리가 다음 상태로 진행할 수 없습니다. 이 플래그를 스토리에 설정하면 스토리가 WIP 한도에 계산되지 않습니다. (WIP 제한에 대한 자세한 내용은 [Kanban 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) 문서를 참조하십시오.\

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 끌어오기 준비]:** 다른 팀원이 다음 상태로 스토리를 이동할 준비가 되었습니다.\

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
