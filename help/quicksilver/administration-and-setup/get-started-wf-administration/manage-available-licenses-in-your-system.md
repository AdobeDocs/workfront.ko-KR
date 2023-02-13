---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 시스템에서 사용 가능한 라이센스 관리
description: Adobe Workfront 관리자는 조직에 대해 구입한 라이선스 수와 현재 사용 중인 라이선스 수를 비롯하여 Workfront 계정에 대한 정보에 액세스할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 5ec772260c965b83824ff307bc84755fe06e1ba0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# 시스템에서 사용 가능한 라이센스 관리

Adobe Workfront 관리자는 조직에 대해 구입한 라이선스 수와 현재 사용 중인 라이선스 수를 비롯하여 Workfront 계정에 대한 정보에 액세스할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 조직의 라이선스 보기

Workfront에 추가하는 사용자에게 액세스 수준을 할당하면 사용 중인 라이선스 수가 자동으로 업데이트됩니다. 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

시스템에서 라이센스 정보를 보려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**.

   이 페이지에 나열된 라이센스에 대한 자세한 내용은 [Adobe Workfront 라이선스 개요](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >증명 라이센스는 Workfront 라이선스 외에 유료 Workfront 증명 추가 기능을 구입한 고객에게만 제공됩니다. 이 추가 기능에 대한 자세한 내용은 [Workfront 증명](../../workfront-proof/workfront-proof.md).

1. (조건부) 메시지가 표시되면 **최대값을 설정하려면 홈 그룹을 추가해야 합니다**&#x200B;섹션에 설명된 대로 시스템에 홈 그룹을 추가합니다. [라이센스 페이지에 홈 그룹 추가 또는 제거](#add-or-remove-a-home-group-to-the-licenses-page) 참조하십시오.

## Workfront 추가 기능의 라이센스에 대한 정보 보기

아래 스크린샷에서 **증명 라이센스 10개 중 5개** 이 조직에 유료 Workfront 증명 추가 기능이 있고 현재 구입한 Workfront 증명 라이선스 10개 중 5개를 사용하고 있음을 나타냅니다.

![](assets/updated-licenses-page.png)

조직에서 Workfront 목표를 구입한 경우 이 제품에 대한 라이선스 정보도 여기에 표시됩니다. 이 경우 다음 정보를 볼 수 있습니다.

* 회사에서 구입한 총 Workfront 목표 라이선스 수
* 사용자와 연결된 Workfront 목표 라이선스 수입니다. 액세스 수준에서 목표에 대한 보기 액세스 권한을 적어도 부여할 사용자 수입니다.

Workfront 목표에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../workfront-goals/goal-management/wf-goals-overview.md). Workfront 목표 액세스에 대한 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront을 사용하면 구입한 Workfront 목표 라이센스를 더 많이 할당할 수 있습니다. 그러나 Workfront 목표 계약에 허용된 것보다 더 많은 라이선스를 할당하면 Workfront 계정 관리자가 사용자에게 연락하여 계약 번호를 초과했음을 알려줍니다.

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>관리자 권한이 없는 사용자는 그룹 보고서를 사용하여 라이선스 수를 볼 수 있습니다. 보고서 탭에서 새 그룹 보고서를 만들고 다음 열을 추가합니다.>
>* 라이선스 유형 제한: 작업자 제한
>* 라이선스 유형 제한: 계획자 제한
>
>보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 라이센스 페이지에 홈 그룹 추가 또는 제거 {#add-or-remove-a-home-group-to-the-licenses-page}

이 기능을 사용하려면 비즈니스 또는 엔터프라이즈 Workfront 플랜이 필요합니다. 사용 가능한 다양한 계획에 대한 자세한 내용은 [Workfront 플랜.](https://www.workfront.com/plans)

각 사용자는 하나의 홈 그룹에만 할당할 수 있습니다. Workfront은 각 홈 그룹에서 현재 할당되고 할당된 라이센스의 수를 계산하여 그룹 지향 라이선스 수를 제공합니다.

메시지가 표시되면 **최대값을 설정하려면 홈 그룹을 추가해야 합니다** 라이센스 페이지에서 하나 이상의 홈 그룹을 라이센스 페이지에 추가해야 합니다.

>[!IMPORTANT]
>
>* 홈 그룹을 사용하여 라이선스를 효과적으로 관리하려면 최대 라이선스 수를 업데이트하기 전에 비즈니스 단위에 특정 홈 그룹을 설정하는 것이 좋습니다. 자세한 내용은 [홈 그룹 개요](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* 최상위 그룹만 홈 그룹으로 추가할 수 있고 하위 그룹은 추가할 수 없습니다. 사용자에게 홈 그룹으로 지정된 하위 그룹이 있는 경우 해당 라이센스가 해당 하위 그룹 위의 최상위 그룹에 대한 라이선스 수에 추가됩니다.
>


라이센스 페이지에 홈 그룹을 추가하거나 제거하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**.

1. 클릭 **그룹 목록 관리**.
1. 에 최상위 그룹 이름을 입력합니다. **홈 그룹** 상자.
1. 그룹을 추가하려면 그룹 이름이 나타나면 그룹 이름을 클릭합니다.

   또는

   그룹을 제거하려면 그룹 이름의 오른쪽에 있는 X 아이콘을 클릭합니다.

1. **저장**&#x200B;을 클릭합니다.

Workfront 관리자는 비즈니스 단위가 다른 비즈니스 단위에 대해 구매한 Workfront 라이센스를 사용하지 못하도록 홈 그룹에 대한 최대 라이선스 수를 설정할 수 있습니다. 자세한 내용은 [홈 그룹에 대한 최대 라이선스 수 설정](#set-the-maximum-license-count-for-a-home-group) 참조하십시오.

## 홈 그룹에 대한 최대 라이선스 수 설정 {#set-the-maximum-license-count-for-a-home-group}

Workfront 관리자는 시스템의 최상위 홈 그룹에 대한 최대 라이선스 수를 설정할 수 있습니다. 이를 통해 비즈니스 부서가 조직 내의 다른 비즈니스 단위에 대해 구입한 Workfront 라이센스를 사용하지 못하도록 할 수 있습니다.

기본적으로 최대 라이선스 수는 N/A로 설정되며, 이는 제한이 없음을 의미합니다.

그룹 관리자는 자신이 관리하는 홈 그룹에 할당되고 사용되는 라이센스 수를 볼 수 있습니다. 자세한 내용은 [새 Adobe Workfront 경험에서 그룹에 할당되고 사용되는 라이선스 수를 봅니다](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

홈 그룹에 대한 최대 라이선스 수를 설정하려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널 아래쪽에서 **시스템** > **라이선스**.

1. 목록에서 홈 그룹을 찾습니다.
1. 에서 **최대** 그룹의 열에서 최대값을 설정할 값을 클릭합니다.
1. 최대 숫자를 입력한 다음 Enter 키를 누릅니다.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >그룹의 최대 라이선스 값을 기본값으로 설정하려면 0을 입력하지 마십시오. 대신 상자에서 숫자를 삭제합니다. 최대 라이선스 값을 0으로 설정하면 해당 그룹에 할당된 라이센스가 없습니다.
