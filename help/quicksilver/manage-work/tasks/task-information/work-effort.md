---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 작업 노력 개요
description: 작업 노력 개요
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 작업 노력 개요

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

프로젝트 관리자는 프로젝트에서 작업을 완료하는 데 필요한 작업량을 예상할 방법을 결정할 수 있습니다. 다음 지표 중 하나를 사용하여 작업을 완료하는 데 필요한 작업량을 예측합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">계획된 시간</td> 
   <td> <p> 작업에 할당된 자원이 완료하는 데 소요되는 시간을 표시하는 수동 숫자 입력 또는 Adobe Workfront 계산. </p> <p>계획된 시간에 대해 다음 사항을 고려하십시오. </p> 
    <ul> 
     <li>기본 방법입니다. </li> 
     <li>기간 유형이 계산된 할당 또는 단순인 작업에 대해서만 계획된 시간을 수동으로 갱신할 수 있습니다. </li> 
    </ul> <p>계획된 시간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획된 시간 개요</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업 노력 </td> 
   <td> <p>사용자가 작업을 완료하는 데 일일 작업량이 작은지, 중간인지 또는 크는지를 정의하는 수동 레이블입니다. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>작업 노력에 대해 다음 사항을 고려하십시오.</p> 
    <ul> 
     <li>이 필드는 단순 기간 유형의 작업에만 사용할 수 있습니다. </li> 
     <li>이 레이블의 사용을 활성화하고 프로젝트 수준에서 이와 연관된 작업 시간의 백분율을 정의할 수 있습니다. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

이 문서에서는 작업 노력의 의미와 작업에 대한 작업량을 추정할 때 작업 노력을 사용하는 방법에 대해 설명합니다.

>[!NOTE]
>
>계획된 시간과 작업 노력은 서로 영향을 줍니다. 계획된 시간을 업데이트하면 작업 노력을 업데이트할 수 있고 작업 노력을 업데이트하면 작업의 계획된 시간을 업데이트할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재: 플랜 </p>
   또는
   <p>새로운 기능: 표준 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 해당 작업에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 노력 사용 시 고려 사항

