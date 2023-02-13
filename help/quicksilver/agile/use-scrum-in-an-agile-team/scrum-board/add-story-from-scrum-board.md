---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 이야기와 문제 추가
description: Screm 보드에서 바로 새로운 스토리나 문제를 만들거나 보드에서 기존 스토리나 문제를 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: d4eec3c5-8cea-467f-b1b4-3f9fab57b10f
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 에서 스토리 및 문제 추가 [!UICONTROL 스크럼] 보드

Screm 보드에서 바로 새로운 스토리나 문제를 만들거나 보드에서 기존 스토리나 문제를 추가할 수 있습니다.

>[!NOTE]
>
>작업 항목 [!UICONTROL 계획 시작 날짜] 및 [!UICONTROL 계획 완료 일자] 의 설정에 의해 영향을 받습니다 [!UICONTROL 팀 편집] 페이지. 자세한 내용은 섹션을 참조하십시오 [[!UICONTROL 구성] 작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 기사 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

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
   <td> <p>작업 또는 문제가 있는 프로젝트에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## Screm 보드에서 새 스토리 또는 문제 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
1. 클릭 **[!UICONTROL 추가]** 스크럼 보드의 오른쪽에 있는 다음 **[!UICONTROL 새 스토리]** 또는 **[!UICONTROL 새 문제]**.
1. 에서 **[!UICONTROL 새로 만들기]** 대화 상자에서 다음 정보를 추가합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Name]</strong></td>
        <td>(필수) 스토리 또는 문제의 이름입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Description]</strong></td>
        <td>항목에 대한 설명입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Estimate]</strong></td>
        <td>항목의 예상 시간 또는 지점 수입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 상위 프로젝트]</strong></td>
        <td>(필수) 새 스토리 또는 문제가 저장되는 프로젝트입니다. 프로젝트 이름을 입력하기 시작한 다음 목록에 표시될 때 선택합니다.</td>
    </tr>
   </table>

1. 클릭 **[!UICONTROL 스토리 추가]** 또는 **[!UICONTROL 문제 추가]**.

## 에서 기존 스토리 또는 문제 추가 [!UICONTROL 스크럼] 보드

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
1. 클릭 **[!UICONTROL 추가]** 스크럼 보드의 오른쪽에 있는 다음 **[!UICONTROL 기존 스토리]** 또는 **[!UICONTROL 기존 문제]**.
1. 에서 **[!UICONTROL 백로그에서 기존 추가]** 대화 상자에서 스토리나 문제 이름을 입력하기 시작한 다음 목록에 표시될 때 선택합니다.
1. 클릭 **[!UICONTROL 스토리 추가]** 또는 **[!UICONTROL 문제 추가]**.
