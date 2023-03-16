---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 시스템 전체 프로젝트 환경 설정 구성
description: 로서의 [!DNL Adobe Workfront] 관리자는 시스템 전체에서 생성된 모든 프로젝트에 대한 기본 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 프로젝트, 작업 및 문제 동작에 영향을 줍니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2509'
ht-degree: 1%

---

# 시스템 전체 프로젝트 환경 설정 구성

로서의 [!DNL Adobe Workfront] 관리자는 시스템 전체에서 생성된 모든 프로젝트에 대한 기본 환경 설정을 구성할 수 있습니다. 이러한 환경 설정은 프로젝트, 작업 및 문제 동작에 영향을 줍니다.

>[!NOTE]
>
>기본적으로 이러한 환경 설정은 잠겨 있으며 그룹 관리자는 시스템 전체의 모든 그룹에 대해 잠금을 해제하지 않으면 그룹 수준에서 수정할 수 없습니다. 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## 전체 조직에 대한 프로젝트 환경 설정 구성

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 프로젝트]**.

1. 표시되는 페이지에서 아래의 4개 섹션 중 하나를 계속 진행하여 다음에 대한 환경 설정을 구성합니다 [!UICONTROL 프로젝트 상태], [!UICONTROL 타임라인], [!UICONTROL 비즈니스 사례], 및 [!UICONTROL 죽음 후의 인생].
1. 조직 전체에서 모든 그룹이 동일한 프로젝트 환경 설정을 사용하도록 하려면 각 기본 설정이 잠겼는지 확인하십시오 ![](assets/lock-toggle-button.png) (기본값입니다.)

   >[!IMPORTANT]
   >
   >프로젝트 기본 설정이 잠기면 해당 기본 설정에 대한 변경 사항이 시스템의 모든 그룹에 의해 상속됩니다. 프로젝트 환경 설정을 구성하는 방식으로 모든 요구 사항을 고려해야 하는지 조직 전체에서 사용자 및 그룹과 통신하는 것이 중요합니다.

   모든 그룹이 자체적으로 기본 설정을 구성하고 관리할 수 있도록 기본 설정의 잠금을 해제하는 방법에 대한 자세한 내용은 [시스템의 모든 그룹에 대한 프로젝트 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

* [[!UICONTROL 프로젝트 상태]](#project-status)
* [[!UICONTROL 타임라인]](#timelines)
* [[!UICONTROL 비즈니스 사례]](#business-cases)
* [[!UICONTROL 사후 세계]](#life-after-death)

### 프로젝트 상태 {#project-status}

시스템 전체에서 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자가 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용]</td> 
   <td>  <p>이 기본 설정을 사용하면 다음 영역에서 프로젝트를 만들 때 템플릿을 사용하지 않고 프로젝트를 만들 수 있습니다. </p>
      <ul>
        <li>
        <p>프로젝트 목록에서 [!UICONTROL 새 프로젝트] 옵션 사용</p>
        </li>
          <li>
          <p>문제의 페이지에서 문제를 프로젝트로 변환</p>
          </li>
         </ul>
        <p>이 기본 설정은 기본적으로 활성화되어 있습니다. </p> 
        <p><b>메모</b></p>
        <p> 그룹 관리자는 그룹에 대한 이 기본 설정을 변경할 수 있습니다. 사용자가 다른 환경 설정을 사용하는 여러 그룹에 속해 있는 경우, 홈 그룹에 이 기본 설정이 활성화되어 있으면 템플릿 없이 프로젝트를 만들 수 있습니다.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL 새 프로젝트의 상태를 로 설정]</td> 
   <td> <p>새 프로젝트의 상태를 확인합니다.</p>  <p><b>메모</b>  
     <ul> 
      <li>만약 [!DNL Workfront] 관리자는 여기에서 선택한 상태를 숨기고, 기본 상태는 상태 목록의 첫 번째 상태로 변경됩니다.</li> 
     </ul> 
     <ul> 
      <li> <p>잠긴 시스템 또는 그룹 상태가 기본 상태로 설정되고 나중에 다른 사용자가 잠금을 해제하면 시스템이 해당 상태를 동일한 상태 유형의 잠긴 상태로 바꾸려고 합니다.</p> <p>찾을 수 없는 경우 필요한 상태를 찾습니다.</p> 
       <ul> 
        <li>잠금 해제된 기본 상태와 같은 필수 상태가 있는 경우 잠금 해제되어 있더라도 필수 상태는 기본 상태가 됩니다.</li> 
        <li>필수 상태 중 잠금 해제된 기본 상태와 같은 상태가 없는 경우 상태 목록의 첫 번째 필수 상태는 기본 상태가 됩니다.</li> 
       </ul> <p>필요한 상태에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 프로젝트 상태 목록에 액세스합니다</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 작업 상태 목록에 액세스합니다</a>, 및 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">시스템 문제 상태 목록에 액세스합니다</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 완료율 계산 기준]</td> 
   <td> <p>프로젝트 또는 상위 작업의 완료율은 전체 작업 진행 상태에 따라 결정됩니다. 이 정보는 프로젝트에 있는 작업의 기간 또는 계획 시간을 기반으로 계산할 수 있습니다.</p> <p>[!UICONTROL 기간]을 선택하면 프로젝트에 있는 각 작업의 기간이 프로젝트에 대한 전체 완료 퍼센트를 결정하고, 각 하위 작업의 기간은 상위 작업에 대한 전체 완료 퍼센트를 결정합니다.</p> <p>[!UICONTROL Duration]을 선택하는 경우 [!UICONTROL Timelines] 섹션에서 [!UICONTROL Common Hours] 및 [!UICONTROL Typical Workbench]를 작업일에 지정합니다. [!DNL Workfront] 작업 완료율을 기간 기준으로 계산할 때 이 정보를 사용합니다. </p> <p>[!UICONTROL Planning Hours]를 선택하는 경우 각 프로젝트의 모든 작업이 [!UICONTROL Planning Hours]의 크기가 정의되어 있고 금액이 0이 아닌지 확인합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 진행 상태에 따라 프로젝트의 조건을 자동으로 설정합니다.]</td> 
   <td> <p>이 기본 설정을 사용하면 프로젝트의 [!UICONTROL 조건]을 수동으로([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trol]) 설정하거나 [!DNL Workfront] 타임라인에서 프로젝트의 진행 상태를 기반으로 자동으로 [!UICONTROL 조건](진행 상태)을 설정합니다. 프로젝트 조건에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">프로젝트 조건 및 조건 유형 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 자동으로 기준선 만들기]</p> </td> 
   <td> <p>이 기본 설정은 프로젝트 상태가 [!UICONTROL Current]로 변경될 때 작업 및 프로젝트 세부 정보의 기준 요소(스냅샷)를 자동으로 만듭니다. 베이스라인 작성에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">프로젝트 기준 요소 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>프로젝트에 대한 PIM(성능 인덱스 메서드)이 메서드를 제어합니다 [!DNL Workfront] 는 [!UICONTROL Cost Performance Index] (CPI) 및 [!UICONTROL Estimate At Completion] (EAC)과 같은 획득값 지표를 계산하는 데 사용됩니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Cost Performance Index] 계산(CPI)</a> 및 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 완료 시 예상 계산] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] 는 [!UICONTROL Planning Hours]를 사용하여 EAC 및 CPI와 같은 성능 지표를 계산합니다. PIM이 시간을 기반으로 계산되면 EAC가 시간 수로 표시됩니다. [!UICONTROL Planning Hours]에 0이 아닌 값이 있는지 확인합니다.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] 는 [!UICONTROL Planning Labor Cost]를 사용하여 EAC 및 CPI와 같은 성능 지표를 계산합니다. 작업 역할이나 사용자가 시간당 비용과 연결되어 있는지 확인합니다. PIM이 비용을 기반으로 계산되면 EAC가 통화 값으로 표시됩니다.</p> <p>프로젝트 관리자는 [!UICONTROL 프로젝트 세부 사항]의 [!UICONTROL Finance] 영역을 사용하여 프로젝트 수준에서 이 설정을 수정할 수 있습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 [!UICONTROL Finance] 영역의 정보 관리</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 완료 시 예상</p> </td> 
   <td> <p>어떤 데이터를 판별할지 결정합니다 [!DNL Workfront] 는 프로젝트의 예상 총 비용을 나타내는 [!UICONTROL 완료 시 예상 비용](EAC)을 계산하는 데 사용됩니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 프로젝트 수준에서 계산]</strong>: 상위 작업 및 프로젝트의 EAC는 EAC Formula에 [!UICONTROL 실제 시간] 또는 [!UICONTROL 실제 인건비]를 입력하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 [!UICONTROL 실제 시간] 또는 [!UICONTROL 비용 및 비용]이 포함됩니다.</li> 
     <li> <p><strong>[!UICONTROL 작업/하위 작업에서 롤업]</strong>: 상위 태스크 및 프로젝트에 대한 EAC는 각 하위 태스크에 대한 EAC를 합하여 결정됩니다. 이 계산에서는 상위 작업 또는 프로젝트에 직접 추가된 [!UICONTROL 실제 시간] 또는 [!UICONTROL 실제 비용 및 비용]을 제외합니다.</p> <p>프로젝트 관리자는 [!UICONTROL Project Details]의 [!UICONTROL Finance] 영역을 사용하여 프로젝트 수준에서 이 설정을 수정할 수 있습니다.자세한 내용은 다음을 참조하십시오 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">프로젝트 [!UICONTROL Finance] 영역의 정보 관리</a>.</p> </li> 
    </ul> <p>EAC 계산 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Estimate At Completion] 계산(EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 타임라인 {#timelines}

시스템 전체에서 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>새 프로젝트를 생성했을 때 시작 날짜부터 또는 완료 날짜부터 예약할지 여부를 결정합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 시작 날짜]</strong>: 새 작업은 기본적으로 [!UICONTROL 가능한 한 빨리] 작업 제약 조건이 되고 프로젝트 관리자에게 프로젝트에 대한 [!UICONTROL 계획 시작 날짜]를 제공하라는 메시지가 표시됩니다.</li> 
     <li><strong>[!UICONTROL 완료 날짜]</strong>: 새 작업은 기본적으로 [!UICONTROL As Late As A Possible] 작업 제약 조건으로 설정되고 프로젝트 관리자에게 프로젝트에 대한 [!UICONTROL 계획 완료 날짜]를 제공하라는 메시지가 표시됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용 시간 초과]</td> 
   <td> <p>태스크의 기본 담당자 시간이 프로젝트에서 해당 태스크에 대한 계획 일자를 조정하는지 여부를 결정합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 작업 기간의 사용자 시간 초과를 고려합니다.]</strong>: 작업 1차 할당자에 대해 예약된 시간이면 작업 기간 동안 시간이 초과되면 해당 작업의 계획된 날짜를 조정합니다. 기본 설정입니다. </p> <p>예를 들어, [!UICONTROL 가능한 한 빨리] 제약 조건이 있는 작업이 6월 1일에 시작되도록 예약되어 6월 3일에 완료되며, 기본 할당자가 6월 2일에 타임오프로 표시된 경우, 작업의 계획 날짜는 6월 1일부터 6월 4일까지 조정됩니다.</p> <p><b>중요 사항</b>: 이 설정을 선택하면 작업 기간이 변경되지 않습니다. 작업 제약 조건에 따라 계획된 날짜만 변경됩니다.</p> </li> 
     <li><strong>[!UICONTROL 작업 기간의 사용자 시간 초과 무시]</strong>: 작업의 기본 할당자가 해당 기간 동안 휴가가 되어도 프로젝트에 있는 각 작업의 계획 날짜는 원래 계획대로 유지됩니다.</li> 
    </ul> <p>이 설정에 대한 옵션을 선택할 때는 다음 사항을 고려하십시오.</p> 
    <ul> 
     <li>이 설정을 변경하면 변경 후 만들어진 프로젝트 및 템플릿만 업데이트된 설정을 상속합니다. </li> 
     <li> <p>작업의 작업 제한 값은 조정할 계획 작업 날짜를 결정합니다. </p> 
      <ul> 
       <li>계획된 시작 일자</li> 
       <li>계획된 완료 일자</li> 
       <li>두 날짜 모두</li> 
       <li>날짜가 아닙니다. </li> 
      </ul> <p>예를 들어, 작업에 [!UICONTROL 고정 날짜] 제한이 있는 경우 [!UICONTROL 작업 기간 내 사용자 시간 초과 고려] 옵션이 선택되어 있어도 기본 할당자가 시간 초과인 경우에는 날짜가 조정되지 않습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">작업 제한 개요</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 프로젝트 타임라인은 자동으로 다시 계산됩니다.]</p> </td> 
   <td> <p>프로젝트의 타임라인이 다시 계산되는 시기를 결정합니다. 프로젝트 타임라인 재계산에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>.</p> <p>다음 옵션은 기본적으로 활성화되어 있습니다. 다음 설정 중 하나 이상을 선택할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 매일 밤]</strong>: 매일 밤 프로젝트 일정을 다시 계산하려면 이 옵션을 선택합니다. 타임라인에 영향을 줄 수 있는 프로젝트의 모든 변경 사항이 즉시 표시되지 않습니다. [!DNL Workfront​​​] 다음 조건이 모두 충족되는 프로젝트에 대해서만 타임라인을 야간에 다시 계산합니다.</p> <p> 
       <ul> 
        <li>상태가 [!UICONTROL Current]입니다.</li> 
        <li>지난 3개월 동안 최신 정보를 얻었습니다</li> 
        <li>다음 중 하나의 업데이트 유형이 있습니다.</li>
        <ul>
        <li>자동 및 변경 시</li>
        <li>변경만</li>
        <li>자동만</li> 
      </ul>       
    <b>팁</b>
    <p>업데이트 유형의 수동 버전만 있는 프로젝트는 이 설정의 영향을 받지 않습니다.</p>
    <li> <p><strong>프로젝트의 범위가 변경되는 경우</strong>: 프로젝트 범위가 변경될 때 프로젝트 타임라인을 즉시 다시 계산하려면 이 옵션을 선택합니다. 프로젝트 범위 변경을 구성하는 사항에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">프로젝트 타임라인 다시 계산</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 작업에 여러 사용자가 할당되면</p> </td> 
   <td> <p>프로젝트에 일정이 할당되지 않았거나 해당 작업에 할당된 사용자에게 일정이 할당되지 않은 경우 [!DNL Workfront] 시스템 기본 일정을 사용하여 작업의 타임라인을 계산합니다.</p> <p>프로젝트에서 동일한 작업에 여러 사용자를 지정하는 경우 작업에 할당된 일정이 있고 작업에 할당된 사용자도 할당된 일정이 있는 경우—[!UICONTROL Workfront]에서는 다음 일정을 사용합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 기본 할당]</strong>: [!DNL Workfront] 작업에 1차 지정 일정을 사용하여 타임라인을 계산합니다.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] 에서는 프로젝트의 일정을 사용하여 각 작업의 타임라인을 계산합니다.</li> 
    </ul> <p>예약에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">예약 만들기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 타임라인 계산] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 업무당 일반적인 시간]</strong>: 프로젝트에서 작업할 사용자의 일반적인 작업 시간을 설정합니다. 기본값은 8시간입니다.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL 매주 일반적인 일 수]</strong>: 프로젝트에 종사할 사용자를 위해 표준 근무제를 설정하라. 기본값은 5일입니다.</li> 
    </ul> <p>이 2개 옵션은 일을 시간으로 변환하거나 주를 일로 변환합니다.</p> <p>예를 들어, 8개의 계획 시간 작업이 있고, 기간이 계획 시간을 기준으로 계산되는 경우, [!DNL Workfront] 기간을 일로 표시하기 위해 해당 시간을 일로 변환합니다.</p> <p>일반 [!UICONTROL 주당 근무 일수] 필드에서 [!DNL Workfront] 시스템의 FTE(Full Time Equivalent) 값을 계산합니다. 이것이 바로 [!DNL Workfront] 사용자에 대한 할당을 계산할 때 을 사용합니다.</p> <p>이 값은 프로젝트 타임라인을 계획하거나, 리소스에 대한 예산을 책정하는 경우 또는 프로젝트에 대한 시간을 로깅하는 데 사용됩니다. </p> <p>이 작업표는 다음에 설명된 대로 시스템에 있는 사용자의 작업표를 설정할 때 사용되지 않습니다. <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 구성] 작업표 및 시간 기본 설정</a>.</p> <p><b>참고</b>: [!DNL Workfront] 관리자는 [!UICONTROL 타임라인 계산] 환경 설정의 잠금을 해제할 수 없습니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 사용자 지정 분기]</p> </td> 
   <td> <p>프로젝트에서 작업할 사용자에 대한 사용자 지정 연간 분기를 구성합니다. 사용자 지정 분기는 일반적으로 달력 연도 동안 기존 분기 분류와 일치하지 않는 분기입니다. 여러 사용자 지정 분기를 추가할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">프로젝트에 대한 사용자 지정 분기 활성화</a>.</p>  <p><b>참고</b>: [!DNL Workfront] 관리자는 [!UICONTROL 사용자 지정 분기] 기본 설정의 잠금을 해제할 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 비즈니스 사례] {#business-cases}

