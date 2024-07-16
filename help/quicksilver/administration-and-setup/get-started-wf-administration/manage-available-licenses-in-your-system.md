---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 시스템에서 사용 가능한 라이선스 관리
description: Adobe Workfront 관리자는 조직에 대해 구매한 라이선스 수와 현재 사용 중인 라이선스 수를 포함하여 Workfront 계정에 대한 정보에 액세스할 수 있습니다.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 834d08d8e9896b80d047d00b2008dd9a002a95da
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# 시스템에서 사용 가능한 라이선스 관리

<!-- Audited: 12/2023 -->

Adobe Workfront 관리자는 조직에 대해 구매한 라이선스 수와 현재 사용 중인 라이선스 수를 포함하여 Workfront 계정에 대한 정보에 액세스할 수 있습니다.

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
    <p>새로운 기능: 표준</p>
    <p>또는</p>
    <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 또는 그룹 관리자여야 합니다. 그룹 관리자의 라이선스 정보 보기는 제한됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

>[!NOTE]
>
>다음 명령문은 신규 계획에만 적용됩니다.
>
>Select 플랜의 경우:
>
>1. 시스템 관리자는 홈 그룹에 대한 제한을 설정할 수 없습니다.
>2. 시스템 관리자는 모든 홈 그룹에서 사용된 총 라이선스 수만 볼 수 있습니다.
>3. 그룹 관리자가 라이선스 페이지에 전혀 액세스할 수 없습니다.
>
>Prime 및 Ultimate 플랜의 경우:
>
>1. 시스템 관리자는 [라이센스] 페이지에 홈 그룹을 추가하여 해당 그룹의 라이센스 활용도를 볼 수 있으며 라이센스 제한도 설정할 수 있습니다.
>2. 그룹 관리자는 라이센스 페이지에 액세스하여 시스템 관리자가 라이센스 페이지에 추가한 그룹에서 라이센스를 사용할 수 있습니다.
>3. 그룹 관리자는 다른 홈 그룹에 대한 정보를 보거나 최대값을 추가할 수 없습니다.

+++

## 조직의 라이선스 보기

Workfront에 추가하는 사용자에게 액세스 수준을 할당하면 사용 중인 라이선스 수가 자동으로 업데이트됩니다. 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

시스템에서 라이센스 정보를 보려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**&#x200B;를 클릭합니다.

   이 페이지에 나열된 라이선스에 대한 자세한 내용은 [라이선스 개요](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)를 참조하십시오.

   >[!NOTE]
   >
   >증명 라이선스는 Workfront 라이선스 외에 유료 Workfront Proof 추가 기능을 구입한 고객에게만 제공됩니다. 이 추가 기능에 대한 자세한 내용은 [Workfront Proof: 문서 색인](../../workfront-proof/workfront-proof.md)을 참조하세요.

1. (조건부) 메시지 **최대값을 설정하려면 이 문서의 [라이선스 페이지에 홈 그룹 추가 또는 제거](#add-or-remove-a-home-group-to-the-licenses-page) 섹션에 설명된 대로 시스템에 홈 그룹을 추가**&#x200B;해야 합니다.

   >[!NOTE]
   >
   >새 플랜의 경우 Select 플랜에서는 관리자가 홈 그룹별로 라이센스를 볼 수 없습니다. 사용된 라이센스의 전체 수만 볼 수 있습니다. Prime 및 Ultimate 플랜은 홈 그룹당 최대 라이선스 수를 설정할 수 있는 기능을 제공합니다.

## Workfront 추가 기능에 대한 라이선스 정보 보기

조직에 유료 Workfront Proof 추가 기능이 있는 경우 사용된 라이선스 수와 사용 가능한 라이선스 수가 표시됩니다. 예를 들어, 10개의 증명 라이선스 중 **5개**&#x200B;는 조직이 현재 구입한 10개의 Workfront Proof 라이선스 중 5개를 사용하고 있음을 나타냅니다.

![Workfront 추가 기능에 대한 라이선스](assets/updated-licenses-page.png)

조직에서 Workfront 목표를 구매한 경우 이 제품에 대한 라이선스 정보도 여기에 표시됩니다. 이 경우 다음 정보를 볼 수 있습니다.

* 귀사에서 구매한 총 Workfront Goals 라이선스 수입니다
* 사용자와 연결된 Workfront Goals 라이선스 수입니다. 액세스 수준에서 목표에 대한 보기 액세스 권한 이상을 부여한 사용자 수입니다.

Workfront 목표에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오. Workfront 목표에 액세스하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표에 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)를 참조하십시오.

