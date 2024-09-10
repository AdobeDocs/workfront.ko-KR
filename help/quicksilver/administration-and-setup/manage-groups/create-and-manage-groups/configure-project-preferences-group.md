---
title: 그룹에 대한 프로젝트 환경 설정 구성
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 그룹 관리자인 경우 Adobe Workfront 관리자가 시스템의 모든 그룹에 대한 프로젝트 기본 설정의 잠금을 해제하면 그룹에서 만드는 모든 후속 프로젝트에 영향을 주도록 해당 그룹에 대한 기본 설정을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '2648'
ht-degree: 2%

---

# 그룹에 대한 프로젝트 환경 설정 구성

그룹 관리자인 경우 Adobe Workfront 관리자가 시스템의 모든 그룹에 대한 프로젝트 기본 설정의 잠금을 해제하면 그룹에서 만드는 모든 후속 프로젝트에 영향을 주도록 해당 그룹에 대한 기본 설정을 구성할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

>[!NOTE]
>
>* 일반적으로 잠금 해제된 환경 설정은 무기한 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 설정한 기본 설정이 손실됩니다.
>* 프로젝트와 관련된 그룹에 대해 설정된 환경 설정은 프로젝트를 작성하는 사용자의 홈 그룹에 대해 설정된 환경 설정보다 우선합니다.
>* 일부 그룹 수준 환경 설정은 그룹에 대해 만드는 프로젝트 템플릿에 영향을 줍니다. 자세한 내용은 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md) 문서의 [그룹 영역에서 그룹의 템플릿 보기, 작업 및 만들기](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 섹션을 참조하십시오.
>
>* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제한 후 구성한 다음 잠궈 그룹 및 하위 그룹의 모든 사용자가 동일한 구성을 사용하도록 할 수 있습니다. 이는 Workfront 관리자가 시스템 내의 모든 사용자에 대한 환경 설정을 구성하고 잠그는 기능과 병행됩니다. 자세한 내용은 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)를 참조하십시오.
>

작업 및 문제 환경 설정, 타임시트 및 시간 환경 설정에 대해서도 그룹 수준 구성이 가능합니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) 및 [그룹에 대한 타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)을 참조하십시오.

Workfront 관리자가 프로젝트 환경 설정을 잠금 해제하는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)를 참조하십시오.

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

## 그룹에 대해 잠금 해제된 프로젝트 환경 설정 구성

>[!TIP]
>
>Workfront 관리자인 경우 설정 > 프로젝트 환경 설정 > 프로젝트로 이동한 다음 페이지 상단에 있는 상자에서 그룹 이름을 검색하여 단계 1-4를 우회할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

1. 프로젝트 환경 설정을 구성할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **프로젝트 환경 설정**&#x200B;을 클릭합니다.
1. 표시되는 페이지에서 아래 나열된 4개 섹션 중 하나를 계속 진행하여 프로젝트 상태, 타임라인, 비즈니스 사례 및 사망 후 삶에 대한 환경 설정을 구성합니다.

   >[!TIP]
   >
   >환경 설정 위로 마우스를 가져가면 도구 설명이 표시되어 잠겨 있음을 알려주는 경우, Workfront 관리자에게 조직의 모든 그룹에 대해 잠금을 해제하도록 요청할 수 있습니다.

