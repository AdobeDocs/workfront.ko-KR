---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 상태 업데이트
description: 작업 상태를 업데이트하여 작업의 위치와 전체 프로젝트 진행 상황을 다른 사용자에게 알릴 수 있습니다.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# 작업 상태 업데이트

작업 상태를 업데이트하여 작업의 위치와 전체 프로젝트 진행 상황을 다른 사용자에게 알릴 수 있습니다.

기본 상태는 신규, 진행 중 및 완료입니다. Adobe Workfront 관리자는 조직에 대한 사용자 정의 상태를 추가할 수 있습니다. 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

작업 상태를 수동으로 업데이트하거나 특정 작업이 발생할 때 Workfront에서 자동으로 업데이트하도록 할 수 있습니다.

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 상태 업데이트에 대한 고려 사항

* 작업을 완료로 표시하면 작업의 완료율이 100%로 업데이트됩니다.
* 상위 작업에 대해 다음과 같은 시나리오가 있습니다.
   * 프로젝트의 요약 완료 모드가 자동으로 설정되고 하위 작업이 완료되지 않은 경우 상위 작업의 상태를 완료로 업데이트할 수 없습니다.
   * 프로젝트의 요약 완료 모드가 수동으로 설정되고 하위 작업이 완료되거나 완료되지 않은 경우 상위 작업의 상태를 완료로 업데이트할 수 있습니다.

  자세한 내용은 [프로젝트 편집](../manage-projects/edit-projects.md).

## 수동으로 작업 상태 업데이트

작업 상태를 업데이트할 때 새 상태에 대한 설명을 입력하고 기한과 같은 다른 작업 정보를 변경할 수도 있습니다.

1. 상태를 업데이트할 할당된 작업으로 이동합니다.
1. 다음을 클릭합니다. **상태** 작업 헤더의 필드에 새 상태를 선택합니다.
1. (선택 사항) 업데이트에 대한 추가 정보를 제공하려면 다음 중 하나를 수행하고, **업데이트** 또는 작업에 **완료** 상태, 클릭 **완료:**

   * 업데이트에 대한 메모를 추가하려면 **업데이트** 영역 및 클릭 **새 업데이트 시작**&#x200B;그런 다음 메모를 입력합니다.

   * 특정 사용자에게 업데이트에 대해 알리려면 **알림** 업데이트에 대한 메모를 입력할 때 나타나는 상자입니다. 자세한 내용은 [업데이트에 다른 사용자 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 작업의 상태를 업데이트하려면 다음을 클릭하십시오. **조건 선택** 의 오른쪽에 **알림** 상자(업데이트에 대한 메모를 입력할 때 표시됨)에서 작업의 현재 상태를 가장 잘 반영하는 조건을 선택합니다.

   * 작업의 커밋 일자를 업데이트하려면 다음을 확장합니다. **커밋 일자** 드롭다운 캘린더에서 새 커밋 일자를 선택합니다.
   * 작업 완료를 시각적으로 나타내려면 완료율 아래의 버블을 끌어 놓거나 더블 클릭하여 백분율 값을 입력합니다.\
     ![](assets/drag-the-progress-bar-350x155.png)

## 작업 상태 자동 업데이트

Workfront은 아래 표에 나열된 작업이 발생할 때 작업의 기존 상태를 다른 상태로 자동으로 업데이트합니다.

>[!NOTE]
>
>다음 표의 상태는 기본 시스템 상태입니다. Workfront 관리자 또는 그룹 관리자는 Workfront 인스턴스의 상태를 변경할 수 있습니다. Workfront에서 상태를 만들고 관리하는 방법에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td>작업 완료율을 100%에서 더 낮은 숫자로 업데이트</td> 
   <td>완료</td> 
   <td>진행 중</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>할당된 작업에 대한 작업을 수락하려면 작업 시작 단추를 클릭하십시오.</span> </td> 
   <td><span>신규</span> </td> 
   <td> <p>홈 팀 설정의 작업 시작 단추와 연결된 모든 상태입니다.</p> <p>[처리 중] 단추를 [작업 시작] 단추로 바꾸는 방법에 대한 자세한 내용은 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">처리 중 단추를 시작 단추로 바꾸기</a></span>.</p> <p>팁: <span>클릭</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">실행 취소 단추</span>작업 시작을 클릭하면 상태가 신규로 되돌아갑니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
