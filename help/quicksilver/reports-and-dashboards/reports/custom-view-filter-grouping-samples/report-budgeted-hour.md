---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보고서: 예산 시간'
description: '보고서: 예산 시간'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# 보고서: 예산 시간

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

리소스 플래너에 대한 액세스 권한이 없는 다른 사용자와 예산 시간 정보를 공유하려면 예산 시간 보고서를 작성하여 공유할 수 있습니다. 그런 다음 보고서를 해당 사용자와 공유할 수 있습니다.

>[!IMPORTANT]
>
>예산 시간은 일반적으로 Adobe Workfront 데이터베이스에서 매시간마다 업데이트됩니다(드물게 최대 3시간이 소요될 수 있습니다). 보고서를 새로 고쳐도 해당 보고서 내의 시간 정보가 새로 고쳐지지 않습니다. 모든 예산 시간 보고서의 오른쪽 상단 모서리에서 마지막 업데이트 이후 경과한 시간을 볼 수 있습니다. 보고서를 새로 고치면 마지막 업데이트 후 1시간 이상 경과한 경우에만 보고서 내의 정보가 새로 고침됩니다.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## 액세스 요구 사항

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 예산 시간 보고서 작성

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-icon.png) 오른쪽 상단에서 을(를) 클릭한 다음 **보고서**.

1. 클릭 **새 보고서 > 예산 시간**.

   기본 보기가 보고서에 적용됩니다.

1. (선택 사항) 보고서를 더 쉽게 읽으려면 **예산 시간** 열, 그런 다음 **텍스트 모드로 전환**&#x200B;을 클릭한 다음 을 변경합니다.

   ```
   valuefield
   ```

   줄 끝

   ```
   valueexpreesion
   ```

   및 반올림 표현식을 입력합니다.

   이렇게 하면 예산 시간이 지정한 소수 자릿수로 반올림됩니다.

   Workfront에서 숫자를 반올림하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [계산된 데이터 표현식 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (선택 사항) **열 추가** 추가 열을 추가합니다.
1. (선택 사항) 보고서를 더 쉽게 읽을 수 있도록 보고서 세트에 그룹화를 추가하는 것이 좋습니다. 다음 그룹화를 제안합니다.

   다음을 클릭합니다. **그룹화** 탭을 누른 후 다음 중 하나 또는 일부를 수행합니다.

   1. 클릭 **그룹화 추가** &quot;프로젝트 이름&quot;을 입력한 다음 목록에 나타나면 선택하십시오.
   1. 클릭 **그룹화 추가** &quot;작업 역할 이름&quot;을 입력한 다음 목록에 표시될 때 선택합니다.
   1. 클릭 **그룹화 추가** 입력을 시작합니다. **할당 일자**&#x200B;목록에 나타나면 선택한 다음 그룹화할 시간대를 선택합니다 **일자 그룹화 기준** 필드.

1. (선택 사항) **필터** 필터를 보고서에 추가합니다.
1. (선택 사항) **차트** 보고서에 차트를 추가합니다.
1. 클릭 **저장 + 닫기**.

## 예산 시간 보고서 검토

예산 시간 보고서에서 기본적으로 다음 정보를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트 </td> 
   <td>예산 시간과 연관된 프로젝트의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>작업 역할</p> </td> 
   <td>예산 시간과 연관된 작업 역할의 이름입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자</td> 
   <td>예산 시간과 연관된 사용자의 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당 일자</td> 
   <td> <p>할당 날짜입니다. 이는 시간 예산을 책정한 주의 첫째 날(일요일)입니다.</p> <p>팁:  <p>한 주가 2개월 동안 걸리면 보고서에 두 개의 행이 생성됩니다. 하나는 첫 번째 요일(첫 번째 달 동안 있는 주의 일요일)에 해당하고 두 번째 하나는 두 번째 달의 첫 번째 요일(해당 주의 어떤 요일일 수 있음)에 해당합니다.</p> <p>예를 들어, 6월 30일(일요일) - 7월 6일(토요일) 주에 대해 사용자에 대해 8시간을 책정하는 경우 두 행에 할당 일자가 6월 30일과 7월 1일로 표시됩니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">예산 시간</td> 
   <td>리소스 플래너에서 사용자에게 할당된 예산 시간입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">계획됨. 예산 시간</td> 
   <td>리소스 플래너의 작업 역할 또는 프로젝트에 할당된 예산 시간입니다.</td> 
  </tr> 
 </tbody> 
</table>
