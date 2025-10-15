---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 상위 작업을 최대 4개 수준 아래에 표시'
description: 이 작업 보기는 첫 번째 열에 작업 이름을 표시하고(있는 경우) 동일한 목록의 별도 열에 최대 4개의 상위 작업을 표시합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 보기: 상위 작업을 최대 4개 수준 아래에 표시

<!--Audited: 11/2024-->

이 작업 보기는 첫 번째 열에 작업 이름을 표시하고(있는 경우) 동일한 목록의 별도 열에 최대 4개의 상위 작업을 표시합니다.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>보기를 수정하기 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.


+++

## 상위 작업을 최대 4단계까지 표시

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.
1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.


   ```
   column.0.descriptionkey=name
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
   column.0.shortview=false
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=parent
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=parent:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=parent:objCode
   column.1.link.valueformat=val
   column.1.linkedname=parent
   column.1.listsort=nested(parent).string(name)
   column.1.namekey=parent
   column.1.querysort=parent:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=parent:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Parent
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=parent:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=parent:parent:objCode
   column.2.link.valueformat=val
   column.2.linkedname=parent
   column.2.listsort=nested(parent:parent).string(name)
   column.2.name=Parent Parent
   column.2.querysort=parent:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=parent:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Parent Parent Parent
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=parent:parent:parent:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=parent:parent:parent:objCode
   column.3.link.valueformat=val
   column.3.linkedname=parent
   column.3.listsort=nested(parent:parent:parent).string(name)
   column.3.name=Parent Parent Parent
   column.3.querysort=parent:parent:parent:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=parent:parent:parent:name
   column.3.valueformat=HTML
   column.3.width=150
   column.4.description=Parent Parent Parent Parent
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=parent:parent:parent:parent:ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.valuefield=parent:parent:parent:parent:objCode
   column.4.link.valueformat=val
   column.4.linkedname=parent
   column.4.listsort=nested(parent:parent:parent:parent).string(name)
   column.4.name=Parent Parent Parent Parent
   column.4.querysort=parent:parent:parent:parent:name
   column.4.shortview=false
   column.4.stretch=100
   column.4.valuefield=parent:parent:parent:parent:name
   column.4.valueformat=HTML
   column.4.width=150
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.

   첫 번째 열에는 작업의 이름이 표시되며 작업에 상위 항목이 있는 경우 나머지 열에는 최대 4개의 상위 항목이 표시됩니다.
