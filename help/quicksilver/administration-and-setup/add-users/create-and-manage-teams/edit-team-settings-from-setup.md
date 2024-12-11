---
title: 설정 영역에서 팀 설정 편집
description: Adobe Workfront 관리자는 설정 영역에서 팀 설정을 편집할 수 있습니다. 팀에 사용자를 추가하고, 팀의 레이아웃 템플릿을 설정하고, 팀이 작업 항목을 완료할 때 상태를 기록하는 방법을 설정할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 6409f8fa5072413444545d2d3a80935dc6e04b4c
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 3%

---

# 설정 영역에서 팀 설정 편집

Adobe Workfront 관리자는 설정 영역에서 팀 설정을 편집할 수 있습니다. 팀에 사용자를 추가하고, 팀의 레이아웃 템플릿을 설정하고, 팀이 작업 항목을 완료할 때 상태를 기록하는 방법을 설정할 수 있습니다.

팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)를 참조하세요.

>[!NOTE]
>
>* 그룹 관리자는 자신이 관리하는 그룹에 대한 팀의 설정을 편집할 수 있습니다. 자세한 내용은 [그룹의 팀 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)을 참조하세요.
>* Standard 또는 Plan 라이선스가 있는 사용자는 팀 영역에서 팀 설정을 편집할 수 있습니다. 자세한 내용은 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 팀 설정 편집

{{step-1-to-setup}}

1. 왼쪽 패널에서 **팀**&#x200B;을 클릭합니다.
1. 팀을 선택한 다음 **편집** ![](assets/edit-icon.png)을(를) 클릭합니다.

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
       <td>이 옵션은 기본적으로 새 팀과 기존 팀에 대해 활성화됩니다. 팀을 비활성화하려면 비활성화하십시오. 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">팀 비활성화</a>를 참조하십시오. </td> 
      </tr>
     <tr> 
      <td role="rowheader">그룹</td> 
      <td> <p>팀과 그룹을 연결합니다. 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> <p><b>참고</b>: 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 해당 그룹의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 주 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘">을(를) 클릭하여 자신이 관리하는 그룹에 할당된 모든 팀을 나열할 수 있습니다.</p> <p>마우스로 팀을 가리키고 그 옆에 표시되는 정보 아이콘 <img src="assets/info-icon.png">을(를) 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">소유자</td> 
      <td>팀에 대한 소유자를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">팀원</td> 
      <td> <p>및 팀원을 추가합니다. 사용자 이름을 입력한 다음 표시될 때 이름을 선택합니다. 이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.</p> 
      <p><b>팁</b>: 팀에 사용자를 추가할 수 있습니다. 그러나 팀의 작업 관리가 너무 복잡해질 수 있으므로 한 팀에 지나치게 많은 수를 추가하지 않는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>팀에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이아웃 템플릿</td> 
      <td> <p>팀에서 사용할 레이아웃 템플릿의 이름을 입력한 다음 표시될 때 클릭합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">애자일</td> 
      <td>애자일 팀인지 여부를 지정합니다. 애자일 팀 및 작업 관리 방법에 대한 자세한 내용은 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>를 참조하십시오.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">처리 중</td> 
      <td> <p>처리 중(Work On It) 단추를 시작(Start) 단추로 변경합니다. 사용자가 시작을 클릭하면 항목의 상태가 자동으로 업데이트됩니다.</p> <p>시작 단추를 구성하는 방법에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">처리 중 단추를 시작 단추로 바꾸기</a>를 참조하십시오.</p> </td> 
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

1. **변경 내용 저장**&#x200B;을 클릭합니다.
