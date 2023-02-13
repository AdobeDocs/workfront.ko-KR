---
product-area: reporting
navigation-topic: reporting-elements
title: 날짜 기반 와일드카드를 사용하여 보고서를 일반화합니다
description: 특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 날짜 기반 와일드카드를 사용하여 보고서를 일반화합니다

특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.

예를 들어 특정 계획 시작 날짜가 있는 작업을 보여 주는 보고서를 생성하려는 경우 필터의 달력 날짜 선택기를 사용하여 특정 날짜를 선택할 수 있습니다. 그러나 보고서에 액세스한 날짜부터 특정 시간 내에 계획 시작 날짜가 있는 작업을 표시하는 보고서를 생성하려는 경우 보고서를 볼 때 보고서를 볼 때 해당 기간에 대한 정보가 표시됨을 나타내는 와일드카드를 사용할 수 있습니다.

예를 들어 지난 주, 지난 연도, 다음 2주 등이 있습니다. 이 방법으로 보고서를 한 번 작성할 수 있지만, 필터에서 와일드카드를 사용하면 보고서를 읽을 때마다 결과가 달라질 수 있습니다. 보고서가 보고서를 실행하는 날에 적용되기 때문입니다.

다음 보고 요소를 작성할 때 날짜 기반 와일드카드를 사용할 수 있습니다.

* 필터
* 사용자 정의 프롬프트
* 열에 대한 규칙을 추가할 때 보기

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 보고 요소를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 보고 요소를 편집합니다</p> <p>보기 또는 필터에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

와일드카드 변수를 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 방법 단계

보고서에 날짜 기반 와일드카드를 삽입하려면

1. 날짜 기반 와일드카드를 삽입할 보고서로 이동합니다.
1. 클릭 **보고서 작업**, 그런 다음 **편집**.

1. 을(를) 클릭합니다. **필터** 탭.
1. 클릭 **필터 규칙 추가**.
1. 필터링할 필드의 이름을 입력하기 시작합니다.\
   날짜를 참조하는 필드를 입력해야 합니다.
1. 선택 **Equal** 를 클릭합니다.

   >[!TIP]
   >
   >항상 을(를) 선택해야 합니다 **Equal** Adobe Workfront에서 와일드카드를 사용할 때 변수를 필터링합니다.

1. 에서 **이름 입력 시작..** 상자, 유형: `$$TODAY` 보고서가 실행되는 당일 발생한 항목에 대한 정보를 표시하려는 경우.

   또는

   유형 `$$NOW` 보고서를 실행하는 날짜와 시간에 발생하는 문제에 대한 정보를 표시하려는 경우

   이 날짜는 사용자가 보고서를 실제로 본 날짜에 따라 변경되므로 항상 다릅니다. 따라서 보고서의 정보는 일별로 다릅니다.

1. (선택 사항) 보고서 실행 날짜 이후 시간 내에 발생하는 정보를 표시하려면 을 입력합니다 `$$TODAY+1w` 다음 주에 정보를 표시하려면 또는 `$$TODAY+2m` 정보를 표시할 수 있습니다. 분기, 시간, 일 또는 연도의 시간대를 표시할 수도 있습니다.
1. (선택 사항) 보고서 실행 날짜 이전 시간 내에 발생한 내용에 대한 정보를 표시하려면 을 입력합니다 `$$TODAY-1w` 이전 주의 정보를 표시하려면 또는 `$$TODAY-2m` 이전 2개월의 정보를 표시하기 위해 분기, 시간, 일 또는 연도의 시간대를 표시할 수도 있습니다.

   날짜 기반 와일드카드에 사용할 수 있는 속성, 구분자 및 연산자의 전체 목록은 문서를 참조하십시오 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. 클릭 **저장 + 닫기**.

## 추가 정보

다음을 참조하십시오.

* [기본 보고서 생성 프로그램](https://one.workfront.com/s/basic-report-creation-program)
* [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
