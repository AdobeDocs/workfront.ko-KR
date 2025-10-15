---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열의 콘텐츠 숨기기'
description: 보기의 열에서 정보를 숨길 수 있습니다. 열의 텍스트 모드를 수정하여 이 작업을 수행할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 보기: 열의 콘텐츠 숨기기

<!--Audited: 11/2024-->

보기의 열에서 정보를 숨길 수 있습니다. 열의 텍스트 모드를 수정하여 이 작업을 수행할 수 있습니다.

>[!NOTE]
>
>* 숨겨진 열을 사용하여 뷰에 표시하지 않으려는 특정 객체별로 정렬할 수 있습니다.\
>  예를 들어 작업 보기에서 작업 번호별로 정렬하고 보기에서 작업 번호 정보를 숨길 수 있습니다. 이 경우 열에서 참조한 객체는 뷰를 정렬하는 데 도움이 되지만 해당 객체의 정보는 뷰에 표시되지 않습니다.
>* 열을 숨길 때는 열의 정보가 숨겨져 있지만 열은 여전히 뷰에 있습니다.

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

## 예: 작업 보기에서 작업 번호 열을 정렬 및 숨깁니다.

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭합니다.

1. **열 추가**&#x200B;를 클릭하고 **이 열에 표시** 필드에 &quot;작업 번호&quot;를 입력한 다음 목록에 표시되면 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   이 코드에서 열을 숨기는 중요한 변경 사항은 다음과 같습니다.

   * `displayname=`: 이 줄은 비어 있어야 합니다.
   * `valuefield=`: 이 줄은 `value=`(으)로 바뀌어야 하며 비어 있어야 합니다.
   * `width=`: 필드에 따라 값이 **0** 또는 **1**&#x200B;이어야 합니다.

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
