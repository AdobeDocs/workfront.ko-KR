---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업 보기에 프로그램 및 Portfolio 정보 표시'
description: 이 작업 보기는 작업의 프로젝트와 연관된 프로그램 및 Portfolio을 표시합니다. 이 정보는 작업 보기를 작성할 때 Report Builder에서 사용할 수 없습니다. 이 정보는 텍스트 모드에서만 사용할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 보기: 작업 보기에 프로그램 및 Portfolio 정보 표시

이 작업 보기는 작업의 프로젝트와 연관된 프로그램 및 Portfolio을 표시합니다. 이 정보는 작업 보기를 작성할 때 Report Builder에서 사용할 수 없습니다. 이 정보는 텍스트 모드에서만 사용할 수 있습니다.

또한 이 보기는 작업 목록에서 프로젝트, 프로그램 및 Portfolio에 대한 링크도 제공합니다.

![](assets/view--program-and-portfolio-350x116.png)

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

## 작업 보기에 프로그램 및 Portfolio 정보 표시

작업 목록에 이 뷰를 적용하려면 다음을 수행합니다.

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valufield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=project:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.value=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=program<br>column.2.displayname=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.value=project:program:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=project:program:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program.string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:이름<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=project:program:이름<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=portfolio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.value=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.value=project:portfolio:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio.string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:이름<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=project:portfolio:이름<br>column.3.valueformat=HTML<br>column.3.width=150 </pre>

1. 클릭 **보기 저장**.
