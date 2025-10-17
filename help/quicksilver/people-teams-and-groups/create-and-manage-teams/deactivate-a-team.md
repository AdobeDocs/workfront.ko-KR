---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 팀 비활성화 또는 삭제
description: 연결된 내역 데이터를 유지하면서 더 이상 사용하지 않는 팀을 비활성화할 수 있습니다. Adobe Workfront 관리자는 설정의 팀 영역에서 언제든지 팀을 다시 활성화할 수 있습니다.
author: Jenny
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 팀 비활성화 또는 삭제

연결된 내역 데이터를 유지하면서 더 이상 사용하지 않는 팀을 비활성화할 수 있습니다. [!DNL Adobe Workfront] 관리자는 설정의 팀 영역에서 언제든지 팀을 다시 활성화할 수 있습니다. 팀을 비활성화하면 팀이 더 이상 다음 영역에 표시되지 않습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>사용자 정의 양식의 자동 완성 필드</p> </li> 
    </ul> 
    <ul> 
     <li> <p>객체에 대한 공유 대화 상자</p> </li> 
     <li> <p>[!UICONTROL 사용자 프로필]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] 영역의 기본 선택 드롭다운 메뉴</p> </li> 
     <li> <p>[!UICONTROL Assignments] 자동 완성</p> </li> 
     <li> <p>프로젝트의 [!UICONTROL Kanban에 추가] 보드 대화 상자</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

비활성화된 팀은 팀을 검색할 때 나타나지 않지만, 비활성화 전에 팀에 할당된 경우 [!UICONTROL 홈 팀] 및 기타 팀에 표시됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 패키지</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr>
   <td>액세스 수준 구성</td>
   <td><p>팀을 비활성화하려면 구성이 필요하지 않습니다.</p>
   <p>팀을 삭제하려면 시스템 관리자여야 합니다.</p></td>
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 팀 비활성화

비활성화 이전에 팀에 할당된 모든 작업은 할당된 상태로 유지됩니다. 팀을 비활성화하기 전에 작업을 재할당하는 것이 좋습니다.

>[!TIP]
>
>비활성화된 팀이 여전히 할당된 작업 또는 문제를 필터링할 보고서를 만들 수 있습니다.

요청 대기열을 사용할 때 라우팅 규칙에서 기본 팀으로 할당된 팀을 비활성화하면 팀이 유지되고 요청이 여전히 비활성화된 팀으로 라우팅됩니다. 팀을 비활성화하기 전에 활성 팀과 함께 라우팅 규칙을 업데이트하는 것이 좋습니다.

{{step1-to-team}}

1. **[!DNL Switch team]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. **[!UICONTROL 자세히]** 메뉴를 클릭한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

   ![](assets/edit-team-settings.png)

1. 팀 설정에서 **[!UICONTROL 활성 상태임]** 확인란의 선택을 취소하십시오.
1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.

## 팀 비활성화의 알려진 제한 사항

비활성화된 팀은 다음 영역에 표시됩니다.

* [!DNL Workfront Goals]의 소유자 필드. [!DNL Adobe Workfront Goals]에 대한 추가 라이선스가 필요합니다. 자세한 내용은 [시작하기 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md)를 참조하십시오.

## 팀 삭제

시스템 관리자만 팀을 삭제할 수 있습니다. 관리자가 아닌 팀 소유자이며 팀을 삭제하려고 하면 오류 메시지가 표시됩니다.

팀을 삭제하려면:

{{step1-to-team}}

1. **[!DNL Switch team]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. **[!UICONTROL 자세히]** 메뉴를 클릭한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

   ![](assets/edit-team-settings.png)

1. 팀을 영구적으로 삭제하려면 확인 메시지에서 [!UICONTROL **확인**]&#x200B;을 클릭합니다. 삭제된 팀은 복구할 수 없습니다.
