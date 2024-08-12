---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 시스템 전체 작업 및 문제 환경 설정 구성
description: 작업 및 문제에 대한 시스템 전체 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 사용자가 Workfront에서 작업 및 문제를 만드는 방식에 영향을 줍니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '2074'
ht-degree: 0%

---

# 시스템 전체에서 작업 및 문제 환경 설정 구성하기

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

[!DNL Adobe Workfront] 관리자는 작업 및 문제에 대한 시스템 전체 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 사용자가 [!DNL Workfront]에서 작업 및 문제를 만드는 방식에 영향을 줍니다.

기본적으로 작업 및 문제 환경 설정은 잠겨 있으며 그룹 관리자는 시스템 전체의 모든 그룹에 대해 잠금을 해제하지 않으면 그룹 수준에서 수정할 수 없습니다. 자세한 내용은 이 문서의 [그룹에 대한 작업 및 문제 환경 설정 잠금](#lock-task-and-issue-preferences-for-groups) 섹션을 참조하십시오.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront]의 모든 사용자에 대한 작업 및 문제 환경 설정 구성

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 환경 설정]** >**[!UICONTROL 작업 및 문제]을 클릭합니다.**

1. 표시되는 페이지에서 아래 나열된 5개 섹션 중 하나를 계속 진행하여 [!UICONTROL 새 작업 기본값], [!UICONTROL 문제], [!UICONTROL 삭제], [!UICONTROL 실제 날짜] 및 [!UICONTROL 액세스]에 대한 설정을 구성합니다.

   * [[!UICONTROL 새 작업 기본값]](#new-task-defaults)
   * [[!UICONTROL 문제]](#issues)
   * [[!UICONTROL 삭제]](#deletion)
   * [[!UICONTROL 실제 날짜]](#actual-dates)
   * [[!UICONTROL 위임]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">작업</a> </li>
  —&gt;

* [[!UICONTROL 액세스]](#access)

### [!UICONTROL 새 작업 기본값] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
    <td> <p>프로젝트 관리자의 새 작업에 대한 기본 시작 날짜를 결정합니다. 새 작업의 시작 일자는 프로젝트의 계획된 시작 일자 또는 작업이 생성된 날짜일 수 있습니다.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL 기간 유형] </p> </td> 
    <td> <p>리소스 수(및 할당 백분율)와 작업 기간 또는 총 작업량 간의 관계를 결정합니다. 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형</a>을 참조하세요.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>작업에 대한 계획 및 실제 수익 추정치를 계산합니다. <strong>[!UICONTROL Revenue Type]</strong>이(가) <strong>[!UICONTROL Not Billable]</strong>(으)로 설정된 경우 계획된 시간과 기록된 실제 시간은 작업에 대한 예상 수익을 생성하지 않으며 작업에 대한 작업이 프로젝트 수준 매출에 기여하지 않습니다.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 비용 유형]</td> 
    <td> <p>작업의 계획 및 실제 비용 추정치를 계산합니다. <strong>[!UICONTROL No Cost]</strong>(으)로 설정된 경우 계획된 시간과 기록된 실제 시간이 작업에 대한 계획된 또는 실제 비용 예측을 생성하지 않으며 작업에 대한 작업이 프로젝트 수준 비용에 기여하지 않습니다.</p> </td> 
    </tr> 
  </tbody> 
</table>

### 문제 {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL 해결 중 오브젝트의 상태가 변경되면 해결 가능한 문제 상태를 자동으로 업데이트]</td> 
    <td> <p>누군가 문제를 프로젝트 또는 작업으로 변환할 때 원래 문제와 변환된 프로젝트 또는 작업이 모두 해결 중인 오브젝트가 됩니다. 이 설정을 사용하면 원래 문제의 해결 방법을 해결 가능한 개체의 해결 방법에 연결할 수 있습니다. 개체 확인에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 및 해결 가능한 개체 개요 </a>을(를) 참조하십시오.</p> <p>이 설정을 적용하려면 <strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업]</strong>에 연결하는 옵션을 선택해야 합니다.</p> 
      <ul> 
      <li>이 설정을 사용하면 문제와 프로젝트 또는 작업 모두에 대해 동일한 키로 사용자 지정 상태를 만들 수 있습니다. 프로젝트 또는 작업(해결 가능한 개체)이 사용자 지정 상태로 전환되면 변경 사항은 문제의 상태도 반영합니다. 상태 키는 문제 및 프로젝트 또는 작업 상태에 대해 동일해야 합니다.</li> 
      <li>이 설정을 사용하지 않으면 해결 중 오브젝트 상태가 사용자 지정 상태가 아닌 기본 상태로 자동 설정됩니다. 기본 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스</a>를 참조하십시오.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 문제를 작업으로 전환할 때]</td> 
    <td> <p>이 섹션의 설정은 문제에서 작업으로 전환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결]</strong>: 문제를 전환할 때 작업이 완료될 때까지 문제로 계속 표시됩니다. 작업이 완료되면 문제의 상태가 자동으로 [!UICONTROL Closed](으)로 변경됩니다. 이 옵션을 선택 취소하면 문제가 삭제됩니다.</p> <p><b>참고</b>:  <p>문제를 삭제할 수 있는 액세스 또는 권한이 없는 사용자는 이 설정의 상태에 관계없이 문제를 전환할 때 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL 기본 담당자가 작업에 액세스할 수 있도록 허용]</strong>: 기본 담당자(문제 작성자)에게 작업에 대한 보기 액세스 권한을 부여하여 작업을 검토하고 진행 상황을 계속 알려주며 작업의 업데이트 섹션에 주석을 답니다.</li> 
      <li> <p><strong>[!UICONTROL 전환 중에 이러한 설정을 변경할 수 있도록 허용]</strong>: 문제를 전환하는 사용자가 문제를 작업으로 전환하는 동안 이러한 옵션을 변경할 수 있도록 허용합니다.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 문제를 프로젝트로 전환할 때]</td> 
    <td> <p>이 섹션의 설정은 문제에서 프로젝트로 전환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 프로젝트에 연결]</strong>: 문제를 전환할 때 프로젝트가 완료될 때까지 문제로 계속 표시됩니다. 프로젝트가 완료되면 문제의 상태가 자동으로 [!UICONTROL Closed](으)로 변경됩니다. 이 옵션을 선택 취소하면 문제가 삭제됩니다. </p> <p><b>참고</b>:  <p>문제를 삭제할 수 있는 액세스 또는 권한이 없는 사용자는 이 설정의 상태에 관계없이 문제를 전환할 때 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL 기본 담당자가 프로젝트에 액세스할 수 있도록 허용]</strong>: 기본 담당자(문제 작성자)에게 프로젝트에 대한 보기 액세스 권한을 부여하여 프로젝트를 검토하고 진행 상황을 계속 알려주며 프로젝트의 업데이트 섹션에 주석을 답니다.</li> 
      <li><strong>[!UICONTROL 전환 중에 이러한 설정을 변경할 수 있도록 허용]</strong>: 문제를 전환하는 사용자가 문제를 프로젝트로 전환하는 동안 나열된 옵션을 변경할 수 있도록 허용합니다.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL 삭제] {#deletion}

**[!UICONTROL 사용자가 기록된 시간이 있는 작업 및 문제를 삭제할 수 있도록 허용]**: 시간이 기록된 작업 또는 문제의 삭제를 허용할지 여부를 결정할 수 있도록 해줍니다. 이 옵션은 기본적으로 선택되어 있습니다.

>[!TIP]
>
>이 설정은 작업 또는 시간이 기록된 문제가 있는 프로젝트 삭제에도 적용됩니다. 이 설정은 프로젝트에 대해 시간이 직접 기록되는 프로젝트 삭제에는 적용되지 않습니다.

* 이 옵션을 선택하면 작업 또는 문제를 삭제할 때 정보 경고가 표시됩니다. 경고는 작업 또는 문제가 시간을 기록한 경우 프로젝트로 이동되거나 삭제됨을 알려줍니다. [!UICONTROL 설정]의 [!UICONTROL 타임시트 및 시간 환경 설정] 영역에서 시간을 삭제할지 또는 프로젝트로 이동할지 여부를 구성할 수 있습니다. 경고가 표시되었는지 확인하면 작업 또는 문제가 삭제됩니다. 타임시트 및 시간 환경 설정 구성에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

  >[!TIP]
  >
  >시간이 기록된 작업 및 문제가 있는 프로젝트를 삭제하면 기록된 시간이 삭제되거나 [!UICONTROL 설정]의 [!UICONTROL 타임시트 및 시간 환경 설정] 영역에 있는 설정에 따라 유지됩니다. 프로젝트를 삭제할 때 경고 메시지가 표시되지 않습니다.

* 이 옵션을 선택 취소하면 작업 또는 시간이 기록된 문제를 삭제하거나 작업 또는 문제에 대한 시간이 기록된 프로젝트를 삭제할 때 금지 경고가 표시됩니다. 경고는 관리자가 기록된 시간이 있는 작업 또는 문제를 삭제할 수 없도록 지정합니다. 작업, 문제 또는 작업 및 문제에 대한 시간이 기록된 프로젝트는 삭제할 수 없습니다.

### [!UICONTROL 실제 날짜] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL 작업 또는 문제가 "신규"에서 "진행 중"으로 변경되면 실제 시작 일자를](으)로 설정합니다.</td> 
    <td> <p>작업 또는 문제가 <strong>[!UICONTROL New]</strong>에서 <strong>[!UICONTROL In Progress]</strong>(으)로 이동할 때 실제 시작 날짜가 [!DNL Workfront]에 기록되는 경우 다음 옵션 중 하나를 선택하십시오.</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> 실제 시작 날짜가 현재 날짜로 설정되어 있습니다.</li> 
      <li><strong>[!UICONTROL 계획된 시작 일자]:</strong> 실제 시작 일자가 작업 또는 문제의 계획된 시작 일자로 설정됩니다.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 작업 또는 문제가 완료되면 실제 완료 일자를](으)로 설정하십시오.</td> 
    <td> <p>작업 또는 문제가 완료될 때 실제 완료 날짜가 [!DNL Workfront]에 기록되는 경우 다음 옵션 중 하나를 선택하십시오.</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> 실제 완료 날짜가 현재 날짜로 설정되어 있습니다.</li> 
      <li> <p><strong>[!UICONTROL 계획된 완료 일자]:</strong> 실제 완료 일자가 작업 또는 문제의 계획된 완료 일자로 설정됩니다.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### 위임

