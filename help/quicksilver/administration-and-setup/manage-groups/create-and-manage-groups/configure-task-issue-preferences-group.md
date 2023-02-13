---
title: 그룹에 대한 작업 및 문제 환경 설정 구성
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 그룹,환경 설정,작업,문제,잠금 해제
navigation-topic: create-and-manage-groups
description: 조직의 그룹이 시스템 수준에서 구성된 방식과 독립적으로 작업이나 문제 환경 설정을 구성해야 하는 경우 Adobe Workfront 관리자가 기본 설정의 잠금을 해제할 수 있습니다. 그런 다음 그룹 관리자로서 그룹에 대한 기본 설정을 구성할 수 있으며 이 기본 설정은 그룹과 관련된 모든 작업 또는 문제에 영향을 줍니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 2%

---

# 그룹에 대한 작업 및 문제 환경 설정 구성

조직의 그룹이 시스템 수준에서 구성된 방식과 독립적으로 작업이나 문제 환경 설정을 구성해야 하는 경우 Adobe Workfront 관리자가 기본 설정의 잠금을 해제할 수 있습니다. 그런 다음 그룹 관리자로서 그룹에 대한 기본 설정을 구성할 수 있으며 이 기본 설정은 그룹과 관련된 모든 작업 또는 문제에 영향을 줍니다.

관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

