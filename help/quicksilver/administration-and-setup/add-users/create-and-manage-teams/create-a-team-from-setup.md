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

Adobe Workfront 관리자는 설정 영역에서 팀을 만들 수 있습니다. 팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 그룹 관리자는 설정 영역에서 관리하는 그룹에 대한 팀을 생성할 수 있습니다. 자세한 내용은 [그룹 팀 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 계획 라이센스가 있는 사용자는 사람 영역에서 팀을 만들 수도 있습니다. 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 팀 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **팀**&#x200B;를 클릭한 다음 **새 팀**.

1. 에서 **새 팀** 표시되는 상자에 다음 정보를 지정합니다.

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
      <td> <p>팀을 그룹과 연결하려면 그룹 이름을 입력한 후 그룹 이름이 나타나면 이름을 선택합니다.</p> <p>마우스로 가리키고 정보 아이콘을 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다 <img src="assets/info-icon.png"> 옆에 표시됩니다. 그룹 위에 있는 그룹 계층 및 해당 관리자와 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> <p><b>참고</b>: 한 팀이 그룹이나 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자가 구성원이 아니더라도 팀을 관리할 수 있습니다. 그룹 관리자는 기본 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표를 클릭할 수 있습니다 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘"> 관리하는 그룹에 할당된 모든 팀을 나열하려면 다음을 수행하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">팀원</td> 
      <td> <p>팀에 속한 사용자의 이름을 입력하기 시작한 다음 드롭다운 목록에 이 나타날 때 이름을 선택합니다. 이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.</p> <p>팀에 추가할 수 있는 사용자 수에는 제한이 없습니다. 하지만 팀의 작업 관리가 너무 복잡해질 수 있으므로 한 팀에 과도하게 많은 사용자가 없도록 하는 것이 좋습니다.</p> </td> 
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
      <td>이 새 팀을 애자일 팀으로 구성하려면 이 항목을 선택합니다. 애자일 팀에 대한 자세한 내용은 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 수행</td> 
      <td>Work On It 단추를 시작 단추로 변경합니다. 사용자가 시작 을 클릭하면 항목의 상태가 자동으로 업데이트됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 버튼</td> 
      <td>완료 단추를 클릭할 때 항목에 대해 설정할 상태를 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **팀 만들기**.

## 팀 소유자

팀을 만들면 기본적으로 팀 소유자가 됩니다.

팀에 대한 보고서를 만들고 보고서에 소유자 이름 필드를 포함할 때 모든 팀의 팀 소유자를 볼 수 있습니다. 보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md))
