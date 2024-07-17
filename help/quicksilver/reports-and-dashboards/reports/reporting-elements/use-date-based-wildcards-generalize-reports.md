---
product-area: reporting
navigation-topic: reporting-elements
title: 날짜 기반 와일드카드를 사용하여 보고서를 일반화합니다.
description: 특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# 날짜 기반 와일드카드를 사용하여 보고서를 일반화합니다.

특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.

예를 들어, 특정 계획된 시작 일자가 있는 작업을 표시하는 보고서를 생성하려는 경우 필터에서 달력 날짜 선택기를 사용하여 특정 일자를 선택할 수 있습니다. 그러나 보고서에 액세스한 날짜로부터 특정 시간대 내에 계획된 시작 일자가 있는 작업을 표시하는 보고서를 생성하려는 경우, 누군가 보고서를 볼 때 해당 보고서를 볼 때와 관련된 시간대에 대한 정보를 표시함을 나타내는 와일드카드를 사용할 수 있습니다.

예를 들어 지난 주, 지난 해, 다음 2주 등입니다. 이렇게 하면 보고서를 한 번 빌드하지만 필터에서 와일드카드를 사용하기 때문에 누군가 보고서를 실행할 날짜에 맞게 수정되므로 읽을 때마다 다른 결과가 생성됩니다.

다음 보고 요소를 작성할 때 날짜 기반 와일드카드를 사용할 수 있습니다.

* 필터
* 사용자 정의 프롬프트
* 열에 대한 규칙을 추가할 때 보기

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서의 보고 요소를 편집합니다.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서에서 보고 요소 편집</p> <p>보기 또는 필터에 대한 권한을 관리하여 편집합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

와일드카드 변수를 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)를 참조하십시오.

## 방법 단계

보고서에 날짜 기반 와일드카드를 삽입하려면 다음을 수행합니다.

1. 날짜 기반 와일드카드를 삽입할 보고서로 이동합니다.
1. **보고서 동작**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. **필터** 탭을 클릭합니다.
1. **필터 규칙 추가**&#x200B;를 클릭합니다.
1. 필터링 기준으로 사용할 필드의 이름을 입력하십시오.\
   날짜를 참조하는 필드를 입력해야 합니다.
1. 필터 변수에 대한 드롭다운 메뉴에서 **같음**&#x200B;을 선택하십시오.

   >[!TIP]
   >
   >Adobe Workfront에서 와일드카드로 작업할 때 항상 **같음** 필터 변수를 선택해야 합니다.

1. **이름 입력 시작...** 상자에 보고서를 실행한 바로 그 날에 발생하는 정보를 표시하려면 `$$TODAY`을(를) 입력하십시오.

   또는

   보고서가 실행되는 날짜와 시간에 발생하는 정보를 표시하려면 `$$NOW`을(를) 입력하십시오.

   이 날짜는 사용자가 보고서를 실제로 본 날짜와 함께 변경되므로 항상 다릅니다. 따라서 보고서의 정보는 매일 다릅니다.

1. (선택 사항) 보고서가 실행된 날짜 이후 일정 기간 내에 발생하는 정보를 표시하려면 `$$TODAY+1w`을(를) 입력하여 다음 주에 정보를 표시하거나 `$$TODAY+2m`을(를) 입력하여 다음 2개월 내에 정보를 표시하십시오. 분기, 시간, 일 또는 연도의 기간을 표시할 수도 있습니다.
1. (선택 사항) 보고서가 실행되기 전 일정 기간 내에 발생한 항목에 대한 정보를 표시하려면 `$$TODAY-1w`을(를) 입력하여 이전 주의 정보를 표시하거나 `$$TODAY-2m`을(를) 입력하여 이전 2개월의 정보를 표시합니다. 분기, 시간, 일 또는 연도의 기간을 표시할 수도 있습니다.

   날짜 기반 와일드카드에 사용할 수 있는 전체 특성, 한정자 및 연산자 목록은 문서 [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)를 참조하십시오.

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 추가 정보

다음도 참조하십시오.

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
