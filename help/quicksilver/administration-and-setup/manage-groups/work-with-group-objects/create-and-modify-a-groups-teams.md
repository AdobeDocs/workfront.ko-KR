---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 팀 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 관련된 팀을 보고 작업할 수 있습니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 5%

---

# 그룹의 팀 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 관련된 팀을 보고 작업할 수 있습니다.

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

플랜 라이선스가 있는 사용자가 팀을 만드는 방법에 대한 자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)를 참조하세요.

Workfront 관리자가 팀을 만드는 방법에 대한 자세한 내용은 [설정 영역에서 팀 만들기](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 영역에서 그룹을 위한 팀 보기, 작업 및 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

1. 팀을 만들거나 수정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **팀** ![팀](assets/teams.png)을(를) 클릭하여 그룹 및 해당 그룹에 포함될 수 있는 하위 그룹과 연결된 팀을 나열합니다.

1. 다음 중 하나를 수행합니다.

   * **팀 추가**: **새 팀**&#x200B;을 클릭한 후 다음 옵션을 사용하여 구성하십시오.

   <!-- WRITER please check table below. I stripped out wonky conditions-->

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
       <td> <p> 시스템이 새 팀의 그룹 필드에 사용자가 보고 있는 그룹을 채웁니다. 팀을 다른 그룹과 연결하려면 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> <p>마우스로 팀을 가리키고 그 옆에 표시되는 정보 아이콘 <img src="assets/info-icon.png">을(를) 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> <p><b>참고</b>: 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 해당 그룹의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 주 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘">을(를) 클릭하여 자신이 관리하는 그룹에 할당된 모든 팀을 나열할 수 있습니다.</p> </td> 
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

   * **팀 편집**: 하나 이상의 팀을 선택하고 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭한 후 다음 옵션을 사용하여 구성하십시오.

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
       <td> <p>팀과 그룹을 연결합니다. 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> <p>마우스로 팀을 가리키고 그 옆에 표시되는 정보 아이콘 <img src="assets/info-icon.png">을(를) 클릭하여 올바른 그룹을 팀과 연결하는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> <p><b>참고</b>: 팀이 그룹 또는 하위 그룹에 할당되면 해당 그룹 또는 하위 그룹의 모든 그룹 관리자는 해당 그룹의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 그룹 관리자는 주 메뉴에서 팀 영역으로 이동하여 팀 전환 화살표 <img src="assets/switch-team-icon.png" alt="팀 전환 아이콘">을(를) 클릭하여 자신이 관리하는 그룹에 할당된 모든 팀을 나열할 수 있습니다.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">소유자</td> 
       <td>팀에 대한 소유자를 선택합니다.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">팀원</td> 
       <td> <p>및 팀원을 추가합니다. 사용자 이름을 입력한 다음 표시될 때 이름을 선택합니다. 이 프로세스를 반복하여 팀에 여러 사용자를 추가합니다.</p> <p><b>팁</b>: 팀에 추가할 수 있는 사용자 수에는 제한이 없습니다. 그러나 팀의 작업 관리가 너무 복잡해질 수 있으므로 한 팀에 지나치게 많은 수의 사용자가 포함되지 않도록 하는 것이 좋습니다.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">설명</td> 
       <td>팀에 대한 설명을 입력합니다.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">레이아웃 템플릿</td> 
       <td> <p>팀에서 사용할 레이아웃 템플릿의 이름을 입력한 다음 표시될 때 클릭합니다.</p> <p>이 레이아웃 템플릿을 사용하는 팀을 홈 사용자 팀으로 지정하면 이 팀의 모든 사용자에게 이 레이아웃 템플릿의 사용자 지정이 표시됩니다.<br>개별 레이아웃 템플릿 설정이 홈 팀 레이아웃 템플릿의 설정보다 우선합니다. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">애자일</td> 
       <td>애자일 팀인지 여부를 지정합니다. 애자일 팀 및 작업 관리 방법에 대한 자세한 내용은 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">애자일 팀 만들기</a>를 참조하십시오.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">처리 중</td> 
       <td> <p>처리 중(Work On It) 단추를 시작(Start) 단추로 변경합니다. 사용자가 시작을 클릭하면 항목의 상태가 자동으로 업데이트됩니다.</p> <p>시작 단추를 구성하는 방법에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">처리 중 단추를 시작 단추로 바꾸기</a>를 참조하십시오.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">완료 버튼</td> 
       <td> <p>완료 단추를 사용자 지정합니다. 자세한 내용은 다음 문서를 참조하십시오.</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">작업에 대한 완료 단추 구성</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">문제에 대한 완료 단추 구성</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **팀 삭제**: 하나 이상의 팀을 선택한 다음 삭제 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.
   * **팀 목록 내보내기**: **내보내기** ![내보내기 아이콘](assets/export.png)을 클릭한 다음 내보낸 목록에 사용할 파일 형식을 선택합니다.
