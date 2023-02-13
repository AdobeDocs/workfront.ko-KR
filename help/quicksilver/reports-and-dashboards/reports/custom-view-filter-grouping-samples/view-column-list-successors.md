---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 열에 작업 승계자 목록 추가'
description: 작업 보기에 열을 추가하여 작업의 후속 항목 목록을 표시할 수 있습니다. 작업 승계자 열에는 후임자 수와 이름이 포함됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 보기: 열에 작업 승계자 목록 추가

작업 보기에 열을 추가하여 작업의 후속 항목 목록을 표시할 수 있습니다. 다음 **작업 승계자** 열에는 후속 멤버 수와 이름이 포함됩니다.

![task_view_with_a_list_of_후임자_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## 열에 작업 승계자 목록 추가

이 열을 작업 보기에 추가하려면 다음을 수행합니다.

1. 기존 작업 보기로 이동합니다.
1. 보기 드롭다운 메뉴를 확장하고 다음을 선택합니다 **보기 사용자 지정**.
1. 클릭 **열 추가**.
1. 클릭 **텍스트 모드로 전환**.
1. 마우스 **이 열에 표시** 영역을 클릭하고 **텍스트를 편집하려면 클릭하십시오.**.

1. 텍스트 모드 상자에서 모든 텍스트를 제거하고 다음 코드로 바꿉니다.

   <pre>displayname=작업 승계자<br>list구분 기호=<br><br>listmethod=nested(beacons).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({sucutor}).{taskNumber},' - ',{sucmandator}.{name})<br>valueformat=HTML</pre>

1. 클릭 **보기 저장**.
