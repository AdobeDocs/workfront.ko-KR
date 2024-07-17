---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업 보기의 동일한 열에 있는 계획된 시간에 대한 실제 시간'
description: 이 작업 보기에서는 각 작업에 대해 계획된 시간 동안 작업에 기록된 실제 시간이 표시됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# 보기: 작업 보기의 동일한 열에 있는 계획된 시간에 대한 실제 시간

이 작업 보기에는 작업에 기록된 실제 시간이 각 작업에 대해 계획된 시간 동안 표시됩니다.

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 플랜*</td> 
   <td> <p>어떤</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 라이선스*</td> 
   <td> <p>보기 수정 요청 </p>
   <p>보고서를 수정하기 위한 플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 권한 편집 - 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정할 수 있는 방법에 대한 자세한 내용은 사용자 지정 액세스 수준</a> 만들기 또는 수정을 참조하십시오<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">개체 사용 권한</td> 
   <td> <p>보고서에 대한 사용 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 객체</a>에 대한 액세스 요청을 참조하십시오 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;사용 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 보기에서 계획된 시간에 대한 실제 시간 보기

이 보기를 적용하려면 다음을 수행합니다.

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭한 다음 텍스트 모드로&#x200B;**전환을 클릭합니다**.
1. 텍스트 모드 영역 위에 마우스를 놓고 [텍스트를&#x200B;**편집하려면 클릭]을 클릭합니다**.
1. 텍스트 모드&#x200B;**상자에서 찾은**&#x200B;텍스트를 제거 후 다음 코드로 바꿉니다.
   <pre>column.0.descriptionkey=이름<br>column.0.링크.linkproperty.0.name=ID<br>column.0.링크.linkproperty.0.valuefield=ID<br>column.0.링크.linkproperty.0.valueformat=int<br>column.0.링크.lookup=링크.view<br>column.0.링크.valuefield=objCode<br>column.0.링크.valueformat=val<br>column.0.linkedName=직접<br>column.0.listSort=string(name)column.0.nameKey<br>=name.abbr<br>column.0.querySort=이름<br>column.0.shortView=false<br>column.0.stretch=100<br>column.0.valuefield=이름<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=할당<br>column.1.displayname=<br>column.1.linkedName=직접<br>column.1.nameKey=할당<br>column.1.valueField=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=실제/계획된 시간<br>column.2.linkedname=직접<br>열.2.namekey=actualWorkRequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=복합<br>column.2.viewalias=actualWorkRequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=복합<br>column.3.displayname=시간 차이<br>column.3.linkedName=직접<br>column.3.textMode=true<br>column.3.valueExpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. **보기 저장**&#x200B;을 클릭합니다.
