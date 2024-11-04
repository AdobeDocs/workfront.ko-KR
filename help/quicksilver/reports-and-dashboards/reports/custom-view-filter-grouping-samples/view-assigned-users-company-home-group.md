---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "보기: 할당된 사용자의 회사 및 홈 그룹"
description: 이 작업 보기에는 작업의 기본 소유자의 회사 및 홈 그룹이 표시됩니다. 이러한 값은 표준 인터페이스에서 사용할 수 없지만 텍스트 모드를 통해 액세스할 수 있는 값입니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 보기: 할당된 사용자의 회사 및 홈 그룹

<!--Audited: 11/2024-->

이 작업 보기에는 작업의 기본 소유자의 회사 및 홈 그룹이 표시됩니다. 이러한 값은 표준 인터페이스에서 사용할 수 없지만 텍스트 모드를 통해 액세스할 수 있는 값입니다.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 할당된 사용자의 회사 및 홈 그룹 보기

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭한 다음 **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

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
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=assignedto
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=assignedTo:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=assignedTo:objCode
   column.1.link.valueformat=val
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Assigned To Company
   column.2.displayname=Assigned To Company
   column.2.linkedname=assignedTo:company
   column.2.listsort=nested(assignedTo:company).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:company:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=assignedTo:company:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Assigned To Home Group
   column.3.displayname=Assigned To Home Group
   column.3.linkedname=assignedTo:homeGroup
   column.3.listsort=nested(assignedTo:homeGroup).string(name)
   column.3.namekey=assignedto
   column.3.querysort=assignedTo:homeGroup:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=assignedTo:homeGroup:name
   column.3.valueformat=HTML
   column.3.width=150
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 보기 이름을 업데이트한 다음 **보기 저장**&#x200B;을 클릭합니다.
