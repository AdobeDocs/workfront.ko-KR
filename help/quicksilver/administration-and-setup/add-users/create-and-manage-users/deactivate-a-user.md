---
title: 사용자 비활성화 또는 재활성화
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront 관리자는 사용자를 비활성화하거나 다시 활성화할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 72d0b8e0e190f774c7e3f14a78904fb1dd3f2b14
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 2%

---

# 사용자 비활성화 또는 다시 활성화 {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="사용자 비활성화"
>abstract="사용자를 비활성화하면 Workfront와 Frame.io에서 해당 사용자가 제거됩니다. 비활성화된 사용자는 나중에 다시 활성화할 수 있습니다."

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

사용자가 조직을 떠나면 다른 사용자를 업데이트에 추가하거나 작업을 할당할 때 혼동을 주지 않도록 시스템에서 비활성화하는 것이 좋습니다. 사용자를 비활성화하면 다른 사용자가 시스템에서 사람을 검색할 때 더 이상 해당 이름이 표시되지 않습니다.

관리자는 설정 영역에서 비활성 사용자를 볼 수 있습니다.

언제든지 사용자를 다시 활성화할 수 있습니다.

>[!IMPORTANT]
>
>* 조직을 떠난 사용자를 삭제하는 것보다 비활성화하는 것이 좋습니다. 사용자가 삭제되면 해당 사용자와 연결된 Workfront의 모든 기록이 손실됩니다. 여기에는 작업 할당, 메모, 시간, 문서 및 한 번 만든 다른 모든 개체와의 연관성이 포함됩니다.
>
>* Workfront에서 사용자를 비활성화하면 Workfront과 디지털 증명 모두에 대한 사용자 라이선스가 제거됩니다. 또한 사용자에게 더 이상 작업을 할당할 수 없습니다. 사용자가 비활성화되면 다른 사용자가 해당 사용자의 Workfront 라이선스 및 증명 라이선스를 사용할 수 있습니다. 비활성화된 사용자 프로필의 다른 모든 정보는 변경되지 않습니다.
>
>* Workfront의 사용자를 비활성화해도 Adobe Admin Console의 Workfront 제품 프로필에서 사용자가 제거되지는 않습니다. 자세한 내용은 [사용자 삭제](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)를 참조하십시오.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <b>에서 두 개의 </b>사용자 관리<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Workfront 관리자 또는 Standard 또는 Plan 라이선스 사용자를 비활성화하려면 먼저 해당 개체 및 활동을 다른 사용자와 연결해야 합니다.

자세한 내용은 이 문서에서 [Workfront 관리자 및 Standard 또는 Plan 라이선스 사용자 비활성화 정보](#about-deactivating-workfront-administrators-and-plan-license-users)를 참조하십시오.

## 사용자 비활성화

사용자를 비활성화할 때는 다음 사항에 유의하십시오.

* 사용자가 시스템에 액세스할 수 없습니다.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* 사용자와 관련된 모든 데이터는 유지됩니다.
* 비활성화된 사용자 라이선스를 다른 사용자에게 할당할 수 있습니다.

사용자를 비활성화하려면:

{{step-1-to-users}}

1. 사용자 목록에서 사용자를 선택합니다.
1. **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png)을 클릭한 다음 **비활성화**&#x200B;를 클릭합니다.

1. **사용자 비활성화** 대화 상자에서 **비활성화**&#x200B;를 클릭합니다.

## 비활성화 예약

관리자는 사용자가 실제로 조직을 떠나기 전에 비활성화 표시를 해야 할 수 있습니다. 예를 들어 계약상으로 바인딩된 사용자와 함께 작업하는 경우 제한된 기간 동안 시스템에 있으며 종료 날짜를 알 수 있습니다. 해당 날짜에 비활성화되도록 예약할 수 있습니다.

Workfront 관리자 및 플랜 라이선스 사용자는 사용자 프로필에서 비활성화 날짜를 볼 수 있습니다.

사용자의 비활성화를 예약하려면 다음을 수행합니다.

{{step-1-to-users}}

1. 사용자 목록에서 사용자를 선택합니다.

   또는

   (선택 사항) 여러 사용자를 선택하여 일괄 비활성화 일정을 예약합니다.

1. **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. **사용자 편집** 상자의 왼쪽 패널에서 **리소스 계획**&#x200B;을 클릭합니다.
1. **비활성화 날짜 설정**&#x200B;을 클릭합니다.

