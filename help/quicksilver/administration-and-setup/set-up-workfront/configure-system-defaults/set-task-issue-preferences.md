---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 시스템 전체 작업 및 문제 환경 설정 구성
description: 작업 및 문제에 대한 시스템 차원의 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 사용자가 Workfront에서 작업 및 문제를 만드는 방식에 영향을 줍니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# 시스템 전체 작업 및 문제 환경 설정 구성

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

로서의 [!DNL Adobe Workfront] 관리자는 작업 및 문제에 대해 시스템 차원의 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 사용자가 작업 및 문제를 만드는 방식에 영향을 줍니다 [!DNL Workfront].

기본적으로 작업 및 문제 환경 설정은 잠겨 있으며 그룹 관리자는 시스템 전체의 모든 그룹에 대해 잠금을 해제하지 않으면 그룹 수준에서 수정할 수 없습니다. 자세한 내용은 섹션을 참조하십시오 [그룹에 대한 작업 잠금 및 문제 환경 설정](#lock-task-and-issue-preferences-for-groups) 참조하십시오.

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 의 모든 사용자에 대한 작업 및 문제 환경 설정 구성 [!DNL Workfront]

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 환경 설정]** >**[!UICONTROL 작업 및 문제].**

1. 표시되는 페이지에서 아래의 5개 섹션 중 하나를 계속 진행하여 설정을 구성합니다 [!UICONTROL 새 작업 기본값], [!UICONTROL 문제], [!UICONTROL 삭제], [!UICONTROL 실제 날짜], 및 [!UICONTROL 액세스].
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

