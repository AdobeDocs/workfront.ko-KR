---
product-area: projects
navigation-topic: task-information
title: 작업 레벨링 지연 업데이트
description: 프로젝트의 작업 일정 간에 충돌이 발생하는 경우가 있습니다. 현실적인 일정 내에서 모든 작업이 완료될 수 있도록 자원 및 작업의 스케줄을 조정하여 자원을 레벨링하거나 자원 충돌을 해결할 수 있습니다. 레벨링 작업에 대한 자세한 내용은 간트 차트에서 리소스 레벨링 을 참조하십시오.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# 작업 레벨링 지연 업데이트

프로젝트의 작업 일정 간에 충돌이 발생하는 경우가 있습니다. 현실적인 일정 내에서 모든 작업이 완료될 수 있도록 자원 및 작업의 스케줄을 조정하여 자원을 레벨링하거나 자원 충돌을 해결할 수 있습니다. 레벨링 작업에 대한 자세한 내용은 [간트 차트에서 리소스 레벨링](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)을 참조하십시오.

프로젝트 관리자 또는 작업 할당자는 리소스 또는 예약 충돌을 고려하여 개별 작업에 레벨링 지연을 추가할 수도 있습니다. 즉, Adobe Workfront에서 작업 수준을 조정할 때 리소스 충돌을 극복하는 보다 현실적인 일정을 만들 수 있도록 작업이 지연될 수 있습니다.

작업에 레벨링 지연을 추가하면 작업의 예상 완료 일자가 조정됩니다. 예상 완료 날짜에 대한 자세한 내용은 [프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)를 참조하십시오.

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리 </p> <p>프로젝트에 대한 Contribute 이상 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업에 레벨링 지연 추가

1. 레벨링 지연을 추가할 작업으로 이동합니다.
1. 작업 이름 오른쪽에 있는 **추가 아이콘**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. **설정**&#x200B;을 클릭합니다.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. **레벨링 지연**&#x200B;을(를) 시간 단위로 지정한 다음 시간 단위를 선택하십시오.\
   자원 충돌로 인해 작업 시작이 지연되는 시기입니다.

   시간 단위에 대해 다음 옵션 중에서 선택합니다.

   * 분
   * 시간. 이것이 기본값입니다.
   * 일
   * 주
   * 개월
   * 경과 시간(분)
   * 경과 시간
   * 경과 일수
   * 경과 주수
   * 경과 기간(월)

   >[!TIP]
   >
   >경과 시간은 작업 기간에 대한 시간 단위입니다. 휴일, 주말 및 휴무를 포함하는 작업의 계획된 시작 일자와 계획된 완료 일자 사이의 시간입니다. 즉, 경과 시간은 역일이 경과된 때이다.

1. **저장**&#x200B;을 클릭합니다. 

 
