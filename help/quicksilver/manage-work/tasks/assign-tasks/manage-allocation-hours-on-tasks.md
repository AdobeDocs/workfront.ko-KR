---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업에 대한 사용자 및 역할 할당 시간 관리
description: 작업에 사용자 또는 역할을 할당할 때 작업을 완료하기 위해 일정 시간 동안 작업에 할당됩니다. 작업 기간 유형이 단순인 경우 각 사용자 또는 작업 역할이 작업에 할당될 때 할당되는 시간을 수동으로 수정할 수 있습니다.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# 작업에 대한 사용자 및 역할 할당 시간 관리

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<div class="preview">

이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기 릴리스의 1주일부터 모든 고객을 위한 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다.

자세한 내용은 [인터페이스 현대화](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)를 참조하십시오.

</div>

할당 시간은 할당된 자원이 작업에 대해 작업할 계획인 총 시간을 나타냅니다. 시간은 작업 기간 동안 주어진 일 또는 평일, 주 또는 월에 사용자가 할당된 시간을 나타냅니다.

작업에 대한 고급 할당을 수행할 때 할당 시간을 수정할 수 있습니다.

>[!NOTE]
>
>작업에 사용자를 할당할 때 예약에 따라 가용성이 작업 및 문제의 계획 및 예상 일자에 영향을 줍니다. 일정에 대한 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>작업 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>작업에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td>
   <td><p>작업에 대한 또는 더 높은 권한 부여</p>
   <p>이전 환경을 사용하여 작업 <span class="preview">을(를) 편집할 때 작업 편집 상자에서 할당 시간을 업데이트할 수 있는 권한을 편집합니다. 새 경험에서 작업을 편집할 때 작업 편집 상자에서 할당 시간을 더 이상 관리할 수 없습니다.</span></p> <p>자세한 내용은 <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">작업 편집</a>을 참조하세요.</p></td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation hours in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.-->


## 작업 할당 시간을 수정하기 위한 고려 사항

>[!IMPORTANT]
>
>작업에 대한 각 할당에 대한 할당을 수동으로 수정하면 작업의 계획된 시간이 그에 따라 업데이트될 수 있습니다. 자세한 내용은 문서 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md#update)에서 [사용자 할당을 관리할 때 작업 계획된 시간 업데이트](../../../manage-work/tasks/task-information/planned-hours.md) 섹션을 참조하십시오.

* 작업에 할당된 개별 리소스에 할당된 총 시간은 작업의 계획된 시간을 나타냅니다.
* 작업에 한 명의 사용자 또는 역할이 할당된 경우 해당 사용자 또는 역할에 할당된 시간이 작업의 계획된 시간과 일치합니다.
* 복수 할당의 경우 태스크 기간 유형이 단순일 경우 기본적으로 각 사용자 또는 작업 역할에는 동일한 시간 동안 태스크에 대한 작업이 지정됩니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [기간 유형 개요: 단순](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 작업에 단순 기간 유형이 있는 경우 각 사용자 또는 작업 역할에 대해 할당된 시간을 수동으로 변경하여 일부 작업 할당자가 다른 사용자보다 작업에 대해 더 많은 시간을 할애할 수 있음을 나타낼 수 있습니다.
* 작업에 할당된 팀에 할당된 시간은 수정할 수 없습니다.
* 문제에 대한 사용자 또는 작업 역할 할당을 수동으로 수정할 수 없습니다.
* 업무 균형자를 사용하여 작업 또는 문제에 대한 사용자의 일별, 주별 또는 월별 할당을 관리할 수도 있습니다. 자세한 내용은 [업무 균형자에서 사용자 할당 관리](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)를 참조하십시오.

## 작업에 대한 사용자 또는 역할 할당 시간 수정

1. 할당 시간을 변경할 할당에 대한 작업으로 이동합니다.
1. 작업 헤더의 **할당** 영역을 클릭한 다음 **고급**&#x200B;을 클릭합니다.
1. 작업의 **기간 유형**&#x200B;이(가) **단순**&#x200B;인지 확인하십시오.
1. 각 작업 할당자에 대한 **할당** 필드를 수정합니다. 작업의 전체 기간 동안 이 작업에 대한 각 할당에 대한 전체 할당입니다. 작업의 전체 **계획된 시간**&#x200B;도 업데이트할 수 있습니다.

   ![할당 수정](assets/advanced-assignments-duration-type-allocations.png)

1. **저장**&#x200B;을 클릭합니다.
