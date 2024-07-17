---
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban 보드에서 WIP(Work In Progress) 한도 관리
description: Kanban 보드의 각 열에 대해 WIP(Work In Progress) 한도를 구성할 수 있습니다. WIP 제한은 단순히 시각적 경고일 뿐 팀이 각 상태 열에 사용자가 설정한 제한보다 더 많은 항목을 보유하는 것을 제한하지 않습니다.
author: Lisa
feature: Agile
exl-id: 540880ad-46af-416b-8e0b-5df869555424
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 칸반 보드에서 [!UICONTROL 진행 중인 작업](WIP) 제한 관리

[Kanban 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) 문서에 설명된 대로 [!UICONTROL Kanban] 보드의 각 열에 대해 [!UICONTROL 진행 중인 작업](WIP) 제한을 구성할 수 있습니다.

WIP 제한은 단순히 시각적 경고일 뿐 팀이 각 상태 열에 사용자가 설정한 제한보다 더 많은 항목을 보유하는 것을 제한하지 않습니다.

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

## [!UICONTROL Kanban] 보드에서 [!UICONTROL 진행 중인 작업](WIP) 제한 보기

애자일 팀에 대해 WIP 제한이 구성된 경우 Kanban 보드의 각 열 오른쪽 상단 모서리에 표시됩니다([!UICONTROL 완료] 열 제외).

[!UICONTROL Kanban] 보드의 열에 대한 제한을 초과할 때마다 제한이 빨간색으로 강조 표시되고 메시지가 표시됩니다.\
![WIP 제한](assets/kanban-wip.png)

## [!UICONTROL Kanban] 보드에서 [!UICONTROL 진행 중인 작업](WIP) 제한 업데이트

[!UICONTROL 편집] 권한이 있는 팀원은 [!UICONTROL Kanban] 보드에서 직접 각 상태 열에 대한 WIP 제한을 업데이트할 수 있습니다. 또는 문서 [Kanban 구성](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)에 설명된 대로 WIP 제한을 업데이트할 수 있습니다.

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 [!UICONTROL Kanban] 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. [!UICONTROL Kanban] 보드에서 Kanban 보드에 있는 각 열의 오른쪽 상단 모서리에서 WIP 제한을 찾습니다.
1. 수정할 WIP 한도를 누른 다음 신규 한도를 지정합니다.
1. **[!UICONTROL Enter]**&#x200B;를 누릅니다.
