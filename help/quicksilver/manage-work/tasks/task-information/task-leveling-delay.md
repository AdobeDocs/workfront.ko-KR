---
product-area: projects
navigation-topic: task-information
title: 작업 평준화 지연 업데이트
description: 프로젝트에 있는 작업 일정 간에 충돌이 있을 수 있습니다. 자원 및 태스크를 스케줄 조정하여 자원 또는 자원 충돌을 레벨링하거나 해결할 수 있으므로 모든 태스크를 실제 스케줄 내에서 완료할 수 있습니다. 평준화 작업에 대한 자세한 내용은 Gantt 차트의 레벨 자원 을 참조하십시오.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# 작업 평준화 지연 업데이트

프로젝트에 있는 작업 일정 간에 충돌이 있을 수 있습니다. 자원 및 태스크를 스케줄 조정하여 자원 또는 자원 충돌을 레벨링하거나 해결할 수 있으므로 모든 태스크를 실제 스케줄 내에서 완료할 수 있습니다. 평준화에 대한 자세한 내용은 [간트 차트의 레벨 리소스](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

프로젝트 관리자 또는 태스크 담당자로서 자원 또는 스케줄링 충돌을 고려하여 개별 태스크에 레벨 조정 지연을 추가할 수도 있습니다. 다시 말해, Adobe Workfront의 수준이 보다 현실적인 스케줄인 작업이 리소스 충돌을 극복하도록 지연과 함께 작업을 예약할 수 있습니다.

작업에 평준화 지연을 추가하면 작업의 예상 완료 날짜가 조정됩니다. 예상 완료 날짜에 대한 자세한 내용은 [프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리 </p> <p>프로젝트에 대한 기여 또는 더 높은 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업에 평준화 지연 추가

1. 평준화 지연을 추가할 작업으로 이동합니다.
1. 을(를) 클릭합니다. **자세히 아이콘** 작업 이름의 오른쪽에 있는 **편집**.

   ![](assets/qs-task-edit-icon-highlighted-350x154.png)

1. 클릭 **설정**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 을(를) 지정합니다. **평준화 지연**&#x200B;를 입력한 다음 시간 단위를 선택합니다.\
   자원 충돌로 인해 리소스가 작업을 시작하는 데 지연되는 시간입니다.

   시간 단위에 대해 다음 옵션 중에서 선택합니다.

   * 분
   * 시간. 기본값입니다.
   * 일
   * 주
   * 개월
   * 경과 시간 (분)
   * 경과 시간
   * 경과 일수
   * 경과 주 수
   * 경과 기간 (월)

   >[!TIP]
   >
   >경과 시간은 작업의 지속 시간에 대한 시간 단위입니다. 휴일, 주말 및 휴일이 포함된 작업의 계획 시작 일자와 계획 완료 일자 사이의 시간입니다. 즉, 경과 시간은 달력 일수의 경과입니다.

1. 클릭 **저장**. 

 
