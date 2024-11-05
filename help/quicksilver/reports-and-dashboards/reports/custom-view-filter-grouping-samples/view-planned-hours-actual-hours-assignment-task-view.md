---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업 보기에서 계획된 시간과 할당당 실제 시간 비교'
description: 이 작업 보기에는 작업의 총 계획된 시간, 각 할당자에게 할당된 계획된 시간 수(작업이 여러 사용자에게 할당된 경우), 작업의 총 실제 시간 및 각 할당자가 기록한 실제 시간 수가 표시됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 보기: 작업 보기에서 계획된 시간과 할당당 실제 시간 비교

<!--Audited: 11/2024-->

이 작업 보기에는 작업의 총 계획된 시간, 각 할당자에게 할당된 계획된 시간 수(작업이 여러 사용자에게 할당된 경우), 작업의 총 실제 시간 및 각 할당자가 기록한 실제 시간 수가 표시됩니다.

![multi_assignment_budget_vs_actual_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p> 현재: 
   <ul>
   <li>보기 수정 요청</li> 
   <li>보고서 수정 계획</li>
   </ul>
     </p>
     <p> 신규: 
   <ul>
   <li>보기를 수정하는 기여자</li> 
   <li>보고서를 수정하는 표준</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 보기에서 계획된 시간과 할당당 실제 시간 보기

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭하고 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   column.0.descriptionkey=name
   column.0.isInlineEditable=false
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=workrequired
   column.1.isInlineEditable=false
   column.1.linkedname=direct
   column.1.listsort=doubleAsDouble(workRequired)
   column.1.namekey=workrequired.abbr
   column.1.querysort=workRequired
   column.1.section=0
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=workFieldLong
   column.1.valueformat=compound
   column.1.viewalias=workrequired
   column.1.width=100
   column.2.listdelimiter=
   column.2.listmethod=nested(assignments).lists
   column.2.name=Wrk Assignment(s)
   column.2.stretch=0
   column.2.type=iterate
   column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})
   column.2.valueformat=HTML
   column.2.width=300
   column.3.descriptionkey=actualworkrequired
   column.3.isInlineEditable=false
   column.3.linkedname=direct
   column.3.listsort=intAsInt(actualWorkRequired)
   column.3.namekey=actualworkrequired.abbr
   column.3.querysort=actualWork
   column.3.section=0
   column.3.shortview=false
   column.3.stretch=100
   column.3.valuefield=actualWorkFieldLong
   column.3.valueformat=compound
   column.3.viewalias=actualworkrequired
   column.3.width=100
   column.4.listdelimiter=
   column.4.listmethod=nested(hours).lists
   column.4.name=Actual Hours
   column.4.stretch=0
   column.4.type=iterate
   column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})
   column.4.valueformat=HTML
   column.4.width=300
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
