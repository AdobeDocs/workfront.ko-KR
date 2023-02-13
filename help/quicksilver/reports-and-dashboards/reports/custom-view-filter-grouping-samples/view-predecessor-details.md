---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 이전 세부 사항'
description: 이 작업 보기는 컬렉션 보기를 사용하여 작업의 선행 작업에 대한 세부 정보를 표시합니다. 컬렉션 보기에서는 "일대다" 관계에 있는 객체에 대한 정보를 표시할 수 있습니다. 이 경우 각 작업(하나)에는 여러 선행 작업(많이)이 있을 수 있습니다. 이 보기에는 작업 이름과 선행 작업 이름, 선행 작업 프로젝트 이름, 선행 작업 계획 완료 날짜, 선행 작업 상태가 표시됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 보기: 이전 세부 사항

이 작업 보기는 컬렉션 보기를 사용하여 작업의 선행 작업에 대한 세부 정보를 표시합니다. 컬렉션 보기에서는 &quot;일대다&quot; 관계에 있는 객체에 대한 정보를 표시할 수 있습니다. 이 경우 각 작업(하나)에는 여러 선행 작업(많이)이 있을 수 있습니다. 이 보기에는 작업 이름과 선행 작업 이름, 선행 작업 프로젝트 이름, 선행 작업 계획 완료 날짜, 선행 작업 상태가 표시됩니다.

보고서의 컬렉션 참조에 대한 자세한 내용은 [보고서에서 컬렉션 참조](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![전임자_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## 이전 세부 정보 보기

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valufield=name<br>column.0.valueformat=HTML<br>column.1.displayname=선행 숫자 및 이름<br>column.1.list구분 기호=<br><br>column.1.listmethod=nested(previous).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({previous}).{taskNumber},' - ',{previous}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=선행 프로젝트 이름<br>column.2.list구분 기호=<br><br>column.2.listmethod=nested(previous).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={previous}.{프로젝트}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=선행 완료 날짜<br>column.3.list구분 기호=<br><br>column.3.listmethod=nested(previous).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={previous}.{planningCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=선행 작업 상태<br>column.4.list구분 기호=<br><br>column.4.listmethod=nested(previous).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={previous}.{status}<br>column.4.valueformat=HTML</pre>

1. 클릭 **보기 저장**.
