---
title: 프로젝트 재무 다시 계산
product-area: projects
navigation-topic: financials
description: 재원은 프로젝트에 기록된 시간 또는 비용 및 수익 계산에 사용되는 비율로 변경되므로 프로젝트에 대해 계산됩니다.
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '1632'
ht-degree: 0%

---

# 프로젝트 재무 다시 계산

재원은 프로젝트에 기록된 시간 또는 비용 및 수익 계산에 사용되는 비율로 변경되므로 프로젝트에 대해 계산됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>프로젝트 및 재무 데이터에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 관리 권한으로 프로젝트에 대한 권한 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Adobe Workfront의 재무 계산에 대한 고려 사항

재원은 다음과 같은 방법으로 프로젝트에 대해 계산됩니다.

* 프로젝트의 재무 다시 계산 옵션을 사용하여 프로젝트의 비용 및 수익을 수동으로 다시 계산할 수 있습니다.
* 또한 일부 작업은 자동 재계산을 트리거합니다.

프로젝트 수명 중 사용자 또는 역할의 비율이 변경되면 다음과 같은 문제가 발생할 수 있습니다.

* 변경이 이루어지면 시간이 기록되고 재무 정보가 계산됨에 따라 해당 시점부터 업데이트된 요금이 사용됩니다. 비율을 변경해도 변경 전에 어떤 결과가 계산되었는지는 영향을 주지 않습니다. 기록된 모든 기존 시간에 대해 이전 요금을 사용하여 재무 정보를 계산합니다.
* 재무 다시 계산 옵션을 사용하여 Adobe Workfront에서 지금까지 기록된 모든 시간에 대해 신규 비율을 소급하여 사용하도록 강제할 수 있습니다. 이렇게 하면 Workfront은 새 요금 정보에 따라 이전에 입력한 모든 시간, 계획된 비용 및 수익을 소급하여 다시 계산합니다.

보고서 유형 프로젝트(재무 데이터)는 재무 데이터의 재계산을 자동으로 수행하지 않습니다. 이 보고서 유형의 데이터를 업데이트하려면 개별 프로젝트의 재무를 수동으로 다시 계산해야 합니다.

>[!CAUTION]
>
>주어진 프로젝트에 대한 재무를 수동으로 다시 계산하기 전에 이미 이전 비율로 계산된 재무 데이터를 보존할 수 있습니다. 기존 정보를 변경하지 않고 있거나 변경하고자 하는 경우에만 재무 재계산 옵션을 사용하는 것이 좋습니다.

## 기존 시간이 있는 작업에 대한 재무 데이터 유지 {#preserve-financial-data-for-tasks-with-existing-hours}

프로젝트에 대한 재무 데이터가 다시 계산되면 Workfront은 신규 또는 업데이트된 재무 정보에 따라 이전에 기록된 모든 시간, 계획, 실제 비용, 계획 및 실제 수익을 소급하여 다시 계산합니다.

