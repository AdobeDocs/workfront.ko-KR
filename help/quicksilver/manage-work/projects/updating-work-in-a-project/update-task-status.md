---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 상태 업데이트
description: 작업의 상태를 업데이트하여 작업의 위치와 전체 프로젝트 진행 상황을 다른 사람에게 알릴 수 있습니다.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# 작업 상태 업데이트

작업의 상태를 업데이트하여 작업의 위치와 전체 프로젝트 진행 상황을 다른 사람에게 알릴 수 있습니다.

기본 상태는 신규, 진행 중 및 완료입니다. Adobe Workfront 관리자는 조직의 사용자 지정 상태를 추가할 수 있습니다. 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

작업 상태를 수동으로 업데이트하거나, 특정 작업이 발생하면 Workfront에서 자동으로 업데이트하도록 할 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

작업을 수동으로 업데이트하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 상태 수동 업데이트

작업 상태를 업데이트할 때 새 상태에 대한 설명을 입력하고 기한 등의 다른 작업 정보를 변경할 수도 있습니다.

1. 상태를 업데이트할 작업에 할당된 작업으로 이동합니다.
1. 을(를) 클릭합니다. **상태** 작업 헤더의 필드를 선택하고 새 상태를 선택합니다.
1. (선택 사항) 업데이트에 대한 추가 정보를 제공하려면 다음 중 하나를 수행한 다음 를 클릭합니다 **업데이트** 또는 작업에 **완료** 상태, **완료:**

   * 업데이트에 대한 메모를 추가하려면 **업데이트** 영역을 클릭하고 **새 업데이트 시작**&#x200B;을 입력한 다음 메모를 입력합니다.

   * 특정 사용자에게 업데이트에 대해 알리려면 **알림** 업데이트에 대한 메모를 입력할 때 표시되는 상자입니다. 자세한 내용은 [업데이트에 다른 사용자에게 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 작업 조건을 업데이트하려면 **조건 선택** 오른쪽 **알림** 상자(업데이트에 대한 메모를 입력할 때 표시됨)를 선택한 다음 작업의 현재 조건을 가장 잘 반영하는 조건을 선택합니다.

   * 작업의 커밋 날짜를 업데이트하려면 **커밋 날짜** 드롭다운 일정을 선택하고 새 커밋 날짜를 선택합니다.
   * 작업 완료의 시각적 표시를 제공하려면 완료율 아래에서 버블을 드래그하거나 두 번 클릭하여 백분율 값을 입력합니다.\
      ![](assets/drag-the-progress-bar-350x155.png)

## 작업 상태 자동 업데이트

Workfront은 아래 표에 나열된 작업이 발생하면 작업의 기존 상태를 다른 상태로 자동으로 업데이트합니다.

>[!NOTE]
>
>다음 표의 상태는 기본 시스템 상태입니다. Workfront 관리자 또는 그룹 관리자는 Workfront 인스턴스에서 상태의 이름을 변경할 수 있습니다. Workfront에서 상태 만들기 및 관리에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>개 액션</td> 
   <td>원래 상태</td> 
   <td>새 상태</td> 
  </tr> 
  <tr> 
   <td>작업 완료율을 100%로 업데이트</td> 
   <td>신규 또는 진행 중</td> 
   <td>완료</td> 
  </tr> 
  <tr> 
   <td>작업 완료율을 100%에서 낮은 숫자로 업데이트합니다.</td> 
   <td>완료</td> 
   <td>진행 중</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>작업 시작 단추를 눌러 자신에게 할당된 작업에 대한 작업을 수락합니다</span> </td> 
   <td><span>신규</span> </td> 
   <td> <p>홈 팀 설정의 작업 시작 단추와 연관된 모든 상태입니다.</p> <p>Work On It 단추를 작업 시작 단추로 대체하는 방법에 대한 자세한 내용은 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a></span>.</p> <p>팁: <span>클릭</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">실행 취소 단추</span>작업 시작을 클릭하면 상태가 새로 시작으로 되돌아갑니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
