---
title: 달력 보기 관리
description: 달력 보기에서 레코드와 해당 필드를 표시할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 달력 보기 관리

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

레코드 유형 페이지에서 레코드와 해당 필드를 달력 보기에 표시할 수 있습니다.

Maestro 보기 및 관리 방법에 대한 자세한 내용은 다음을 참조하십시오. [레코드 보기 관리](../views/manage-record-views.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준 구성</td>
   <td> <p>Maestro에 대한 액세스 수준 제어 없음 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 달력 보기 관리 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

다음 사항을 고려하십시오.

* 레코드 유형과 연결된 날짜 필드가 두 개 이상 있는 경우에만 달력 보기를 만들 수 있습니다. 레코드 유형과 연결된 날짜 필드가 하나 또는 없으면 달력 보기 옵션이 흐리게 표시됩니다.
* 다음 시나리오:

   * 시작 및 종료 날짜에 값이 없으면 레코드가 달력에 표시되지 않습니다
   * 시작 또는 종료 날짜에 값이 없으면 레코드가 1일 이벤트로 표시됩니다
   * 시작 날짜가 종료 날짜 이후인 경우 레코드가 캘린더에 표시되지 않습니다.

달력 보기를 관리하려면:

1. 달력을 보려는 레코드 유형 페이지로 이동합니다.
1. 문서에 설명된 대로 달력 보기를 만듭니다 [레코드 보기 관리](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   선택한 레코드 유형과 연관된 레코드가 달력에 막대로 표시됩니다.

1. 다음 중 하나를 수행하여 달력을 탐색합니다.

   * 왼쪽 및 오른쪽 아이콘을 클릭하거나 가로 스크롤을 사용하여 달력에서 앞뒤로 이동합니다.
   * 클릭 **오늘** 캘린더를 오늘 날짜로 맞춰야 합니다.
   * 시간 증가를 업데이트하려면 시간대 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

      * 월