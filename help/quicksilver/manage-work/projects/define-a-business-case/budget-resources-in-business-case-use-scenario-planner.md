---
navigation-topic: business-case-and-scorecards
title: 시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원
description: 리소스 계획의 일부로, Adobe Workfront 시나리오 계획자를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할을 예산을 책정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

리소스 계획의 일부로, Adobe Workfront 시나리오 계획자를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할을 예산을 책정할 수 있습니다.

비즈니스 사례 만들기에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>시스템 레벨 시나리오 계획자에 입력하는 프로젝트에 연결된 이니셔티브에 대한 작업 역할 정보는 이니셔티브를 게시하면 프로젝트 업무 사례의 자원 예산 책정 영역에 표시됩니다. 시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md).

자원 계획자를 사용하여 업무 사례에서 자원을 예측할 수도 있습니다. 자세한 내용은 다음을 참조하십시오.

* [비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>프로젝트 작업을 시작할 때 리소스 계획자 또는 시나리오 계획자를 사용할지 여부를 결정하는 것이 좋습니다. 프로젝트 수명 중에 두 버전 간을 자주 전환하면 프로젝트에 대한 리소스를 할당하는 방식으로 일치하지 않을 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>비즈니스 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 시나리오 플래너에 대한 추가 라이센스를 구매해야 합니다.</p> <p>Workfront 시나리오 플래너를 가져오는 방법에 대한 자세한 내용은 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">시나리오 플래너를 사용하는 데 필요한 액세스</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음에 대한 액세스 편집: </p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>재무 데이터</p> </li> 
     <li> <p>시나리오 플래너 </p> </li> 
    </ul> <p>예산 자원에 필요한 액세스에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Adobe Workfront의 예산 리소스에 대한 액세스 필요</a>.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Adobe Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 시나리오 계획자를 사용하여 계획을 생성합니다.

   자세한 내용은 [시나리오 계획자에서 계획 생성 및 편집](../../../scenario-planner/create-and-edit-plans.md).

* 계획에 대한 이니셔티브를 생성하여 프로젝트에 연결합니다.

   이니셔티브에 필요한 작업 역할 정보를 표시하고 이 정보로 연결된 프로젝트를 업데이트해야 합니다.

   자세한 내용은 다음 문서를 참조하십시오.

   * [시나리오 플래너에서 이니셔티브 생성 및 편집](../../../scenario-planner/create-and-edit-initiatives.md)
   * [시나리오 플래너의 계획에 프로젝트 가져오기](../../../scenario-planner/import-projects-to-plans.md)
   * [시나리오 계획자에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 생성합니다](../../../scenario-planner/publish-scenarios-update-projects.md).

* 이러한 전제 조건은 아니지만 다음 조건을 권장합니다.

   * 시나리오 계획자에서 예산책정된 작업 역할에 프로젝트의 작업을 지정합니다.
   * 프로젝트의 작업에 대한 계획 시간 수를 나타냅니다.

      이렇게 하면 작업이 완료되어야 할 작업의 양을 이해할 수 있으므로, 작업을 완료하기 위해 리소스를 예산을 책정해야 하는 시간을 결정할 수 있습니다.

      작업과 계획 시간 연관에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 이니셔티브 관련 프로젝트에 대해 시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원

>[!IMPORTANT]
15년 동안 자원을 편성할 수 있습니다. 기간이 15년을 초과하는 프로젝트에 대한 자원을 예산을 책정하는 경우 예산 정보가 정확하지 않을 수 있습니다.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. 자원을 예산을 편성할 프로젝트로 이동합니다.

   >[!TIP]
   이 프로젝트는 Scenario Planner의 이니셔티브에 연결되어 있으며 연결된 이니셔티브가 적어도 한 번 게시된 프로젝트입니다.

1. 클릭 **비즈니스 사례** 왼쪽 패널에 표시됩니다.
1. (조건부) in **리소스 예산 책정** 섹션에서 다음 중 하나를 수행합니다.

   * 시나리오 계획자에서 정보를 방금 게시한 경우, **프로젝트의 예산책정된 노무비 계산에 사용할 시간을 선택합니다** 자원 예산 영역의 필드에서 **선택**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * 이전에 프로젝트에 대한 예산 자원을 위해 자원 계획자를 선택한 경우 **변경** > **시나리오 플래너** > **선택**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront은 연결된 이니셔티브의 필수 직무 시간을 사용하여 프로젝트의 예산책정된 노무비 및 예산책정된 시간을 계산합니다. 권장되는 옵션입니다. 원가는 프로젝트 통화로 비즈니스 사례에 표시됩니다.

      <!--drafted for Budgeted Hours:
   <span class="preview">프로젝트를 복사하고 예산책정된 시간을 새 프로젝트에 복사하도록 선택하면 시나리오 계획자를 사용하여 설정한 시간이 새 프로젝트에 복사되지 않습니다. Resource Planner에 책정된 시간만 복사됩니다. 자세한 내용은 [프로젝트 복사](../manage-projects/copy-project.md)</span>
—>

   >[!IMPORTANT]
   시나리오 계획자를 사용하여 프로젝트에 대한 자원을 예산을 책정하는 경우 예산책정된 노무비는 Workfront의 다음 영역에 표시됩니다.
   * 업무 사례의 자원 예산 영역
   * 시스템 레벨 시나리오 계획자는 프로젝트에 연결된 이니셔티브의 인력 비용입니다. 자세한 내용은 [시나리오 플래너에서 이니셔티브 생성 및 편집](../../../scenario-planner/create-and-edit-initiatives.md).


1. (선택 사항) **시나리오 계획자에서 보기** 프로젝트에 연결된 이니셔티브가 포함된 계획을 열려면 다음을 수행하십시오. 이렇게 하면 새 브라우저 탭에서 시나리오 계획자가 열립니다.
1. (선택 사항) 이니셔티브에 대한 정보를 업데이트합니다. 자세한 내용은 [시나리오 플래너에서 이니셔티브 생성 및 편집](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   프로젝트의 Resource Budgeting 영역이 업데이트될 때마다 변경 후 이니셔티브를 게시해야 합니다.
