---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업 및 프로젝트의 원래 문제 세부 정보'
description: 문제가 작업 또는 프로젝트로 변환되면 작업 또는 프로젝트와 문제 간에 해결되는 개체 관계가 설정됩니다. 이 보기에는 작업이나 프로젝트가 완료되면 자동으로 완료되는 문제에 대한 다음 필드가 표시됩니다. EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# 보기: 작업 및 프로젝트의 원래 문제 세부 정보

문제가 작업 또는 프로젝트로 변환되면 작업 또는 프로젝트와 문제 간에 해결되는 개체 관계가 설정됩니다. 이 보기에는 작업이나 프로젝트가 완료될 때 자동으로 완료되는 문제에 대한 다음 필드가 표시됩니다.

* 이름
* 시작 날짜
* 계획된 완료 일자
* 실제 완료 일자
* 요청 유형
* 작성자 이름
* 지정 대상 사용자

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

자세한 내용은 [보기: 작업 및 프로젝트 목록에 원래 문제 정보 표시](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## 작업 및 프로젝트에 대한 원래 문제 세부 정보 보기

1. 작업 목록 또는 프로젝트 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 제외한 모든 열을 제거합니다.
1. 나머지 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 클릭 **보기 저장**.
