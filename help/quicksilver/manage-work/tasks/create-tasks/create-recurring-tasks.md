---
product-area: projects
navigation-topic: create-tasks
title: 반복 작업 만들기
description: 단일 프로젝트의 일부로 반복해야 하는 작업에 대한 반복 작업을 만들 수 있습니다.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# 반복 작업 만들기

단일 프로젝트의 일부로 반복해야 하는 작업에 대한 반복 작업을 만들 수 있습니다.

기존 반복 작업 편집의 영향을 비롯하여 반복 작업에 대한 일반적인 정보는 [반복 작업 개요](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 작업 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">작업에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 추가 기능을 사용하여 프로젝트에 사용 권한을 제공합니다.</p> <p>작업을 만들면 작업에 대한 관리 권한을 자동으로 받게 됩니다</p> <p> 작업 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">작업 공유 </a>. </p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 반복 작업 만들기

>[!NOTE]
>
>기존 작업을 수정하여 반복 작업을 만들 수 없습니다. 작업을 처음부터 새로 만들어야 합니다.

1. 반복 작업을 만들 프로젝트로 이동한 다음 **작업** 왼쪽 패널의 섹션에 있습니다.
1. 클릭 **새 작업**.

   새 작업 대화 상자가 표시됩니다.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 클릭 **추가 옵션** 그런 다음 작업 이름을 **작업 이름** 필드.
1. 새 작업을 추가한 것과 같은 방식으로 작업을 계속 업데이트합니다. 새 작업 추가에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. 클릭 **개요** 왼쪽 패널에 표시됩니다.
1. 아래로 스크롤하여 **되풀이 일정** 섹션을 선택한 다음 **반복 작업으로 만들기** 선택 사항입니다.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 에서 **빈도** 드롭다운 목록에서 작업을 수행할 시간 단위 수와 시간 단위 유형을 선택합니다. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>자동연장 유형</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>일</strong> </td> 
      <td> <p>작업은 선택한 간격에 따라 매일, 2일, 3일 등을 반복합니다. 6일마다 최대 반복 작업을 구성할 수 있습니다. 기본 설정은 1일입니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작업일</strong> </td> 
      <td> <p> 작업은 선택한 간격에 따라 매일, 2일에 한 번씩, 3일에 한 번씩, 매주 6번째 작업일까지 반복되도록 작업을 구성할 수 있습니다.</p> <p>이 옵션은 시스템 관리자가 정의한 기본 스케줄을 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong></strong>주 </td> 
      <td> <p> 이 작업은 선택한 간격에 따라 매주, 2주, 3주 등 여러 번 반복됩니다.</p> <p>에서 <strong>반복</strong> 필드에서 각 작업을 수행할 요일을 선택합니다. 여러 일을 선택할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>월</strong> </td> 
      <td> <p>이 작업은 사용자가 선택한 cadence에 따라 매월, 2개월, 3개월 등을 반복합니다. 1개월에서 12개월 중에서 선택할 수 있습니다. </p> <p>에서 <strong>반복</strong> 필드에서 작업을 수행하려는 경우 다음 옵션 중에서 선택합니다.</p> 
       <ul> 
        <li> <p><strong>매월 &lt;month date=""&gt;</strong> </p> <p>1일에서 30일까지 일수를 선택하거나 다음을 선택할 수 있습니다 <strong>마지막</strong>. 예를 들어 "매월 30일에"를 선택할 수 있습니다. </p> </li> 
        <li> <p><strong>매월 &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>첫 번째 드롭다운 메뉴에서 해당 월의 주 수에 대해 1과 4 사이의 숫자를 선택하거나 "last"를 선택할 수 있습니다. </p> <p>두 번째 드롭다운 메뉴에서 요일을 선택할 수 있습니다. </p> <p>예를 들어 "매월 2일 화요일"을 선택할 수 있습니다. </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >프로젝트 예약과 연관된 예약 예외가 있는 경우 예외 중에 반복 작업을 시작할 수 없습니다. 예약 예외 중에 발생하는 반복 작업은 예외를 따르는 첫 번째 업무일에 시작하도록 예약됩니다. 예약 예외에 대한 자세한 내용은 문서를 참조하십시오 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. 에서 **시작** 필드에서 반복 작업을 시작할 날짜 및 시간을 선택합니다.
1. 에서 **종료** 필드에서 반복 작업을 완료하려는 날짜 및 시간을 선택합니다

   또는

   선택 **after `<number>` 발생 횟수** 반복 작업이 몇 번 발생해야 하는지를 나타냅니다. Workfront은 이 필드에 지정하는 수와 동일한 수의 작업에 대한 재귀를 만듭니다.

1. 클릭 **작업 만들기.**

   작업 목록이 표시됩니다. 되풀이 작업은 상위 작업으로 만들어지며 모든 반복은 해당 하위 작업입니다. Workfront에서 상위 항목에 대해 입력한 이름 뒤에 숫자가 있는 하위 작업의 이름을 자동으로 생성했습니다. 상위 반복 작업에서 자동으로 채워지는 필드에 대한 자세한 내용은 [반복 작업 개요](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (선택 사항) 프로젝트에서 다른 작업에서처럼 각 반복 작업을 수정합니다.

   예를 들어, 지정, 선행 작업, 지속 기간을 추가하고 사용자 정의 필드를 포함한 작업에 대한 기타 정보를 수정할 수 있습니다.

   >[!IMPORTANT]
   >
   >1차 하위 구성요소를 개별적으로 수정한 후 상위 반복을 수정하면 1차 하위 구성요소 간 또는 1차 하위 구성요소와 상위 구성요소 간의 정보가 달라질 수 있습니다. 자세한 내용은 [반복 작업 개요](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
