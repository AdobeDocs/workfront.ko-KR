---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 작업 및 팀 요청 관리
description: 요청은 보류 중인 작업 또는 문제 지정을 나타냅니다. 작업 요청은 개인에게 수행되고, 팀 요청은 팀에 이루어집니다.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 작업 및 팀 요청 관리

요청은 보류 중인 작업 또는 문제 지정을 나타냅니다. 작업 요청은 개인에게 수행되고, 팀 요청은 팀에 이루어집니다.

>[!NOTE]
>
>애자일 팀에는 팀 요청이 없습니다.

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
   <td> <p>요청을 할당하거나 작업하려면 검토 이상 요청을 재지정할 작업 또는 그 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 팀에 요청 할당 {#assign-a-request-to-a-team}

프로젝트 관리자 및 문제 요청자는 작업을 수행할 수 있는 리소스가 무엇인지 모르거나 작업 완료자와 상관 없이 작업을 팀에 할당할 수 있습니다.

팀에 할당된 작업은 [!UICONTROL 팀 요청] 팀 지원자의 사용자가 요청에 대해 작업할 때까지 탭합니다.

팀 및 팀 구성원이 아닌 사용자 모두에 요청이 할당되면 요청이 두 팀 모두에 표시됩니다 [!UICONTROL 팀 요청] 탭하고 사용자의 작업 요청 영역에서 사용할 수 있습니다. 팀 자원봉사자에 없는 사용자가 작업을 수행할 경우 해당 작업은 여전히 [!UICONTROL 팀 요청] 팀 자원봉사자의 사용자가 작업을 수행할 때까지 탭합니다.

다음과 같은 방법으로 작업 및 문제에 팀을 지정할 수 있습니다.

* 사용 [!UICONTROL 간트 차트]
* 작업 또는 문제 목록(개별적으로 또는 대량으로)
* 작업이나 문제가 만들어지거나 수정될 때
* 요청에 대한 라우팅 규칙 사용(문제만)

이 섹션에 설명된 대로 팀 페이지에서 팀에 요청을 수동으로 할당할 수 있습니다.

팀 페이지에서 팀에 요청을 수동으로 할당하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png)를 선택하고 을 선택합니다. **[!UICONTROL 작업 요청 보내기]**.

   ![](assets/edit-team-settings-350x205.png)

1. 열리는 상자에 정보를 입력합니다.
1. 클릭 **[!UICONTROL 요청 보내기]**.\
   이제 팀에 팀 요청 탭에 표시되는 새 작업이 할당됩니다. 이 작업은 현재 프로젝트와 연결되어 있지 않지만 다음에 설명된 대로 이동할 수 있습니다. [작업 이동](../../manage-work/tasks/manage-tasks/move-tasks.md).

## 요청 재할당 {#reassign-requests}

팀에 지정된 요청을 재할당할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 왼쪽 탐색 패널에서 를 선택합니다 **[!UICONTROL 팀 요청]**.
1. 을(를) 클릭합니다. **[!UICONTROL 재지정]** 아이콘.

1. 요청을 재지정할 사용자, 그룹 또는 팀의 이름을 입력한 다음 **[!UICONTROL 지정]**.\
   요청이 재할당됩니다.
