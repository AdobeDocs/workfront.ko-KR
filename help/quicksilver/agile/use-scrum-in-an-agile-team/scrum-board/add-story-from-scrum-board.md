---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 스토리 및 문제 추가
description: 스크럼 보드에서 직접 새로운 스토리나 문제를 만들거나 보드에서 기존 스토리나 문제를 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: d4eec3c5-8cea-467f-b1b4-3f9fab57b10f
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# [!UICONTROL 스크럼] 보드에서 스토리 및 문제 추가

스크럼 보드에서 직접 새로운 스토리나 문제를 만들거나 보드에서 기존 스토리나 문제를 추가할 수 있습니다.

>[!NOTE]
>
>작업 항목 [!UICONTROL 계획된 시작 일자] 및 [!UICONTROL 계획된 완료 일자]가 [!UICONTROL 팀 편집] 페이지의 설정에 영향을 받습니다. 자세한 내용은 문서 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)에서 [[!UICONTROL 구성], 작업 항목을 반복에 추가할 때 날짜가 적용되는 방법](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 섹션을 참조하십시오.

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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업 또는 문제가 있는 프로젝트에 대한 [!UICONTROL 관리] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 스크럼 보드에서 새 스토리 또는 문제 만들기

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.
1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.
1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택하여 특정 반복을 선택하거나 **[!UICONTROL 현재 반복]**&#x200B;을 선택합니다.
1. 스크럼 보드 오른쪽의 **[!UICONTROL 추가]**&#x200B;를 클릭하고 **[!UICONTROL 새 스토리]** 또는 **[!UICONTROL 새 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 새로 만들기]** 대화 상자에서 다음 정보를 추가합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 이름]</strong></td>
        <td>(필수) 스토리 또는 문제의 이름입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 설명]</strong></td>
        <td>항목에 대한 설명.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Estimate]</strong></td>
        <td>항목에 대한 예상 시간 또는 포인트 수입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 상위 프로젝트]</strong></td>
        <td>(필수) 새 스토리 또는 문제가 저장되는 프로젝트입니다. 프로젝트의 이름을 입력한 다음 목록에 표시될 때 선택합니다.</td>
    </tr>
   </table>

1. **[!UICONTROL 스토리 추가]** 또는 **[!UICONTROL 문제 추가]**&#x200B;를 클릭합니다.

## [!UICONTROL 스크럼] 보드에서 기존 스토리 또는 문제 추가

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.
1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.
1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택하여 특정 반복을 선택하거나 **[!UICONTROL 현재 반복]**&#x200B;을 선택합니다.
1. 스크럼 보드 오른쪽의 **[!UICONTROL 추가]**&#x200B;를 클릭하고 **[!UICONTROL 기존 스토리]** 또는 **[!UICONTROL 기존 문제]**&#x200B;를 선택합니다.
1. **[!UICONTROL 백로그에서 기존 항목 추가]** 대화 상자에서 스토리 또는 문제의 이름을 입력한 다음 목록에 표시될 때 선택합니다.
1. **[!UICONTROL 스토리 추가]** 또는 **[!UICONTROL 문제 추가]**&#x200B;를 클릭합니다.
