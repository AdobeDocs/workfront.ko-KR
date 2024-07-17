---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 홈 영역에서 작업 및 팀 요청 관리
description: 작업 작업 및 문제가 할당되면 [!UICONTROL Home] 영역의 [!UICONTROL 작업 목록]에 나열됩니다. 요청을 보고, 재할당하거나, 응답하고, 작업하거나, 제거할 수 있습니다. [!UICONTROL Home] 영역의 작업 요청은 요청 대기열과 관련된 문제로 제한되지 않습니다.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# [!UICONTROL Home] 영역에서 작업 및 팀 요청 관리

작업 작업 및 문제가 할당되면 [!UICONTROL Home] 영역의 [!UICONTROL 작업 목록]에 나열됩니다. 요청을 보고, 재할당하거나, 응답하고, 작업하거나, 제거할 수 있습니다. [!UICONTROL Home] 영역의 작업 요청은 요청 대기열과 관련된 문제로 제한되지 않습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 대한 Contribute 권한 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 작업 요청 보기

사용자에게 할당된 작업 요청은 [!UICONTROL Home]의 왼쪽 패널에 표시됩니다. [!UICONTROL 작업 목록]의 맨 위에 있는 필터를 사용하여 [!UICONTROL Home]에 표시되는 요청을 구성할 수 있습니다.

작업할 준비가 된 항목 또는 현재 이미 작업 중인 항목을 표시하는 필터를 선택할 수 있습니다.

이 문서에서는 [!UICONTROL Home] 영역의 필터를 사용하여 현재 작업 중이거나 작업을 시작할 것으로 예상되는 항목을 보는 방법에 대해 설명합니다. [!UICONTROL Home] 영역의 모든 필터에 대한 자세한 내용은 [작업 목록에서 [!UICONTROL Home] 영역의 항목 표시](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)를 참조하십시오.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 필터]** 드롭다운 메뉴를 클릭합니다.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 작업에 대해 다음 옵션 중 하나 또는 모두를 클릭합니다.

   **[!UICONTROL 시작할 준비]:** 시작할 준비가 된 작업과 문제만 표시합니다. 다음 문은 모두 true여야 합니다.

   * 과제와 그 부모에게는 작업을 할 수 없는 전임자나 과업 제한이 없다.
   * 작업 또는 문제의 [!UICONTROL 계획된 시작 일자]가 과거 또는 최대 2주 후입니다.

   **[!UICONTROL 준비 안 됨]**: 아직 시작할 준비가 되지 않은 작업 및 문제만 표시합니다. 다음 문 중 하나가 true여야 합니다.

   * 작업 및 상위 사용자에게 작업을 수행할 수 없는 선행 작업 또는 작업 제한이 있을 수 있습니다.
   * 작업 또는 문제의 [!UICONTROL 계획된 시작 일자]가 향후 2주 이상입니다.


1. [!UICONTROL 작업] 또는 [!UICONTROL 문제]에서 **[!UICONTROL 작업 중]**&#x200B;을 클릭하여 현재 작업 중인 작업 및 문제를 표시합니다.
1. [!UICONTROL 문제] 아래의 **[!UICONTROL 요청됨]**&#x200B;을(를) 클릭하여 귀하로부터 요청된 문제(귀하에게 할당된 문제)를 표시하지만 아직 작업에 동의하지 않았습니다.

## 팀 요청 액세스

[!UICONTROL Home] 영역에서 팀에 직접 할당된 요청에 액세스할 수 있습니다. 팀 요청에 대한 자세한 내용은 [팀 요청 개요](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md)를 참조하십시오.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 작업 목록]** 영역에서 **[!UICONTROL 팀 요청]** 그룹화를 확장하려면 클릭하세요.

   팀에 할당된 요청이 없으면 그룹화가 표시되지 않습니다.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. 팀 이름을 클릭합니다.\
   **[!UICONTROL 팀 요청]** 섹션에 팀에 할당된 모든 요청이 표시되고 표시됩니다. 팀 요청 작업에 대한 자세한 내용은 [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)를 참조하십시오.

## 요청 재할당

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 작업 목록]** 영역에서 재할당할 요청을 선택합니다.