**[!UICONTROL 사용자가 자신의 작업 및 문제를 위임하도록 허용]** 설정을 사용하면 의 모든 사용자가 자신의 작업을 다른 사용자에게 임시로 위임할 수 있습니다.

이 설정을 사용하면 사용자에게 다음이 표시됩니다.

* [!UICONTROL Home] 영역의 [!UICONTROL Delegate] 링크 여기에서 승인 또는 작업 및 문제 할당을 위임할 수 있습니다.
* 작업 또는 문제 헤더의 [!UICONTROL 할당 및 위임] 영역에서 작업 또는 문제가 다른 사용자에게 위임되었음을 나타냅니다.

  [!UICONTROL 사용자가 자신의 작업 및 문제를 위임하도록 허용] 설정을 사용하지 않도록 설정하면 현재 예약된 위임이 중지되고 위임된 사용자는 위임이 중지되었다는 이메일 알림을 받게 됩니다.

다른 사용자에게 작업을 위임하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 위임 개요](../../../manage-work/delegate-work/delegate-work-overview.md)
* [작업 및 문제 위임 관리](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL 액세스] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL 누군가가 작업에 할당되었을 때]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL 사용자에게 작업에 대한 액세스 권한을 부여합니다...]</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</li> 
      <li> <p><strong>[!UICONTROL 또한 사용자에게 프로젝트에 대한 액세스 권한을 부여]</strong>: 사용자에게 작업이 할당된 프로젝트에 대한 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 누군가가 문제에 할당되었을 때]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL 사용자에게 작업에 대한 액세스 권한을 부여합니다...]</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>를 참조하십시오.</li> 
      <li> <p><strong>[!UICONTROL 또한 사용자에게 프로젝트에 대한 액세스 권한을 부여]</strong>: 사용자에게 작업이 할당된 프로젝트에 대한 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 누군가가 요청을 제출했을 때]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL 사용자에게 문제에 대한 액세스 권한 부여]</strong>: 사용자가 제출한 요청에 대해 갖는 기본 권한을 정의합니다. 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a>를 참조하십시오.</li> 
      <li> <p><strong>[!UICONTROL 같은 회사의 직원들은 모든 요청에 대해 동일한 권한을 상속합니다]</strong>: 사용자가 같은 회사의 다른 사용자가 제출한 요청을 볼 수 있도록 허용합니다. 이러한 요청은 제출된 자체 요청에 대한 권한과 동일한 권한을 갖습니다.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 그룹에 대한 작업 및 문제 환경 설정 잠금 {#lock-task-and-issue-preferences-for-groups}

조직의 그룹에서 고유한 워크플로우에 대해 다르게 구성된 작업 또는 문제 환경 설정이 필요한 경우 조직 전체에서 모든 그룹에 대한 환경 설정을 잠금 해제하여 그룹 스스로 구성할 수 있습니다. 환경 설정이 잠금 해제되고 그룹 관리자가 수정할 때 그룹과 관련된 작업 또는 문제는 시스템 수준 설정 대신 환경 설정에 대한 그룹 수준 설정의 영향을 받습니다.

그룹 관리자가 그룹에 대한 작업 및 문제 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

>[!NOTE]
>
>[!DNL Workfront] 관리자가 시스템 수준에서 환경 설정을 잠금 해제하면 모든 그룹 관리자가 이를 구성한 다음 잠가 그룹의 모든 사용자와 아래의 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이는 [!DNL Workfront] 관리자가 시스템 내의 모든 사용자에 대한 환경 설정을 구성하고 잠그는 기능과 비슷합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)를 참조하십시오.

그룹이 구성할 수 있도록 작업 또는 문제 환경 설정을 잠그거나 잠금 해제하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 작업 및 문제]**&#x200B;를 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 그룹 아래의 그룹 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 ![](assets/unlock-toggle-button.png) 잠금을 해제하세요.
   * 그룹 및 그 아래의 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 해당 그룹이 잠겨 있는지 확인합니다(기본값).

     >[!IMPORTANT]
     >
     >모든 요구 사항이 잠긴 기본 설정을 구성하는 방식으로 처리되도록 시스템 전체에서 그룹 관리자 및 사용자와 통신하는 것이 좋습니다. 이 구성을 잠그면 시스템의 모든 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 그룹 관리자가 수행했을 수 있는 설정을 대체합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
