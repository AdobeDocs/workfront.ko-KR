---
title: 프로젝트 재무 재계산
product-area: projects
navigation-topic: financials
description: 재정은 프로젝트에 대해 기록된 시간 또는 비용 및 수익을 계산하는 데 사용되는 요율에 따라 프로젝트에서 계산됩니다.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# 프로젝트 재무 재계산

재정은 프로젝트에 대해 기록된 시간 또는 비용 및 수익을 계산하는 데 사용되는 요율에 따라 프로젝트에서 계산됩니다.

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
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>Finance 관리 권한을 사용하여 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## Adobe Workfront에서 재무 계산에 대한 고려 사항

재정은 다음과 같은 방법으로 Enhanced Analytics에서 계산됩니다.

* 프로젝트에서 재무 재계산 옵션을 사용하여 프로젝트의 비용과 수익을 수동으로 재계산할 수 있습니다.
* 또한 일부 작업은 자동 다시 계산을 트리거합니다.

프로젝트 수명 동안 사용자 또는 역할의 비율이 변경되면 다음과 같은 문제가 발생할 수 있습니다.

* 변경 사항이 적용되면, 시간이 기록되고 재무 정보가 계산될 때 갱신된 비율이 해당 시점부터 사용됩니다. 비율을 변경하는 것은 변경이 이루어지기 전에 계산된 방법에는 영향을 주지 않습니다. 기존의 기록된 모든 시간에 대해, 이전 비율은 재무 정보를 계산하는 데 사용됩니다.
* 재계산 재무 옵션을 사용하여 Adobe Workfront에서 지금까지 기록된 모든 시간에 대해 소급하여 새 비율을 사용하도록 강제할 수 있습니다. 따라서 Workfront은 이전에 입력한 모든 시간, 계획 비용 및 매출을 새로운 비율 정보에 따라 소급하여 재계산합니다.

>[!CAUTION]
>
>주어진 프로젝트에 대한 재정을 수동으로 다시 계산하기 전에 이전 비율로 이미 계산된 재무 데이터를 보존해야 할 수 있습니다. 기존 정보를 변경하지 않거나 해당 변경이 필요한 경우에만 재계산 재무 옵션을 사용하는 것이 좋습니다.

## 기존 시간의 작업에 대한 재무 데이터 보존 {#preserve-financial-data-for-tasks-with-existing-hours}

프로젝트에 대한 재무 데이터가 다시 계산되면 Workfront은 이전에 기록된 모든 시간, 계획, 실제 비용, 계획 및 실제 수익을 신규 또는 업데이트된 재무 정보에 따라 소급하여 재계산합니다.

