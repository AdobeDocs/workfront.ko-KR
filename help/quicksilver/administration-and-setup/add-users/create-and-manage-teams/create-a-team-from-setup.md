---
title: 설정 영역에서 팀 만들기
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Adobe Workfront 관리자는 설정 영역에서 팀을 만들 수 있습니다.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# 설정 영역에서 팀 만들기

Adobe Workfront 관리자는 설정 영역에서 팀을 만들 수 있습니다. 팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)를 참조하세요.

>[!NOTE]
>
>* 그룹 관리자는 설정 영역에서 관리하는 그룹에 대한 팀을 만들 수 있습니다. 자세한 내용은 [그룹의 팀 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)을 참조하세요.
>* 플랜 라이선스가 있는 사용자는 사람 영역에서 팀을 만들 수도 있습니다. 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)를 참조하세요.
>

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 팀 만들기

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **팀**&#x200B;을 클릭한 다음 **새 팀**&#x200B;을 클릭합니다.

1. 표시되는 **새 팀** 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">팀 이름</td> 
      <td>팀 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹</td> 
      <td> <p>팀과 그룹을 연결하려면 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> <p>마우스로 팀을 가리키고 그 옆에 표시되는 정보 아이콘 <img src="assets/info-icon.png">을(를) 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> <p><b>참고</b>: 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 해당 그룹의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 주 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘">을(를) 클릭하여 자신이 관리하는 그룹에 할당된 모든 팀을 나열할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">팀원</td> 
      <td> <p>팀에 속한 사용자의 이름을 입력한 다음 드롭다운 목록에 이 나타날 때 이름을 선택합니다. 이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.</p> <p>팀에 추가할 수 있는 사용자 수에는 제한이 없습니다. 그러나 팀의 작업 관리가 너무 복잡해질 수 있으므로 한 팀에 지나치게 많은 수의 사용자가 포함되지 않도록 하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>팀에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">캘린더</td> 
      <td>이 팀에 표시할 캘린더 탭을 선택합니다.</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">애자일 팀입니다.</td> 
      <td>이 새 팀을 애자일 팀으로 구성하려면 이 항목을 선택하십시오. 애자일 팀에 대한 자세한 내용은 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>를 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">처리 중</td> 
      <td>처리 중(Work On It) 단추를 시작(Start) 단추로 변경합니다. 사용자가 시작을 클릭하면 항목의 상태가 자동으로 업데이트됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 버튼</td> 
      <td>완료 단추를 클릭할 때 항목에 대해 설정할 상태를 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **팀 만들기**&#x200B;를 클릭합니다.

## 팀 소유자

팀을 만들면 기본적으로 팀 소유자가 됩니다.

팀에 대한 보고서를 만들 때 모든 팀에 대한 팀 소유자를 볼 수 있고 보고서에 소유자 이름 필드를 포함할 수 있습니다. 보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.
