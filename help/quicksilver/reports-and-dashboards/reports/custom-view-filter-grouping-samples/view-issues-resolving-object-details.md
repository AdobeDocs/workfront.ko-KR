---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 오브젝트 세부 정보 해결 문제'
description: 이 문제 보기에는 문제의 해결 중 오브젝트의 이름과 완료율이 표시되므로 문제 작성자는 해결 중 작업 또는 프로젝트에 액세스하지 않고도 insight을 문제의 진행 중으로 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 보기: 오브젝트 세부 정보 해결 문제

<!--Audited: 11/2024-->

이 문제 보기에는 문제의 해결 중 오브젝트의 이름과 완료율이 표시되므로 문제 작성자는 해결 중 작업 또는 프로젝트에 액세스하지 않고도 insight을 문제의 진행 중으로 사용할 수 있습니다.

이 보기는 `sharecol=true` 태그를 사용하여 동일한 열 머리글 아래에 여러 필드를 결합합니다. `sharecol` 태그에 대한 자세한 내용은 [보기: 하나의 공유 열에 있는 여러 열의 정보 병합](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)을 참조하십시오.

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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

## 오브젝트 세부 정보 해결 문제 보기

1. 문제 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭하고 **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   column.0.querysort=name
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=sourceobject
   column.1.linkedname=direct
   column.1.listsort=nested(referenceObject).HTML(name)
   column.1.namekey=sourceobject.abbr
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=referenceObject:name
   column.1.valueformat=HTML
   column.1.viewalias=source
   column.1.width=100
   column.2.descriptionkey=assignedto
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=assignedTo:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=assignedTo:objCode
   column.2.link.valueformat=val
   column.2.linkedname=assignedTo
   column.2.listsort=nested(assignedTo).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=assignedTo:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=entrydate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(entryDate)
   column.3.namekey=entrydate.abbr
   column.3.querysort=entryDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=entryDate
   column.3.valueformat=atDate
   column.3.width=150
   column.4.descriptionkey=description
   column.4.linkedname=direct
   column.4.listsort=string(description)
   column.4.namekey=description.abbr
   column.4.querysort=description
   column.4.shortview=false
   column.4.stretch=75
   column.4.valuefield=description
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=status
   column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.5.linkedname=direct
   column.5.listsort=string(status)
   column.5.namekey=status.abbr
   column.5.querysort=status
   column.5.shortview=false
   column.5.stretch=0
   column.5.type=enum
   column.5.valuefield=status
   column.5.valueformat=val
   column.5.width=150
   column.6.displayname=Resolving Object Name
   column.6.linkedname=resolveTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=resolveTask
   column.6.namekeyargkey.1=name
   column.6.querysort=resolveTask:name
   column.6.sharecol=true
   column.6.textmode=true
   column.6.valuefield=resolveTask:name
   column.6.valueformat=HTML
   column.7.displayname=
   column.7.linkedname=resolveOpTask
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=resolveOpTask
   column.7.namekeyargkey.1=name
   column.7.querysort=resolveOpTask:name
   column.7.sharecol=true
   column.7.textmode=true
   column.7.valuefield=resolveOpTask:name
   column.7.valueformat=HTML
   column.8.displayname=
   column.8.linkedname=resolveProject
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=resolveProject
   column.8.namekeyargkey.1=name
   column.8.querysort=resolveProject:name
   column.8.textmode=true
   column.8.valuefield=resolveProject:name
   column.8.valueformat=HTML
   column.9.displayname=Resolving Object Percent Complete
   column.9.textmode=true
   column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},''))
   column.9.valueformat=doubleAsPercentRounded
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 보기 이름을 업데이트한 다음 **보기 저장**&#x200B;을 클릭합니다.
