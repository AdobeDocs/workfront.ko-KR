---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 만들기
description: 대시보드를 만들어 Adobe Workfront의 정보에 빠르게 액세스할 수 있습니다. 최적의 공동 작업을 위해 다른 사용자와 공유할 수 있는 보고서, 캘린더 및 외부 페이지를 대시보드에 추가할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 39a8d670baa19aa37e29b0312e6c9a296569f44c
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 4%

---

# 대시보드 만들기

<!--Audited: 01/2025-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리 보기 환경에서만 사용할 수 있습니다.</span>


대시보드를 만들어 Adobe Workfront의 정보에 빠르게 액세스할 수 있습니다. 최적의 공동 작업을 위해 다른 사용자와 공유할 수 있는 대시보드에 최대 25개의 보고서, 캘린더 및 외부 페이지를 추가할 수 있습니다.

대시보드에 대한 자세한 내용은 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)을 참조하세요.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

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
      <p>표준</p>
      <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>만든 대시보드에 대한 관리 권한을 갖게 됩니다</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

대시보드에 추가하려면 먼저 다음 개체를 만들어야 합니다.

* **보고서**: 보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

* **캘린더**: 캘린더 만들기에 대한 자세한 내용은 [캘린더 보고서 개요](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)를 참조하십시오.

기존 외부 페이지를 대시보드에 추가하거나 새 대시보드에서 만들 수 있습니다. 외부 페이지 만들기에 대한 자세한 내용은 [외부 웹 페이지를 대시보드에 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)을 참조하십시오.

## 대시보드 만들기

{{step1-to-dashboards}}

1. **새 대시보드**&#x200B;를 클릭합니다.\
   새 대시보드 대화 상자가 표시됩니다.

1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>이름</strong></td>
      <td><p>대시보드 이름입니다. 호환성 문제를 방지하려면 UTF-8 문자만 사용하는 것이 좋습니다.</p><p>이름을 지정하지 않으면 기본적으로 대시보드에 있는 첫 번째 보고서의 이름이 대시보드 이름이 됩니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>설명 (선택 사항)</strong></td>
      <td>대시보드에 대한 설명입니다.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>통화</strong></td>
      <td><span class="preview">대시보드의 기본 통화 유형입니다. <br>
      <br>대시보드를 필터링할 때 사용자가 다른 통화 유형을 전환할 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md">통화 유형별로 대시보드 필터링</a>을 참조하십시오.</span></td>
     </tr>
    </tbody>
   </table>

1. **레이아웃/보고서 추가/캘린더 추가** 섹션 맨 위에서 해당 라디오 단추를 클릭하여 레이아웃을 선택합니다. 보고서, 캘린더 또는 외부 페이지가 대시보드에 표시되는 레이아웃입니다.

   단일 열 레이아웃이 기본값입니다.

   대시보드의 보고서 레이아웃에 대한 자세한 내용은 [보고서가 대시보드에 표시되는 방식 이해](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md)를 참조하십시오.

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. **사용 가능한 보고서 및 일정** 섹션에서 검색 막대에 보고서, 일정 또는 외부 페이지의 이름을 입력한 다음 레이아웃 창의 보고서, 일정 또는 외부 페이지를 오른쪽으로 끌어서 놓습니다.

   >[!NOTE]
   >
   >항목을 검색할 때 가장 최근에 생성된 2,000개의 보고서 중 하나가 반환됩니다. 유니코드 문자가 포함된 보고서 이름은 검색 결과에 반환되지 않습니다. 다른 소스에서 이름을 복사하고 붙여넣는 대신 이름을 입력하여 Workfront에서 객체 이름을 지정할 때 유니코드 문자를 포함하지 않는 것이 좋습니다.

   ![보고서 검색](assets/unshimmed-dashboard-ui.png)

1. (선택 사항) 대시보드에 새 외부 페이지를 추가하려면 **외부 페이지 추가**&#x200B;를 클릭합니다.

   외부 페이지를 만들고 대시보드에 포함하는 방법에 대한 자세한 내용은 [외부 웹 페이지를 대시보드에 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)을 참조하십시오.

1. **저장 및 닫기**&#x200B;를 클릭합니다.

   타임스탬프가 대시보드의 오른쪽 위 모서리에 표시됩니다. 타임스탬프에는 대시보드를 마지막으로 새로 고친 날짜, 시간 및 시간대가 포함됩니다.
