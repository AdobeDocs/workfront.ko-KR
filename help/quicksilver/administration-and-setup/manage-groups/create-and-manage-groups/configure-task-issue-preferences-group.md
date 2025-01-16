---
title: 그룹에 대한 작업 및 문제 환경 설정 구성
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 그룹,환경 설정,작업,문제,잠금 해제
navigation-topic: create-and-manage-groups
description: 조직의 그룹이 시스템 수준에서 구성된 방식과 별도로 작업 또는 문제 환경 설정을 구성해야 하는 경우 Adobe Workfront 관리자가 환경 설정을 잠금 해제할 수 있습니다. 그런 다음 그룹 관리자는 그룹에 대한 기본 설정을 구성할 수 있으며 이는 그룹과 관련된 모든 작업 또는 문제에 영향을 미칩니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 2%

---

# 그룹에 대한 작업 및 문제 환경 설정 구성

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

조직의 그룹이 시스템 수준에서 구성된 방식과 별도로 작업 또는 문제 환경 설정을 구성해야 하는 경우 Adobe Workfront 관리자가 환경 설정을 잠금 해제할 수 있습니다. 그런 다음 그룹 관리자는 그룹에 대한 기본 설정을 구성할 수 있으며 이는 그룹과 관련된 모든 작업 또는 문제에 영향을 미칩니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

Workfront 관리자가 환경 설정을 잠금 해제하는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)를 참조하십시오.

>[!TIP]
>
>프로젝트 환경 설정에 대해서도 그룹 수준 구성이 가능합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)을 참조하십시오.

>[!NOTE]
>
>* 일반적으로 잠금 해제된 환경 설정은 무기한 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 설정한 기본 설정이 손실됩니다.
>* 프로젝트와 관련된 그룹에 대해 설정된 환경 설정은 프로젝트를 작성하는 사용자의 홈 그룹에 대해 설정된 환경 설정보다 우선합니다.
>* 일부 그룹 수준 환경 설정은 그룹에 대해 만드는 프로젝트 템플릿에 영향을 줍니다. 자세한 내용은 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md) 문서의 [그룹 영역에서 그룹의 템플릿 보기, 작업 및 만들기](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 섹션을 참조하십시오.
>
>* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제한 후 구성한 다음 잠궈 그룹 및 하위 그룹의 모든 사용자가 동일한 구성을 사용하도록 할 수 있습니다. 이는 Workfront 관리자가 시스템 내의 모든 사용자에 대한 환경 설정을 구성하고 잠그는 기능과 병행됩니다. 자세한 내용은 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)를 참조하십시오.
>

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
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 최상위 그룹에 대해 잠금 해제된 작업 및 문제 환경 설정 구성

>[!TIP]
>
>Workfront 관리자인 경우 설정 > 프로젝트 환경 설정 > 작업 및 문제로 이동한 다음 페이지 맨 위의 상자에서 그룹 이름을 검색하여 1-4단계를 건너뛸 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

