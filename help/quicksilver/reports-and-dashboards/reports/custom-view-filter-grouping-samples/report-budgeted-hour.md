---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보고서: 예산책정 시간'
description: '보고서: 예산책정 시간'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# 보고서: 예산책정 시간

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Resource Planner에 액세스할 수 없는 다른 사용자와 예산책정된 시간 정보를 공유하려는 경우, 예산책정된 시간 보고서를 작성하면 됩니다. 그런 다음 해당 사용자와 보고서를 공유할 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>예산책정 시간은 Adobe Workfront 데이터베이스에서 매시간마다 업데이트됩니다. 보고서를 새로 고치면 반드시 보고서의 시간 정보가 새로 고쳐지는 것은 아닙니다. 각 예산책정 시간 보고서의 오른쪽 상단 모서리에서 마지막 갱신 이후 경과 시간을 볼 수 있습니다. 보고서를 새로 고치면 마지막 업데이트 이후 1시간 이상 있었던 경우에만 보고서의 정보가 새로 고쳐집니다.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 예산책정된 시간 보고서 작성

1. 을(를) 클릭합니다. **기본 메뉴** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.

1. 클릭 **신규 보고서 > 예산 책정된 시간**.

   기본 보기가 보고서에 적용됩니다.

1. (선택 사항) 보고서를 더 쉽게 읽을 수 있도록 하려면 **예산책정된 시간** 열, **텍스트 모드로 전환**&#x200B;를 변경한 다음

   ```
   valuefield
   ```

   라인 대상

   ```
   valueexpreesion
   ```

   반올림 표현식을 입력합니다.

   예산책정된 시간 수를 지정한 소수 수로 반올림합니다.

   Workfront에서 숫자를 반올림하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (선택 사항) **열 추가** 추가 열을 추가하려면
1. (선택 사항) 보고서를 더 쉽게 읽을 수 있도록 그룹을 추가하는 것이 좋습니다. 다음 그룹을 권장합니다.

   을(를) 클릭합니다. **그룹화** 탭한 다음, 다음 중 하나 또는 여러 작업을 수행합니다.

   1. 클릭 **그룹화 추가** 프로젝트 이름 입력을 시작한 다음 목록에 표시될 때 선택합니다.
   1. 클릭 **그룹화 추가** 작업 역할 이름 입력을 시작한 다음 목록에 표시될 때 선택합니다.
   1. 클릭 **그룹화 추가** 입력을 시작합니다. **할당 날짜**&#x200B;를 클릭하고 목록에 표시될 때 해당 일정을 선택한 다음, **그룹화 기준 날짜** 필드.

1. (선택 사항) **필터** 보고서에 필터를 추가합니다.
1. (선택 사항) **차트** 보고서에 차트를 추가하려면 다음을 수행하십시오.
1. 클릭 **저장 + 닫기**.

## 예산책정된 시간 보고서 검토

다음 정보는 기본적으로 예산책정된 시간 보고서에서 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트 </td> 
   <td>예산책정된 시간과 연관된 프로젝트의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>작업 역할</p> </td> 
   <td>예산책정된 시간과 연관된 작업 역할의 이름입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자</td> 
   <td>예산책정된 시간과 연관된 사용자의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당 일자</td> 
   <td> <p>할당 일자입니다. 해당 시간을 계획한 주의 첫 번째 날(일요일)입니다.</p> <p>팁:  <p>1주가 2개월 동안 지속되는 경우 보고서에서 두 개의 행을 생성합니다. 첫째 날(첫째 달 동안의 주 일요일) 및 둘째 달 첫째 날에 해당하는 둘째 날(그 주의 어느 날)입니다.</p> <p>예를 들어, 6월 30일(일요일) - 7월 6일(토요일) 주에 대해 사용자에 대해 8시간을 평가하는 경우 두 행은 6월 30일 및 7월 1일의 할당 날짜를 보여줍니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">예산 시간</td> 
   <td>자원 계획자에서 사용자에게 할당된 예산책정된 시간입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. 예산 시간</td> 
   <td>자원 계획자의 작업 역할 또는 프로젝트에 할당된 예산책정된 시간입니다.</td> 
  </tr> 
 </tbody> 
</table>
