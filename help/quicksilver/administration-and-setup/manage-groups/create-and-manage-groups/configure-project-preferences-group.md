---
title: 그룹에 대한 프로젝트 환경 설정 구성
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 그룹 관리자이고 Adobe Workfront 관리자가 시스템의 모든 그룹에 대한 프로젝트 기본 설정을 잠금 해제하는 경우, 그룹이 생성하는 모든 후속 프로젝트에 영향을 미치도록 그룹에 대한 해당 기본 설정을 구성할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 2%

---

# 그룹에 대한 프로젝트 환경 설정 구성

그룹 관리자이고 Adobe Workfront 관리자가 시스템의 모든 그룹에 대한 프로젝트 기본 설정을 잠금 해제하는 경우, 그룹이 생성하는 모든 후속 프로젝트에 영향을 미치도록 그룹에 대한 해당 기본 설정을 구성할 수 있습니다.

관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

>[!NOTE]
>
>* 일반적으로 잠금 해제된 환경 설정은 무한정 잠금 해제된 상태로 유지됩니다. Workfront 관리자가 다시 잠근 경우 시스템 설정이 다시 적용되며 그룹 관리자가 만든 기본 설정에 대한 설정이 손실됩니다.
>* 프로젝트와 연관된 그룹에 대해 설정된 기본 설정은 프로젝트를 생성하는 사용자의 홈 그룹에 대해 설정된 기본 설정에 우선합니다.
>* 일부 그룹 수준 환경 설정은 그룹에 대해 만드는 프로젝트 템플릿에 영향을 줍니다. 자세한 내용은 섹션을 참조하십시오 [그룹 영역에서 그룹 템플릿을 보고, 작업하고, 생성할 수 있습니다](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 기사 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Workfront 관리자가 시스템 수준에서 환경 설정을 잠금 해제한 후에 이를 구성한 다음 잠금으로 잠근 후 그룹 및 해당 하위 그룹의 모든 사용자가 동일한 구성을 사용하고 있는지 확인할 수 있습니다. 이는 Workfront 관리자가 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그던 기능과 병렬입니다. 자세한 내용은 [하위 그룹에 대한 프로젝트, 작업 또는 문제 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


작업 및 문제 환경 설정, 작업표 및 시간 환경 설정에 대해 그룹 수준 구성이 가능합니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) 및 [그룹에 대한 작업표 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Workfront 관리자가 프로젝트 기본 설정의 잠금을 해제하는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## 그룹에 대해 잠금 해제된 프로젝트 환경 설정 구성

>[!TIP]
>
>Workfront 관리자의 경우, 설정 > 프로젝트 환경 설정 > 프로젝트로 이동한 다음 페이지 상단에 있는 상자에서 그룹 이름을 검색하여 1-4단계를 건너뛸 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 프로젝트 환경 설정을 구성할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **프로젝트 환경 설정**.
1. 표시되는 페이지에서 아래 나열된 4개 섹션 중 하나를 계속 수행하여 프로젝트 상태, 일정, 비즈니스 사례 및 사망 이후 기간에 대한 기본 설정을 구성합니다.

   >[!TIP]
   >
   >마우스로 기본 설정을 가리키면 도구 설명이 표시되어 잠긴 상태임을 알 수 있는 경우 Workfront 관리자에게 조직의 모든 그룹에 대해 잠금을 해제하도록 요청할 수 있습니다.

* [프로젝트 상태](#project-status)
* [타임라인](#timelines)
* [비즈니스 사례](#business-cases)
* [사후 세계](#life-after-death)

### 프로젝트 상태 {#project-status}

그룹과 연관된 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>사용자들이 템플릿 없이 프로젝트를 만들 수 있도록 허용</td>
<td><p>이 기본 설정을 사용하면 다음 영역에서 프로젝트를 만들 때 템플릿을 사용하지 않고 프로젝트를 만들 수 있습니다.</p>
<ul>
<li><p>프로젝트 목록에서 새 프로젝트 옵션 사용</p></li>

<li><p>문제의 페이지에서 문제를 프로젝트로 변환</p></li>
</ul>

<p>이 기본 설정은 시스템 수준에서 기본적으로 활성화됩니다.</p>
<p><b>메모</b></p>
<p>사용자가 다른 환경 설정을 사용하는 여러 그룹에 속해 있는 경우, 해당 그룹 중 하나 이상에 이 기본 설정이 활성화되어 있는 경우 템플릿 없이 프로젝트를 만들 수 있습니다.</p>
</td></tr>
  <tr> 
   <td role="rowheader">새 프로젝트의 상태를 다음으로 설정</td> 
   <td> <p>새 프로젝트의 상태를 확인합니다.</p> <p><b>메모</b>   
     <ul> 
      <li>사용자나 다른 Workfront 관리자가 여기에서 선택한 상태를 숨긴 경우 기본 상태가 상태 목록의 첫 번째 상태로 변경됩니다.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">그룹 프로젝트 환경 설정의 경우 잠긴 상태나 필수 상태만 기본 상태로 선택할 수 있습니다.</li> 
      <li> <p>잠긴 시스템 또는 그룹 상태가 기본 상태로 설정되고 나중에 다른 사용자가 잠금을 해제하면 시스템이 해당 상태를 동일한 상태 유형의 잠긴 상태로 바꾸려고 합니다.</p> <p>찾을 수 없는 경우 필요한 상태를 찾습니다.</p> 
       <ul> 
        <li>잠금 해제된 기본 상태와 같은 필수 상태가 있는 경우 잠금 해제되어 있더라도 필수 상태는 기본 상태가 됩니다.</li> 
        <li>필수 상태 중 잠금 해제된 기본 상태와 같은 상태가 없는 경우 상태 목록의 첫 번째 필수 상태는 기본 상태가 됩니다.</li> 
       </ul> <p>필요한 상태에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 프로젝트 상태 목록에 액세스합니다</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 작업 상태 목록에 액세스합니다</a>, 및 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 문제 상태 목록에 액세스합니다</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">완료율 계산 기준</td> 
   <td> <p>프로젝트 또는 상위 작업의 완료율은 전체 작업 진행 상태에 따라 결정됩니다. 이 정보는 프로젝트에 있는 작업의 기간 또는 계획 시간을 기반으로 계산할 수 있습니다.</p> <p>기간 을 선택하면 프로젝트에 있는 각 작업의 기간 이 프로젝트에 대한 전체 완료 퍼센트를 결정하고, 각 하위 작업의 기간 은 상위 작업에 대한 전체 완료 퍼센트를 결정합니다.</p> <p>지속 기간을 선택하는 경우 [타임라인] 섹션에서 작업일별 일반 시간 및 매주 일반 작업 일을 지정합니다. Workfront에서는 지속 시간을 기반으로 작업의 완료 비율을 계산할 때 이 정보를 사용합니다. </p> <p>계획 시간을 선택하는 경우, 각 프로젝트의 모든 태스크가 정의된 계획 시간의 양을 가지고 있고 금액이 0이 아닌지 확인합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">진행 상태를 토대로 프로젝트 상태 자동 설정</td> 
   <td> <p>이 환경 설정을 사용하면 사용자가 프로젝트의 조건(Target 시, 위험 시, 문제 발생)을 수동으로 설정하거나 Workfront에서 타임라인에서 프로젝트 진행 상태에 따라 자동으로 조건(진행 상태)을 설정하도록 할 수 있습니다. 프로젝트 조건에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">프로젝트 조건 및 조건 유형 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>자동으로 기준선 만들기</p> </td> 
   <td> <p>이 기본 설정은 프로젝트 상태가 [현재]로 변경될 때 작업 및 프로젝트 세부 정보의 기준 요소(스냅샷)를 자동으로 생성합니다. 베이스라인 작성에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">프로젝트 기준 요소 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>성과 지수 방법 </p> </td> 
   <td> <p>프로젝트에 대한 PIM(성능 인덱스 방법)은 Workfront에서 CPI(비용 성과 인덱스) 및 EAC(완료 시 추정)와 같은 획득값 지표를 계산하는 데 사용하는 방법을 제어합니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">원가 성과 지수 계산(CPI)</a>및 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">완료 시 예상 계산(EAC)</a></p> 
    <ul> 
     <li><strong>시간 기반</strong>: Workfront은 계획된 시간을 사용하여 EAC 및 CPI와 같은 성능 지표를 계산합니다. PIM이 시간을 기반으로 계산되면 EAC가 시간 수로 표시됩니다. 계획 시간 값이 0이 아닌 값이 있는지 확인합니다.</li> 
     <li> <p><strong>비용 기반</strong>: Workfront은 EAC 및 CPI와 같은 성과 지표를 계산하기 위해 계획된 인건비 비용을 사용합니다. 작업 역할이나 사용자가 시간당 비용과 연결되어 있는지 확인합니다. PIM이 비용을 기반으로 계산되면 EAC가 통화 값으로 표시됩니다.</p> <p>프로젝트 관리자는 프로젝트 세부 정보의 재무 영역을 사용하여 프로젝트 레벨에서 이 설정을 수정할 수 있습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 재무 영역의 정보 관리</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>완료 시점 예측 </p> </td> 
   <td> <p>Workfront에서 프로젝트의 예상 총 비용을 나타내는 EAC(완료 시 예상)를 계산하는 데 사용하는 데이터를 결정합니다.</p> 
    <ul> 
     <li><strong>프로젝트 수준에서 계산</strong>: 상위 태스크 및 프로젝트에 대한 EAC는 EAC 공식에 실제 시간 또는 실제 노무비를 입력하여 결정됩니다. 이 계산에는 상위 태스크 또는 프로젝트에 직접 추가된 실제 시간 또는 원가 및 비용이 포함됩니다.</li> 
     <li> <p><strong>작업/하위 작업에서 롤업</strong>: 상위 태스크 및 프로젝트에 대한 EAC는 각 하위 태스크에 대한 EAC를 합하여 결정됩니다. 이 계산에는 상위 태스크 또는 프로젝트에 직접 추가된 실제 시간 또는 실제 원가 및 비용이 제외됩니다.</p> <p>프로젝트 관리자는 프로젝트 세부 정보의 재무 영역을 사용하여 프로젝트 레벨에서 이 설정을 수정할 수 있습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 재무 영역의 정보 관리</a>.</p> </li> 
    </ul> <p>EAC 계산 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">완료 시 예상 계산(EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 타임라인 {#timelines}

그룹과 연관된 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">일정 출처:</td> 
   <td> <p>새 프로젝트를 생성했을 때 시작 날짜부터 또는 완료 날짜부터 예약할지 여부를 결정합니다.</p> 
    <ul> 
     <li><strong>시작 날짜</strong>: 새 작업은 가능한 한 빨리 작업 제약 조건으로 기본 설정되며 프로젝트 관리자에게 프로젝트에 대한 계획 시작 날짜를 제공하라는 메시지가 표시됩니다.</li> 
     <li><strong>완료 날짜</strong>: 새 태스크는 기본적으로 가능한 지연 태스크 제한으로 설정되며 프로젝트 관리자에게 프로젝트에 대한 계획 완료 일자를 제공하라는 메시지가 표시됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 휴무</td> 
   <td> <p>태스크의 기본 담당자 시간이 프로젝트에서 해당 태스크에 대한 계획 일자를 조정하는지 여부를 결정합니다.</p> 
    <ul> 
     <li> <p><strong>작업 기간의 사용자 시간 비우기 고려</strong>: 작업 1차 할당자에 대해 예약된 시간이면 작업 기간 동안 시간이 초과되면 해당 작업의 계획된 날짜를 조정합니다. 기본 설정입니다. </p> <p>예를 들어, 가능한 한 빨리 제약 조건이 있는 작업이 6월 1일에 시작하여 6월 3일에 완료되도록 예약되어 있고 기본 할당자가 6월 2일에 타임오프로 표시되어 있는 경우, 작업의 계획 날짜는 6월 1일부터 6월 4일까지 조정됩니다.</p> <p><b>중요 사항</b>: 이 설정을 선택하면 작업 기간이 변경되지 않습니다. 작업 제약 조건에 따라 계획된 날짜만 변경됩니다.</p> </li> 
     <li><strong>작업 기간의 사용자 시간 초과 무시</strong>: 작업의 기본 할당자가 해당 기간 동안 휴가가 되어도 프로젝트에 있는 각 작업의 계획 날짜는 원래 계획대로 유지됩니다.</li> 
    </ul> <p>이 설정에 대한 옵션을 선택할 때는 다음 사항을 고려하십시오.</p> 
    <ul> 
     <li>이 설정을 변경하면 변경 후 만들어진 프로젝트 및 템플릿만 업데이트된 설정을 상속합니다. </li> 
     <li> <p>작업의 작업 제한 값은 조정할 계획 작업 날짜를 결정합니다. </p> 
      <ul> 
       <li>계획된 시작 일자</li> 
       <li>계획된 완료 일자</li> 
       <li>두 날짜 모두</li> 
       <li>날짜가 아닙니다. </li> 
      </ul> <p>예를 들어, 작업에 고정 날짜의 제약 조건이 있는 경우, 작업 기간의 사용자 시간 해제 고려 옵션을 선택하더라도 기본 할당자의 시간 제한 시기를 조정하지 않습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">작업 제한 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트 타임라인은 자동으로 다시 계산됩니다</strong> </p> </td> 
   <td> <p>프로젝트의 타임라인이 다시 계산되는 시기를 결정합니다. 프로젝트 타임라인 재계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>.</p> <p>다음 옵션은 기본적으로 활성화되어 있습니다. 다음 설정 중 하나 이상을 선택할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>매일 밤</strong>: 매일 밤 프로젝트 일정을 다시 계산하려면 이 옵션을 선택합니다. 타임라인에 영향을 줄 수 있는 프로젝트의 모든 변경 사항이 즉시 표시되지 않습니다. Workfront​​​은 다음 조건이 모두 충족되는 프로젝트에 대해서만 야간에 타임라인을 다시 계산합니다.</p> <p> 
       <ul> 
        <li>현재 상태 있음</li> 
        <li>지난 3개월 동안 최신 정보를 얻었습니다</li> 
       </ul> </p> </li> 
     <li> <p><strong>프로젝트의 범위가 변경되는 경우</strong>: 프로젝트 범위가 변경될 때 프로젝트 타임라인을 즉시 다시 계산하려면 이 옵션을 선택합니다. 프로젝트 범위 변경을 구성하는 사항에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>여러 사용자가 작업에 할당되면</strong> </p> </td> 
   <td> <p>프로젝트에 일정이 할당되지 않았거나 해당 작업에 할당된 사용자에게 일정이 할당되지 않은 경우 Workfront에서는 시스템 기본 일정을 사용하여 작업의 타임라인을 계산합니다.</p> <p>프로젝트에 있는 동일한 작업에 여러 사용자를 지정하는 경우 작업에 지정된 예약이 있고 작업에 할당된 사용자도 예약을 갖고 있는 경우 Workfront에서는 다음 일정을 사용합니다.</p> 
    <ul> 
     <li><strong>기본 지정</strong>: Workfront은 작업에 1차 할당 일정을 사용하여 타임라인을 계산합니다.</li> 
     <li><strong>프로젝트</strong>: Workfront은 프로젝트 일정을 사용하여 각 작업의 타임라인을 계산합니다.</li> 
    </ul> <p>예약에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">예약 만들기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>타임라인 계산 </p> </td> 
   <td> 
    <ul> 
     <li><strong>업무일 기준 시간</strong>: 프로젝트에서 작업할 사용자의 일반적인 작업 시간을 설정합니다. 기본값은 8시간입니다.</li> 
    </ul> 
    <ul> 
     <li><strong>주간 일반 근무 일수</strong>: 프로젝트에 종사할 사용자를 위해 표준 근무제를 설정하라. 기본값은 5일입니다.</li> 
    </ul> <p>이 2개 옵션은 일을 시간으로 변환하거나 주를 일로 변환합니다.</p> <p>예를 들어, 8개의 계획 시간 작업이 있고 지속 시간이 계획 시간을 기반으로 계산되는 경우, Workfront은 기간을 일로 표시하기 위해 해당 시간을 일로 변환합니다.</p> <p>Workfront은 일반 주당 근무 일수 필드에서 시스템의 FTE(Full Time Equivalent) 값을 계산합니다. Workfront이 사용자에 대한 할당을 계산할 때 사용하는 것입니다.</p> <p>이 값은 프로젝트 타임라인을 계획하거나, 리소스에 대한 예산을 책정하는 경우 또는 프로젝트에 대한 시간을 로깅하는 데 사용됩니다. </p> <p>이 작업표는 다음에 설명된 대로 시스템에 있는 사용자의 작업표를 설정할 때 사용되지 않습니다. <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">작업표 및 시간 환경 설정 구성</a>.</p> <p><b>참고</b>: Workfront 관리자는 타임라인 계산 환경 설정을 잠금 해제할 수 없습니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>사용자 정의 영역</strong> </p> </td> 
   <td> <p>프로젝트에서 작업할 사용자에 대한 사용자 지정 연간 분기를 구성합니다. 사용자 지정 분기는 일반적으로 달력 연도 동안 기존 분기 분류와 일치하지 않는 분기입니다. 여러 사용자 지정 분기를 추가할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">프로젝트에 대한 사용자 지정 분기 활성화</a>.</p> <p><b>참고</b>: Workfront 관리자는 사용자 지정 분기 기본 설정의 잠금을 해제할 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 비즈니스 사례 {#business-cases}

그룹과 연관된 새로 생성된 프로젝트에 대한 비즈니스 사례를 생성하여 프로젝트 요청을 제출할 수 있습니다. 환경 설정을 정의하여 **비즈니스 사례** 양식. Portfolio 최적화 프로그램과 같은 다른 도구가 제대로 업데이트되도록 이러한 옵션을 활성화하는 것이 좋습니다. 각 필드에 표시되는 내용에 대한 자세한 내용은 [비즈니스 사례 정의](../../../manage-work/projects/define-a-business-case/define-business-case.md).

그러면 Workfront 관리자가 비즈니스 사례에서 섹션을 활성화하면 프로젝트 소유자가 프로젝트 수준에서 비즈니스 사례를 생성할 수 있습니다. 비즈니스 사례 생성에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### 사후 세계  {#life-after-death}

그룹과 연관된 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트가 완료로 표시된 후에도 사용자는 여전히 다음을 수행할 수 있습니다</strong> </p> </td> 
   <td> <p>프로젝트 상태가 완료로 표시된 후 태스크나 문제를 삭제할 수 있는지 여부에 대한 조직(또는 그룹에 대한 프로젝트 환경 설정을 구성하는 경우 그룹)의 규칙을 결정합니다.</p> 
    <ul> 
     <li><strong>작업 삭제</strong>: 프로젝트가 완료됨으로 표시된 후 프로젝트에서 작업을 삭제할 수 있습니다.<br></li> 
     <li><strong>삭제 문제</strong>: 프로젝트가 완료 로 표시된 후 프로젝트에서 문제를 삭제할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>프로젝트가 완료, 사용 중지 또는 승인 보류 중으로 표시된 후에도 사용자는 여전히</strong> </p> </td> 
   <td> <p>프로젝트 상태가 표시된 후 프로젝트의 작업, 문제, 문서 및 기타 개체에 대해 발생하는 작업에 대한 조직(또는 그룹에 대한 프로젝트 환경 설정을 구성하는 경우 그룹)의 규칙을 결정합니다 <strong>완료</strong>, <strong>데드</strong>, 또는 <strong>승인 보류 중</strong>.</p> 
    <ul> 
     <li><strong>작업 추가 및 편집</strong> 사용자가 다음을 수행할 수 있습니다. 
      <ul> 
       <li>프로젝트가 완료, 완료 또는 승인 보류 중으로 표시된 후 프로젝트 내의 작업을 편집합니다. 여기에는 시간 추가 및 작업 비용 항목 변경이 포함됩니다.</li> 
       <li>프로젝트에 작업을 추가합니다.</li> 
      </ul></li> 
     <li><strong>문제 추가 및 편집</strong>: 사용자가 다음을 수행할 수 있습니다. 
      <ul> 
       <li>프로젝트가 완료, 완료 또는 승인 보류 중으로 표시된 후 프로젝트 내의 문제를 편집합니다.</li> 
       <li>프로젝트가 완료 또는 없음으로 표시된 후 프로젝트에 문제를 추가합니다. (승인 보류 중인 프로젝트에 문제를 추가할 수 없습니다.)</li> 
      </ul></li> 
     <li> <p><strong>프로젝트 및 해당 작업 및 문제에 문서 추가</strong>: 프로젝트가 완료 또는 없음으로 표시된 후 프로젝트에 문서를 추가하거나 프로젝트 내의 작업 및 문제에 문서를 추가할 수 있습니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
     <li> <p><strong>템플릿 첨부</strong>: 프로젝트가 완료 또는 없음으로 표시된 후 프로젝트에 템플릿을 첨부할 수 있습니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
