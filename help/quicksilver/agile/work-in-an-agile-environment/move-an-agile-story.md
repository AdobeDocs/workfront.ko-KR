---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 민첩한 스토리 이동
description: 민첩한 스토리를 다른 반복(스크럼 팀의 경우) 또는 백로그(간판 및 스크럼 팀의 경우)로 이동할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 민첩한 스토리 이동

민첩한 스토리를 다른 반복(스크럼 팀의 경우) 또는 백로그(간판 및 스크럼 팀의 경우)로 이동할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>[!UICONTROL Manage] 스토리 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 반복 또는 간판 보드에서 백로그로 스토리를 이동합니다

1. 백로그로 이동하려는 스토리가 포함된 반복 또는 간판 보드로 이동합니다.
1. 페이지 맨 위에서 반복 머리글을 클릭합니다.
1. 설정 **[!UICONTROL 스토리]** 이동할 스토리를 선택합니다.
1. 클릭 **[!UICONTROL 자세히]** > **[!UICONTROL 이동 위치]**.

   다음 **[!UICONTROL 스토리 이동]** 대화 상자가 표시됩니다.

   ![스토리 이동 대화 상자](assets/iteration-story-move.png)

1. 선택 *team_name*&#x200B;백로그\
   위의 예에서 팀 이름은 &#x200B; 입니다 **마케팅.**

1. 클릭 **[!UICONTROL 스토리 이동]**.

## 스토리를 다른 반복으로 이동

스크럼 팀을 위해 스토리를 다른 반복으로 이동할 수 있습니다.

>[!NOTE]
>
>다음 **[!UICONTROL 이동 위치]** 반복의 상위 스토리에는 옵션을 사용할 수 없습니다. 하위 작업을 다른 반복으로만 이동할 수 있습니다.

1. 이동할 스토리가 포함된 반복으로 이동합니다.
1. 페이지 맨 위에서 반복 머리글을 클릭합니다.
1. 설정 **[!UICONTROL 스토리]** 이동할 스토리를 선택합니다.
1. 클릭 **[!UICONTROL 자세히]** > **[!UICONTROL 이동 위치]**.

   다음 **[!UICONTROL 스토리 이동]** 대화 상자가 표시됩니다.

   ![스토리 이동 대화 상자](assets/iteration-story-move.png)

1. 선택 **[!UICONTROL 다른 반복]**&#x200B;그런 다음 드롭다운 메뉴에서 스토리를 이동할 이터레이션을 선택합니다.

   >[!NOTE]
   >
   >작업 항목 [!UICONTROL 계획 시작 날짜] 및 [!UICONTROL 계획 완료 일자] 의 설정에 의해 영향을 받습니다 [!UICONTROL 팀 편집] 페이지. 자세한 내용은 섹션을 참조하십시오 [[!UICONTROL 구성] 작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 기사 [스크럼 구성](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. 클릭 **[!UICONTROL 스토리 이동]**.
