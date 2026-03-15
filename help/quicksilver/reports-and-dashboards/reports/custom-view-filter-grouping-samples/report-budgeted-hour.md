---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보고서: 예산 책정 시간'
description: '보고서: 예산 책정 시간'
author: Courtney
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 4%

---

# 보고서: 예산 책정 시간

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Resource Planner에 액세스할 수 없는 다른 사용자와 예산책정된 시간 정보를 공유하려면 예산책정된 시간 보고서를 작성하면 됩니다. 그런 다음 보고서를 공유할 수 있습니다.

>[!IMPORTANT]
>
>예산책정된 시간은 일반적으로 Adobe Workfront 데이터베이스에서 매시간(가끔, 최대 3시간이 소요될 수 있음)마다 업데이트됩니다. 보고서를 새로 고치면 보고서의 시간 정보가 반드시 새로 고쳐지는 것은 아닙니다. 모든 예산 책정 시간 보고서의 오른쪽 상단 모서리에서 마지막 갱신 이후 경과된 시간을 조회할 수 있습니다. 보고서를 새로 고치면 마지막 업데이트 이후 1시간 이상이 지난 경우에만 보고서 내의 정보가 새로 고쳐집니다.
>
>![예산책정 시간 보고서 동기화 경고](assets/budgeted-hour-report-time-sync-warning-350x74.png)

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
   <td role="rowheader">Adobe Workfront 라이센스</td> 
   <td> 
   <p>참여자 또는 필터 수정 요청 </p>
   <p>표준 또는 계획: 보고서 수정</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스를 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표에 있는 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 예산책정 시간 보고서 작성

1. 오른쪽 상단에 있는 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png) 또는 왼쪽 상단에 있는 **주 메뉴** 아이콘 ![주 메뉴 줄](assets/lines-main-menu.png)을 클릭한 다음 **보고서**&#x200B;를 클릭합니다.

1. **새 보고서** > **자세히** > **예산 책정 시간**&#x200B;을 클릭합니다.

   기본 보기가 보고서에 적용됩니다.

1. (선택 사항) 보고서를 더 쉽게 읽을 수 있도록 하려면 **버드를 클릭하십시오.** 열을 사용한 다음 **텍스트 모드로 전환**&#x200B;한 다음 **텍스트 모드 편집**&#x200B;을 클릭하세요.
1. `valuefield` 줄을 `valueexpreesion`(으)로 변경하고 반올림 식을 입력하십시오.

   이렇게 하면 예산 책정된 시간 수가 지정한 소수 수로 반올림됩니다.

   Workfront에서 숫자를 반올림하는 방법에 대한 자세한 내용은 문서 [계산된 데이터 식의 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **완료**&#x200B;를 클릭합니다.
1. (선택 사항) 열을 더 추가하려면 **열 추가**&#x200B;를 클릭하십시오.
1. (선택 사항) 보고서를 쉽게 읽을 수 있도록 그룹화를 추가하는 것이 좋습니다. 다음 그룹을 사용하는 것이 좋습니다.

   **그룹화** 탭을 클릭한 후 다음 중 하나 또는 여러 가지를 수행합니다.

   * **그룹화 추가**&#x200B;를 클릭하고 &quot;프로젝트 이름&quot;을 입력한 다음 목록에 표시될 때 선택합니다.
   * **그룹화 추가**&#x200B;를 클릭하고 &quot;작업 역할 이름&quot; 입력을 시작한 다음 목록에 표시될 때 선택합니다.
   * **그룹화 추가**&#x200B;를 클릭하고 &quot;할당 날짜&quot; 입력을 시작한 후 목록에 표시될 때 선택한 다음 **그룹화 날짜 기준** 필드에서 그룹화할 기간을 선택합니다.

1. (선택 사항) 보고서에 필터를 추가하려면 **필터**&#x200B;를 클릭합니다.
1. (선택 사항) 보고서에 차트를 추가하려면 **차트**&#x200B;를 클릭하십시오.
1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 예산 책정 시간 보고서 검토

예산책정 시간 보고서에서는 기본적으로 다음 정보를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트 </td> 
   <td>예산 책정 시간과 연관된 프로젝트의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>작업 역할</p> </td> 
   <td>예산 책정 시간과 연관된 Job 역할의 이름입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자</td> 
   <td>예산 책정 시간과 연관된 사용자의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당 일자</td> 
   <td> <p>할당 날짜입니다. 시간을 예산으로 설정한 주의 첫 번째 날(일요일)입니다.</p> <p>팁:  <p>주가 2개월을 걸쳐 있는 경우 보고서에 두 개 행, 즉 첫 번째 요일(첫 번째 달 동안의 일요일)에 해당하는 행과 두 번째 달의 첫 번째 요일에 해당하는 두 번째 행(특정 요일 수 있음)이 생성됩니다.</p> <p>예를 들어, 6월 30일(일요일) - 7월 6일(토요일)이라는 주에 대해 한 사용자의 8시간을 계획하는 경우, 두 행은 할당 날짜를 6월 30일과 7월 1일로 표시합니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">예산 시간</td> 
   <td>Resource Planner에서 사용자에게 할당된 예산책정 시간입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln 예산 시간</td> 
   <td>Job 역할 또는 Resource Planner의 프로젝트에 할당된 예산책정된 시간입니다.</td> 
  </tr> 
 </tbody> 
</table>