* 프로젝트 작업에 계획된 시간이 0이고 작업 노력 사용을 활성화하여 프로젝트에 대한 작업 계획된 시간 설정을 자동으로 계산하는 경우 연결된 기본 작업 노력 수준은 Medium입니다. 단순 기간 유형 작업에 대해 계획된 시간이 자동으로 업데이트됩니다. 자세한 내용은 이 문서의 [작업 노력 수준](#levels-of-work-effort) 섹션을 참조하십시오.
* 프로젝트 작업의 계획된 시간이 0보다 많고 작업 노력 사용을 활성화하여 프로젝트에 대한 작업 계획 시간 설정을 자동으로 계산하는 경우 단순 기간 유형 작업의 계획된 시간 크기를 변경하지 않고 계획된 시간 크기에 따라 작업 노력 수준이 업데이트됩니다. 자세한 내용은 이 문서의 [Workfront에서 계획된 시간을 기준으로 작업 노력을 계산하는 방법](#how-workfront-calculates-work-effort-based-on-planned-hours) 섹션을 참조하십시오.
* 프로젝트 작업에 계획된 시간이 0이고 작업 노력 사용을 활성화하여 프로젝트에 대한 작업 계획 시간 설정을 자동으로 계산한 다음 작업 노력 수준을 Medium에서 작거나 크게 업데이트하면 계획된 시간도 업데이트됩니다. 자세한 내용은 이 문서의 [Workfront에서 작업 노력에 따라 계획된 시간을 계산하는 방법](#how-workfront-calculates-planned-hours-based-on-work-effort) 섹션을 참조하십시오.
* 작업을 인라인 편집하고 작업에 대한 계획된 시간과 작업 노력 필드를 동시에 수정하면 계획된 시간이 사용자가 지정한 값으로 업데이트되지만 작업 노력 값은 업데이트된 계획된 시간을 기반으로 계산됩니다.
* 작업의 작업 노력 값을 업데이트할 때 기간이 계획된 시간을 기준으로 더 이상 자동 계산되지 않습니다. 단순 기간 작업에 대해 기간이 계산되는 방법에 대한 자세한 내용은 [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)을 참조하십시오.
* 작업의 기간 유형을 단순에서 다른 유형으로 변경하면 작업에 작업 노력 필드가 숨겨집니다. 계획된 시간은 변경되지 않습니다.
* 상위 작업에 대한 작업 노력 수준을 업데이트할 수 없습니다. 상위 작업의 작업 노력 수준은 모든 하위 작업의 롤업인 작업의 계획된 시간 수를 기반으로 자동으로 계산됩니다. 상위 작업에 대한 자세한 내용은 [하위 작업 만들기](../../../manage-work/tasks/create-tasks/create-subtasks.md)를 참조하십시오.

## 계획된 시간 대신 작업 노력을 사용할 수 있도록 설정

1. 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.
1. **작업 설정**&#x200B;을 클릭한 다음 옵션&#x200B;**작업 노력을 사용하여 작업 계획 시간을 자동으로 계산**&#x200B;합니다. 기본적으로 선택되어 있지 않습니다.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   프로젝트에서 작업 노력을 사용하도록 설정하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서의 &quot;작업 설정&quot; 섹션을 참조하십시오.

1. 왼쪽 패널에서 **작업**&#x200B;을(를) 클릭한 다음 액세스할 작업의 이름을 클릭합니다.
1. **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다. 작업에 단순 기간 유형이 있는지 확인합니다.

   >[!TIP]
   >
   >작업 세부 정보 섹션에서 작업에 대한 작업 노력을 업데이트할 수도 있습니다.

1. **개요** 영역에서 작업 노력 드롭다운 메뉴를 클릭하여 작업을 완료하는 데 필요한 작업량을 수정합니다.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   작업의 작업 노력 필드를 업데이트하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 문서의 &quot;개요&quot; 섹션
   * [작업 세부 정보 개요 영역에서 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 작업 노력 수준 {#levels-of-work-effort}

프로젝트 관리자는 프로젝트에 대한 세 가지 작업 노력 수준을 식별할 수 있습니다. 각 작업 수준은 사용자가 작업을 완료하는 데 필요한 일일 시간의 백분율과 같습니다.

작업 노력 수준을 설정할 때 &quot;이 작업에 할당된 사용자가 매일 얼마나 많은 시간을 할애하여 시간 내에 작업을 완료해야 합니까?&quot;라는 질문을 자신에게 던져야 합니다.

다음 표는 가능한 작업 노력 수준과 기본 해당 백분율을 보여 줍니다. 프로젝트 관리자는 조직의 요구 사항에 맞게 백분율을 업데이트할 수 있습니다. 프로젝트를 편집할 때 이 작업을 수행합니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

Workfront 관리자는 설정의 프로젝트 환경 설정 영역에서 근무일당 일반 시간을 정의합니다. 이는 근로 시간으로 간주되는 일일 시간입니다. Workfront 인스턴스의 프로젝트 환경 설정을 구성하는 방법에 대한 자세한 내용은 [시스템 차원의 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

>[!NOTE]
>
>아래 예에서는 Workfront 관리자가 근무일당 일반 시간을 8시간으로 설정했다고 가정합니다.

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
   <td>작업 완료를 위한 작은 작업 수준은 근무일당 일반 시간의 25%로 설정됩니다. 즉, 이 수준의 작업 노력이 할당된 작업이 하루에 완료하는 데 최대 2시간이 소요됩니다. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>중간</td> 
   <td> <p>작업 완료를 위한 Medium 작업 수준은 근무일당 일반 시간의 50%로 설정됩니다. 즉, 이 수준의 작업 노력이 할당된 작업이 하루에 완료하는 데 2시간 이상 6시간 미만이 소요됩니다. <code>(0.50*80=4)</code> </p> <p>주: 프로젝트에서 작업 노력을 사용하여 작업 계획 시간 자동 계산 설정이 활성화된 경우, 이 설정이 활성화되기 전에 작업에 계획된 시간이 0일 경우 작업의 기본 설정입니다. 이렇게 하면 작업 계획 시간이 4시간으로 업데이트됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>대형</td> 
   <td>작업 완료를 위한 대규모 작업량은 근무일당 일반 시간의 75%로 설정됩니다. 즉, 이 수준의 작업 노력이 할당된 작업이 하루에 완료하는 데 6시간 이상 걸립니다. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront에서 작업 노력을 기반으로 계획된 시간을 계산하는 방법 {#how-workfront-calculates-planned-hours-based-on-work-effort}

작업 노력을 사용하여 프로젝트에 대한 작업 계획 시간 설정을 자동으로 계산할 수 있는 경우 Workfront은 다음 공식을 사용하여 단순 기간 유형의 작업에 대한 계획 시간을 계산합니다.

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

예를 들어 지속 시간이 3일이고 Medium의 작업 노력이 있는 작업에는 12개의 계획된 시간이 있습니다.

```
Planned Hours = 3*4=12
```

여기서 작업일당 일반 시간 값은 8시간입니다.

>[!TIP]
>
>작업이 여러 리소스에 할당되면 작업 기간 각 날에 대해 계획된 시간이 각 리소스에 균등하게 분배됩니다.

## Workfront에서 계획된 시간을 기반으로 작업 노력을 계산하는 방법 {#how-workfront-calculates-work-effort-based-on-planned-hours}

작업 노력 사용을 활성화하여 프로젝트에 대한 작업 계획 시간 설정을 자동으로 계산하고 작업에 이미 계획된 시간이 있거나 작업의 계획된 시간 수를 편집하면 Workfront에서 작업 노력 값을 업데이트합니다.

Workfront은 다음 공식을 사용하여 계획된 시간에 따라 작업 노력 수준을 업데이트합니다.

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

예를 들어, 지속 시간이 2일인 작업이 있고 계획된 시간을 8시간에서 20시간으로 업데이트하는 경우 작업에 대한 작업 노력은 Medium에서 크게 업데이트됩니다.

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 작업 및 프로젝트에 대한 작업 노력 찾기

* [프로젝트에 대한 작업 노력](#work-effort-for-projects)
* [작업에 대한 작업 노력](#work-effort-for-tasks)

### 프로젝트에 대한 작업 노력 {#work-effort-for-projects}

다음 영역에서 프로젝트의 작업 노력 섹션을 찾을 수 있습니다.

* 프로젝트 편집 상자의 작업 설정 영역

### 작업에 대한 작업 노력 {#work-effort-for-tasks}

다음 영역에서 작업에 대한 작업 노력 필드를 찾을 수 있습니다.

* 작업 편집 상자의 개요 영역
* 작업 시간 영역의 작업 세부 정보 섹션에 있는 개요 영역
* 작업 목록 또는 보고서
