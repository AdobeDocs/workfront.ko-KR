---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 만들기
description: 대시보드를 만들어 Adobe Workfront의 정보에 빠르게 액세스할 수 있습니다. 최적의 공동 작업을 위해 다른 사용자와 공유할 수 있는 보고서, 캘린더 및 외부 페이지를 대시보드에 추가할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 008713ef6587041310388c05909ad5f78fb9fa4c
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---

# 대시보드 만들기

<!--Audited: 01/2024-->

대시보드를 만들어 Adobe Workfront의 정보에 빠르게 액세스할 수 있습니다. 최적의 공동 작업을 위해 다른 사용자와 공유할 수 있는 보고서, 캘린더 및 외부 페이지를 대시보드에 추가할 수 있습니다.

대시보드에 대한 자세한 내용은 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront 플랜</strong></p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront 라이센스*</strong></p> </td> 
   <td> <p>현재: 플랜 </p>
   또는
   <p>새로운 기능: 표준 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>액세스 수준 구성</strong> </td> 
   <td> <p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>만든 대시보드에 대한 관리 권한을 갖게 됩니다</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

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
      <td><p>대시보드 이름입니다.</p><p>이름을 지정하지 않으면 기본적으로 대시보드에 있는 첫 번째 보고서의 이름이 대시보드 이름이 됩니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>설명 (선택 사항)</strong></td>
      <td>대시보드에 대한 설명입니다.</td>
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
