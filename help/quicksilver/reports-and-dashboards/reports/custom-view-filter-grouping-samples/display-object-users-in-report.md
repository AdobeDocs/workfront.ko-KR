---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보고서 또는 목록: 객체와 연관된 사용자를 표시합니다.'
description: 보고서나 목록의 오브젝트와 연관된 사용자, 작업 역할 및 팀을 표시할 수 있으며, 필터에서 참조할 수 있습니다. 오브젝트와 연계된 사용자, 작업 역할 또는 팀별로 그룹화할 수 없습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# 보고서 또는 목록: 객체와 연관된 사용자를 표시합니다.

보고서나 목록의 오브젝트와 연관된 사용자, 작업 역할 및 팀을 표시할 수 있으며, 필터에서 참조할 수 있습니다. 오브젝트와 연계된 사용자, 작업 역할 또는 팀별로 그룹화할 수 없습니다.

다음 오브젝트와 연관된 사용자, 작업 역할 또는 팀별로 표시하거나 필터링할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">오브젝트</td> 
   <td>연결된 사용자 또는 작업 역할</td> 
  </tr> 
  <tr> 
   <td role="rowheader">프로젝트</td> 
   <td> <p>프로젝트 보고서에 프로젝트에서 이행하는 모든 사용자와 작업 역할을 표시할 수 있습니다. 프로젝트 보고서에서 사용자 또는 사용자와 연관된 작업 역할별로 필터링할 수 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업</td> 
   <td>작업 보고서에서 작업에 할당된 모든 사용자, 작업 역할 및 팀별로 표시하고 필터링할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문제</td> 
   <td>문제 보고서에서 문제에 할당된 모든 사용자, 작업 역할 및 팀별로 표시하고 필터링할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">포트폴리오</td> 
   <td>프로젝트에서 수행하는 모든 사용자 및 작업 역할을 프로젝트 보고서에 표시하고 Portfolio별로 보고서를 그룹화할 수 있습니다. 프로젝트 보고서에서 사용자 또는 사용자와 연관된 작업 역할별로 필터링할 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">프로그램</td> 
   <td>프로젝트에서 수행하는 모든 사용자와 작업 역할을 프로젝트 보고서에 표시하고 프로그램별로 보고서를 그룹화할 수 있습니다. 프로젝트 보고서에서 사용자 또는 사용자와 연관된 작업 역할별로 필터링할 수 없습니다.</td> 
  </tr> 
 </tbody> 
</table>

## 프로젝트와 연계된 모든 사용자 및 작업 역할 표시

프로젝트 목록 또는 보고서의 보기에서 프로젝트와 연관된 모든 사용자를 표시할 수 있습니다. 여기에는 프로젝트의 사람 섹션에 나열된 모든 사용자가 포함됩니다. 프로젝트 보고서에서 프로젝트의 작업 또는 문제에 할당되었을 때 연결되는 역할을 볼 수도 있습니다.

![사용자 및 역할 정보가 있는 프로젝트](assets/project-with-user-and-role-information-report-350x100.png)

프로젝트에 대한 모든 사용자와 사용자의 역할을 표시하는 프로젝트 보고서를 작성하는 방법에 대한 자세한 내용은 [보기: 작업 역할이 있는 프로젝트 사용자 목록](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)을 참조하십시오.

프로젝트 필터에서 프로젝트와 연결된 사용자 또는 작업 역할을 필터링할 수 없습니다.

## 작업에 할당된 모든 사용자, 작업 역할 또는 팀 표시

할당 필드를 보기에 추가하여 작업에 할당된 모든 사용자, 역할 또는 팀을 작업 목록 또는 보고서 보기에 표시할 수 있습니다.

![할당 필드](assets/assignments-field-task-view-350x124.png)

작업 필터의 다음 필드를 참조하여 작업에 할당된 사용자, 작업 역할 또는 팀별로 필터링할 수 있습니다.

* 할당 사용자
* 할당 역할
* 팀

![작업 필터의 할당 사용자 및 역할](assets/assignment-users-roles-task-filter-350x334.png)

## 문제에 할당된 모든 사용자, 작업 역할 또는 팀 표시

할당 필드를 보기에 추가하여 문제에 할당된 모든 사용자, 역할 또는 팀을 문제 목록 또는 보고서 보기에 표시할 수 있습니다.

문제 필터의 다음 필드를 참조하여 문제에 할당된 사용자, 작업 역할 또는 팀별로 필터링할 수 있습니다.

* 할당 사용자
* 할당 역할
* 팀

## 포트폴리오와 연결된 모든 사용자 및 작업 역할 표시

포트폴리오와 연결된 모든 사용자 및 역할을 프로젝트 보고서에 표시한 다음 Portfolio으로 그룹화하여 표시할 수 있습니다.

프로젝트에 대한 모든 사용자와 사용자의 역할을 표시하는 프로젝트 보고서를 작성하는 방법에 대한 자세한 내용은 [보기: 작업 역할이 있는 프로젝트 사용자 목록](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)을 참조하십시오.

포트폴리오 또는 프로젝트 필터에서 프로젝트와 연결된 사용자 또는 작업 역할을 필터링할 수 없습니다.

## 프로그램과 연결된 모든 사용자 및 작업 역할 표시

프로젝트 보고서에 사용자와 역할을 표시한 다음 프로그램별로 보고서를 그룹화하여 프로그램과 연관된 모든 사용자와 역할을 표시할 수 있습니다.

프로젝트에 대한 모든 사용자와 사용자의 역할을 표시하는 프로젝트 보고서를 작성하는 방법에 대한 자세한 내용은 [보기: 작업 역할이 있는 프로젝트 사용자 목록](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)을 참조하십시오.

프로그램 또는 프로젝트 필터에서 프로젝트와 연결된 사용자 또는 작업 역할을 필터링할 수 없습니다.
