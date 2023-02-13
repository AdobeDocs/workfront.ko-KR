---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Screm 보드에서 스토리 및 문제 관리
description: 스크럼 보드에서 다른 반복 또는 백로그로 스토리나 문제를 이동하거나 스크럼 보드에서 삭제할 수 있습니다. 스토리나 문제를 삭제하면 30일 동안 휴지통으로 이동되며 시스템 관리자만 복구할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 의 스토리 및 문제 관리 [!UICONTROL 스크럼] 보드

스토리나 문제를 [!UICONTROL 스크럼] 다른 반복 또는 백로그에 게시하거나 백로그에서 삭제합니다 [!UICONTROL 스크럼] 보드. 스토리나 문제를 삭제하면 30일 동안 휴지통으로 이동되며 시스템 관리자만 복구할 수 있습니다.

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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업 또는 문제에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 다음에서 스토리 또는 문제 이동 [!UICONTROL 스크럼] 보드

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 설명이나 문제에 대한 아이콘을 클릭하고 **[!UICONTROL 이동 위치]**.

   ![스크럼 보드에서 스토리 삭제 또는 이동](assets/scrum-delete-move-story.png)

1. 확인 메시지에서 다음 중 하나를 선택합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 다른 반복]</strong></td>
        <td>항목을 다른 이터레이션으로 이동하려면 를 선택하고 스토리나 문제가 이동할 이터레이션을 선택합니다. 향후 이터레이션이 정의되어 있지 않으면 항목을 이동할 수 없습니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 백로그]</strong></td>
        <td>스토리나 문제를 팀의 백로그로 이동하려면 선택합니다.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >작업 항목 [!UICONTROL 계획 시작 날짜] 및 [!UICONTROL 계획 완료 일자] 의 설정에 의해 영향을 받습니다 [!UICONTROL 팀 편집] 페이지. 자세한 내용은 섹션을 참조하십시오 [[!UICONTROL 구성] 작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 기사 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. 클릭 **[!UICONTROL 이동]**.

## 에서 스토리 또는 문제 삭제 [!UICONTROL 스크럼] 보드

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 설명이나 문제에 대한 아이콘을 클릭하고 **[!UICONTROL 스토리 삭제]** 또는 **[!UICONTROL 문제 삭제]**.

   ![스크럼 보드에서 스토리 삭제 또는 이동](assets/scrum-delete-move-story.png)

1. 확인 메시지에서 **[!UICONTROL 예, 삭제합니다]**.