* [프로젝트 매출 유지](#preserve-project-revenue)
* [프로젝트 비용 유지](#preserve-project-cost)

### 프로젝트 매출 유지  {#preserve-project-revenue}

수익률은 프로젝트 수명 동안 변경될 수 있습니다.

청구 비율 및 매출에 대한 자세한 내용은 문서를 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

수익률은 다음 수준에서 변경될 수 있습니다.

* 시스템 수준(작업 역할용)\
   시스템 수준에서 청구 비율을 사용하여 작업 역할을 생성하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 사용자 수준\
   사용자의 청구 비율 정보 변경에 대한 자세한 내용은 문서를 참조하십시오 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 회사 수준(Job 역할용)\
   자세한 내용은 [회사 레벨에서 직무 역할 청구 비율 대체](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* 프로젝트 수준(작업 역할용)\
   프로젝트 수준에서 작업 역할 비율 재지정에 대한 자세한 내용은 문서를 참조하십시오 [Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

예를 들어, 프로젝트 진행 중에 사용자의 청구 비율이 시간당 $50에서 $75로 변경되며 기존 데이터를 모두 이전 비율($50 및 시간)로 계산하려는 경우 그러나 프로젝트 재정이 재계산되면 기존 재무 데이터가 이미 있는 태스크에는 새로운 청구 비율(시간당 75달러)을 반영하도록 갱신된 수익이 있습니다.

* [청구 레코드를 생성하여 프로젝트 수익 보존](#preserve-project-revenue-by-creating-a-billing-record)
* [복수 청구 비율 대체를 사용하여 프로젝트 수익 유지](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 청구 레코드를 생성하여 프로젝트 수익 보존 {#preserve-project-revenue-by-creating-a-billing-record}

위에 언급된 레벨에서 청구 비율이 변경되면 수동 재계산 재무 옵션을 사용하지 않거나 프로젝트에 기록된 시간을 잠그고 이전 비율을 청구 상태로 청구 레코드로 계산하여 프로젝트에서 이미 계산된 기존 수익을 유지할 수 있습니다.

프로젝트에서 재정을 재계산하지 않거나 청구 레코드에 로그된 시간을 잠그는 경우 비율 변경 후 기록된 시간은 신규 비율로 계산되며, 비용 비율 변경 전에 기록된 시간은 이전 비율로 계산됩니다.

청구 레코드 생성에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

#### 복수 청구 비율 대체를 사용하여 프로젝트 수익 유지 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

프로젝트 레벨에서 작업 역할에 대한 청구 비율이 변경되면 지정된 기간 내에 잠긴 복수 청구 비율 대체를 사용하여 프로젝트에서 이미 계산된 기존 수익을 유지할 수 있습니다.

복수 청구 단가 대체를 사용하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>이는 프로젝트 레벨에서 변경된 직무 역할 청구 요율에만 적용됩니다.

### 프로젝트 비용 유지 {#preserve-project-cost}

비용 비율은 다음 레벨에서 변경될 수 있습니다.

* 시스템 수준(작업 역할용)\
   시스템 수준에서 비용 비율로 작업 역할을 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 사용자 수준\
   사용자의 원가율 정보 변경에 대한 자세한 내용은 문서를 참조하십시오 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

위에 언급된 레벨에서 청구 비율이 변경되는 경우, 프로젝트에 기록된 시간을 잠그고 이전 비율을 청구 상태로 청구 레코드로 계산하여 프로젝트에 이미 계산된 기존 비용을 유지할 수 있습니다. 청구 레코드 생성에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

섹션에 설명된 대로 청구 레코드를 생성하지 않으려는 경우 수동 재계산 재무 옵션을 사용하지 않을 수도 있습니다 [프로젝트에 대한 재무 수동 재계산](#manually-recalculate-finances-for-a-project) 참조하십시오.

프로젝트에서 재정을 재계산하지 않거나 청구 레코드에 로그된 시간을 잠그는 경우 비율 변경 후 기록된 시간은 신규 비율로 계산되며, 비용 비율 변경 전에 기록된 시간은 이전 비율로 계산됩니다.

## 프로젝트에 대한 재무 수동 재계산 {#manually-recalculate-finances-for-a-project}

프로젝트 수명 동안 비율이 변경되고 비용 및 수익 계산이 신규 비율을 반영하도록 하려면 프로젝트의 재정을 수동으로 재계산해야 합니다.

>[!NOTE]
>
>섹션의 단계를 수행하여 수동으로 통화를 재계산할 때 수익 값이 신규 환율을 반영하도록 업데이트되지 않도록 할 수 있습니다 [기존 시간의 작업에 대한 재무 데이터 보존](#preserve-financial-data-for-tasks-with-existing-hours) 이 문서의 프로젝트에서 재무 재계산을 수동으로 재계산할 때 신규 비율을 반영하도록 원가 값이 항상 갱신됩니다.

프로젝트 페이지나 프로젝트 목록 또는 보고서에서 Workfront에서 프로젝트의 재정을 다시 계산할 수 있습니다.

일괄 편집하는 동안 재무 재계산을 수행할 수 있습니다. 자세한 내용은 [프로젝트 편집 상자에서 수동으로 재무 일괄 재계산](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) 섹션에 자세히 설명되어 있습니다.

1. 재무 재계산하려는 프로젝트로 이동하여 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png) 프로젝트 이름의 오른쪽에 있습니다.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   또는

   프로젝트 목록 또는 보고서로 이동하고 하나 이상의 프로젝트를 선택한 다음 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png) 를 클릭합니다.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 예산을 일괄 재계산할 때 많은 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당 또는 많은 사용자 지정 필드일 수 있습니다.

1. 클릭 **재무 재계산**.

   프로젝트에 대한 모든 계획 비용 및 수익은 새로운 정보로 재계산됩니다.

   브라우저 맨 위에서 프로젝트의 재정이 성공적으로 재계산되었다는 확인을 받아야 합니다.\
   기존 비용 값 및 잠기지 않은 일부 수익 값은 신규 비율을 반영하도록 갱신됩니다.

## 프로젝트 편집 상자에서 수동으로 재무 일괄 재계산 {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

여러 프로젝트의 재정을 일괄적으로 편집하여 수동으로 다시 계산할 수 있습니다. 이로 인해 프로젝트의 매출이 소급하여 재계산됩니다.

>[!IMPORTANT]
>
>섹션의 단계를 수행하여 수동으로 통화를 재계산할 때 수익 값이 신규 환율을 반영하도록 업데이트되지 않도록 할 수 있습니다 [기존 시간의 작업에 대한 재무 데이터 보존](#preserve-financial-data-for-tasks-with-existing-hours) 이 문서의 프로젝트에서 재정을 수동으로 재계산할 때 신규 비율을 반영하도록 원가 값이 항상 갱신됩니다.

여러 프로젝트의 재정을 수동으로 재계산하려면

1. 프로젝트 목록으로 이동합니다.
1. 목록에서 여러 프로젝트를 선택한 다음 를 클릭합니다 **편집**.

   >[!TIP]
   >
   >프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 프로젝트를 일괄적으로 편집할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당 또는 많은 사용자 지정 필드일 수 있습니다.

1. 클릭 **설정**&#x200B;를 선택하고 을 선택합니다. **비용 및 수익 재계산**.

1. 클릭 **변경 내용 저장**.

## 재무 자동 재계산을 트리거하는 조치

다음 작업은 Workfront에서 프로젝트의 재무 재계산을 트리거합니다.

* 작업 상태 변경
* 여러 시간이 포함된 작업을 다른 프로젝트로 이동
* 프로젝트 상태를 완료에서 활성 상태로 변경

>[!NOTE]
>
>프로젝트 상태를 변경하면 계획된 값만 재계산됩니다.

또한 **자세히** 메뉴 ![](assets/qs-more-menu.png) 프로젝트 수준에서 **재무 재계산**.