1. 잠금 해제된 작업 및 문제 환경 설정을 구성할 그룹의 이름을 클릭합니다.
1. 그룹에 대해 표시되는 페이지의 왼쪽 패널에서 **작업 및 문제 환경 설정**&#x200B;을 클릭합니다.
1. 표시되는 페이지에서 이 단계 아래의 5개 섹션 중 하나를 계속하여 새 작업 기본값, 문제, 삭제, 실제 날짜 및 액세스 영역에 대한 설정을 구성한 다음 **저장**&#x200B;을 클릭합니다.

   구성해야 하는 환경 설정을 위해 잠금 아이콘 ![](assets/lock-toggle-button-dimmed.png) 위로 마우스를 가져가면 잠긴 도구 설명이 표시됩니다. Workfront 관리자에게 조직의 모든 그룹에 대해 잠금을 해제하도록 요청할 수 있습니다.

   잠금이 해제된 경우 사용자와 다른 그룹 관리자는 고유한 그룹에 대해 별도로 구성할 수 있습니다. 또한 그룹 및 그룹 아래의 모든 하위 그룹에 대해 잠글 수 있습니다.

   * [새 작업 기본값](#new-task-defaults)
   * [문제](#issues)
   * [삭제](#deletion)
   * [이동](#move)
   * [실제 일자](#actual-dates)
   * [위임](#delegation)
   * [액세스](#access)

### 새 작업 기본값 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">새 작업의 시작 일자</td> 
      <td> <p>프로젝트 관리자의 새 작업에 대한 기본 시작 날짜를 결정합니다. 새 작업의 시작 일자는 프로젝트의 계획된 시작 일자 또는 작업이 생성된 날짜일 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>기간 유형 </p> </td> 
      <td> <p>리소스 수(및 할당 백분율)와 작업 기간 또는 총 작업량 간의 관계를 결정합니다. 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형: 문서 인덱스</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수익 유형</td> 
      <td> <p>작업에 대한 계획 및 실제 수익 추정치를 계산합니다. <strong>수익 유형</strong>이(가) <strong>청구할 수 없음</strong>(으)로 설정된 경우 계획된 시간과 기록된 실제 시간은 작업에 대한 예상 수익을 생성하지 않으며 작업에 대한 작업이 프로젝트 수준 수익에 기여하지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">비용 유형</td> 
      <td> <p>작업의 계획 및 실제 비용 추정치를 계산합니다. <strong>비용 없음</strong>(으)로 설정된 경우 계획된 시간과 기록된 실제 시간이 작업에 대한 계획된 또는 실제 비용 예측을 생성하지 않으며 작업에 대한 작업이 프로젝트 수준 비용에 기여하지 않습니다.</p> </td> 
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
      <td> <p>누군가 문제를 프로젝트 또는 작업으로 변환할 때 원래 문제와 변환된 프로젝트 또는 작업이 모두 해결 중인 오브젝트가 됩니다. 이 설정을 사용하면 원래 문제의 해결 방법을 해결 가능한 개체의 해결 방법에 연결할 수 있습니다. 개체 확인에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 및 해결 가능한 개체 개요 </a>을(를) 참조하십시오.</p> <p>이 설정을 적용하려면 <strong>원래 문제를 유지하고 해결 방법을 작업에 연결</strong>하는 옵션을 선택해야 합니다.</p> 
       <ul> 
        <li>이 설정을 사용하면 문제와 프로젝트 또는 작업 모두에 대해 동일한 키로 사용자 지정 상태를 만들 수 있습니다. 프로젝트 또는 작업(해결 가능한 개체)이 사용자 지정 상태로 전환되면 변경 사항은 문제의 상태도 반영합니다. 상태 키는 문제 및 프로젝트 또는 작업 상태에 대해 동일해야 합니다.</li> 
        <li>이 설정을 사용하지 않으면 해결 중 오브젝트 상태가 사용자 지정 상태가 아닌 기본 상태로 자동 설정됩니다. 기본 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스</a>를 참조하십시오.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제를 작업으로 전환할 때</td> 
      <td> <p>이 섹션의 설정은 문제에서 작업으로 전환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
       <ul> 
        <li><strong>원래 문제를 유지하고 해결 방법을 작업에 연결</strong>: 문제를 전환할 때 작업이 완료될 때까지 문제로 계속 표시됩니다. 작업이 완료되면 문제의 상태가 자동으로 [닫힘]으로 변경됩니다.</li> 
        <li><strong>기본 담당자가 작업에 액세스할 수 있도록 허용</strong>: 기본 담당자(문제 작성자)에게 작업을 검토하고 업데이트하며 진행 상황에 대한 최신 정보를 제공할 수 있는 액세스 권한을 부여합니다.</li> 
        <li> <p><strong>전환 중에 이러한 설정을 변경할 수 있도록 허용</strong>: 문제를 전환하는 사용자가 문제를 작업으로 전환하는 동안 이러한 옵션을 변경할 수 있도록 허용합니다.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제를 프로젝트로 전환할 때</td> 
      <td> <p>이 섹션의 설정은 문제에서 프로젝트로 전환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
       <ul> 
        <li><strong>원래 문제를 유지하고 해결 방법을 프로젝트에 연결</strong>: 문제를 전환할 때 프로젝트가 완료될 때까지 문제로 계속 표시됩니다. 프로젝트가 완료되면 문제의 상태가 자동으로 마감으로 변경됩니다.</li> 
        <li><strong>기본 담당자가 프로젝트에 액세스할 수 있도록 허용</strong>: 기본 담당자(문제 작성자)에게 프로젝트에 대한 액세스 권한을 부여하여 프로젝트를 검토하고 업데이트하며 진행 상황을 계속 알 수 있습니다.</li> 
        <li><strong>전환 중에 이러한 설정을 변경할 수 있도록 허용</strong>: 문제를 전환하는 사용자가 문제를 프로젝트로 전환하는 동안 나열된 옵션을 변경할 수 있도록 허용합니다.</li> 
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
      <td> <p> 시간이 기록되는 작업 또는 문제의 삭제를 허용할지 여부를 결정할 수 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.</p> 
       <div> 
        <p><b>팁</b>: 이 설정은 작업 또는 시간이 기록된 문제가 있는 프로젝트를 삭제하는 데에도 적용됩니다. 이 설정은 프로젝트에 대해 시간이 직접 기록되는 프로젝트 삭제에는 적용되지 않습니다. </p> 
        <p>다음 사항을 고려하십시오.</p> 
        <ul> 
         <li> <p>이 옵션을 선택하면 작업 또는 문제를 삭제할 때 정보 경고가 표시됩니다. 경고는 작업 또는 문제가 시간을 기록한 경우 프로젝트로 이동되거나 삭제됨을 알려줍니다. 설정의 타임시트 및 시간 환경 설정 영역에서 시간을 삭제할지 또는 프로젝트로 이동할지 여부를 구성할 수 있습니다. 경고가 표시되었는지 확인하면 작업 또는 문제가 삭제됩니다. 타임시트 및 시간 환경 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">타임시트 및 시간 환경 설정 구성</a>을 참조하십시오. </p> <p>팁: <span>시간이 기록된 작업 및 문제가 있는 프로젝트를 삭제하면 기록된 시간이 삭제되거나 설정의 타임시트 및 시간 환경 설정 영역의 설정에 따라 보존됩니다</span>. </p> </li> 
         <li><span>이 옵션을 선택 취소하면 작업 또는 시간이 기록된 문제를 삭제하거나 작업 또는 문제에 대한 시간이 기록된 프로젝트를 삭제할 때 금지 경고가 표시됩니다</span> <span>.</span> 경고는 관리자가 기록된 시간이 있는 작업 또는 문제를 삭제할 수 없도록 지정합니다. 작업, 문제<span> 또는 작업 및 문제</span>에 대해 기록된 시간이 있는 프로젝트는 삭제할 수 없습니다. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


### 이동

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자가 기록된 시간이 있는 작업 및 문제를 이동할 수 있도록 허용</td> 
      <td> <p> 시간이 기록되는 작업 또는 문제의 이동을 허용할지 여부를 결정할 수 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.</p> 
       <p>다음 사항을 고려하십시오.</p> 
        <ul> 
         <li> 이 옵션을 선택하면 시간이 기록된 작업 및 문제를 이동할 수 있습니다. 작업 또는 문제와 함께 시간도 이동합니다. </li>
      <li>이 옵션을 선택 취소하면 작업 또는 기록된 시간이 있는 문제를 이동할 때 금지 경고가 표시됩니다. 경고는 관리자가 기록된 시간이 있는 작업 또는 문제를 이동할 수 없도록 지정합니다. 시간이 기록된 작업 또는 문제는 다른 프로젝트로 이동할 수 없습니다. 이 옵션을 선택 취소한 경우에도 기록된 시간이 있는 작업을 동일한 프로젝트 내에서 이동할 수 있습니다.  </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

### 실제 일자 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업 또는 문제가 "신규"에서 "진행 중"으로 변경되면 실제 시작 일자를 다음으로 설정하십시오.</td> 
      <td> <p>작업 또는 문제가 <strong>새로 만들기</strong>에서 <strong>진행 중</strong>(으)로 진행될 때 Workfront에 실제 시작 날짜가 기록되는 경우에 대한 다음 옵션 중 하나를 선택하십시오.</p> 
       <ul> 
        <li><strong>지금:</strong> 실제 시작 날짜가 현재 날짜로 설정되어 있습니다.</li> 
        <li><strong>계획된 시작 일자:</strong> 실제 시작 일자가 작업 또는 문제의 계획된 시작 일자로 설정됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 또는 문제가 완료되면 실제 완료 일자를 다음으로 설정하십시오.</td> 
      <td> <p>작업 또는 문제가 완료될 때 Workfront에 실제 완료 일자가 기록되는 경우 다음 옵션 중 하나를 선택합니다.</p> 
       <ul> 
        <li><strong>지금:</strong> 실제 완료 날짜가 현재 날짜로 설정되어 있습니다.</li> 
        <li> <p><strong>계획된 완료 일자:</strong> 실제 완료 일자가 작업 또는 문제의 계획된 완료 일자로 설정됩니다.</p> </li> 
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

### 위임

**[!UICONTROL 사용자가 작업 및 문제를 위임하도록 허용]** 설정을 사용하면 그룹의 모든 사용자가 작업을 다른 사용자에게 임시로 위임할 수 있습니다.

이 설정을 사용하면 그룹 사용자에게 다음이 표시됩니다.

* [!UICONTROL 홈] 영역의 [!UICONTROL 내 작업], [!UICONTROL 내 작업] 또는 [!UICONTROL 내 문제] 위젯에 있는 [!UICONTROL **대리인**] 링크입니다. 여기에서 작업 및 문제 할당을 위임할 수 있습니다.

  >[!NOTE]
  >
  >  [!UICONTROL **승인 위임**] 링크는 항상 [!UICONTROL Home] 영역에서 활성화됩니다.

* 작업 또는 문제 헤더의 [!UICONTROL 할당 및 위임] 영역에서 작업 또는 문제가 다른 사용자에게 위임되었음을 나타냅니다.
* 작업 또는 문제가 [!UICONTROL Home]의 [!UICONTROL 내 작업] 위젯에서 다른 사용자에게 위임되었음을 나타냅니다.

  [!UICONTROL 사용자가 자신의 작업 및 문제를 위임하도록 허용] 설정을 사용하지 않도록 설정하면 현재 예약된 위임이 중지되고 위임된 사용자는 위임이 중지되었다는 전자 메일 알림을 받게 됩니다.

다른 사용자에게 작업을 위임하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 위임 개요](../../../manage-work/delegate-work/delegate-work-overview.md)
* [작업 및 문제 위임](../../../manage-work/delegate-work/how-to-delegate-work.md)

### 액세스 {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">누군가가 작업에 할당되었을 때</td> 
      <td> 
       <ul> 
        <li><strong>사용자에게 작업에 대한 액세스 권한을 부여합니다.</strong>: 사용자가 할당된 작업에 대해 갖는 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> 사용자에게 액세스 권한 부여</a>를 참조하십시오.</li> 
        <li> <p><strong>또한 사용자에게 프로젝트에 대한 액세스 권한을 부여합니다.</strong>: 사용자에게 작업이 할당된 프로젝트에 대한 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">누군가가 문제에 할당되었을 때</td> 
      <td> 
       <ul> 
        <li><strong>사용자에게 작업에 대한 액세스 권한을 부여합니다.</strong>: 사용자가 할당된 작업에 대해 갖는 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</li> 
        <li> <p><strong>또한 사용자에게 프로젝트에 대한 액세스 권한을 부여합니다.</strong>: 사용자에게 작업이 할당된 프로젝트에 대한 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">누군가가 요청을 제출했을 때</td> 
      <td> 
       <ul> 
        <li><strong>사용자에게 문제에 대한 액세스 권한을 부여합니다.</strong>: 사용자가 제출한 요청에 대해 갖는 기본 권한을 정의합니다. 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유</a>를 참조하십시오.</li> 
        <li> <p><strong>같은 회사의 직원들이 모든 요청에 대해 동일한 권한을 상속합니다</strong>: 사용자가 같은 회사의 다른 사용자가 제출한 요청을 볼 수 있도록 허용합니다. 이러한 요청은 제출된 자체 요청에 대한 권한과 동일한 권한을 갖습니다.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