* [[!UICONTROL 새 작업 기본값]](#new-task-defaults)
* [[!UICONTROL 문제]](#issues)
* [[!UICONTROL 삭제]](#deletion)
* [[!UICONTROL 실제 일자]](#actual-dates)
* [[!UICONTROL 위임]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL 액세스]](#access)

### [!UICONTROL 새 작업 기본값] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 작업의 시작 날짜]</td> 
   <td> <p>프로젝트 관리자의 새 작업에 대한 기본 시작 날짜를 결정합니다. 새 작업의 시작 날짜는 프로젝트의 계획 시작 날짜이거나 작업이 생성된 날짜일 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 기간 유형] </p> </td> 
   <td> <p>자원 수(및 해당 할당 퍼센트)와 작업의 기간 또는 총 투입 사이의 관계를 결정합니다. 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Revenue Type]</td> 
   <td> <p>작업에 대한 계획 및 실제 매출 예측을 계산합니다. 이 <strong>[!UICONTROL Revenue Type]</strong> 가 로 설정되어 있습니다.<strong>[!UICONTROL 과금 불가]</strong>, 계획된 시간과 실제 기록된 시간은 작업에 대한 예상 수익을 생성하지 않으며, 작업에 대한 작업은 프로젝트 레벨 매출에 기여하지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 비용 유형]</td> 
   <td> <p>태스크에 대한 계획 및 실제 원가 예측을 계산합니다. 로 설정된 경우 <strong>[!UICONTROL 비용 없음]</strong>그리고 계획 시간 및 기록된 실제 시간은 작업에 대한 계획 또는 실제 예상 비용을 생성하지 않으며, 작업 작업이 프로젝트 레벨 원가에 기여하지 않습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 문제 {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 해결 상태가 변경될 때 해결 가능한 문제 상태를 자동으로 업데이트합니다.]</td> 
   <td> <p>문제가 프로젝트나 작업으로 변환되면 원래 문제와 변환된 프로젝트 또는 작업이 모두 개체를 해결할 수 있습니다. 이 설정을 사용하면 원래 문제의 해결 방법을 해결할 수 있는 개체의 해결책과 상호 연관시킬 수 있습니다. 개체 해결에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> <p>이 설정이 어떤 영향을 주려면 <strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결합니다.]</strong> 을 선택해야 합니다.</p> 
    <ul> 
     <li>이 설정이 활성화되면 문제와 프로젝트 또는 작업 모두에 대해 동일한 키로 사용자 지정 상태를 만들 수 있습니다. 프로젝트나 작업(해결 가능한 개체)이 사용자 지정 상태로 전환되면 변경 내용은 문제의 상태도 반영합니다. 문제 및 프로젝트 또는 작업 상태에 대해 상태 키는 동일해야 합니다.</li> 
     <li>이 설정을 비활성화하면 사용자 지정 상태 대신 개체 상태를 자동으로 기본 상태로 설정합니다. 기본 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스합니다</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>문제를 작업으로 변환할 때]</td> 
   <td> <p>이 섹션의 설정은 문제 대비 변환 프로세스 중에 발생하는 작업을 결정합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 작업에 연결합니다.]</strong>: 문제를 변환하면 작업이 완료될 때까지 문제가 계속 표시됩니다. 작업이 완료되면 문제 상태가 자동으로 [!UICONTROL Closed]로 변경됩니다. 이 옵션을 선택 취소하면 문제가 삭제됩니다.</p> <p><b>메모</b>:  <p>문제에 대한 액세스 권한 또는 삭제 권한이 없는 사용자는 이 설정의 상태에 관계없이 변환 중인 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL 기본 연락처가 작업에 액세스할 수 있도록 허용]</strong>: 작업을 검토하고 업데이트하며 진행 상황을 계속 파악할 수 있도록 작업에 대한 기본 연락처(문제 생성자) 액세스 권한을 제공합니다.</li> 
     <li> <p><strong>[!UICONTROL 전환 중에 이러한 설정을 변경할 수 있도록 허용합니다.]</strong>: 문제를 작업으로 변환하는 동안 문제를 변환한 사용자가 이러한 옵션을 변경할 수 있도록 해줍니다.</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제를 프로젝트로 변환할 때]</td> 
   <td> <p>이 섹션의 설정은 문제 및 프로젝트에서 프로젝트로 변환 프로세스 중에 발생하는 상황을 결정합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 원래 문제를 유지하고 해결 방법을 프로젝트에 연결합니다.]</strong>: 문제를 변환하면 프로젝트가 완료될 때까지 문제로 계속 표시됩니다. 프로젝트가 완료되면 문제 상태가 [!UICONTROL Closed]로 자동으로 변경됩니다. 이 옵션을 선택 취소하면 문제가 삭제됩니다. </p> <p><b>메모</b>:  <p>문제에 대한 액세스 권한 또는 삭제 권한이 없는 사용자는 이 설정의 상태에 관계없이 변환 중인 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL 기본 연락처가 프로젝트에 액세스할 수 있도록 허용]</strong>: 프로젝트에 대한 기본 연락처(문제 생성자) 액세스 권한을 제공하여 프로젝트를 검토하고 업데이트하며 진행 상황을 계속 파악할 수 있습니다.</li> 
     <li><strong>[!UICONTROL 전환 중에 이러한 설정을 변경할 수 있도록 허용합니다.]</strong>: 문제를 프로젝트로 변환하는 동안 나열된 옵션을 변경할 수 있도록 문제를 변환하는 사용자가 허용합니다.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 삭제] {#deletion}

**[!UICONTROL 사용자가 로그된 시간 관련 작업 및 문제를 삭제할 수 있도록 허용]**: 작업이 삭제되도록 허용할지 또는 시간이 기록되는 문제를 삭제하도록 허용할지 결정할 수 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.

>[!TIP]
>
>이 설정은 작업 또는 로그된 시간 내에 문제가 있는 프로젝트를 삭제하는 경우에도 적용됩니다. 이 설정은 프로젝트에 대해 시간이 직접 기록되는 프로젝트를 삭제하는 경우에는 적용되지 않습니다.

* 이 옵션을 선택하면 작업이나 문제를 삭제할 때 정보 경고가 표시됩니다. 경고에 따르면 작업이나 문제가 로그된 시간이 있으면 해당 작업이 프로젝트로 이동되거나 삭제된다는 메시지가 나타납니다. 에서 시간을 삭제할지 아니면 프로젝트로 이동할지를 구성할 수 있습니다 [!UICONTROL 작업표 및 시간 기본 설정] 의 영역 [!UICONTROL 설정]. 경고 메시지가 표시되는지 확인하면 작업이나 문제가 삭제됩니다. 작업표 및 시간 기본 설정 구성에 대한 자세한 내용은 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >로그된 시간이 있는 작업 및 문제가 있는 프로젝트를 삭제하면 기록된 시간이 삭제되거나 의 설정에 따라 보존됩니다 [!UICONTROL 작업표 및 시간 기본 설정] 영역 [!UICONTROL 설정]. 프로젝트를 삭제할 때 경고 메시지가 표시되지 않습니다.

* 이 옵션을 선택 해제하면 작업을 삭제하거나 로그된 시간 문제를 해결할 때 또는 해당 작업이나 문제에 대해 기록된 시간이 있는 프로젝트를 삭제할 때 금지 경고가 표시됩니다. 이 경고는 관리자가 로그된 시간 관련 작업 또는 문제를 삭제할 수 없도록 허용한다는 것을 나타냅니다. 작업 및 문제에 대해 로그된 시간이 있는 작업, 문제 또는 프로젝트는 삭제할 수 없습니다.

### [!UICONTROL 실제 일자] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업이나 문제가 "새로 만들기"에서 "진행 중"으로 변경되면 실제 시작 날짜를 로 설정합니다.]</td> 
   <td> <p>실제 시작 일자가 기록될 때 다음 옵션 중 하나를 선택합니다 [!DNL Workfront] 작업 또는 문제가 <strong>[!UICONTROL New]</strong> to <strong>[!UICONTROL In Progress]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 실제 시작 일자는 현재 일자로 설정됩니다.</li> 
     <li><strong>[!UICONTROL 계획된 시작 날짜]:</strong> 실제 시작 일자는 태스크 또는 문제의 계획 시작 일자로 설정됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 또는 문제가 완료되면 실제 완료 날짜를 로 설정합니다.]</td> 
   <td> <p>실제 완료 일자가 기록될 경우 다음 옵션 중 하나를 선택합니다 [!DNL Workfront] 작업 또는 문제가 완료되면</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 실제 완료 일자는 현재 일자로 설정됩니다.</li> 
     <li> <p><strong>[!UICONTROL 계획된 완료 날짜]:</strong> 실제 완료 일자는 태스크 또는 출고 계획 완료 일자로 설정됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 위임

