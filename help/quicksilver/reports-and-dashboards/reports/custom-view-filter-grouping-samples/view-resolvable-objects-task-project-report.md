---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업 또는 프로젝트 보고서의 해결 가능한 개체'
description: 프로젝트나 작업 보기 또는 보고서에 모든 해결 가능 객체 목록을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 보기: 작업 또는 프로젝트 보고서의 해결 가능한 개체

프로젝트나 작업 보기 또는 보고서에 모든 해결 가능 객체 목록을 표시할 수 있습니다.

해결 가능한 개체에 대한 자세한 내용은 문서를 참조하십시오 [해결 가능한 객체 해결 및 해결 방법 개요](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

이 보기를 적용하는 것은 작업 및 프로젝트에 대해 동일합니다.

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

## 작업 또는 프로젝트 보고서에서 해결 가능한 객체 보기

1. 문제로부터 변환된 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 에서&#x200B;**열 미리 보기** 영역을 클릭합니다. **열 추가**.

1. 새 열의 헤더를 클릭한 다음 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   <pre>displayname=Resolvable<br>list구분 기호=<br><br>listmethod=nested(resolvables).lists<br>textmode=true<br>type=iterate<br>value=name<br>valueformat=HTML<br></pre>

1. 클릭 **보기 저장**.\
   모든 해결 가능 객체 목록이 새 열에 표시됩니다. 목록에 있는 개체의 이름을 개체에 직접 연결할 수 없습니다.
