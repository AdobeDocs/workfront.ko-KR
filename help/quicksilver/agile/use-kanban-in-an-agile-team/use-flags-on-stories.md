---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 간판 보드의 스토리에 플래그 사용
description: 설정 [!DNL Kanban] 보드, 플래그는 스토리가 다음 상태로 이동할 준비가 되었는지 시각적으로 나타냅니다. 이를 통해 간판 팀이 여러 상태에 걸쳐 스토리를 이동할 때 "푸시" 방식이 아닌 "풀" 접근 방식을 사용할 수 있습니다.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 스토리에 플래그 사용 [!UICONTROL 간판] 보드

설정 [!DNL Kanban] 보드, 플래그는 스토리가 다음 상태로 이동할 준비가 되었는지 시각적으로 나타냅니다. 이렇게 하면 [!UICONTROL 간판] 여러 상태로 스토리를 이동할 때 &quot;푸시&quot; 방식이 아니라 &quot;가져오기&quot; 방법을 사용하는 팀

**예:** &quot;가져오기&quot; 방법을 사용하는 팀의 다음 예를 생각해 보십시오. 팀의 그래픽 디자이너인 올리비아는 자신의 작업을 끝낸 다음 이야기 플래그를 &quot;[!UICONTROL 풀 준비].&quot; 이 플래그는 팀의 카피라이터인 Tony에게 스토리가 다음 상태로 이동할 준비가 되어 있다는 것을 시각적으로 보여 줍니다. Tony는 그 일을 시작할 준비가 되면 그 이야기를 다음 상태로 옮깁니다.

스토리에 플래그를 사용할 때 다음 사항을 고려하십시오.

* 플래그는 상태가 아니라 팀의 다른 구성원이 스토리를 다음 상태로 이동할 준비가 되었다는 시각적 표시입니다.
* Story 카드에 플래그가 표시되지 않습니다 [!UICONTROL 백로그] 열 또는 [!UICONTROL 완료] 열(또는 열의 상태가 [!UICONTROL 완료]).

   스토리 상태에 대한 자세한 내용은 [간판 보드의 스토리에 플래그 사용](#updating-the-status-of-stories-and-subtasks)

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 스토리에 플래그 사용 [!UICONTROL 간판] 보드

스토리의 플래그를 변경하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 선택한 다음, 새로 만들기를 선택합니다 [!UICONTROL 간판] 드롭다운 메뉴에서 팀이나 검색 막대에서 팀을 검색합니다.

1. 로 이동합니다. [!UICONTROL 간판] 스토리의 깃발을 바꾸려는 보드
1. 스토리 타일을 확장하여 플래그를 봅니다.\
   플래그가 로 설정되어 있습니다. **[!UICONTROL On Track]** 기본적으로 각 스토리에 대해 설명합니다.\
   ![간판 카드](assets/agile-storycard-kanban-2021-350x308.png)

1. 현재 플래그를 클릭한 다음 다음 플래그 옵션 중에서 선택합니다.

   * **[!UICONTROL On Track]:** 스토리가 적절한 상태에 있으며 현재 작업을 수행할 필요가 없습니다.\

      간판 보드의 각 스토리에 대한 기본 플래그입니다.\
      ![kand_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL 차단됨]:** 스토리가 다음 상태로 이동할 수 없습니다. 스토리에 이 플래그를 설정하면 스토리는 WIP 제한에 포함되지 않습니다. (WIP 제한에 대한 자세한 내용은 문서를 참조하십시오 [간판 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![간판_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 풀 준비]:** 팀의 다른 구성원이 스토리를 다음 상태로 이동할 준비가 되었습니다.\

      ![간판_flag_ready.png](assets/kanban-flag-ready.png)