시스템 전체에서 새로 생성된 프로젝트에 대한 비즈니스 사례를 생성하여 프로젝트 요청을 제출할 수 있습니다. 환경 설정을 정의하여 **[!UICONTROL 비즈니스 사례]** 양식. 다음과 같은 다른 도구가 활성화되도록 이러한 옵션을 활성화하는 것이 좋습니다 [!UICONTROL Portfolio 최적화 프로그램]를 업데이트하면 됩니다. 각 필드에 표시되는 내용에 대한 자세한 내용은 [비즈니스 사례 정의](../../../manage-work/projects/define-a-business-case/define-business-case.md).

다음 이후 [!DNL Workfront] 관리자는 [!UICONTROL 비즈니스 사례]그런 다음 프로젝트 소유자가 프로젝트 수준에서 비즈니스 사례를 생성할 수 있습니다. 비즈니스 사례 생성에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 사후 세계] {#life-after-death}

시스템 전체에서 새로 만든 프로젝트에 대해 다음 환경 설정을 구성합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 프로젝트가 완료로 표시된 후에도 사용자는 계속] </p> </td> 
   <td> <p>프로젝트 상태가 [!UICONTROL 완료]로 표시된 후 작업 또는 문제를 삭제할 수 있는지 여부에 대한 조직(또는 그룹에 대한 프로젝트 환경 설정을 구성하는 경우 그룹)의 규칙을 결정합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 작업 삭제]</strong>: 프로젝트가 [!UICONTROL 완료]로 표시된 후 프로젝트에서 작업을 삭제할 수 있습니다.<br></li> 
     <li><strong>[!UICONTROL 삭제 문제]</strong>: 프로젝트가 [!UICONTROL 완료]로 표시된 후 프로젝트에서 문제를 삭제할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 프로젝트가 완료, 완료 또는 승인 보류 중으로 표시되면 사용자는 계속]</p> </td> 
   <td> <p>프로젝트 상태가 표시된 후 프로젝트의 작업, 문제, 문서 및 기타 개체에 대해 발생하는 작업에 대한 조직(또는 그룹에 대한 프로젝트 환경 설정을 구성하는 경우 그룹)의 규칙을 결정합니다 <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, 또는 <strong>[!UICONTROL 승인 보류 중]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL 작업 추가 및 편집]</strong> 사용자가 다음을 수행할 수 있습니다.
      <ul>
       <li>프로젝트가 [!UICONTROL Complete], [!UICONTROL Dead] 또는 [!UICONTROL Pending Approval]으로 표시된 후 프로젝트 내에서 작업을 편집합니다. 여기에는 시간 추가 및 작업 비용 항목 변경이 포함됩니다.</li>
       <li>프로젝트에 작업을 추가합니다.</li>
      </ul></li> 
     <li><strong>[!UICONTROL 문제 추가 및 편집]</strong>: 사용자가 다음을 수행할 수 있습니다.
      <ul>
       <li>프로젝트가 [!UICONTROL Complete], [!UICONTROL Dead] 또는 [!UICONTROL Pending Approval]로 표시된 후 프로젝트 내의 문제를 편집합니다.</li>
       <li>프로젝트가 [!UICONTROL 완료] 또는 [!UICONTROL 데드]로 표시된 후에 프로젝트에 문제를 추가합니다. ([!UICONTROL Pending Approval]인 프로젝트에는 문제를 추가할 수 없습니다.)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL 프로젝트 및 해당 작업 및 문제에 문서 추가]</strong>: [!UICONTROL Complete] 또는 [!UICONTROL Dead]로 표시된 후 프로젝트에 문서를 추가(또는 프로젝트 내의 작업 및 문제에 문서 추가)할 수 있습니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 템플릿 첨부]</strong>: 프로젝트가 [!UICONTROL 완료] 또는 [!UICONTROL 데드]로 표시된 후 프로젝트에 템플릿을 첨부할 수 있습니다.</p> <p>이 옵션은 승인 보류 중인 프로젝트에는 적용되지 않습니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
