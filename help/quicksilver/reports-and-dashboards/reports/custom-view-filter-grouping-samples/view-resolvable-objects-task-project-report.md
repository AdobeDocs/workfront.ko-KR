---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업 또는 프로젝트 보고서의 해결 가능한 객체'
description: 프로젝트, 작업 보기 또는 보고서에 모든 해결 가능한 객체 목록을 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 보기: 작업 또는 프로젝트 보고서의 해결 가능한 객체

<!--Audited: 11/2024-->

프로젝트, 작업 보기 또는 보고서에 모든 해결 가능한 객체 목록을 표시할 수 있습니다.

해결 가능한 개체에 대한 자세한 내용은 [해결 및 해결 가능한 개체 개요](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md) 문서를 참조하십시오.

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

이 보기를 적용하는 것은 작업 및 프로젝트에 대해 동일합니다.

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

## 작업 또는 프로젝트 보고서에서 해결 가능한 객체 보기

1. 문제에서 전환된 작업 또는 프로젝트 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭합니다.

1. **열 미리 보기** 영역에서 **열 추가**&#x200B;를 클릭합니다.

1. 새 열의 헤더를 클릭한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.\
   모든 해결 가능한 객체 목록이 새 열에 표시됩니다. 목록에 있는 개체 이름은 개체에 직접 연결할 수 없습니다.