Workfront 관리자가 기본 설정을 잠금 해제하는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>그룹 수준의 구성은 프로젝트 환경 설정에도 가능합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* 일반적으로 잠금 해제된 환경 설정은 무한정 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 만든 기본 설정에 대한 설정이 손실됩니다.
>* 프로젝트와 연관된 그룹에 대해 설정된 기본 설정은 프로젝트를 생성하는 사용자의 홈 그룹에 대해 설정된 기본 설정에 우선합니다.
>* 일부 그룹 수준 환경 설정은 그룹에 대해 만드는 프로젝트 템플릿에 영향을 줍니다. 자세한 내용은 섹션을 참조하십시오 [그룹 영역에서 그룹 템플릿을 보고, 작업하고, 생성할 수 있습니다](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 기사 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제한 후에 이를 구성한 다음 잠금으로 잠근 후 그룹 및 해당 하위 그룹의 모든 사용자가 동일한 구성을 사용하고 있는지 확인할 수 있습니다. 이는 Workfront 관리자가 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그던 기능과 병렬입니다. 자세한 내용은 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 최상위 그룹에 대해 잠금 해제된 작업 및 문제 환경 설정 구성

>[!TIP]
>
>Workfront 관리자의 경우, 설정 > 프로젝트 환경 설정 > 작업 및 문제 로 이동한 다음, 페이지 상단에 있는 상자에서 그룹 이름을 검색하여 1-4단계를 건너뛸 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 잠금 해제된 작업 및 문제 환경 설정을 구성할 그룹의 이름을 클릭합니다.
1. 그룹에 대해 표시되는 페이지의 왼쪽 패널에서 **작업 및 문제 환경 설정**.
1. 나타나는 페이지에서 이 단계 아래에 나열된 5개 섹션 중 하나를 사용하여 새 작업 기본값, 문제, 삭제, 실제 날짜 및 액세스 영역에 대한 설정을 구성한 다음 **저장**.

   잠금 아이콘을 마우스로 가리키면 ![](assets/lock-toggle-button-dimmed.png) 구성해야 하는 기본 설정을 지정하고 도구 설명이 표시되어 잠기고 있음을 알려줍니다. 조직의 모든 그룹에 대해 Workfront 관리자에게 잠금을 해제하도록 요청할 수 있습니다.

   잠금이 해제되면 사용자와 다른 그룹 관리자가 사용자 그룹에 대해 별도로 구성할 수 있습니다. 또한 그룹 및 그룹 아래에 있는 모든 하위 그룹에 대해 잠글 수 있습니다.

   * [새 작업 기본값](#new-task-defaults)
   * [문제](#issues)
   * [삭제](#deletion)
   * [실제 일자](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [액세스](#access)

### 새 작업 기본값 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">새 작업의 시작 날짜</td> 
      <td> <p>프로젝트 관리자의 새 작업에 대한 기본 시작 날짜를 결정합니다. 새 작업의 시작 날짜는 프로젝트의 계획 시작 날짜이거나 작업이 생성된 날짜일 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>기간 유형 </p> </td> 
      <td> <p>자원 수(및 해당 할당 퍼센트)와 작업의 기간 또는 총 투입 사이의 관계를 결정합니다. 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수익 유형</td> 
      <td> <p>작업에 대한 계획 및 실제 매출 예측을 계산합니다. 이 <strong>매출 유형</strong> 가 로 설정되어 있습니다.<strong>청구 불가</strong>, 계획된 시간과 실제 기록된 시간은 작업에 대한 예상 수익을 생성하지 않으며, 작업에 대한 작업은 프로젝트 레벨 매출에 기여하지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">비용 유형</td> 
      <td> <p>태스크에 대한 계획 및 실제 원가 예측을 계산합니다. 로 설정된 경우 <strong>비용 없음</strong>그리고 계획 시간 및 기록된 실제 시간은 작업에 대한 계획 또는 실제 예상 비용을 생성하지 않으며, 작업 작업이 프로젝트 레벨 원가에 기여하지 않습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### 문제 {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">해결 중 오브젝트의 상태가 변경되면 해결 가능한 문제 상태를 자동으로 업데이트</td> 
      <td> <p>문제가 프로젝트나 작업으로 변환되면 원래 문제와 변환된 프로젝트 또는 작업이 모두 개체를 해결할 수 있습니다. 이 설정을 사용하면 원래 문제의 해결 방법을 해결할 수 있는 개체의 해결책과 상호 연관시킬 수 있습니다. 개체 해결에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> <p>이 설정이 어떤 영향을 주려면 <strong>원래 문제를 유지하고 해결 방법을 작업에 연결합니다</strong> 을 선택해야 합니다.</p> 
       <ul> 
        <li>이 설정이 활성화되면 문제와 프로젝트 또는 작업 모두에 대해 동일한 키로 사용자 지정 상태를 만들 수 있습니다. 프로젝트나 작업(해결 가능한 개체)이 사용자 지정 상태로 전환되면 변경 내용은 문제의 상태도 반영합니다. 문제 및 프로젝트 또는 작업 상태에 대해 상태 키는 동일해야 합니다.</li> 
        <li>이 설정을 비활성화하면 사용자 지정 상태 대신 개체 상태를 자동으로 기본 상태로 설정합니다. 기본 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스합니다</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제를 작업으로 변환할 때</td> 
      <td> <p>이 섹션의 설정은 문제 대비 변환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
       <ul> 
        <li><strong>원래 문제를 유지하고 해결 방법을 작업에 연결합니다</strong>: 문제를 변환하면 작업이 완료될 때까지 문제가 계속 표시됩니다. 작업이 완료되면 문제 상태가 자동으로 종료됨으로 변경됩니다.</li> 
        <li><strong>기본 연락처가 작업에 액세스할 수 있도록 허용</strong>: 작업을 검토하고 업데이트하며 진행 상황을 계속 파악할 수 있도록 작업에 대한 기본 연락처(문제 생성자) 액세스 권한을 제공합니다.</li> 
        <li> <p><strong>전환 중에 이러한 설정을 변경할 수 있도록 허용합니다</strong>: 문제를 작업으로 변환하는 동안 문제를 변환한 사용자가 이러한 옵션을 변경할 수 있도록 해줍니다.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제를 프로젝트로 변환할 때</td> 
      <td> <p>이 섹션의 설정은 문제 및 프로젝트에서 프로젝트로 변환 프로세스 중에 발생하는 상황을 결정합니다.</p> 
       <ul> 
        <li><strong>원래 문제를 그대로 두고 그 해결책을 프로젝트에 연결합니다</strong>: 문제를 변환하면 프로젝트가 완료될 때까지 문제로 계속 표시됩니다. 프로젝트가 완료되면 문제 상태가 자동으로 종료됨으로 변경됩니다.</li> 
        <li><strong>기본 연락처가 프로젝트에 액세스할 수 있도록 허용</strong>: 프로젝트에 대한 기본 연락처(문제 생성자) 액세스 권한을 제공하여 프로젝트를 검토하고 업데이트하며 진행 상황을 계속 파악할 수 있습니다.</li> 
        <li><strong>전환 중에 이러한 설정을 변경할 수 있도록 허용합니다</strong>: 문제를 프로젝트로 변환하는 동안 나열된 옵션을 변경할 수 있도록 문제를 변환하는 사용자가 허용합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 삭제 {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자가 기록된 시간이 있는 작업 및 문제를 삭제할 수 있도록 허용</td> 
      <td> <p> 작업이 삭제되도록 허용할지 또는 시간이 기록되는 문제를 삭제하도록 허용할지 결정할 수 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.</p> 
       <div> 
        <p><b>팁</b>: 이 설정은 작업 또는 로그된 시간 내에 문제가 있는 프로젝트를 삭제하는 경우에도 적용됩니다. 이 설정은 프로젝트에 대해 시간이 직접 기록되는 프로젝트를 삭제하는 경우에는 적용되지 않습니다. </p> 
        <p>다음 사항을 고려하십시오.</p> 
        <ul> 
         <li> <p>이 옵션을 선택하면 작업이나 문제를 삭제할 때 정보 경고가 표시됩니다. 경고에 따르면 작업이나 문제가 로그된 시간이 있으면 해당 작업이 프로젝트로 이동되거나 삭제된다는 메시지가 나타납니다. 설치 프로그램의 작업표 및 시간 환경 설정 영역에서 시간을 삭제할지 아니면 프로젝트로 이동할지 여부를 구성할 수 있습니다. 경고 메시지가 표시되는지 확인하면 작업이나 문제가 삭제됩니다. 작업표 및 시간 기본 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">작업표 및 시간 환경 설정 구성</a>. </p> <p>팁: <span>로그된 시간과 작업이 있는 프로젝트를 삭제하면 기록되는 시간이 삭제되거나 설치 프로그램의 작업표 및 시간 기본 설정 영역에 있는 설정에 따라 보존됩니다</span>. </p> </li> 
         <li><span>이 옵션을 선택 해제하면 작업을 삭제하거나 로그된 시간 문제를 해결할 때 또는 해당 작업이나 문제에 대해 기록된 시간이 있는 프로젝트를 삭제할 때 금지 경고가 표시됩니다</span> <span>.</span> 이 경고는 관리자가 로그된 시간 관련 작업 또는 문제를 삭제할 수 없도록 허용한다는 것을 나타냅니다. 작업, 문제<span>, 또는 작업 및 문제에 대해 시간(분)이 기록되는 프로젝트</span> 삭제할 수 없습니다. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### 실제 일자 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업 또는 문제가 "신규"에서 "진행 중"으로 전환되면 실제 시작 날짜를 로 설정합니다.</td> 
      <td> <p>작업 또는 문제가 발생할 때 실제 시작 날짜가 Workfront에 기록될 때 다음 옵션 중 하나를 선택합니다 <strong>새로 만들기</strong> to <strong>진행 중</strong>:</p> 
       <ul> 
        <li><strong>지금:</strong> 실제 시작 일자는 현재 일자로 설정됩니다.</li> 
        <li><strong>계획 시작 일자:</strong> 실제 시작 일자는 태스크 또는 문제의 계획 시작 일자로 설정됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 또는 문제가 완료되면 실제 완료 날짜를 로 설정합니다.</td> 
      <td> <p>작업 또는 문제가 완료될 때 Workfront에 실제 완료 날짜가 기록될 때 다음 옵션 중 하나를 선택합니다.</p> 
       <ul> 
        <li><strong>지금:</strong> 실제 완료 일자는 현재 일자로 설정됩니다.</li> 
        <li> <p><strong>계획 완료 일자:</strong> 실제 완료 일자는 태스크 또는 출고 계획 완료 일자로 설정됩니다.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### 액세스 {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업이 할당되면</td> 
      <td> 
       <ul> 
        <li><strong>작업에 대한 액세스 권한을 제공합니다.</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> 사용자에게 액세스 권한 부여</a>.</li> 
        <li> <p><strong>프로젝트에 대한 액세스 권한을 부여합니다.</strong>: 사용자에게 할당된 작업이 있는 프로젝트에 대한 사용자의 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제에 다른 사람이 할당되면</td> 
      <td> 
       <ul> 
        <li><strong>작업에 대한 액세스 권한을 제공합니다.</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</li> 
        <li> <p><strong>프로젝트에 대한 액세스 권한을 부여합니다.</strong>: 사용자에게 할당된 작업이 있는 프로젝트에 대한 사용자의 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">누군가 요청을 제출할 때</td> 
      <td> 
       <ul> 
        <li><strong>해당 문제에 대한 액세스 권한을 부여합니다.</strong>: 사용자가 제출한 요청에 대한 기본 권한을 정의합니다. 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유</a>.</li> 
        <li> <p><strong>동일한 회사의 사용자는 모든 요청에 대해 동일한 권한을 상속받게 됩니다</strong>: 사용자는 동일한 회사의 다른 사용자가 제출한 요청을 볼 수 있습니다. 보유한 요청 수와 동일한 권한이 있습니다.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
