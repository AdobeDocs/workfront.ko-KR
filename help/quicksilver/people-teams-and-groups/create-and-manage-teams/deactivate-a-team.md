---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 팀 비활성화
description: 연결된 이전 데이터를 유지하면서 더 이상 사용하지 않는 팀을 비활성화할 수 있습니다. Adobe Workfront 관리자는 설정의 팀 영역에서 언제든지 팀을 다시 활성화할 수 있습니다.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 팀 비활성화

연결된 이전 데이터를 유지하면서 더 이상 사용하지 않는 팀을 비활성화할 수 있습니다. [!DNL Adobe Workfront] 관리자는 설정의 팀 영역에서 언제든지 팀을 다시 활성화할 수 있습니다. 팀을 비활성화하면 팀이 더 이상 다음 영역에 표시되지 않습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>사용자 지정 양식의 필드 입력</p> </li> 
    </ul> 
    <ul> 
     <li> <p>객체에 대한 공유 대화 상자</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] 영역의 기본 선택 드롭다운 메뉴</p> </li> 
     <li> <p>[!UICONTROL Assignments] typeahead</p> </li> 
     <li> <p>프로젝트의 [!UICONTROL 간판 추가] 보드 대화 상자</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

비활성화된 팀은 팀을 검색할 때 나타나지 않지만, 여전히 [!UICONTROL 홈 팀] 및 다른 팀(사용자가 비활성화 전에 팀에 할당된 경우)

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
   <td> <p>플랜</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 팀 비활성화

비활성화하기 전에 팀에 할당된 모든 작업은 할당된 상태로 유지됩니다. 팀을 비활성화하기 전에 작업을 다시 할당하는 것이 좋습니다.

>[!TIP]
>
>보고서를 만들어 비활성화된 팀이 아직 지정된 작업이나 문제에 대해 필터링할 수 있습니다.

요청 큐를 사용할 때 라우팅 규칙에서 기본 팀으로 지정된 팀을 비활성화하면 팀이 남아 있고 요청이 여전히 비활성화된 팀으로 라우팅됩니다. 팀을 비활성화하기 전에 활성 팀과 함께 라우팅 규칙을 업데이트하는 것이 좋습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 팀]**.
1. 을(를) 클릭합니다. **[!DNL Switch team]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.

   ![](assets/edit-team-settings-350x205.png)

1. 지우기 **[!UICONTROL 활성 상태]** 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 알려진 제한 사항

비활성화된 팀은 다음 영역에 표시됩니다.

* 의 소유자 필드 [!DNL Workfront Goals]. 이에 대한 추가 라이센스가 필요합니다 [!DNL Adobe Workfront Goals]. 자세한 내용은 [시작하기 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
