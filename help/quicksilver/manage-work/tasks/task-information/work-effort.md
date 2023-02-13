---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 시간 개요
description: 작업 시간 개요
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# 작업 시간 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

프로젝트 관리자는 프로젝트에서 작업이 완료되는 데 필요한 작업량을 예상하는 방법을 결정할 수 있습니다. 다음 지표 중 하나를 사용하여 작업을 완료하는 데 필요한 작업의 양을 예측합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">계획된 시간</td> 
   <td> <p> 작업에 할당된 리소스가 작업을 완료하는 데 걸리는 시간을 표시하는 수동 숫자 입력 또는 Adobe Workfront 계산입니다. </p> <p>계획 시간에 대해 다음 사항을 고려하십시오. </p> 
    <ul> 
     <li>기본 방법입니다. </li> 
     <li>기간 유형이 계산된 지정 또는 단순 발령인 태스크에 대해서만 계획된 시간만 수동으로 갱신할 수 있습니다. </li> 
    </ul> <p>계획된 시간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획 시간 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업 노력 </td> 
   <td> <p>작업을 완료하는 데 사용자에게 작은 작업, 중간 작업 또는 많은 양의 노력이 필요한지 여부를 정의하는 수동 레이블입니다. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>작업 노력에 대해 다음 사항을 고려하십시오.</p> 
    <ul> 
     <li>이 필드는 단순 기간 유형이 있는 작업에만 사용할 수 있습니다. </li> 
     <li>이 레이블을 사용할 수 있도록 설정하고 프로젝트 수준에서 해당 레이블과 연관된 작업 시간 비율을 정의할 수 있습니다. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

이 문서에서는 작업 투입의 정의와 작업에 대한 작업 시간을 예측할 때 작업 투입의 사용 방법을 설명합니다.

>[!NOTE]
>
>계획된 시간과 작업 노력이 서로 영향을 줍니다. 계획 시간을 갱신하면 작업 노력이 갱신되고 작업 노력이 갱신되면 작업의 계획 시간이 갱신될 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 해당 작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 시간 사용에 대한 고려 사항

