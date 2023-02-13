---
title: 리소스 관리에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront에서 리소스 관리에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# 리소스 관리에 대한 액세스 권한 부여

Adobe Workfront 관리자는 다음과 같이 액세스 수준을 사용하여 리소스 관리에 대한 사용자의 액세스를 정의할 수 있습니다. [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 지정 액세스 수준을 사용하여 리소스 관리 도구에 대한 사용자 액세스 구성

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) on **보기** 또는 **편집** 자원 관리 오른쪽에 있는 버튼을 선택한 다음 아래에서 부여할 기능을 선택합니다 **설정 세부 조정**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">플래너에서 우선 순위 및 예산 시간 편집</td> 
      <td> <p>이 라이센스가 있는 사용자는 다음을 수행할 수 있습니다.</p> <p>리소스 계획자에서 프로젝트의 우선 순위를 지정합니다.</p> <p>Resource Planning 도구(프로젝트의 Business Case의 Resource Planner 및 Resource Budgeting 섹션)의 자원에 대한 예산 배부</p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 풀 관리</td> 
      <td> <p>이 라이센스가 있는 사용자는 리소스 풀을 생성, 편집 및 삭제할 수 있습니다. 이 옵션은 기본적으로 비활성화됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>업무 균형자에서 계획된 시간 업데이트</span> </td> 
      <td> <p>이 라이센스를 가진 사용자는 작업 로드 밸런서에서 사용자 할당을 업데이트할 때 작업 항목의 계획 시간을 업데이트할 수 있습니다. 할당된 총 시간 수는 작업 항목의 계획 시간이 됩니다.</p> <p>이 옵션은 기본적으로 비활성화됩니다.</p> <p> 자세한 내용은 <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">작업 로드 밸런서에서 사용자 할당 관리</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 완료되면 를 클릭합니다 **저장**.

   액세스 수준이 만들어지면 사용자에게 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 라이선스 유형별 리소스 관리 액세스

각 액세스 수준의 사용자가 리소스 관리를 사용하여 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [리소스 관리](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 공유 문제에 대한 액세스

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

객체를 다른 사용자와 공유할 때 객체에 대한 예산 또는 자원 할당을 볼 수 있는 수신자의 권한은 세 가지 항목의 조합으로 결정됩니다.

* 리소스 관리에 대한 수신자의 액세스 수준 설정입니다
* 다음에 설명된 대로 재무 데이터에 대한 사용자의 액세스 권한 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* 공유자가 개체에 대해 부여한 재무 데이터에 대한 모든 권한

사용자가 객체를 공유할 때 객체의 재무 데이터에 부여할 수 있는 권한에 대한 자세한 내용은 [개체에 대한 재무 권한 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
