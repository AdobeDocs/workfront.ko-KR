---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업에 대한 사용자 또는 역할 할당 백분율 관리
description: 할당 백분율은 할당된 자원이 하루 동안 작업에 대해 작업할 계획인 시간을 나타냅니다. 작업 기간 동안 자원이 할당되는 근무일(사용자 또는 프로젝트 일정에 따라)의 백분율입니다.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 1%

---

# 작업에 대한 사용자 또는 역할 할당 백분율 관리

할당 백분율은 할당된 자원이 하루 동안 작업에 대해 작업할 계획인 시간을 나타냅니다. 작업 기간 동안 자원이 할당되는 근무일(사용자 또는 프로젝트 일정에 따라)의 백분율입니다.

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
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p> 
   <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 Contribute 이상 권한</p> <p>작업 편집 상자에서 할당 비율을 업데이트하는 권한 편집</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업에 대한 비율 할당 수정에 대한 고려 사항

* 사용자에게는 기본적으로 할당된 작업에 동일한 시간의 비율이 할당됩니다.
* 작업의 기간 유형이 계산된 작업 또는 작업량 고정 인 경우에만 작업에 할당된 사용자 및 작업 역할에 대한 할당 비율을 수동으로 수정할 수 있습니다.

  자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)를 참조하십시오.

* 작업에 할당된 팀에 대한 비율 할당은 수정할 수 없습니다.
* 문제에 할당된 사용자 및 작업 역할에 대한 백분율 할당을 수정할 수 없습니다.

## 작업에 대한 사용자 또는 역할 비율 할당 수정

1. 퍼센트 할당을 변경할 자원에 대한 작업으로 이동합니다.
1. 작업 이름 옆에 있는 **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.

   또는

   작업 헤더의 **할당** 영역을 클릭한 다음 **고급**&#x200B;을 클릭합니다.

1. 작업의 **기간 유형**&#x200B;이(가) 다음 중 하나인지 확인하십시오.

   * 계산된 작업
   * 작업량 고정

   >[!TIP]
   >
   >* 계산된 할당 기간 유형의 경우 Workfront에서는 다음 수식을 사용하여 각 할당자의 할당 백분율을 계산합니다. `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* 단순 기간 유형의 경우 할당 퍼센트가 아니라 각 자원에 할당된 시간을 예상할 수 있습니다.

1. **할당**&#x200B;을 클릭한 다음 각 작업 할당자에 대해 **할당**&#x200B;을 수정합니다.

   사용자 및 작업 역할 할당에 대한 할당 퍼센트만 수정할 수 있습니다.

   작업에 할당된 팀의 할당 백분율을 수정할 수 없습니다.

   ![할당 백분율 수정](assets/advanced-assignments-allocation-percentage.png)

1. **저장**&#x200B;을 클릭합니다.
