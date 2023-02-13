---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업에 대한 사용자 및 역할 할당 시간 관리
description: 사용자 또는 역할을 작업에 할당할 때 특정 시간 동안 작업을 완료하도록 할당됩니다. 작업 기간 유형이 단순인 경우, 각 사용자 또는 작업 역할이 작업에 할당될 때 할당되는 시간을 수동으로 수정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 작업에 대한 사용자 및 역할 할당 시간 관리

사용자 또는 역할을 작업에 할당할 때 특정 시간 동안 작업을 완료하도록 할당됩니다. 작업 기간 유형이 단순인 경우, 각 사용자 또는 작업 역할이 작업에 할당될 때 할당되는 시간을 수동으로 수정할 수 있습니다.

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
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 부여 이상</p> <p>작업 편집 상자에서 할당 시간을 갱신하기 위한 권한 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업의 할당 시간 수정을 위한 고려 사항

>[!IMPORTANT]
>
>작업에 대한 각 발령에 대한 할당을 수동으로 수정한 후 작업의 계획 시간이 그에 따라 업데이트될 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [사용자 할당을 관리할 때 작업 계획 시간 업데이트](../../../manage-work/tasks/task-information/planned-hours.md#update) 기사 [계획 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).

* 작업에 할당된 개별 자원에 할당된 총 시간(시간)은 작업의 계획 시간을 나타냅니다.
* 작업에 사용자 또는 역할 할당이 한 개 있는 경우 사용자 또는 역할에 할당된 시간이 작업의 계획 시간과 일치합니다.
* 여러 발령의 경우, 작업 기간 유형이 단순인 경우 기본적으로 각 사용자 또는 작업 롤에는 동일한 시간 내에 작업이 할당됩니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 작업에 단순 기간 유형이 있는 경우, 각 사용자 또는 작업 역할에 대해 할당된 시간 크기를 수동으로 변경하여 일부 작업 할당자가 다른 사용자보다 작업 시간을 더 많이 가질 수 있음을 나타낼 수 있습니다.
* 작업에 할당된 팀에 할당된 시간은 수정할 수 없습니다.
* 문제에 대한 사용자 또는 작업 역할 할당은 수동으로 수정할 수 없습니다.
* 작업 로드 밸런서를 사용하여 작업이나 문제에 대한 사용자의 일별, 주별 또는 월별 할당을 관리할 수도 있습니다. 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 작업에 대한 사용자 또는 역할 할당 시간 수정

1. 할당 시간을 변경하고자 하는 발령의 태스크로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 작업 이름 옆에 있는 **편집**, 그런 다음 **지정**.

   또는

   을(를) 클릭합니다. **지정** 작업 헤더에서 영역을 클릭한 다음 **고급**.

1. 다음을 확인합니다. **기간 유형** 작업 **단순**.
1. 수정 **할당** 각 작업 할당자에 대해 작업 전체 기간 동안 이 작업에 대한 각 할당에 대한 전체 할당입니다. 이 경우 작업의 전체 계획 시간을 업데이트할 수도 있습니다.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. **저장**&#x200B;을 클릭합니다.
