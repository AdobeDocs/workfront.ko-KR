---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 작업 제한 개요
description: 작업 제한 사항은 프로젝트에서 작업이 시작 및 종료되는 시기를 결정합니다.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 6%

---

# 작업 제한 개요

작업 제한 사항은 프로젝트에서 작업이 시작 및 종료되는 시기를 결정합니다.

## 작업 제한 개요

프로젝트 계획을 세울 때 프로젝트에 대한 작업의 시퀀스 및 시간대에 대해 결정을 내립니다. 작업은 작업 순서와 관계없이 작동할 수 있지만 프로젝트 타임라인에 영향을 줄 수 있습니다. 작업 제한 사항을 사용하면 프로젝트 관리자가 프로젝트에서 특정 작업을 시작하거나 완료할 수 있는 시기를 계획할 수 있습니다.

사용하는 제한 사항에 따라 작업에 대해 계획된 시작 일자, 계획된 완료 일자 또는 두 가지 모두를 지정해야 할 수 있습니다.

정의된 날짜가 필요한 제한 유형은 전임 작업 관계에 영향을 줍니다.

>[!TIP]
>
>작업 간 전임 작업 관계를 사용하는 경우 특정 날짜가 필요하지 않은 제한 유형을 사용하는 것이 좋습니다.

다음 표에는 각 제약 조건과 그 약어가 나와 있습니다. 약어는 작업 목록 및 킥스타트 가져오기 파일을 만들 때 사용됩니다. 해당 제한 유형에 대한 자세한 내용을 보려면 각 작업 제한 사항의 연결된 제목을 클릭하십시오.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>제한 이름</strong> </p> </th> 
   <th> <p><strong>약어</strong> </p> </th> 
   <th> <p><strong>설명</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">작업 제한 개요: 가능한 한 빨리</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>작업의 시작 시간을 가능한 프로젝트 시작 시간과 가깝게 배치합니다.</p> 
   <p>프로젝트가 시작 일자부터 일정 모드를 사용하고 새 작업에 대한 시스템 기본 시작 일자가 프로젝트 계획 일자 기준으로 설정된 경우 기본 제약 조건입니다. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">작업 제한 개요: 가능한 한 늦게 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>작업의 완료 시간을 가능한 한 프로젝트 끝에 가깝게 배치합니다.</p> 
   <p>이는 프로젝트 일정 모드가 완료 일자부터 이고 작업 시작 일자에 대한 시스템 또는 그룹 기본값이 프로젝트 계획 일자를 기준으로 할 때의 기본 제한입니다. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">작업 제한 개요: 사용 가능한 가장 이른 시간</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>전임 작업 관계를 고려한 후 가능한 가장 빠른 시간에 작업을 시작하도록 예약합니다.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">작업 제한 개요: 사용 가능한 최신 시간</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>프로젝트의 전임 작업-후임 작업 관계를 고려한 후 가능한 가장 늦은 시간에 작업을 시작하도록 예약합니다.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">작업 제한 개요: 다음 이후에 시작:</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>지정한 날짜 이후에 작업을 시작하도록 예약합니다.</p> 
   <p>프로젝트 일정 모드가 시작 일자와 시스템 또는 그룹의 새 작업에 대한 기본 시작 일자가 오늘로 설정된 경우 이 제한이 기본 제한입니다.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">작업 제한 개요: 다음 이후에 시작</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>지정한 날짜 이전에 작업을 시작하도록 예약합니다.</p> 
   <p>프로젝트 일정 모드가 완료 일자부터 이며 작업의 시작 일자에 대한 시스템 또는 그룹 기본값이 오늘인 경우 STis는 기본 제한입니다. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">작업 제한 개요: 다음 이후에 완료:</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>지정한 날짜 이후에 작업을 완료하도록 예약합니다.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">작업 제한 개요: 다음 이후에 완료</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>지정한 날짜 이전에 작업이 완료되도록 예약합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">작업 제한 개요: 다음 일자에 시작</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>특정 날짜에 정확히 시작되도록 작업을 예약합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">작업 제한 개요: 다음 일자에 완료되어야 함</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>특정 날짜에 작업이 종료되도록 예약합니다.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">작업 제한 개요: 고정 날짜</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>특정 날짜에 작업이 시작되고 끝나도록 예약합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 제한 개요

새 작업을 만들 때 Workfront에서 작업 제한 사항을 자동으로 선택합니다.

Workfront은 두 개의 변수를 사용하여 새 작업에 대해 기본적으로 선택되는 작업 제한 사항을 결정합니다.

* 다음 **프로젝트 일정 출처:** 프로젝트의 필드입니다.

  프로젝트 일정 시작 필드에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

* 다음 **시작일** 에서 Workfront 또는 그룹 관리자가 구성한 환경 설정 **작업 및 문제** 영역 **설정**.

  작업 및 문제 환경 설정에 대한 자세한 내용은 의 &quot;새 작업 기본값&quot; 섹션을 참조하십시오. [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

다음 표에서는 프로젝트 및 새 작업에 대해 서로 다른 변수를 선택할 때의 기본 작업 제한 사항을 보여 줍니다.

| 프로젝트 일정 출처: | 작업 시작 일자 | 작업 제한 조건 기본값 |
|---|---|---|
| 시작 일자 | 프로젝트 계획된 일자 기준 | 빠른 시일 내에 |
| 시작 일자 | 오늘 | 다음 이후에 시작: |
| 완료 일자 | 프로젝트 계획된 일자 기준 | 가능한 한 늦게 |
| 완료 일자 | 오늘 | 다음 이전에 시작 |