* [프로젝트 상태](#project-status)
* [타임라인](#timelines)
* [비즈니스 사례](#business-cases)
* [사후 세계](#life-after-death)

### 프로젝트 상태 {#project-status}

그룹과 관련하여 새로 생성된 프로젝트에 대해 다음 환경 설정 중 하나를 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>사용자들이 템플릿 없이 프로젝트를 만들 수 있도록 허용</td>
<td><p>이 환경 설정을 통해 사용자는 다음 영역에서 프로젝트를 만들 때 템플릿을 사용하지 않고 프로젝트를 만들 수 있습니다.</p>
<ul>
<li><p>프로젝트 목록에서 새 프로젝트 옵션 사용</p></li>

<li><p>문제의 페이지에서 문제를 프로젝트로 전환</p></li>
</ul>

<p>이 환경 설정은 시스템 수준에서 기본적으로 활성화됩니다.</p>
<p><b>메모</b></p>
<p>사용자가 환경 설정이 다른 여러 그룹에 속해 있는 경우 그룹 중 하나 이상에서 이 환경 설정이 활성화된 경우 템플릿 없이 프로젝트를 만들 수 있습니다.</p>
</td></tr>
  <tr> 
   <td role="rowheader">새 프로젝트의 상태를 다음으로 설정</td> 
   <td> <p>새 프로젝트의 상태를 확인합니다.</p> <p><b>참고</b>   
     <ul> 
      <li>귀하 또는 다른 Workfront 관리자가 여기에서 선택한 상태를 숨기는 경우, 기본 상태가 상태 목록의 첫 번째 상태로 변경됩니다.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">그룹 프로젝트 환경 설정의 경우 잠김 상태 또는 필수 상태만 기본 상태로 선택할 수 있습니다.</li> 
      <li> <p>잠긴 시스템 또는 그룹 상태가 기본 상태로 설정되어 있고 나중에 누군가가 잠금을 해제하면 시스템은 동일한 상태 유형의 잠긴 상태로 대체하려고 합니다.</p> <p>찾을 수 없는 경우 필수 상태를 찾습니다.</p> 
       <ul> 
        <li>잠금 해제된 기본 상태와 동일한 필수 상태가 있는 경우 잠금 해제된 경우에도 필수 상태가 기본 상태가 됩니다.</li> 
        <li>필요한 상태 중 잠금 해제된 기본 상태와 일치하는 상태가 없으면 상태 목록의 첫 번째 필수 상태가 기본 상태가 됩니다.</li> 
       </ul> <p>필수 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 프로젝트 상태 목록 액세스</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 작업 상태 목록 액세스</a> 및 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 문제 상태 목록 액세스</a> 문서를 참조하십시오.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">다음을 기반으로 완료율 계산</td> 
   <td> <p>프로젝트 또는 상위 작업의 완료율은 작업의 전체 진행 상황을 기반으로 합니다. 이 정보는 프로젝트에 대한 작업의 기간 또는 계획된 시간을 기반으로 계산할 수 있습니다.</p> <p>기간 을 선택하면 프로젝트에 있는 각 작업의 기간에 따라 프로젝트의 전체 완료율이 결정되고 각 하위 작업의 기간에 따라 상위 작업의 전체 완료율이 결정됩니다.</p> <p>기간 을 선택하는 경우 타임라인 섹션에서 근무일당 일반 근로시간 및 주당 일반 근로일을 지정해야 합니다. Workfront은 기간을 기준으로 작업의 완료율을 계산할 때 이 정보를 사용합니다. </p> <p>계획된 시간을 선택하는 경우 각 프로젝트의 모든 작업에 정의된 계획된 시간의 양이 있고 금액이 0이 아닌지 확인합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">진행 상태를 토대로 프로젝트 상태 자동 설정</td> 
   <td> <p>이 환경 설정을 통해 사용자는 프로젝트의 상태를 수동으로(타깃에 있음, 위험에 있음, 문제에 있음) 설정하거나 Workfront이 타임라인에서 프로젝트의 진행에 따라 상태(진행 상태)를 자동으로 설정하도록 할 수 있습니다. 프로젝트 상태에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">프로젝트 상태 및 상태 유형 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>자동으로 기준선 만들기</p> </td> 
   <td> <p>이 환경 설정은 프로젝트의 상태가 현재로 변경될 때 작업 및 프로젝트 세부 정보의 기준선(스냅샷)을 자동으로 만듭니다. 기준선 만들기에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">프로젝트 기준선 만들기</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>성과 지수 방법 </p> </td> 
   <td> <p>프로젝트에 대한 성과 지수 방법(PIM)은 Workfront이 원가 성과 지수(CPI) 및 완료 시 추정(EAC)과 같은 성과 가치 지표를 계산하는 데 사용하는 방법을 제어합니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">CPI(비용 성과 지수) 계산</a>및 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">EAC(완료 시 추정 비용) 계산</a>을 참조하십시오.</p> 
    <ul> 
     <li><strong>시간 기반</strong>: Workfront은 계획된 시간을 사용하여 EAC 및 CPI와 같은 성능 지표를 계산합니다. PIM이 시간을 기반으로 계산되면 EAC는 시간을 나타내는 숫자로 표시됩니다. 0이 아닌 계획된 시간 값이 있는지 확인합니다.</li> 
     <li> <p><strong>비용 기반</strong>: Workfront은 계획된 인건비를 사용하여 EAC 및 CPI와 같은 성과 지표를 계산합니다. 작업 역할 또는 사용자가 시간당 비용 요율과 연결되어 있는지 확인합니다. PIM이 비용을 기반으로 계산되면 EAC는 통화 값으로 표시됩니다.</p> <p>프로젝트 관리자는 프로젝트 세부 정보의 재무 영역을 사용하여 프로젝트 수준에서 이 설정을 수정할 수 있습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 재무 영역의 정보 관리</a>를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>완료 시점 예측 </p> </td> 
   <td> <p>Workfront에서 프로젝트의 예상 총 비용을 나타내는 EAC(완료 시 추정 비용)를 계산하는 데 사용하는 데이터를 결정합니다.</p> 
    <ul> 
     <li>상위 작업 및 프로젝트에 대한 <strong>프로젝트 수준에서 계산</strong>:EAC는 EAC 수식에 실제 시간 또는 실제 인건비를 입력하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간 또는 비용 및 비용이 포함됩니다.</li> 
     <li> <p><strong>작업/하위 작업에서 롤업</strong>: 상위 작업 및 프로젝트에 대한 EAC는 각 하위 작업에 대한 EAC를 합하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간 또는 실제 비용 및 경비가 제외됩니다.</p> <p>프로젝트 관리자는 프로젝트 세부 정보의 재무 영역을 사용하여 프로젝트 수준에서 이 설정을 수정할 수 있습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 재무 영역의 정보 관리</a>를 참조하십시오.</p> </li> 
    </ul> <p>EAC가 계산되는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">EAC(완료 시 추정 비용) 계산</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 타임라인 {#timelines}

그룹과 관련하여 새로 생성된 프로젝트에 대해 다음 환경 설정 중 하나를 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">일정 기준</td> 
   <td> <p>새 프로젝트를 만들 때 시작 일자 또는 완료 일자에서 예약할지 여부를 결정합니다.</p> 
    <ul> 
     <li><strong>시작 날짜</strong>: 새 작업의 기본값은 가능한 한 빨리 작업 제한으로 설정되며 프로젝트 관리자에게 프로젝트의 계획된 시작 날짜를 입력하라는 메시지가 표시됩니다.</li> 
     <li><strong>완료 날짜</strong>: 새 작업의 기본값은 가능한 한 늦은 작업 제한으로 설정되며 프로젝트 관리자에게 프로젝트의 계획된 완료 날짜를 입력하라는 메시지가 표시됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 휴무</td> 
   <td> <p>작업의 기본 할당자의 휴무 시간이 프로젝트의 해당 작업에 대한 계획된 일자를 조정하는지 여부를 결정합니다.</p> 
    <ul> 
     <li> <p><strong>작업 기간에서 사용자 휴무를 고려하십시오</strong>: 작업의 기본 피할당자에 대해 예약된 휴무는 작업 기간 동안 휴무가 발생하는 경우 작업의 계획된 일자를 조정합니다. 기본 설정입니다. </p> <p>예를 들어, '가능한 한 빨리'라는 제한이 있는 작업이 6월 1일에 시작하여 6월 3일에 완료되도록 예약되어 있고 기본 피할당자가 6월 2일에 휴무로 표시된 경우, 작업의 계획된 일자는 6월 1일부터 6월 4일까지로 조정됩니다.</p> <p><b>중요</b>: 이 설정을 선택하면 작업 기간이 변경되지 않습니다. 계획된 일자만 작업 제한에 따라 변경됩니다.</p> </li> 
     <li><strong>작업 기간에서 사용자 휴무 무시</strong>: 작업의 기본 피할당자가 작업 기간 동안 휴무하더라도 프로젝트에 있는 각 작업의 계획된 일자는 원래 계획된 일자에 그대로 유지됩니다.</li> 
    </ul> <p>이 설정에 대한 옵션을 선택할 때는 다음 사항을 고려하십시오.</p> 
    <ul> 
     <li>이 설정을 변경하면 변경 후에 만들어진 프로젝트 및 템플릿만 업데이트된 설정을 상속합니다. </li> 
     <li> <p>작업의 작업 제한 값에 따라 조정할 계획 작업 날짜가 결정됩니다. </p> 
      <ul> 
       <li>계획된 시작 일자</li> 
       <li>계획된 완료 일자</li> 
       <li>두 날짜 모두</li> 
       <li>두 날짜 모두. </li> 
      </ul> <p>예를 들어 작업에 고정 날짜 제한이 있는 경우 작업 기간에서 사용자 휴가 고려 옵션을 선택하더라도 기본 할당자가 휴가를 갖는 경우에는 날짜가 조정되지 않습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">작업 제한 개요</a>를 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트 타임라인이 자동으로 다시 계산됩니다</strong> </p> </td> 
   <td> <p>프로젝트의 타임라인이 언제 다시 계산되는지 결정합니다. 프로젝트 타임라인을 다시 계산하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>을 참조하십시오.</p> <p>다음 옵션은 기본적으로 활성화되어 있습니다. 다음 설정 중 하나 이상을 선택할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>매일 밤</strong>: 매일 밤 프로젝트 타임라인을 다시 계산하려면 이 항목을 선택하십시오. 타임라인에 영향을 줄 수 있는 프로젝트에 대한 변경 사항은 즉시 표시되지 않습니다. Workfront​​​은 다음 조건이 모두 충족되는 프로젝트에 대해서만 야간 타임라인을 다시 계산합니다.</p> <p> 
       <ul> 
        <li>현재 상태</li> 
        <li>지난 3개월 동안 업데이트가 있었습니다.</li> 
       </ul> </p> </li> 
     <li> <p><strong>프로젝트의 범위가 변경되면</strong>: 프로젝트 범위가 변경되면 프로젝트 타임라인을 즉시 다시 계산하려면 이 항목을 선택하십시오. 프로젝트 범위 변경을 구성하는 항목에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>을 참조하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>작업에 여러 사용자가 할당되면 </strong>의 일정을 사용합니다. </p> </td> 
   <td> <p>프로젝트에 할당된 일정이 없거나 작업에 할당된 사용자에게 할당된 일정이 없는 경우 Workfront은 시스템 기본 일정을 사용하여 작업의 타임라인을 계산합니다.</p> <p>프로젝트에 있는 동일한 작업에 여러 명의 사용자를 할당하면 할당된 일정이 있고 작업에 할당된 사용자에게도 할당된 일정이 있는 경우 Workfront은 다음 일정을 사용합니다.</p> 
    <ul> 
     <li><strong>기본 할당</strong>: Workfront에서는 작업에 대한 기본 할당의 일정을 사용하여 타임라인을 계산합니다.</li> 
     <li><strong>프로젝트</strong>: Workfront에서는 프로젝트 일정을 사용하여 각 작업의 타임라인을 계산합니다.</li> 
    </ul> <p>일정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">일정 만들기</a>를 참조하세요.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>타임라인 계산 </p> </td> 
   <td> 
    <ul> 
     <li><strong>일반 근무일 시간</strong>: 프로젝트를 작업할 사용자의 일반 근무일 시간을 설정합니다. 기본값은 8시간입니다.</li> 
    </ul> 
    <ul> 
     <li><strong>주당 일반 근무일</strong>: 프로젝트에서 작업할 사용자에 대한 표준 주간을 설정합니다. 기본값은 5일입니다.</li> 
    </ul> <p>이 두 가지 옵션은 일을 시간으로, 또는 주를 일로 변환합니다.</p> <p>예를 들어, 8개의 계획된 시간이 있는 작업이 있고 기간이 계획된 시간을 기반으로 계산되는 경우 Workfront은 기간을 일로 표시하기 위해 해당 시간을 일로 변환합니다.</p> <p>Workfront은 일반적인 주당 근무일 필드에서 시스템의 FTE(Full Time Equivalent) 값을 계산합니다. Workfront이 사용자에 대한 할당을 계산할 때 사용하는 것입니다.</p> <p>이러한 값은 프로젝트 타임라인, 리소스 예산 책정 또는 프로젝트에 대한 시간을 기록할 때 사용됩니다. </p> <p><a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">타임시트 및 시간 환경 설정 구성</a>에 설명된 대로 시스템에서 사용자에 대한 타임시트를 설정할 때는 사용되지 않습니다.</p> <p><b>참고</b>: Workfront 관리자는 타임라인 계산 기본 설정을 잠금 해제할 수 없습니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>사용자 지정 분기</strong> </p> </td> 
   <td> <p>프로젝트에서 작업할 사용자를 위해 사용자 정의 연간 분기를 구성하십시오. 사용자 정의 분기는 일반적으로 한 해 동안의 기존 분기 분류와 일치하지 않는 분기입니다. 여러 개의 사용자 정의 영역을 추가할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">프로젝트에 대한 사용자 지정 분기 사용</a>을 참조하세요.</p> <p><b>참고</b>: Workfront 관리자는 사용자 지정 분기 환경 설정을 잠금 해제할 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 비즈니스 사례 {#business-cases}

그룹과 관련하여 새로 생성된 프로젝트에 대한 비즈니스 사례를 만들어 프로젝트 요청을 제출할 수 있습니다. 환경 설정을 정의하여 **비즈니스 사례** 양식에 표시되는 영역을 결정할 수 있습니다. Portfolio 최적화 프로그램과 같은 다른 도구가 제대로 업데이트되도록 이러한 옵션을 활성화하는 것이 좋습니다. 각 필드에 표시되는 내용에 대한 자세한 내용은 [비즈니스 사례 정의: 문서 색인](../../../manage-work/projects/define-a-business-case/define-business-case.md)을 참조하세요.

Workfront 관리자가 비즈니스 사례에 대한 섹션을 활성화하면 프로젝트 소유자가 프로젝트 수준에서 비즈니스 사례를 만들 수 있습니다. 비즈니스 사례 만들기에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하세요.

### 사후 세계  {#life-after-death}

그룹과 관련하여 새로 생성된 프로젝트에 대해 다음 환경 설정 중 하나를 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트가 완료로 표시된 후에도 사용자는 </strong>할 수 있습니다. </p> </td> 
   <td> <p>프로젝트 상태가 완료로 표시된 후 작업 또는 문제를 삭제할 수 있는지 여부와 관련하여 조직(그룹에 대한 프로젝트 환경 설정을 구성하는 경우 그룹)에 대한 규칙을 결정합니다.</p> 
    <ul> 
     <li><strong>작업 삭제</strong>: 프로젝트가 완료로 표시된 후 사용자가 프로젝트에서 작업을 삭제할 수 있도록 허용합니다.<br></li> 
     <li><strong>문제 삭제</strong>: 프로젝트가 완료로 표시된 후 사용자가 프로젝트에서 문제를 삭제할 수 있도록 허용합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트가 완료, 중단 또는 승인 보류 중으로 표시된 후에도 사용자는 여전히</strong>할 수 있습니다. </p> </td> 
   <td> <p>프로젝트 상태가 <strong>완료</strong>, <strong>중단</strong> 또는 <strong>승인 보류 중</strong>으로 표시된 후 프로젝트의 작업, 문제, 문서 및 기타 개체에 어떤 일이 발생하는지 조직(그룹에 대한 프로젝트 환경 설정을 구성하는 경우)에 대한 규칙을 결정합니다.</p> 
    <ul> 
     <li><strong>작업 추가 및 편집</strong>을 통해 사용자는 다음을 수행할 수 있습니다. 
      <ul> 
       <li>프로젝트가 완료, 중단 또는 승인 보류 중으로 표시된 후 프로젝트 내에서 작업을 편집합니다. 여기에는 작업에 대한 시간 추가 및 경비 항목 변경이 포함됩니다.</li> 
       <li>프로젝트에 작업을 추가합니다.</li> 
      </ul></li> 
     <li><strong>문제 추가 및 편집</strong>: 사용자가 다음을 수행할 수 있도록 허용: 
      <ul> 
       <li>프로젝트가 완료, 중단 또는 승인 보류 중으로 표시된 후 프로젝트 내의 문제를 편집합니다.</li> 
       <li>프로젝트가 완료 또는 정지됨으로 표시된 후 프로젝트에 문제를 추가하십시오. (승인 보류 중인 프로젝트에는 문제를 추가할 수 없습니다.)</li> 
      </ul></li> 
     <li> <p><strong>프로젝트와 프로젝트 작업 및 문제에 문서 추가</strong>: 프로젝트가 완료 또는 정지됨으로 표시된 후 사용자가 프로젝트에 문서를 추가하거나 프로젝트 내의 작업 및 문제에 문서를 추가할 수 있습니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
     <li> <p><strong>템플릿 첨부</strong>: 프로젝트가 완료 또는 정지됨으로 표시된 후 사용자가 프로젝트에 템플릿을 첨부할 수 있도록 허용합니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
