---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업 뷰의 할당당 계획 시간과 실제 시간 비교'
description: 이 작업 뷰에는 작업의 총 계획 시간, 각 할당자에게 할당된 계획 시간 수, 총 실제 시간 및 각 할당자가 로그한 실제 시간 수가 표시됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 보기: 작업 뷰의 발령당 계획 시간과 실제 시간 비교

이 작업 뷰에는 작업의 총 계획 시간, 각 할당자에게 할당된 계획 시간 수, 총 실제 시간 및 각 할당자가 로그한 실제 시간 수가 표시됩니다.

![multi_assignment_budget_vs_actual_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

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

## 작업 뷰에서 계획된 시간과 할당당 실제 시간 보기

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   ```
   column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=workrequired<br>column.1.isInlineEditable=false<br>column.1.linkedname=direct<br>column.1.listsort=doubleAsDouble(workRequired)<br>column.1.namekey=workrequired.abbr<br>column.1.querysort=workRequired<br>column.1.section=0<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=workFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=workrequired<br>column.1.width=100<br>column.2.listdelimiter=<br>column.2.listmethod=nested(assignments).lists<br>column.2.name=Wrk Assignment(s)<br>column.2.stretch=0<br>column.2.type=iterate<br>column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})<br>column.2.valueformat=HTML<br>column.2.width=300<br>column.3.descriptionkey=actualworkrequired<br>column.3.isInlineEditable=false<br>column.3.linkedname=direct<br>column.3.listsort=intAsInt(actualWorkRequired)<br>column.3.namekey=actualworkrequired.abbr<br>column.3.querysort=actualWork<br>column.3.section=0<br>column.3.shortview=false<br>column.3.stretch=100<br>column.3.valuefield=actualWorkFieldLong<br>column.3.valueformat=compound<br>column.3.viewalias=actualworkrequired<br>column.3.width=100<br>column.4.listdelimiter=<br>column.4.listmethod=nested(hours).lists<br>column.4.name=Actual Hours<br>column.4.stretch=0<br>column.4.type=iterate<br>column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})<br>column.4.valueformat=HTML<br>column.4.width=300
   ```

1. 클릭 **보기 저장**.
