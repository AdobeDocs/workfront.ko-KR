---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 불완전한 프로젝트 간 전임 작업 표시'
description: 이 작업 필터는 불완전한 프로젝트 간 전임 작업을 반환합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 필터: 불완전한 프로젝트 간 전임 작업 표시

<!--Audited: 10/2024-->

이 작업 필터는 불완전한 프로젝트 간 전임 작업을 반환합니다.

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

## 프로젝트 간 전임 작업 필터링

이 필터를 적용하려면:

1. 작업 목록 또는 작업 보고서로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. (조건부) 목록에서 필터에 액세스한 경우 **텍스트 모드**&#x200B;를 클릭하고, 보고서에서 필터에 액세스한 경우 **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 새 영역에 다음 코드를 붙여넣습니다.
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (조건부) 보고서에서 필터에 액세스한 경우 **필터 저장**&#x200B;을 클릭하고 작업 목록에서 필터에 액세스한 경우 **적용**&#x200B;을 클릭한 다음 **새 필터로 저장**&#x200B;을 클릭합니다.