* 프로젝트 태스크에 계획 시간 0이 있고, 작업 노력 사용으로 프로젝트의 작업 계획 시간 설정을 자동으로 계산하면, 프로젝트 태스크와 연관된 기본 작업 투입 레벨은 보통이 됩니다. 계획 시간은 단순 기간 유형 작업에 대해 자동으로 업데이트됩니다. 자세한 내용은 섹션을 참조하십시오  [작업 노력 수준](#levels-of-work-effort) 참조하십시오.
* 프로젝트 태스크에 0보다 많은 계획 시간이 있고 작업 노력 사용으로 프로젝트의 태스크 계획 시간 설정을 자동으로 계산할 경우 단순 기간 유형 태스크의 계획 시간 크기를 변경하지 않고 작업 투입 레벨이 계획 시간 양에 따라 갱신됩니다. 자세한 내용은 섹션을 참조하십시오 [Workfront이 계획된 시간을 기반으로 작업 노력을 계산하는 방법](#how-workfront-calculates-work-effort-based-on-planned-hours) 참조하십시오.
* 프로젝트 태스크에 계획 시간이 0이고 작업 노력 사용을 사용으로 설정하여 프로젝트에 대한 태스크 계획 시간 설정을 자동으로 계산한 다음 작업 투입 레벨을 중간에서 소량 또는 대규모 로 갱신하면 계획 시간도 갱신됩니다. 자세한 내용은 섹션을 참조하십시오 [Workfront이 작업 노력을 기반으로 계획된 시간을 계산하는 방법](#how-workfront-calculates-planned-hours-based-on-work-effort) 참조하십시오.
* 작업을 인라인 편집하고 태스크에 대한 계획 시간 및 작업 투입 필드를 모두 동시에 수정하면 계획 시간이 지정된 값으로 갱신되지만 작업 투입 값은 갱신된 계획 시간을 기준으로 계산됩니다.
* 태스크의 작업 투입 값을 갱신할 때, 기간은 더 이상 계획 시간을 기반으로 자동으로 계산되지 않습니다. 단순 기간 작업에 대해 기간 계산 방법에 대한 자세한 내용은 [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* 작업의 기간 유형을 단순 유형에서 다른 유형으로 변경하면 작업 투입 필드가 작업에 숨겨집니다. 계획 시간은 변경되지 않은 상태로 유지됩니다.
* 상위 작업에서 작업 노력 수준을 업데이트할 수 없습니다. 상위 태스크에 대한 작업 투입 레벨은 모든 하위 태스크의 롤업인 태스크에 대한 계획 시간 수를 기준으로 자동으로 계산됩니다. 상위 작업에 대한 자세한 내용은 [하위 작업 만들기](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## 계획 시간 대신 작업 투입 사용

1. 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집**.
1. 클릭 **작업 설정**&#x200B;를 선택한 다음 옵션을 선택합니다&#x200B;**작업 노력을 사용하여 작업 계획 시간 자동 계산**. 이 옵션은 기본적으로 선택되어 있지 않습니다.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   프로젝트에서 작업 작업의 사용을 활성화하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서.

1. 클릭 **작업** 왼쪽 패널에서 작업 이름을 클릭하여 액세스합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집**. 작업에 단순 기간 유형이 있는지 확인합니다.

   >[!TIP]
   >
   >작업 세부 정보 섹션에서 작업에 대한 작업 노력을 갱신할 수도 있습니다.

1. 에서 **개요** 작업을 완료하는 데 필요한 작업량을 수정하려면 작업 투입 드롭다운 메뉴를 누릅니다.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   작업의 작업 노력 필드 업데이트에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * 의 &quot;개요&quot; 섹션 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 문서
   * [작업 세부 정보 개요 영역의 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 작업 노력 수준 {#levels-of-work-effort}

프로젝트 관리자는 프로젝트에 대한 3가지 작업 노력을 식별할 수 있습니다. 각 작업 수준은 사용자가 작업을 완료해야 하는 일별 시간의 백분율과 같습니다.

작업 시간 수준을 설정할 때 자신에게 질문을 해야 합니다. &quot;이 작업에 할당된 사용자가 제시간에 작업을 수행하기 위해 매일 얼마나 많은 시간을 사용해야 합니까?&quot; 

다음 표에서는 가능한 작업 노력 수준 및 기본 해당 백분율을 보여줍니다. 프로젝트 관리자는 조직의 요구 사항에 맞게 백분율을 업데이트할 수 있습니다. 프로젝트를 편집할 때 이렇게 합니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

Workfront 관리자는 설정의 프로젝트 환경 설정 영역에서 작업일별 일반 시간 을 정의합니다. 근무 시간으로 간주되는 일별 시간입니다. Workfront 인스턴스에 대한 프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>아래 예에서는 Workfront 관리자가 근무일당 평균 시간 을 8시간으로 설정했다고 가정합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>작업 노력 수준</td> 
   <td>백분율 값</td> 
  </tr> 
  <tr> 
   <td>소형 </td> 
   <td>작업을 완료하기 위한 작은 작업 수준은 작업일별 일반 시간의 25%로 설정됩니다. 즉, 이 작업 수준을 할당한 작업은 하루에 최대 2시간 내에 완료해야 합니다. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>중간</td> 
   <td> <p>작업을 완료하기 위한 중간 작업 수준은 작업일당 일반 시간의 50%로 설정됩니다. 즉, 이 작업 수준을 할당한 작업은 하루 안에 완료하는 데 2시간 이상 6시간 미만의 시간이 소요됩니다. <code>(0.50*80=4)</code> </p> <p>참고: 프로젝트에서 작업 수행을 자동으로 계산하기 위한 작업 노력 사용 설정이 활성화되면 이 설정이 사용으로 설정되기 전에 작업에 0시간 계획됨 시간이 있었던 경우 작업에 대한 기본 설정이 됩니다. 이로 인해 Planning Hours 작업이 4시간으로 업데이트됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>대형</td> 
   <td>작업을 완료하기 위한 많은 노력이 하루 평균 작업 시간의 75%로 설정됩니다. 즉, 이 수준의 작업 노력을 할당한 작업은 하루에 6시간 이상 완료해야 합니다. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront이 작업 노력을 기반으로 계획된 시간을 계산하는 방법 {#how-workfront-calculates-planned-hours-based-on-work-effort}

프로젝트에서 작업 노력 사용을 사용하여 작업 계획 시간 설정을 자동으로 계산하면, Workfront은 다음 공식을 사용하여 단순 기간 유형으로 태스크에 대한 계획 시간 수를 계산합니다.

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

예를 들어, 기간이 3일이고 작업 노력이 중간인 태스크에는 12개의 계획 시간이 있습니다.

```
Planned Hours = 3*4=12
```

여기서 근무일 당 일반 시간 값은 8시간입니다.

>[!TIP]
>
>작업이 여러 자원에 할당되면 계획 시간은 작업 기간 중 각 하루 동안 각 자원에 균등하게 분배됩니다.

## Workfront이 계획된 시간을 기반으로 작업 노력을 계산하는 방법 {#how-workfront-calculates-work-effort-based-on-planned-hours}

Use Work Pure to to calculate task Planning Hours 설정을 프로젝트에 자동으로 계산하도록 설정하고 작업에 대해 이미 계획 시간이 있거나 작업에서 계획 시간 수를 편집하면 Workfront은 작업 투입 값을 갱신합니다.

Workfront은 다음 공식을 사용하여 계획 시간에 따라 작업 투입 레벨을 갱신합니다.

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

예를 들어, 지속 기간이 2일인 태스크가 있고 계획 시간을 8시간에서 20시간으로 갱신하는 경우, 태스크에 대한 작업 투입이 중간에서 대수로 갱신됩니다.

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 작업 및 프로젝트에 대한 작업 노력 찾기

* [프로젝트에 대한 작업 시간](#work-effort-for-projects)
* [작업에 대한 작업](#work-effort-for-tasks)

### 프로젝트에 대한 작업 시간 {#work-effort-for-projects}

다음 영역에서 프로젝트에서 작업 투입 섹션을 찾을 수 있습니다.

* 프로젝트 편집 상자의 작업 설정 영역

### 작업에 대한 작업 {#work-effort-for-tasks}

다음 영역에서 작업에 대한 작업 투입 필드를 찾을 수 있습니다.

* 작업 편집 상자의 개요 영역
* 작업 시간 영역에서 작업 세부 정보 섹션의 개요 영역
* 작업 목록 또는 보고서
