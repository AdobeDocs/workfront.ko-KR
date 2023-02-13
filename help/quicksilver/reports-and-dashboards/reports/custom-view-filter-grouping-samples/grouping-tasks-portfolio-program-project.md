---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 포트폴리오, 프로그램 및 프로젝트별 작업'
description: 이 작업 그룹을 사용하여 작업을 포트폴리오별로 그룹화한 다음, 프로그램별로 그룹화한 다음, 관련된 프로젝트를 기준으로 그룹화합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 그룹화: 포트폴리오, 프로그램 및 프로젝트별 작업

이 작업 그룹을 사용하여 작업을 포트폴리오별로 그룹화한 다음, 프로그램별로 그룹화한 다음, 관련된 프로젝트를 기준으로 그룹화합니다.

![](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## 포트폴리오, 프로그램 및 프로젝트별로 작업 그룹화

이 그룹을 적용하려면

1. 작업 목록으로 이동합니다.
1. 에서 **그룹화** 드롭다운 메뉴에서 **새 그룹화**.

1. 클릭 **텍스트 모드로 전환**.
1. 에서 텍스트 제거 **보고서 그룹화** 영역.
1. 텍스트를 다음 코드로 바꿉니다.

   <pre>group.0.linkedname=project<br>group.0.namekey=portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:이름<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valuefield=project:program:이름<br>group.1.valueformat=string<br>group.2.name=프로젝트<br>group.2.valuefield=project:name<br>group.2.valueformat=HTML<br>textmode=true<br></pre>

1. 클릭 **그룹화 저장**.
