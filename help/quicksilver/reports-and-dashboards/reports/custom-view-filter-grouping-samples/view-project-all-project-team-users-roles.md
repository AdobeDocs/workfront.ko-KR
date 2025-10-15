---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 모든 프로젝트 팀 사용자 및 역할이 있는 프로젝트'
description: 이 프로젝트 보기에는 프로젝트 팀에 할당된 사용자 및 작업 역할 목록이 표시됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 보기: 모든 프로젝트 팀 사용자 및 역할이 있는 프로젝트

<!--Audited: 11/2024-->

이 프로젝트 보기에는 프로젝트 팀에 할당된 사용자 및 작업 역할 목록이 표시됩니다.

>[!NOTE]
>
>작업 역할이 사용자와 동일한 행에 나열되는 경우, 이는 사용자가 프로젝트에서 해당 역할을 채우거나 사용자에게 프로필의 해당 역할이 할당되었음을 의미하지 않습니다.

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

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

## 모든 프로젝트 팀 사용자 및 역할이 있는 프로젝트 보기

1. 프로젝트 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.




   <pre>/userView.cmd column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objA code<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.link.link.linkproperty.0.valuefield=userID 사용자).lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=iterate<br>column.1.valuefield=user:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=팀 역할<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID <br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10<br>column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.width=150.stretch=0<br><br><br><br><br></pre>

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
