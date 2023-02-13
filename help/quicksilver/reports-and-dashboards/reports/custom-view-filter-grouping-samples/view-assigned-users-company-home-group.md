---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "보기: 지정된 사용자의 회사 및 홈 그룹"
description: 이 작업 보기는 작업의 주 소유자의 회사 및 홈 그룹을 표시합니다. 이러한 값은 표준 인터페이스에서 사용할 수 없지만 텍스트 모드를 통해 액세스할 수 있는 값입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 보기: 지정된 사용자 회사 및 홈 그룹

이 작업 보기는 작업의 주 소유자의 회사 및 홈 그룹을 표시합니다. 이러한 값은 표준 인터페이스에서 사용할 수 없지만 텍스트 모드를 통해 액세스할 수 있는 값입니다.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 지정된 사용자의 회사 및 홈 그룹 보기

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valufield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo).string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=회사에 지정됨<br> column.2.displayname=회사에 할당됨<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:이름<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:이름<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=홈 그룹에 할당됨<br> column.3.displayname=홈 그룹에 할당됨<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:이름<br> column.3.shortview=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:이름<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. 클릭 **변경 내용 저장**.
