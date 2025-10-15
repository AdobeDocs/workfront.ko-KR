---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 표준 인터페이스에 포함되지 않은 객체를 표시합니다.'
description: 표준 모드 인터페이스에 포함되지 않은 객체를 뷰에 표시할 수 있습니다. 이 작업은 텍스트 모드를 통해 참조해야만 수행할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 보기: 표준 인터페이스에 포함되지 않은 객체를 표시합니다.

표준 모드 인터페이스에 포함되지 않은 객체를 뷰에 표시할 수 있습니다. 이 작업은 텍스트 모드를 통해 참조해야만 수행할 수 있습니다.\
다음 방법 중 하나로 보기에 포함할 수 있는 필드를 결정할 수 있습니다.

* [API 탐색기](../../../wf-api/general/api-explorer.md)를 사용하여 텍스트 모드를 통해 참조할 수 있는 다른 개체를 검색합니다.\
  API 탐색기에 문서화된 모든 필드가 텍스트 모드에 유효한 필드는 아닙니다. 일부 필드는 API를 통해서만 보고할 수 있습니다.

* 열에서 개체의 ID 필드를 찾습니다. 필드 ID가 있는 대부분의 개체에는 표준 모드 인터페이스를 통해 액세스할 수 없는 해당 열 또는 필드 이름도 있습니다.

  텍스트 모드를 사용하여 `fieldnameID`을(를) `fieldname:name`(으)로 바꾸면 ID 대신 열 또는 필드 이름을 보기에 포함할 수 있습니다.

  예를 들어 표준 모드 인터페이스에서 **Portfolio 소유자 ID** 필드는 프로젝트 보기에서 사용할 수 있지만 **Portfolio 소유자 이름** 필드는 사용할 수 없습니다. 텍스트 모드를 사용하여 보기의 열에 **Portfolio 소유자 이름**&#x200B;을 표시할 수 있습니다.

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

## 예: 프로젝트 보기에 Portfolio 소유자 이름 열 추가

1. 프로젝트 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭합니다.

1. **열 추가**&#x200B;를 클릭한 다음 **이 열에 표시** 필드에 &quot;Portfolio 소유자 ID&quot;를 입력한 다음 목록에 표시될 때 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. `valuefield` 줄(`valuefield=portfolio:ownerID`)을 다음 줄로 바꿉니다.

   `valuefield=portfolio:owner:name`

   또는

   **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   이 특정 예에서 보고서는 `querysort` 줄에 표시된 대로 Portfolio 소유자 ID별로 보고서를 정렬합니다.

   >[!TIP]
   >
   >텍스트 모드를 사용하여 필드 `ID`을(를) 필드 `name`(으)로 바꾸려면 항상 `ID` 줄의 `:name`을(를) `valuefield`(으)로 바꾸십시오.

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