활성화 [!UICONTROL 사용자가 작업 및 문제를 위임할 수 있도록 허용] 을 설정하면 의 모든 사용자가 일시적으로 다른 사용자에게 작업을 위임할 수 있습니다.

이 설정을 사용하면 다음을 볼 수 있습니다.

* 다음 [!UICONTROL 위임] 링크 [!UICONTROL 홈] 영역. 여기에서 승인 또는 작업 및 문제 지정을 위임할 수 있습니다.
* 작업 또는 문제가 [!UICONTROL 지정 및 위임] 작업 또는 문제 헤더의 영역.

을 비활성화하는 경우 [!UICONTROL 사용자가 작업 및 문제를 위임할 수 있도록 허용] 설정을 지정하면 현재 예약된 위임이 중지되고 위임된 사용자는 위임이 중지되었다는 이메일 알림을 받게 됩니다.

다른 사람에게 작업을 위임하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 개요 위임](../../../manage-work/delegate-work/delegate-work-overview.md)
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
   <td role="rowheader">[!UICONTROL 작업이 할당되면]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 사용자에게 작업에 대한 액세스 권한을 제공합니다..]</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</li> 
     <li> <p><strong>[!UICONTROL 프로젝트에 대한 액세스 권한도 부여합니다..]</strong>: 사용자에게 할당된 작업이 있는 프로젝트에 대한 사용자의 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제에 지정된 경우]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 사용자에게 작업에 대한 액세스 권한을 제공합니다..]</strong>: 사용자가 할당된 작업에 대한 기본 권한을 정의합니다. 작업 권한에 대한 자세한 내용은<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</li> 
     <li> <p><strong>[!UICONTROL 프로젝트에 대한 액세스 권한도 부여합니다..]</strong>: 사용자에게 할당된 작업이 있는 프로젝트에 대한 사용자의 기본 권한을 정의합니다. 프로젝트 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자가 요청을 제출할 때]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 사용자에게 문제에 대한 액세스 권한을 제공합니다..]</strong>: 사용자가 제출한 요청에 대한 기본 권한을 정의합니다. 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a>.</li> 
     <li> <p><strong>[!UICONTROL 동일한 회사의 사람은 모든 요청에 대해 동일한 권한을 상속합니다.]</strong>: 사용자는 동일한 회사의 다른 사용자가 제출한 요청을 볼 수 있습니다. 보유한 요청 수와 동일한 권한이 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 그룹에 대한 작업 잠금 및 문제 환경 설정 {#lock-task-and-issue-preferences-for-groups}

조직의 그룹이 고유한 워크플로우에 대해 다르게 구성된 작업 또는 문제 환경 설정이 필요한 경우 조직의 모든 그룹에 대한 환경 설정을 잠금 해제하여 그룹이 자체적으로 구성할 수 있습니다. 기본 설정이 잠금 해제되어 그룹 관리자가 변경하면 그룹과 연관된 작업이나 문제는 시스템 수준 설정 대신 기본 설정에 대한 그룹 수준 설정의 영향을 받습니다.

그룹 관리자가 그룹에 대한 작업 및 문제 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>후 [!DNL Workfront] 관리자는 시스템 수준에서 기본 설정을 잠금 해제하면 모든 그룹 관리자가 해당 설정을 구성한 다음 잠근 후 해당 그룹의 모든 사람과 아래 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이것은 [!DNL Workfront] 관리자는 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그어야 합니다. 자세한 내용은 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 및 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

그룹이 구성할 수 있도록 작업 또는 문제 환경 설정을 잠그거나 잠금 해제하려면 다음을 수행하십시오

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 작업 및 문제]**.

1. 다음 중 하나를 수행합니다.

   * 그룹 아래 그룹의 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 그룹 잠금을 해제하십시오 ![](assets/unlock-toggle-button.png).
   * 사용자 그룹 및 이 그룹 아래의 모든 그룹이 기본 설정에 대한 구성을 사용하려면 구성이 잠겼는지(기본값) 확인합니다.

      >[!IMPORTANT]
      >
      >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리하도록 시스템 전체에서 관리자 및 그룹의 사용자와 통신하는 것이 좋습니다. 잠글 때 시스템의 모든 그룹에 의해 구성이 상속됩니다. 그리고 특정 기간 동안 기본 설정 잠금이 해제되어 있으면 해당 그룹 관리자가 만들 수 있는 구성 대신

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
