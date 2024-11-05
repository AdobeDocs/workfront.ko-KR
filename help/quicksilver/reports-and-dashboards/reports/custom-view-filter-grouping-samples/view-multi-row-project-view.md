---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 다중 행 프로젝트 보기'
description: 보고서의 여러 행 프로젝트 보기에 대해 알아봅니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 보기: 다중 행 프로젝트 보기

<!--Audited: 11/2024-->

이 프로젝트 보기에서 다음 작업을 수행할 수 있습니다.

* 여러 행 형식으로 프로젝트 정보를 표시합니다.\
  보기는 `sharecol=true` 태그를 사용하여 동일한 열 머리글 아래에 여러 필드를 결합합니다. 이 태그에 대한 자세한 내용은 [보기: 하나의 공유 열에 있는 여러 열의 정보 병합](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)을 참조하세요.

* 예를 들어 HTML 줄 바꿈 태그(`<br>`)를 포함하는 자리 표시자 열을 사용하여 프로젝트 이름 아래에 설명을 강제로 표시합니다.
* 프로젝트 이름 뒤에 프로젝트 소유자를 괄호로 묶어 표시합니다.
* 프로젝트 이름을 프로젝트에 대한 링크로 표시합니다.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## 다중 행 프로젝트 보기 작성

1. 프로젝트 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭합니다.
1. 한 열을 제외하고 뷰의 모든 열을 제거합니다.
1. 나머지 열을 선택하고 **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집**&#x200B;에서 텍스트를 제거한 다음 아래 텍스트 모드를 복사하여 열 내부에 붙여넣습니다.

   ```
   column.0.linkedname=direct
   column.0.link.valueformat=val
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.valuefield=objCode
   column.0.link.lookup=link.view
   column.0.sharecol=true
   column.0.descriptionkey=name
   column.0.width=150
   column.0.querysort=name
   column.0.valuefield=name
   column.0.name=Project Name / Manager / Description
   column.0.shortview=false
   column.0.stretch=100
   column.0.textmode=true
   column.0.listsort=string(name)
   column.0.valueformat=HTML
   column.1.valueexpression=CONCAT(" (",{owner}.{name},")")
   column.1.listsort=nested(owner).string(name)
   column.1.width=1
   column.1.linkedname=direct
   column.1.querysort=owner:name
   column.1.textmode=true
   column.1.shortview=false
   column.1.stretch=0
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.width=1
   column.2.value=
   column.2.shortview=false
   column.2.sharecol=true
   column.2.stretch=0
   column.2.textmode=true
   column.2.valueformat=HTML
   column.3.styledef.style=font-color:#ccc;
   column.3.descriptionkey=description
   column.3.linkedname=direct
   column.3.valuefield=description
   column.3.listsort=string(description)
   column.3.querysort=description
   column.3.namekey=description.abbr
   column.3.textmode=true
   column.3.sharecol=true
   column.3.stretch=0
   column.3.shortview=false
   column.3.valueformat=HTML
   column.3.width=1
   column.4.shortview=false
   column.4.value=
   column.4.sharecol=true
   column.4.width=1
   column.4.textmode=true
   column.4.valueformat=HTML\
   column.4.stretch=0
   column.5.name=Planned Dates / Duration
   column.5.width=150
   column.5.querysort=plannedStartDate
   column.5.sharecol=true
   column.5.stretch=0
   column.5.textmode=true
   column.5.shortview=false
   column.5.linkedname=direct
   column.5.listsort=atDateAsAtDate(plannedStartDate)
   column.5.valuefield=plannedStartDate
   column.5.valueformat=atDate
   column.6.sharecol=true
   column.6.stretch=0
   column.6.width=1
   column.6.textmode=true
   column.6.value=-
   column.6.valueformat=HTML
   column.6.shortview=false
   column.7.namekey=plannedcompletiondate.abbr
   column.7.width=1
   column.7.sharecol=true
   column.7.shortview=false
   column.7.stretch=0
   column.7.listsort=atDateAsAtDate(plannedCompletionDate)
   column.7.linkedname=direct
   column.7.descriptionkey=plannedcompletiondate
   column.7.textmode=true
   column.7.querysort=plannedCompletionDate
   column.7.valueformat=atDate
   column.7.valuefield=plannedCompletionDate
   column.8.value=
   column.8.width=1
   column.8.textmode=true
   column.8.sharecol=true
   column.8.valueformat=HTML
   column.8.stretch=0
   column.9.textmode=true
   column.9.listsort=intAsInt(durationMinutes)
   column.9.stretch=0
   column.9.valuefield=durationFieldLong
   column.9.descriptionkey=duration
   column.9.viewalias=duration
   column.9.querysort=durationMinutes
   column.9.sharecol=true
   column.9.width=100
   column.9.shortview=false
   column.9.namekey=duration.abbr
   column.9.linkedname=direct
   column.9.valueformat=compound
   column.10.textmode=true
   column.10.stretch=0
   ```


1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
