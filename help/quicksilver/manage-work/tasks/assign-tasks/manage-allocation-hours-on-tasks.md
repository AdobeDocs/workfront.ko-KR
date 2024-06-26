---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업에 대한 사용자 및 역할 할당 시간 관리
description: 작업에 사용자 또는 역할을 할당할 때 작업을 완료하기 위해 일정 시간 동안 작업에 할당됩니다. 작업 기간 유형이 단순인 경우 각 사용자 또는 작업 역할이 작업에 할당될 때 할당되는 시간을 수동으로 수정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 작업에 대한 사용자 및 역할 할당 시간 관리

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경 또는 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">현재 릴리스에 대한 자세한 내용은 [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

작업에 사용자 또는 역할을 할당할 때 작업을 완료하기 위해 일정 시간 동안 작업에 할당됩니다. 작업 기간 유형이 단순인 경우 각 사용자 또는 작업 역할이 작업에 할당될 때 할당되는 시간을 수동으로 수정할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 또는 더 높은 권한 부여</p> <p>작업 편집 상자에서 할당 시간을 업데이트할 권한 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 할당 시간을 수정하기 위한 고려 사항

>[!IMPORTANT]
>
>작업에 대한 각 할당에 대한 할당을 수동으로 수정하면 작업의 계획된 시간이 그에 따라 업데이트될 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [사용자 할당 관리 시 작업 계획 시간 업데이트](../../../manage-work/tasks/task-information/planned-hours.md#update) 이 문서에서 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

* 작업에 할당된 개별 리소스에 할당된 총 시간은 작업의 계획된 시간을 나타냅니다.
* 작업에 한 명의 사용자 또는 역할이 할당된 경우 해당 사용자 또는 역할에 할당된 시간이 작업의 계획된 시간과 일치합니다.
* 복수 할당의 경우 태스크 기간 유형이 단순일 경우 기본적으로 각 사용자 또는 작업 역할에는 동일한 시간 동안 태스크에 대한 작업이 지정됩니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 작업에 단순 기간 유형이 있는 경우 각 사용자 또는 작업 역할에 대해 할당된 시간을 수동으로 변경하여 일부 작업 할당자가 다른 사용자보다 작업에 대해 더 많은 시간을 할애할 수 있음을 나타낼 수 있습니다.
* 작업에 할당된 팀에 할당된 시간은 수정할 수 없습니다.
* 문제에 대한 사용자 또는 작업 역할 할당을 수동으로 수정할 수 없습니다.
* 업무 균형자를 사용하여 작업 또는 문제에 대한 사용자의 일별, 주별 또는 월별 할당을 관리할 수도 있습니다. 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 작업에 대한 사용자 또는 역할 할당 시간 수정

1. 할당 시간을 변경할 할당에 대한 작업으로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 작업 이름 옆에 있는 을 클릭합니다. **편집**, 그런 다음 **할당**.

   또는

   다음을 클릭합니다. **할당** 작업 머리글의 영역을 클릭한 다음 **고급**.

1. 다음을 확인합니다. **기간 유형** 작업 중: **단순**.
1. 수정 **할당** 각 작업 할당자에 대해. 작업의 전체 기간 동안 이 작업에 대한 각 할당에 대한 전체 할당입니다. 작업의 전체 계획된 시간도 업데이트할 수 있습니다.

   프로덕션 환경의 샘플 이미지:
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">미리보기 환경의 샘플 이미지:</span>
   ![할당 수정](assets/advanced-assignments-duration-type-allocations.png)

1. **저장**&#x200B;을 클릭합니다.
