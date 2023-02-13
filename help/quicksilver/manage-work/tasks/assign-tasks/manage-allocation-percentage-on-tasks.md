---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 작업에 대한 사용자 또는 역할 할당 비율 관리
description: 할당 백분율은 지정된 자원이 하루에 작업에 대해 작업하도록 계획되는 시간을 나타냅니다. 작업 기간 동안 리소스가 할당된 작업 일의 비율(사용자 또는 프로젝트 일정에 따라)입니다.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# 작업에 대한 사용자 또는 역할 할당 비율 관리

할당 백분율은 지정된 자원이 하루에 작업에 대해 작업하도록 계획되는 시간을 나타냅니다. 작업 기간 동안 리소스가 할당된 작업 일의 비율(사용자 또는 프로젝트 일정에 따라)입니다.

>[!NOTE]
>
>사용자를 작업에 지정할 때 해당 스케줄에 따른 가용성은 작업 및 문제의 계획 및 예상 날짜에 영향을 줍니다. 예약에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>작업에 대한 권한 부여 이상</p> <p>작업 편집 상자에서 할당 비율을 갱신하기 위한 권한 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업에 대한 퍼센트 할당 수정에 대한 고려 사항

* 사용자는 기본적으로 할당되는 작업에 동일한 시간 백분율로 할당됩니다.
* 작업의 기간 유형이 계산된 작업 또는 작업 중심인 경우에만 작업에 할당된 사용자 및 작업 역할에 대한 할당 퍼센트를 수동으로 수정할 수 있습니다.

   자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* 작업에 할당된 팀에 대한 퍼센트 할당은 수정할 수 없습니다.
* 문제에 할당된 사용자 및 작업 역할에 대한 비율 할당은 수정할 수 없습니다.

## 작업에 대한 사용자 또는 역할 퍼센트 할당을 수정합니다

1. 퍼센트 할당을 변경하는 자원이 있는 작업으로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 작업 이름 옆에 있는 **편집**.

   또는

   을(를) 클릭합니다. **지정** 작업 헤더에서 영역을 클릭한 다음 **고급**.

1. 다음을 확인합니다. **기간 유형** 작업은 다음 중 하나입니다.

   * 계산된 작업
   * 작업량 고정

   >[!TIP]
   >
   >* 계산된 지정 기간 유형의 경우 Workfront에서는 다음 공식을 사용하여 각 할당자의 할당 퍼센트를 계산합니다. `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* 단순 기간 유형의 경우 할당 비율이 아니라 각 리소스에 지정된 시간을 예측할 수 있습니다.


1. 클릭 **지정**, 그런 다음 를 수정합니다 **할당** 각 작업 할당자에 대해

   사용자 및 Job 역할 지정에 대한 할당 백분율만 수정할 수 있습니다.

   작업에 지정된 팀의 할당 비율은 수정할 수 없습니다.

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. **저장**&#x200B;을 클릭합니다.
