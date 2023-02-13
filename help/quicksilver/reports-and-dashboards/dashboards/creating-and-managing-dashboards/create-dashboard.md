---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 만들기
description: 대시보드를 만들어 보고서, 달력 및 외부 페이지의 정보에 빠르게 액세스할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 대시보드 만들기

대시보드를 만들어 보고서, 달력 및 외부 페이지의 정보에 빠르게 액세스할 수 있습니다.

대시보드에 대한 자세한 내용은 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront 플랜*</strong></p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront 라이선스*</strong></p> </td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>보고서, 대시보드 및 달력에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>새 대시보드에 대한 관리 권한을 받습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.<br>대시보드 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">보고서, 대시보드 및 달력 공유 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

다음 개체를 먼저 만들어야 대시보드에 추가할 수 있습니다.

* **보고서**: 보고서 만들기에 대한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **달력**: 달력 만들기에 대한 내용은 [달력 보고서 개요](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **외부 페이지**: 외부 페이지 만들기에 대한 내용은 [대시보드에 외부 웹 페이지 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 대시보드 만들기

1. Main Menu 아이콘을 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 **대시보드.**
1. 클릭 **새 대시보드**.\
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
      <td role="rowheader"><strong>설명(선택 사항)</strong></td>
      <td>대시보드에 대한 설명입니다.</td>
     </tr>
    </tbody>
   </table>

1. 해당 라디오 단추를 클릭하여 레이아웃을 선택합니다.

   단일 열 레이아웃이 기본값입니다.

   대시보드의 보고서 레이아웃에 대한 자세한 내용은 [보고서가 대시보드에 표시되는 방식을 이해합니다](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. 기존 보고서, 달력 또는 외부 페이지를 **이름 또는 유형별로 검색..** 필드를 만든 다음 목록에 표시될 때 레이아웃 창으로 드래그합니다.

   >[!NOTE]
   >
   >항목을 검색할 때 검색 결과에 가장 최근에 작성된 보고서 2,000개가 반환됩니다. 유니코드 문자를 포함하는 보고서 이름은 검색 결과에 반환되지 않습니다. 가장 좋은 방법은 다른 소스의 이름을 복사하여 붙여넣는 대신 이름을 입력하여 Workfront에서 개체의 이름을 지정할 때 유니코드 문자를 포함하지 않는 것입니다.

   ![보고서 검색](assets/qs-new-dashboard-ui-0722.png)

1. (선택 사항) **외부 페이지 추가** 대시보드에 외부 페이지를 추가하려면\
   외부 페이지를 만들어 대시보드에 포함시키는 방법에 대한 자세한 내용은 [대시보드에 외부 웹 페이지 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. 클릭 **저장 + 닫기**.\
   대시보드의 오른쪽 위 모서리에 타임스탬프가 표시됩니다. 타임스탬프에는 대시보드를 마지막으로 새로 고친 날짜, 시간 및 시간대가 포함됩니다.
