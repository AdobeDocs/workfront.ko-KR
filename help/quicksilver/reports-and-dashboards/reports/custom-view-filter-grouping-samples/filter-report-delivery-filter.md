---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 배달 예약된 보고서 표시'
description: 이 보고서 필터는 Adobe Workfront에서 자동으로 배달되도록 예약된 모든 보고서를 표시합니다. 표준 보기와 함께 사용하는 것이 가장 좋습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# 필터: 배달 예약된 보고서 표시

<!--Audited: 10/2024-->

이 보고서 필터는 Adobe Workfront에서 자동으로 배달되도록 예약된 모든 보고서를 표시합니다. 표준 보기와 함께 사용하는 것이 가장 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
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

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보고서 게재 필터

이 필터를 적용하려면:

1. 보고서 목록으로 이동합니다.

1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.

1. **보고서에 대한 필터 규칙 설정** 영역에서 다음 코드를 복사하여 붙여 넣습니다.

   ```
   scheduledReportID=0
   scheduledReportID_Mod=notnull
   ```

1. **필터 저장**&#x200B;을 클릭합니다.