* [프로젝트 수익 유지](#preserve-project-revenue)
* [프로젝트 비용 유지](#preserve-project-cost)

### 프로젝트 수익 유지  {#preserve-project-revenue}

수익률은 프로젝트 기간 동안 변경될 수 있습니다.

청구 요금 및 매출에 대한 자세한 내용은 문서 [청구 및 매출 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

수익률은 다음 수준에서 변경될 수 있습니다.

* 시스템 수준(작업 역할의 경우)\
  시스템 수준에서 청구 요금이 포함된 작업 역할을 만드는 방법에 대한 자세한 내용은 문서 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

* 사용자 수준\
  사용자의 청구 요금 정보를 변경하는 방법에 대한 자세한 내용은 문서 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

* 회사 수준(작업 역할의 경우)\
  자세한 내용은 [회사 수준에서 작업 역할 청구 요금 대체](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)를 참조하십시오.

* 프로젝트 수준(작업 역할의 경우)\
  프로젝트 수준에서 작업 역할 요율 재정의에 대한 자세한 내용은 문서 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.

예를 들어 프로젝트 진행 중 사용자의 청구 요금이 시간당 $50에서 $75로 변경되고 기존의 모든 데이터를 이전 요금($50 및 시간)으로 계속 계산되게 하려는 경우, 그러나 프로젝트 재정이 다시 계산되면 기존 재무 데이터가 있는 작업의 매출은 새 청구 요금(시간당 75달러)을 반영하도록 업데이트됩니다.

* [청구 기록을 만들어 프로젝트 수익 유지](#preserve-project-revenue-by-creating-a-billing-record)
* [여러 청구 요금 무시를 사용하여 프로젝트 수익 유지](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 청구 기록을 생성하여 프로젝트 수익 보존 {#preserve-project-revenue-by-creating-a-billing-record}

위에서 언급한 모든 수준에서 청구 요금이 변경되면 수동 재무 다시 계산 옵션을 사용하지 않거나 프로젝트에 기록된 시간을 잠그고 이전 요율로 계산된 기존 수익을 청구됨 상태의 청구 기록에 잠궈 프로젝트에서 이미 계산된 기존 수익을 보존할 수 있습니다.

프로젝트에 대한 재무를 다시 계산하지 않거나 청구된 청구 기록에 기록된 시간을 잠글 때, 요금 변경 후 기록된 시간은 새로운 요율로 계산되며, 비용 요금 변경 전 기록된 시간은 이전 요율로 계속 계산됩니다.

청구 기록 만들기에 대한 자세한 내용은 문서 [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)를 참조하십시오.

#### 여러 청구 요금 무시를 사용하여 프로젝트 수익 유지 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

프로젝트 수준에서 작업 역할에 대한 청구 요금이 변경되면 지정된 기간 내에 잠긴 여러 청구 요금 무시를 사용하여 프로젝트에서 이미 계산된 기존 수익을 유지할 수 있습니다.

여러 청구 요율 재정의 사용에 대한 자세한 내용은 문서 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.

>[!NOTE]
>
>이는 프로젝트 수준에서 변경된 작업 역할 청구 요금에만 적용됩니다.

### 프로젝트 비용 유지 {#preserve-project-cost}

원가율은 다음 레벨에서 변경될 수 있습니다.

* 시스템 수준(작업 역할의 경우)\
  시스템 수준에서 비용 요율로 작업 역할을 만드는 방법에 대한 자세한 내용은 문서 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

* 사용자 수준\
  사용자의 비용 정보를 변경하는 방법에 대한 자세한 내용은 문서 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

위에서 언급한 모든 수준에서 청구 요금이 변경되면 프로젝트에 기록되고 이전 요율을 사용하여 계산된 시간을 청구됨 상태의 청구 기록에 잠궈 프로젝트에서 이미 계산된 기존 비용을 보존할 수 있습니다. 청구 기록 만들기에 대한 자세한 내용은 문서 [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)를 참조하십시오.

청구 기록을 만들지 않으려면 이 문서의 [프로젝트에 대한 재무 수동 다시 계산](#manually-recalculate-finances-for-a-project) 섹션에 설명된 대로 재무 수동 다시 계산 옵션을 사용하지 않을 수도 있습니다.

프로젝트에 대한 재무를 다시 계산하지 않거나 청구된 청구 기록에 기록된 시간을 잠글 때, 요금 변경 후 기록된 시간은 새로운 요율로 계산되며, 비용 요금 변경 전 기록된 시간은 이전 요율로 계속 계산됩니다.

## 프로젝트의 재무 수동으로 다시 계산 {#manually-recalculate-finances-for-a-project}

프로젝트 수명 동안 요금이 변경되고 원가 및 수익 계산에 신규 요금이 반영되도록 하려면 프로젝트의 재무를 수동으로 다시 계산해야 합니다.

>[!NOTE]
>
>이 문서의 [기존 시간이 있는 작업에 대한 재무 데이터 유지](#preserve-financial-data-for-tasks-with-existing-hours) 섹션의 단계를 따라 재무를 수동으로 다시 계산할 때 수익 값이 새 요금을 반영하도록 업데이트되지 않도록 할 수 있습니다. 프로젝트의 재무 정보를 수동으로 다시 계산할 때 새 단가를 반영하도록 비용 값이 항상 업데이트됩니다.

프로젝트 페이지나 프로젝트 목록 또는 보고서에서 Workfront의 프로젝트 재무 정보를 다시 계산할 수 있습니다.

일괄적으로 편집하면서 재무 정보를 다시 계산할 수 있습니다. 자세한 내용은 이 문서에서 [재무 정보를 수동으로 다시 계산](#manually-recalculate-finances-in-bulk) 섹션을 참조하십시오.

1. 재무 정보를 다시 계산하려는 프로젝트로 이동한 다음 프로젝트 이름 오른쪽에 있는 **자세히** 아이콘 ![추가 메뉴](assets/qs-more-icon-on-an-object.png)를 클릭합니다.

   ![프로젝트 수준 추가 드롭다운](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   또는

   프로젝트 목록 또는 보고서로 이동하여 하나 또는 여러 프로젝트를 선택한 다음 목록 맨 위에 있는 **자세히** 아이콘 ![추가 메뉴](assets/qs-more-icon-on-an-object.png)를 클릭합니다.

   ![표현식 다시 계산](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 재무 상태를 대량으로 재계산할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.

1. **재무 다시 계산**&#x200B;을 클릭합니다.

   프로젝트의 모든 계획된 비용 및 수익은 새로운 정보로 다시 계산됩니다.

   브라우저 맨 위에 프로젝트의 재무 정보가 성공적으로 다시 계산되었다는 확인 메시지가 표시됩니다.
잠기지 않은 기존 비용 값과 일부 수익 값은 새 비율을 반영하도록 업데이트됩니다.

## 수동으로 재무 일괄 재계산{#manually-recalculate-finances-in-bulk}

여러 프로젝트를 일괄적으로 편집하여 여러 프로젝트의 재무를 수동으로 다시 계산할 수 있습니다. 이로 인해 프로젝트의 수입이 소급하여 다시 계산됩니다.

>[!IMPORTANT]
>
>이 문서의 [기존 시간이 있는 작업에 대한 재무 데이터 유지](#preserve-financial-data-for-tasks-with-existing-hours) 섹션의 단계를 따라 재무를 수동으로 다시 계산할 때 수익 값이 새 요금을 반영하도록 업데이트되지 않도록 할 수 있습니다. 프로젝트의 재무 정보를 수동으로 다시 계산할 때 비용 값은 항상 새로운 요율을 반영하도록 업데이트됩니다.

여러 프로젝트의 재무 정보를 수동으로 다시 계산하려면

1. 프로젝트 목록으로 이동합니다.
1. 목록에서 여러 프로젝트를 선택한 다음 목록 맨 위에 있는 **자세히** 아이콘 ![추가 메뉴](assets/qs-more-icon-on-an-object.png)를 클릭합니다.

   ![표현식 다시 계산](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >프로젝트의 복잡성에 따라 최적의 성능을 보장하기 위해 일괄 편집할 때 많은 수의 프로젝트를 선택하지 않는 것이 좋습니다. 프로젝트를 너무 복잡하게 만들 수 있는 몇 가지 사항은 여러 종속성 또는 할당이거나 사용자 정의 필드의 수가 많을 수 있습니다.

1. **재무 다시 계산**&#x200B;을 클릭합니다.

   선택한 프로젝트의 모든 계획된 비용 및 수익은 새로운 정보로 다시 계산됩니다.

   프로젝트의 재무 정보가 성공적으로 다시 계산되었다는 확인 메시지가 브라우저 맨 위에 표시됩니다.

## 재무 자동 재계산을 트리거하는 작업

다음 작업은 Workfront에서 프로젝트의 재무 재계산을 트리거합니다.

* 작업 상태 변경 중
* 시간이 있는 작업을 다른 프로젝트로 이동
* 프로젝트 상태를 완료에서 활성 상태로 변경

>[!NOTE]
>
>프로젝트 상태를 변경하면 계획된 값만 다시 계산됩니다.

**재무 다시 계산**&#x200B;을 클릭하여 프로젝트 수준의 **기타** 메뉴 ![기타 메뉴](assets/qs-more-menu.png)에서 재무 정보를 수동으로 다시 계산할 수도 있습니다.