1. **[!UICONTROL 할당]** 위젯을 클릭하고 요청에서 자신을 제거한 다음 요청을 재할당할 사용자의 이름을 입력합니다.

   >[!TIP]
   >
   >작업 요청이 아직 시작 준비 또는 준비 안 됨 상태인 경우 [!UICONTROL 작업 목록]의 **[!UICONTROL 자세히]** 메뉴에서 **[!UICONTROL 재할당]** 단추를 사용할 수 있습니다.\
   >![재할당 단추](assets/reassign-in-left-panel-350x204.png)

1. 작업이 완료된 후 작업 상태가 [!UICONTROL 새로 만들기] 또는 [!UICONTROL 진행 중](으)로 변경된 경우 작업을 할당 취소하고 작업을 저장한 다음 사용자를 재할당하여 작업을 홈 작업 목록에 다시 표시해야 합니다.

## 요청에 응답

요청을 더 명확하게 하거나 새 날짜를 제안하기 위해 요청에 응답할 수 있습니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 작업 목록]** 영역에서 회신할 요청을 선택합니다.
1. 요청을 할당한 개인을 찾습니다.

   이 정보는 작업의 [!UICONTROL 업데이트] 탭에서 찾을 수 있습니다. **[!UICONTROL 시스템 업데이트 표시]** 옵션이 활성화되어 있는지 확인하십시오.

1. **[!UICONTROL 새 업데이트 시작]**&#x200B;을 클릭하고 회신을 입력하세요.
1. **[!UICONTROL 알림]** 상자에 받는 사람의 이름을 입력한 다음 **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >작업 요청이 아직 시작 준비 또는 [!UICONTROL 준비 안 됨] 상태인 경우 [!UICONTROL 작업 목록]의 **[!UICONTROL 자세히]** 메뉴에서 **[!UICONTROL 회신]** 단추를 사용할 수 있습니다.\
   >![[!UICONTROL 회신 단추]](assets/reassign-in-left-panel-350x204.png)   >

## 요청 작업

[!UICONTROL 처리 중] 단추를 클릭하면 요청을 제출한 사용자와 요청에 할당할 수 있는 다른 사용자에게 요청 작업을 시작할 것임을 나타냅니다. 요청 작업에 대한 자세한 내용은 [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)를 참조하십시오.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 작업 목록]** 영역에서 작업할 요청을 선택한 다음 **[!UICONTROL 작업]**&#x200B;을 클릭합니다.\
   문제에 대한 정보가 오른쪽 패널에 표시됩니다.

## 요청 제거

요청에 대해 작업하지 않기로 결정한 경우 작업 또는 문제를 다시 요청으로 전환하거나 목록에서 제거할 수 있습니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 작업 목록]**&#x200B;에서 작업 대기 중인 항목을 가리킵니다.
1. **[!UICONTROL 할당]** 위젯을 클릭하고 자신을 제거합니다. 그러면 작업 목록에서 작업 항목이 제거됩니다. 요청이 다른 사람, 다른 팀 또는 작업 역할에 할당되지 않은 경우 요청이 할당 해제된 상태로 유지됩니다.

   또는

   [!UICONTROL 홈 작업] 목록에서 작업 또는 문제 이름 오른쪽에 있는 **[!UICONTROL 자세히]** 메뉴 아이콘 ![](assets/more-icon.png)을(를) 클릭합니다.

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 다음 옵션 중에서 선택합니다.

   * **[!UICONTROL 작업 요청으로 전환]:** 작업 항목을 작업 요청으로 다시 전환하려면 이 옵션을 선택하십시오.\

     작업 항목이 요청으로 다시 전환되고 사용자는 요청에 할당된 상태로 유지됩니다.\
      **[!UICONTROL 다시 작업]**&#x200B;을 클릭하여 나중에 요청을 수락할 수 있습니다.

   * **[!UICONTROL 제거]:** [!UICONTROL 작업 목록]에서 요청을 제거하려면 이 옵션을 선택하십시오.\

     요청에서 할당이 취소되어 요청이 [!DNL Adobe Workfront]의 사용자 이름과 더 이상 연결되지 않습니다.\
      요청이 다른 사람, 다른 팀 또는 작업 역할에 할당되지 않은 경우 요청이 할당 해제된 상태로 유지됩니다.
