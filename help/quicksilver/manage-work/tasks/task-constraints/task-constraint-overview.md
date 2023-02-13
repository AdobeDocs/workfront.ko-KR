---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 작업 제한 개요
description: 작업 제약 조건은 프로젝트에서 작업을 시작 및 종료해야 하는 시기를 결정합니다.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# 작업 제한 개요

작업 제약 조건은 프로젝트에서 작업을 시작 및 종료해야 하는 시기를 결정합니다.

## 작업 제한 개요

프로젝트 계획을 작성할 때 프로젝트에서 작업의 순서 및 시간 프레임을 결정합니다. 작업은 모든 작업 시퀀스와 독립적으로 작동할 수 있지만 프로젝트 타임라인에 영향을 줄 수 있습니다. 작업 제약 조건을 사용하면 프로젝트 관리자가 프로젝트에서 특정 작업을 시작하거나 완료할 수 있는 시기를 계획할 수 있습니다.

사용하는 제약 조건에 따라 작업에 대해 계획 시작 일자, 계획 완료 일자 또는 둘 다 지정해야 할 수 있습니다.

정의된 날짜가 필요한 제약 조건 유형은 이전 관계의 영향을 받습니다.

>[!TIP]
>
>작업 간의 이전 관계를 사용하는 경우 특정 날짜가 필요하지 않은 제한 유형을 사용하는 것이 좋습니다.

다음 표에는 각 제약 조건과 약어가 표시됩니다. 약어는 작업 목록과 킥시작 가져오기 파일을 만들 때 사용됩니다. 해당 제한 유형에 대한 자세한 내용을 보려면 각 작업 제약 조건의 연결된 제목을 클릭합니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>제한 이름</strong> </p> </th> 
   <th> <p><strong>약어</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">작업 제한 개요: 가능한 한 빨리</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">작업 제한 개요: 가능한 늦게 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">작업 제한 개요: 가장 이른 가용 시간</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">작업 제한 개요: 최신 사용 가능 시간</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">작업 제한 개요: 보다 일찍 시작</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">작업 제한 개요: 늦어도 시작</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">작업 제한 개요: 보다 빨리 완료</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">작업 제한 개요: 늦어도 다음 날짜 전까지 완료</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">작업 제한 개요: 시작 시기</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">작업 제한 개요: 다음 작업을 완료해야 함</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">작업 제한 개요: 고정 날짜</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 구속 개요

새 작업을 만들면 Workfront에 의해 작업 제한이 자동으로 선택됩니다.

Workfront은 두 개의 변수를 사용하여 새 작업에 대해 기본적으로 선택된 작업 제한을 결정합니다.

* 다음 **프로젝트 일정 시작** 프로젝트의 필드입니다.

   프로젝트 스케줄 시작 필드에 대한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

* 다음 **시작 날짜** 기본 설정은 Workfront 또는 그룹 관리자가 **작업 및 문제** 영역 **설정**.

   작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

다음 표는 프로젝트와 새 작업에 대해 다른 변수를 선택할 때 기본 작업 제약 조건을 보여줍니다.

| 프로젝트 일정 시작 | 작업 시작 날짜 | 작업 제한 기본값 |
|---|---|---|
| 시작일 | 프로젝트 계획된 일자 기준 | 빠른 시일 내에 |
| 시작일 | 오늘 | 다음 이후에 시작: |
| 완료 일자 | 프로젝트 계획된 일자 기준 | 가능한 늦게 |
| 완료 일자 | 오늘 | 다음 이전에 시작 |
