---
title: 설정 영역에서 팀 설정 편집
description: Adobe Workfront 관리자는 설정 영역에서 팀 설정을 편집할 수 있습니다. 팀에 사용자를 추가하고, 팀의 레이아웃 템플릿을 설정하고, 팀이 작업 항목을 완료할 때 상태가 기록되는 방식을 설정할 수 있습니다.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 3%

---

# 설정 영역에서 팀 설정 편집

Adobe Workfront 관리자는 설정 영역에서 팀 설정을 편집할 수 있습니다. 팀에 사용자를 추가하고, 팀의 레이아웃 템플릿을 설정하고, 팀이 작업 항목을 완료할 때 상태가 기록되는 방식을 설정할 수 있습니다.

팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 그룹 관리자는 관리하는 그룹에 대한 팀 설정을 편집할 수 있습니다. 자세한 내용은 [그룹 팀 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 계획 라이센스가 있는 사용자는 사람 영역에서 팀 설정을 편집할 수 있습니다. 자세한 내용은 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
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

## 팀 설정 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **팀** 왼쪽 패널에 표시됩니다.
1. 팀을 선택한 다음 **편집** ![](assets/edit-icon.png).

1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">팀 이름</td> 
      <td>팀 이름을 입력합니다.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">활성화됨 </td> 
       <td>이 옵션은 기본적으로 새 팀과 기존 팀에 대해 활성화되어 있습니다. 팀 비활성화하려면 비활성화합니다. 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">팀 비활성화</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">그룹</td> 
      <td> <p>팀을 그룹과 연결합니다. 그룹 이름을 입력하기 시작한 다음 그룹 이름이 나타나면 이름을 선택합니다.</p> <p><b>참고</b>: 한 팀이 그룹이나 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자가 구성원이 아니더라도 팀을 관리할 수 있습니다. 그룹 관리자는 기본 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표를 클릭할 수 있습니다 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘"> 관리하는 그룹에 할당된 모든 팀을 나열하려면 다음을 수행하십시오.</p> <p>마우스로 가리키고 정보 아이콘을 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다 <img src="assets/info-icon.png"> 옆에 표시됩니다. 그룹 위에 있는 그룹 계층 및 해당 관리자와 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">소유자</td> 
      <td>팀의 소유자를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">팀원</td> 
      <td> <p>및 팀 구성원을 추가합니다. 사용자 이름을 입력하기 시작한 다음, 나타날 때 이름을 선택합니다. 이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.</p> 
      <p><b>팁</b>: 팀에 원하는 수의 사용자를 추가할 수 있습니다. 하지만 팀의 작업 관리가 너무 복잡해질 수 있으므로 한 팀에 너무 많은 수를 추가하지 않는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>팀에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이아웃 템플릿</td> 
      <td> <p>팀에서 사용할 레이아웃 템플릿의 이름을 입력하기 시작한 다음 레이아웃 서식 파일이 나타나면 클릭합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">애자일</td> 
      <td>민첩한 팀인지 여부를 지정합니다. 애자일 팀 및 작업 관리 방법에 대한 자세한 내용은 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">작업 수행</td> 
      <td> <p>Work On It 단추를 시작 단추로 변경합니다. 사용자가 시작 을 클릭하면 항목의 상태가 자동으로 업데이트됩니다.</p> <p>시작 단추를 구성하는 방법에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 버튼</td> 
      <td> <p>완료 단추를 사용자 지정합니다. 자세한 내용은 다음을 참조하십시오.</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">작업에 대한 완료 단추 구성</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">문제에 대한 완료 단추 구성</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **변경 내용 저장**.
