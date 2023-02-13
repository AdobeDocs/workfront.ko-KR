---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 다중 행 프로젝트 보기'
description: 이 프로젝트 보기에서 ME를 편집할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 보기: 다중 행 프로젝트 보기

이 프로젝트 보기에서 다음을 수행할 수 있습니다.

* 프로젝트 정보를 여러 행 형식으로 표시합니다.\
   이 보기는 를 사용합니다

   ```
   sharecol=true
   ```

   태그로 여러 필드를 동일한 열 헤더 아래에 결합합니다. 이 태그에 대한 자세한 내용은 [보기: 하나의 공유 열에 있는 여러 열의 정보 병합](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* HTML 줄 바꿈 태그를 포함하는 자리 표시자 열 사용(

   ```
   <br>
   ```

   )을 클릭하여 예를 들어 프로젝트 이름 아래에 설명을 강제로 표시합니다.
* 프로젝트 이름 뒤에 프로젝트 소유자를 괄호로 표시합니다.
* 프로젝트 이름으로 프로젝트 이름을 프로젝트 링크로 표시합니다.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## 여러 행 프로젝트 보기 작성

1. 새 프로젝트 보기를 만듭니다. 새 보기를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. 뷰를 작성할 때 뷰를 제외한 모든 열을 삭제합니다.
1. 나머지 열을 선택하고 을(를) 클릭합니다 **텍스트 모드로 전환**.
1. 열 내부에 텍스트 모드를 복사하여 붙여 넣습니다.
   <pre>column.0.linkedname=direct<br>column.0.link.valueformat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.valuefield=objCode<br>column.0.link.lookup=link.view<br>column.0.sharcol=true<br>column.0.descriptionkey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valufield=name<br>column.0.name=프로젝트 이름 / 관리자 / 설명<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueformat=HTML<br>column.1.valueexpression=CONCAT(",{owner}){name},")"<br>column.1.listsort=nested(owner.string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueformat=HTML<br>column.1.sharcol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.shortview=false<br>column.2.sharcol=true<br>column.2.stretch=0<br>column.2.textmode=true<br>column.2.valueformat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.description=description<br>column.3.linkedname=direct<br>column.3.valuefield=description<br>column.3.listsort=string(설명)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharcol=true<br>column.3.stretch=0<br>column.3.shortview=false<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.shortview=false<br>column.4.value=<br><br>column.4.sharcol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueformat=HTML\<br>column.4.stretch=0<br>column.5.name=계획된 날짜 / 기간<br>column.5.width=150<br>column.5.querysort=planningStartDate<br>column.5.sharcol=true<br>column.5.stretch=0<br>column.5.textmode=true<br>column.5.shortview=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(planningStartDate)<br>column.5.valuefield=planningStartDate<br>column.5.valueformat=atDate<br>column.6.sharcol=true<br>column.6.stretch=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueformat=HTML<br>column.6.shortview=false<br>column.7.namekey=plannedcompletiondate.abbr<br>column.7.width=1<br>column.7.sharcol=true<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.listsort=atDateAsAtDate(planningCompletionDate)<br>column.7.linkedname=direct<br>column.7.description 키=plannedcompletiondate<br>column.7.textmode=true<br>column.7.querysort=planningCompletionDate<br>column.7.valueformat=atDate<br>column.7.valuefield=planningCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharcol=true<br>column.8.valueformat=HTML<br>column.8.stretch=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.stretch=0<br>column.9.valuefield=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viviewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharcol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueformat=compound<br>column.10.textmode=true<br>column.10.stretch=0</pre>

1. 클릭 **보기 저장**.