>[!NOTE]
>
>Workfront을 사용하면 구입한 더 많은 Workfront Goals 라이선스를 할당할 수 있습니다. 그러나 Workfront 목표 계약에서 허용하는 것보다 더 많은 라이선스를 할당하면 Workfront 계정 관리자가 연락하여 계약 번호를 초과했음을 알려 줍니다.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>관리 액세스 권한이 없는 사용자는 그룹 보고서를 사용하여 라이선스 수를 볼 수 있습니다. 보고서 탭에서 새 그룹 보고서를 만들고 다음 열을 추가합니다.
>
>* 라이선스 유형 제한: 작업자 제한
>* 라이선스 유형 제한: 플래너 제한
>
>보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

## 월별 증명 및 문서 결정 할당에 대한 정보 보기

>[!IMPORTANT]
>
>증명 및 문서 결정 제한은 새 라이선스의 사용자에게만 적용됩니다. 자세한 내용은 [새 라이선스 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)를 참조하세요.

모든 비유료 Workfront 라이선스에 대해 증명 및 문서 결정이 제한됩니다. 한도는 매월 사용자별로 재설정됩니다.

사용 중인 플랜에 따라 각 라이센스의 결정 제한이 다릅니다. 설정 > 라이센스에서 월별 할당을 볼 수 있습니다.

증명 및 문서 결정 제한에 대한 자세한 내용은 [비유료 사용자에 대한 제한된 문서 및 증명 결정 개요](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)를 참조하십시오.

![월별 결정 할당](assets/monthly-decision-allotment.png)

## 라이선스 페이지에 홈 그룹 추가 또는 제거 {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

각 사용자는 하나의 홈 그룹에만 할당할 수 있습니다. Workfront은 각 홈 그룹에 할당되어 현재 사용되는 라이선스 수를 계산하여 그룹 중심의 라이선스 수를 제공합니다.

**최대값을 설정하려면 [라이선스] 페이지에서 [홈 그룹]을 추가**&#x200B;해야 합니다. 메시지가 표시되면 [라이선스] 페이지에 하나 이상의 홈 그룹을 추가해야 합니다.

>[!IMPORTANT]
>
>* 홈 그룹을 사용하여 라이선스를 효과적으로 관리하려면 사업부용 특정 홈 그룹을 설정한 후 최대 라이선스 수를 업데이트하는 것이 좋습니다. 자세한 내용은 [홈 그룹 개요](../../administration-and-setup/manage-groups/groups-overview/home-groups.md)를 참조하세요.
>* 최상위 그룹만 홈 그룹으로 추가할 수 있으며 하위 그룹은 추가할 수 없습니다. 사용자에게 홈 그룹으로 할당된 하위 그룹이 있는 경우 해당 하위 그룹 위의 최상위 그룹에 대한 라이선스 수에 라이센스가 추가됩니다.
>

라이선스 페이지에 홈 그룹을 추가하거나 제거하려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**&#x200B;를 클릭합니다.

1. **그룹 목록 관리**&#x200B;를 클릭합니다.
1. **홈 그룹** 상자에 최상위 그룹 이름을 입력하십시오.
1. 그룹을 추가하려면 표시될 때 해당 이름을 클릭합니다.

   또는

   그룹을 제거하려면 그룹 이름 오른쪽에 있는 X 아이콘을 클릭합니다.

1. **저장**&#x200B;을 클릭합니다.

Workfront 관리자는 홈 그룹에 대해 최대 라이선스 수를 설정하여 사업부가 다른 사업부용으로 구입한 Workfront 라이선스를 사용하지 못하도록 할 수 있습니다. 자세한 내용은 이 문서에서 [홈 그룹의 최대 라이선스 수 설정](#set-the-maximum-license-count-for-a-home-group)을 참조하십시오.

## 홈 그룹에 대한 최대 라이선스 수 설정 {#set-the-maximum-license-count-for-a-home-group}

Workfront 관리자는 시스템의 최상위 홈 그룹에 대해 최대 라이선스 수를 설정할 수 있습니다. 이를 통해 사업부가 조직 내 다른 사업부용으로 구입한 Workfront 라이선스를 사용하지 못하도록 할 수 있습니다.

기본적으로 최대 라이선스 수는 N/A로 설정되어 있으며, 이는 제한이 없음을 의미합니다.

그룹 관리자는 자신이 관리하는 홈 그룹에서 할당되고 사용되는 라이선스 수를 볼 수 있습니다. 자세한 내용은 [그룹에 할당되어 사용되는 라이선스 수 보기](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)를 참조하십시오.

홈 그룹에 대한 최대 라이선스 수를 설정하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**&#x200B;를 클릭합니다.

1. 목록에서 홈 그룹을 찾습니다.
1. 그룹의 **Max** 열에서 최대값을 설정할 값을 클릭합니다.
1. 최대 숫자를 입력한 다음 Enter 키를 누릅니다.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >그룹의 최대 라이선스 값을 다시 기본값으로 설정하려면 0을 입력하지 마십시오. 대신 상자에서 숫자를 삭제합니다. 최대 라이선스 값을 0으로 설정하면 해당 그룹에 할당된 라이선스가 없음을 의미합니다.