1. **비활성화 날짜**&#x200B;에 대한 날짜와 시간을 선택하십시오.

   >[!NOTE]
   >
   >* 시간 상자에서 분이 아닌 전체 시간 증가만 선택할 수 있습니다.
   >* 경과한 현재 날짜의 시간을 선택하면 Workfront은 오전 12:00에 다음 날짜의 비활성화를 예약합니다.
   >* 선택한 시간은 비활성화를 예약하는 사용자의 컴퓨터 시간대와 일치합니다.

1. **저장**&#x200B;을 클릭합니다.

사용자는 선택한 날짜 이후에 비활성화됩니다. 여러 사용자를 일괄 비활성화하도록 선택한 경우 선택한 모든 사용자는 선택한 시간 이후에 선택한 날짜에 비활성화됩니다.

비활성화하도록 예약한 사용자에 대한 보고서를 작성하여 어떤 사용자가 비활성화될 것인지에 대한 최신 정보를 지속적으로 제공하는 것이 좋습니다. 사용자가 비활성화된 후에 비활성화가 발생했다는 확인이 없습니다.

## 사용자 다시 활성화

{{step-1-to-users}}

1. 사용자를 선택하고 **자세히** 아이콘 ![추가 아이콘](assets/more-icon.png)을 클릭한 다음 **활성화**&#x200B;를 클릭합니다.

1. **사용자 다시 활성화** 대화 상자에서 드롭다운 메뉴에서 새 **액세스 수준**&#x200B;을 선택한 다음 **다시 활성화**&#x200B;을 클릭합니다.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### 사용자를 다시 활성화하면 증명이 미치는 영향

비활성화된 사용자는 할당된 기본 증명 역할과 증명 라이선스를 잃게 됩니다(Workfront Premium 레거시 플랜을 사용하는 경우). 사용자를 다시 활성화하도록 선택하는 경우 다음을 수행해야 합니다.

* 라이센스를 재할당합니다(Workfront Premium 레거시 플랜을 사용하는 경우). Workfront 증명 계획에 대한 자세한 내용은 [Workfront의 증명 기능에 액세스](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)를 참조하십시오.
* 올바른 증명 역할이 있는지 확인합니다. 재활성화된 증명 사용자에게는 새 사용자에 대한 기본 증명 역할로 지정된 모든 항목이 할당됩니다. 자세한 내용은 [기본 증명 역할 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)을 참조하십시오.

## Workfront 관리자 및 Standard 또는 Plan 라이선스 사용자 비활성화 정보

Workfront 관리자 또는 플랜 라이선스가 있는 사용자를 비활성화하기 전에 해당 사용자와 관련된 Workfront 개체 및 활동을 확인한 후 필요에 따라 다른 Workfront 관리자 또는 플랜 라이선스 사용자와 연결해야 합니다.

이러한 개체 및 활동에는 다음이 포함될 수 있습니다.

* 사용자에게 할당된 작업 또는 문제입니다.
* 사용자가 소유한 프로젝트.
* 사용자의 액세스 권한으로 실행되도록 설정된 보고서입니다.
* 사용자가 소유한 템플릿.
* 사용자가 리소스 관리자로 설정된 프로젝트 및 템플릿입니다.
* Workfront 관리자 또는 플랜 라이선스 사용자가 기본 피할당자인 요청 대기열 라우팅 규칙입니다.
* 사용자를 포함하는 단계가 있는 승인 프로세스(특히 해당 단계가 단계의 유일한 승인자인 경우).
* 사용자를 승인자로 나열하는 타임시트.
* 사용자를 승인자로 나열하는 타임시트 프로필.
* 사용자를 포함하는 자동화된 워크플로 증명.

## 사용자를 비활성화하도록 예약할 때 리소스 계획에 미치는 영향

사용자를 비활성화하도록 예약하면 예산 시간에 사용할 수 있는 것으로 리소스 플래너에 더 이상 표시되지 않습니다. 리소스 풀의 일부로 남아 있는 경우 리소스 플래너에 표시되지만, 예정된 비활성화 날짜부터 가용성이 0시간으로 설정됩니다.

리소스 플래너는 사용자의 모든 작업 역할과 작업의 계획된 완료 일자를 고려하고 그에 따라 리소스를 계산합니다.

리소스 플래너에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

