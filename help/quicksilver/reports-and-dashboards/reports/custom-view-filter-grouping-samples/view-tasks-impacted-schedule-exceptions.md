---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 예약 예외의 영향을 받는 작업'
description: 이 작업 보기는 주말, 개인 시간 해제 또는 기타 일정 예외로 인해 늦게 완료해야 하는 작업을 식별합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 보기: 예약 예외에 영향을 주는 작업

이 작업 보기는 주말, 개인 시간 해제 또는 기타 일정 예외로 인해 늦게 완료해야 하는 작업을 식별합니다.

이 보기에는 다음 내용이 표시됩니다.

* 작업 기간
* 작업의 계획 시작 및 계획 완료 일자
* 작업의 계획 시작 및 계획 완료 일자 사이의 일 수에 따른 작업 기간(달력 기간)
* 작업이 시작되는 프로젝트 예약의 일 수(달력 시작 날짜)
* 작업의 계획 시작 및 계획 완료 일자 사이의 평일 수에 따른 작업의 주 일 기간(주 일 기간)
* 주 요일 기간이 작업의 기간보다 크면 작업 기간에 예외 일이 있음을 나타내는 작업이 &quot;예외&quot;로 표시됩니다.\
   ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 예약 예외의 영향을 받는 작업 보기

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valufield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.description 키=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(planningStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=planningStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=planningStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.description 키=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(planningCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=planningCompletionDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=planningCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({계획된 완료 날짜},<br>{planningStartDate})+1<br>column.4.aggregator.valueFormat=intAsInt<br>column.4.description-key=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=달력 기간<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({planningCompletionDate},{planningStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({planningStartDate},{project}).<br>{planningStartDate})+0<br>column.5.aggregator.valueFormat=intAsInt<br>column.5.description-key=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=달력 시작 날짜<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF({planningStartDate},{project}).{planningStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({계획된 시작 날짜},<br>{planningCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({planningStartDate},{planningCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({계획됨StartDate},{계획됨CompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.aggregator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=예약<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({계획됨StartDate},{계획됨CompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. 클릭 **보기 저장**.
