---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 시간대별 보고서 필터링
description: 오브젝트에 있는 날짜의 시간대별로 보고서를 필터링할 수 있습니다. 예를 들어, 시간이 입력된 특정 시간대에 대한 시간 보고서를 필터링할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 5%

---

# 시간대별 보고서 필터링

<!-- Audited: 11/2024 -->

오브젝트에 있는 날짜의 시간대별로 보고서를 필터링할 수 있습니다. 예를 들어, 시간이 입력된 특정 시간대에 대한 시간 보고서를 필터링할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
      <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>플랜</p></li>
         </ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

결과를 필터링하기 전에 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)를 참조하십시오.

## 날짜의 시간대별로 보고서 필터링 {#filter-a-report-by-the-time-frame-of-a-date}

1. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고**&#x200B;를 클릭합니다.

1. **새 보고서**&#x200B;를 클릭한 다음 원하는 보고서 유형을 선택합니다.\
   예를 들어 **시간 보고서**&#x200B;를 선택합니다.

1. **필터** 탭을 선택합니다.
1. **필터 규칙 추가**&#x200B;를 클릭한 다음 **시간 항목 날짜**&#x200B;를 선택합니다.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 다음 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">같음(대소문자 구분)</td> 
      <td>이 수정자를 선택한 후 시간을 입력한 날짜를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">같지 않음(대소문자 구분)</td> 
      <td>이 수정자를 선택한 후 시간이 입력된 날짜를 지정하여 이 날짜를 보고서에서 제외합니다. 이 보고서는 지정한 날짜에 대한 예상 시간을 모든 날짜에 기록한 시간을 보여줍니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>입력 일자가 누락된 시간만 표시하려면 이 수정자를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null 아님</td> 
      <td>입력 일자에 값이 있는 시간만 표시하려면 이 수정자를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사이</td> 
      <td>이 수정자를 선택한 후 시간을 입력한 날짜 범위를 지정합니다. 보고서에는 지정된 날짜 사이에 입력된 시간이 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음보다 작음</td> 
      <td>이 수정자를 선택한 후 시간을 입력하기 전에 날짜를 지정합니다. 보고서에는 지정된 날짜 이전에 입력된 시간이 표시되며 지정된 날짜는 포함되지 않습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">동일값 미만</td> 
      <td>이 수정자를 선택한 후 시간을 입력하기 전에 날짜를 지정합니다. 이 보고서는 지정된 날짜를 포함하여 지정된 날짜 이전에 입력한 시간을 보여줍니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음보다 큼</td> 
      <td>이 수정자를 선택한 후 시간을 입력한 날짜를 지정합니다. 보고서에는 지정된 날짜 이후에 입력된 시간이 표시되며 지정된 날짜는 포함되지 않습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">크거나 같음</td> 
      <td> <p>이 수정자를 선택한 후 시간을 입력한 날짜를 지정합니다. 이 보고서는 지정된 날짜를 포함하여 지정된 날짜 이후에 입력한 시간을 보여줍니다.</p> <p><a href="#built-in-time-frame-modifiers" class="MCXref xref">기본 제공 시간 프레임 수정자</a>에 설명된 대로 기본 제공 시간 프레임 수정자를 선택합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 이러한 수정자는 보고서의 필터 또는 프롬프트에 있는 날짜 필드에 사용할 수 있습니다.
1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 기본 제공 시간대 수정자 {#built-in-time-frame-modifiers}

Adobe Workfront에는 특정 날짜를 정의하지 않고 사용할 수 있는 시간대 수정자가 내장되어 있습니다. 

이러한 수정자는 보고서의 필터 또는 프롬프트에 있는 날짜 필드에 사용할 수 있습니다. 

날짜와 연결된 시간대별로 보고서를 필터링하는 방법에 대한 자세한 내용은  [날짜를 기준으로 보고서를 필터링합니다](#filter-a-report-by-the-time-frame-of-a-date).

예를 들어, 시간 보고서를 작성하고 특정 시간대에 입력한 시간을 표시하려는 경우 다음의 기본 제공 시간대 필터 옵션 중에서 선택할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">오늘</td> 
   <td>입력 일자가 오늘인 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">이번 주</td> 
   <td>현재 주의 시작 일자가 날짜인 시간, 즉 주말이 일요일에 시작하여 토요일에 끝나는 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">다음 주</td> 
   <td>시작 일자가 현재 주의 다음 주에 있는 일자인 시간을 표시합니다. 이 주는 일요일에 시작해서 토요일에 끝납니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">지난주</td> 
   <td>시작 일자가 현재 주의 이전 주 일자인 시간을 표시합니다. 이 주는 일요일에 시작되고 토요일에 끝납니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">이번 달</td> 
   <td>입력 일자가 현재 월의 일자인 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">다음 달</td> 
   <td>입력 일자가 현재 월의 다음 달 날짜인 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">지난 달</td> 
   <td>입력 일자가 현재 월의 이전 월인 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">이번 분기</td> 
   <td> <p>입력 일자가 현재 분기의 일자인 시간을 표시합니다. 여기서 분기는 다음과 같이 정의됩니다.</p> 
    <ul> 
     <li>1분기: 1월 1일 - 3월 30일</li> 
     <li>2분기: 4월 1일 - 6월 30일</li> 
     <li>3분기: 7월 1일 - 9월 30일</li> 
     <li>4분기: 10월 1일 - 12월 31일</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">다음 분기</td> 
   <td>입력 일자가 현재 분기 다음 분기의 일자인 시간을 표시합니다. 여기서 분기는 위에 정의됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">지난 분기</td> 
   <td> <p>입력 일자가 현재 분기 이전 분기의 일자인 시간을 표시합니다. 여기서 분기는 위에 정의됩니다.</p> <p>참고: Workfront 관리자가 시스템에 대한 사용자 정의 분기를 활성화하고 정의한 경우 분기의 기본 제공 필터는 사용자 정의 분기 정보로 대체됩니다. 사용자 지정 분기 활성화에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">프로젝트에 대한 사용자 지정 분기 활성화</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">올해</td> 
   <td>입력 일자가 현재 연도의 일자인 시간을 표시합니다. 여기에서 현재 연도는 1월 1일에 시작하여 12월 31일에 끝납니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">지난 해</td> 
   <td>입력 일자가 지난 연도의 일자이고 지난 연도가 현재 일자보다 12개월 먼저 시작되는 시간을 표시합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작년</td> 
   <td> <p>입력 일자가 지난 해의 일자인 시간을 표시합니다. 이때 마지막 연도는 1월 1일에 시작하여 현재 연도 이전 연도의 12월 31일에 끝납니다.</p> <p>주: 회계 연도에는 내장 기간이 없습니다. 조직에서 정의한 회계 연도의 날짜 범위에 대해 사용자 정의 수정자를 사용하여 보고서를 생성하고 날짜별로 정보를 필터링할 수 있습니다. 즉석에서 회계 연도의 시간대를 선택하려면 필터 대신 프롬프트를 사용해야 합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
