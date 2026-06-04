---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업을 들여써서 작업에 상위-하위 관계 표시'
description: 작업 목록에 사용자 정의 보기를 추가하고 목록을 내보내기 전에 이 보기를 선택하여 내보낸 작업 목록에서 상위-하위 관계를 구분할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QSBA40vOIbB8cm0YydDuJN9NS2X6SoXNF-dCBUHFniM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 6%

---

# 보기: 작업을 들여써서 작업의 상위-하위 관계를 표시합니다.

<!--Audited: 11/2024-->

작업 목록에 사용자 정의 보기를 추가하고 목록을 내보내기 전에 이 보기를 선택하여 내보낸 작업 목록에서 상위-하위 관계를 구분할 수 있습니다.

![부모 자식 들여쓰기](assets/parent-child-indented-custom-view-350x94.png)

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
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

## 작업을 들여써서 작업에 상위-하위 관계 표시

1. 내보낼 작업 목록이 있는 프로젝트로 이동합니다.
1. **보기** 드롭다운 메뉴를 클릭하고 **새 보기**&#x200B;를 선택합니다.
1. **작업 이름** 열 머리글을 클릭합니다.
1. 오른쪽 상단에서 **텍스트 모드로 전환**&#x200B;을 선택합니다.
1. **텍스트 모드 편집**&#x200B;을 클릭하고 기존 텍스트를 모두 제거합니다.
1. 다음 텍스트를 붙여넣습니다.


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
