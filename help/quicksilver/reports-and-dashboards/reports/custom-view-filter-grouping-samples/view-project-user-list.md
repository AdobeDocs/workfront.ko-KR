---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업 역할이 있는 프로젝트 사용자 목록'
description: 프로젝트 목록 또는 보고서에서 이 보기를 적용하여 프로젝트와 연관된 사용자 목록과 프로젝트에서 수행 중인 작업 역할 목록을 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 보기: 작업 역할이 있는 프로젝트 사용자 목록

<!--Audited: 11/2024-->

프로젝트 목록 또는 보고서에서 이 보기를 적용하여 프로젝트와 연관된 사용자 목록과 프로젝트에서 수행 중인 작업 역할 목록을 표시할 수 있습니다.

이 보고서의 정보는 프로젝트의 사람 영역에서도 찾을 수 있습니다.

>[!TIP]
>
>사용자에 대해 작업 역할이 나열되지 않지만 사용자 프로필의 작업 역할과 연결되어 있다는 것을 알고 있는 경우, 작업 및 문제에 할당되었지만 작업 또는 문제의 작업 역할과 연결되어 있지 않거나 보고서에 나열된 사용자가 작업 및 문제의 할당자가 아니지만 프로젝트의 다른 역할(예: 소유자 또는 스폰서)을 이행한다는 의미일 수 있습니다.

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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


## 작업 역할이 있는 프로젝트 사용자 목록 보기

1. 프로젝트 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.
1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
