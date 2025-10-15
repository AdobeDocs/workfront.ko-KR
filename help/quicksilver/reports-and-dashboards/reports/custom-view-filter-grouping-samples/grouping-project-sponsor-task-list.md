---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 작업 목록에 대한 프로젝트 스폰서'
description: 이 작업 그룹화를 사용하면 프로젝트 스폰서별로 작업을 그룹화할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 1%

---

# 그룹화: 작업 목록에 대한 프로젝트 스폰서

<!--Audited: 11/2024-->

이 작업 그룹화를 사용하면 프로젝트 스폰서별로 작업을 그룹화할 수 있습니다.

![프로젝트 스폰서별 그룹](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## 작업 목록에 대해 프로젝트 스폰서별로 그룹화


이 그룹화를 적용하려면:

1. 작업 목록으로 이동합니다.
1. **그룹화** 드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 표시되는 영역에서 텍스트를 제거하고 다음 코드로 대체합니다.

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. **완료**&#x200B;를 클릭합니다.
1. 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.

