---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열에 작업 후임 작업 목록 추가'
description: 작업 보기에 열을 추가하여 작업 후임 작업 목록을 표시할 수 있습니다. 작업 승계자 열에는 승계자 수와 이름이 포함됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%

---

# 보기: 열에 작업 후임 작업 목록 추가

<!--Audited: 11/2024-->

작업 보기에 열을 추가하여 작업 후임 작업 목록을 표시할 수 있습니다. **작업 후임 작업** 열에는 후임 작업의 수와 이름이 포함됩니다.

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <p>필터 수정을 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 열에 작업 후임 작업 목록 추가

이 열을 작업 보기에 추가하려면 다음 작업을 수행하십시오.

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴를 확장하고 **새 보기**&#x200B;를 클릭합니다.
1. **열 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 모든 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
