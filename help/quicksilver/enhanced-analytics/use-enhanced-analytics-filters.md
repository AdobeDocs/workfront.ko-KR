---
title: 향상된 분석에서 필터 적용
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Adobe Workfront의 향상된 분석 영역에 있는 필터를 사용하면 특정 프로젝트 또는 특정 유형의 데이터에 집중할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# 향상된 분석에서 필터 적용

>[!IMPORTANT]
>
>향상된 Analytics가 5월 27일에 Workfront에서 제거되었습니다. Workfront Data Connect는 새로운 대체 솔루션이며 현재 사용하는 향상된 Analytics 시각화를 복제하는 데 사용할 수 있습니다. <br>자세한 내용은 [향상된 Analytics 사용 중단](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) 안내서를 참조하십시오.


<!-- Audited: 12/2023 -->

Adobe Workfront의 향상된 분석 영역에 있는 필터를 사용하면 특정 프로젝트 또는 특정 유형의 데이터에 집중할 수 있습니다. 사용하는 필터 유형은에서 insight에 제공할 수 있습니다.

* 소유한 프로젝트
* 특정 포트폴리오 또는 프로그램 보기
* 특정 시간대(주, 분기, 회계 연도)에 대한 주요 성과 지표

필요에 따라 필터를 추가하거나 제거할 수 있으며 Workfront은 로그아웃한 경우에도 적용한 필터를 유지합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>
      <p>새로 만들기: 모두</p>
      <p>또는</p>
      <p>현재: 비즈니스 이상</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
      <p>새로운 기능: 밝게 또는 높음</p>
      <p>또는</p>
      <p>현재: 검토 이상</p>
   </td> 
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <p>특정 프로젝트 필드 필터 옵션을 보려면 작업, 포트폴리오 및 사용자에 대한 보기 액세스 권한도 있어야 합니다.</p> <p>참고: 액세스 수준 편집 대화 상자의 <strong>추가 제한 설정</strong> 섹션에서 제한을 선택하면 필터가 적용된 후 필터 또는 향상된 분석 페이지에 일부 정보가 표시되지 않을 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

향상된 Analytics를 사용하기 위한 필수 구성 요소는 [향상된 Analytics 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 [필수 구성 요소](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites)를 참조하십시오.

## 날짜 범위 필터 변경 {#change-the-date-range-filter}

기본적으로 향상된 분석 영역의 시각화는 지난 60일과 다음 15일 동안의 데이터를 보여 줍니다. 새 날짜 범위를 선택하여 향상된 분석 영역의 모든 시각화에 적용할 수 있습니다. 페이지에서 멀리 이동하는 경우 다음 페이지로 다시 이동할 때 기본 날짜 범위가 적용됩니다.

>[!TIP]
>
>키보드의 키를 사용하여 달력 위젯에서 날짜 범위를 이동하고, 열고, 선택할 수도 있습니다.\
>자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md) 문서의 [키보드 단축키](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) 섹션을 참조하십시오.

새 날짜 범위를 선택하려면 다음을 수행하십시오.

{{step1-to-analytics}}

1. 오른쪽 상단에서 날짜 범위 필드를 클릭하여 달력 보기를 엽니다.
1. 달력 위에 있는 화살표를 사용하여 시작 날짜의 월을 찾은 다음 시작 날짜를 선택합니다.

   ![날짜 범위 선택](assets/filters-select-date-range-350x344.png)

1. 달력 위에 있는 화살표를 사용하여 종료 날짜의 월을 찾은 다음 종료 날짜를 선택합니다.
1. (선택 사항) 더 작은 날짜 범위를 확대하려면 시각화 중 하나에 있는 특정 날짜에서 다른 날짜로 마우스를 끕니다.

   화면의 모든 시각화가 선택한 일정에 맞게 업데이트되며 기존 필터 옆에 일정 필터가 표시됩니다. 이 필터는 로그아웃하거나 고급 분석 영역에서 벗어나는 경우 유지되지 않습니다.

   ![일정 필터](assets/timeframe-filter-350x220.png)

## 필터 추가

기본 프로젝트 필드, 사용자 정의 양식 필드 및 프로젝트에 할당된 홈 팀에 따라 필터를 추가할 수 있습니다.

>[!TIP]
>
>키보드의 키를 사용하여 새 필터로 이동하고 추가할 수도 있습니다.\
>자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md) 문서의 [키보드 단축키](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 섹션을 참조하십시오.

* [프로젝트 필드 필터 추가](#add-a-project-field-filter)
* [프로젝트 사용자 정의 양식 필터 추가](#add-a-project-custom-form-filter)
* [팀 필터 추가](#add-a-team-filter)

### 프로젝트 필드 필터 추가 {#add-a-project-field-filter}

프로젝트 필드 필터를 사용하면 기본적으로 프로젝트에 포함된 필드에 입력한 값을 기반으로 프로젝트 및 작업에 대한 데이터를 필터링할 수 있습니다.

다음 프로젝트 필드 필터 유형을 사용할 수 있습니다.

| 필드 | 표시된 데이터 |
|---|---|
| **프로젝트** | 선택한 프로젝트에 대한 데이터만 표시합니다. |
| **프로그램** | 선택한 프로그램의 프로젝트에 대한 데이터만 표시합니다. |
| **Portfolio** | 선택한 포트폴리오의 프로젝트에 대한 데이터만 표시 |
| **조건** | 가장 최근에 선택한 상태(대상, 위험 또는 문제 발생)가 있는 프로젝트에 대한 데이터만 표시합니다. |
| **상태** | 가장 최근에 선택한 상태(완료, 현재, 보류, 취소 등)가 있는 프로젝트에 대한 데이터만 표시합니다. |
| **스폰서** | 선택한 스폰서가 있는 프로젝트에 대한 데이터만 표시합니다. |
| **프로젝트 소유자** | 선택한 프로젝트 소유자가 있는 프로젝트에 대한 데이터만 표시합니다. |

사용자 정의 양식 필터는 다르게 작동합니다. 자세한 내용은 [프로젝트 사용자 정의 양식 필터 추가](#add-a-project-custom-form-filter)를 참조하십시오.

프로젝트 필드 필터를 추가하려면:

{{step1-to-analytics}}

1. 왼쪽 상단에서 **필터 추가**&#x200B;를 클릭한 다음 원하는 필터 유형을 선택합니다.

   >[!NOTE]
   >
   >필터 유형에 따라 다른 데이터가 표시됩니다. 필터에는 필터 유형을 하나만 사용할 수 있습니다. 필터 유형을 선택한 후에는 다른 프로젝트 필드 필터에서 사용할 수 없습니다.

1. **검색** 필드에 최소 3자의 텍스트를 입력하여 데이터를 보려는 값을 찾은 다음 필터에 포함할 각 값을 선택합니다.

   현재 값을 모두 선택하려면 **모두 선택**&#x200B;을 클릭하십시오.

   ![필터 값 선택](assets/select-filter-value-350x251.png)

1. 원하는 값을 모두 선택한 후 **필터 적용**&#x200B;을 클릭합니다.

   적용된 필터를 반영하도록 오른쪽 상단 업데이트에 프로젝트가 카운트됩니다.

1. 추가할 각 필터에 대해 이 단계를 반복합니다.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 아래 시각화에 표시됩니다.

   >[!TIP]
   >
   >기본적으로 표시되는 50개 이상의 프로젝트에 대한 데이터를 보려면 다음을 수행할 수 있습니다.
   >
   >   * 왼쪽 하단의 화살표를 사용하여 해당 시각화에 있는 다음 50개의 프로젝트를 표시합니다.\
   >     ![페이지 매김 화살표](assets/pagination-350x118.png)
   >   
   >   * 시각화의 **정렬 기준** 드롭다운 메뉴를 사용하여 다른 순서로 프로젝트를 봅니다.\
   >     ![메뉴별 정렬](assets/sort-by-menu-350x247.png)

   날짜 범위를 조정하려면 [날짜 범위 필터 변경](#change-the-date-range-filter)을 참조하세요.

### 프로젝트 사용자 정의 양식 필터 추가

사용자 정의 양식 필터 유형을 사용하면 프로젝트의 사용자 정의 양식 필드에 입력한 값을 기반으로 프로젝트 및 작업의 데이터를 필터링할 수 있습니다. 다른 향상된 분석 필터 유형과 달리, 사용자 정의 양식 필터를 두 개 이상 추가할 수 있습니다. 각 사용자 정의 양식 필터에는 특정 사용자 정의 양식의 선택한 필드 내에서만 입력한 값이 포함됩니다.

사용자 정의 양식 필터를 추가하려면:

{{step1-to-analytics}}

1. 화면 왼쪽 상단 모서리에서 **필터 추가**&#x200B;를 클릭한 다음 **사용자 정의 양식**&#x200B;을 선택합니다.

   ![사용자 정의 양식 필터 선택](assets/select-custom-form-filter-350x271.png)

1. **검색** 필드에 최소 3자의 텍스트를 입력하여 원하는 사용자 정의 양식을 찾은 다음 사용자 정의 양식을 선택합니다.
1. 원하는 필드를 선택한 다음 필터에 추가할 필드 유형에 따라 다음 작업 중 하나를 완료합니다.

   >[!NOTE]
   >
   >일부 사용자 정의 corm 필드 유형은 필터에 추가할 수 없습니다. 현재 Enhanced Analytics에서는 아래에 나열된 필드 유형만 지원합니다.

   * **확인란**, **드롭다운** 또는 **라디오 단추**: 필터에 포함할 필드의 각 값을 선택하거나 **모두 선택** 확인란을 클릭합니다.\
     ![확인란 값](assets/custom-form-filter-checkbox-350x255.png)

   * **날짜**: 화살표를 사용하여 특정 월로 이동한 다음 필터에 포함할 필드에서 날짜를 선택합니다.\
     ![날짜 값](assets/custom-form-filter-date-350x348.png)

   * **텍스트**: 필터에 포함할 필드 내에 텍스트를 입력합니다.\
     ![텍스트 값](assets/custom-form-filter-text-350x90.png)

   * **숫자**: 필터에 포함할 필드 내의 숫자를 입력합니다.\
     ![숫자 값](assets/custom-form-filter-number-350x93.png)

1. 필터링할 값을 입력하거나 선택한 후 **필터 적용**&#x200B;을 클릭합니다.

   적용된 필터를 반영하도록 오른쪽 상단 업데이트에 프로젝트가 카운트됩니다.

1. 추가할 각 필터에 대해 이 단계를 반복합니다.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 아래 시각화에 표시됩니다.

   >[!TIP]
   >
   >기본적으로 표시되는 50개 이상의 프로젝트에 대한 데이터를 보려면 다음을 수행할 수 있습니다.
   >  
   >   * 왼쪽 하단의 화살표를 사용하여 해당 시각화에 있는 다음 50개의 프로젝트를 표시합니다.\
   >     ![페이지 매김 화살표](assets/pagination-350x118.png)
   >   
   >   * 시각화의 **정렬 기준** 드롭다운 메뉴를 사용하여 다른 순서로 프로젝트를 봅니다.\
   >     ![메뉴별 정렬](assets/sort-by-menu-350x247.png)

   날짜 범위를 조정하려면 [날짜 범위 필터 변경](#change-the-date-range-filter)을 참조하세요.

### 팀 필터 추가 {#add-a-team-filter}

{{step1-to-analytics}}

1. 왼쪽 패널에서 **사용자**&#x200B;를 클릭합니다.

   ![사람 선택](assets/people-area-cropped-qs-350x276.png)

1. 화면 왼쪽 상단에서 **필터 추가**&#x200B;를 클릭한 다음 **팀** 필터를 선택합니다.
1. **검색** 필드에 최소 3자의 텍스트를 입력하여 데이터를 보려는 팀을 찾은 다음 필터에 포함할 각 팀을 선택하십시오. 모든 팀을 선택하려면 **모두 선택**&#x200B;을 클릭하세요.

   ![팀 선택](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >액세스 수준에 관계없이 모든 팀이 필터 옵션으로 포함됩니다.

1. 원하는 팀을 모두 선택한 후 **필터 적용**&#x200B;을 클릭하세요.

   필터를 추가하면 아래의 시각화에 데이터가 표시됩니다.

   날짜 범위를 조정하려면 [날짜 범위 필터 변경](#change-the-date-range-filter)을 참조하세요.

## 필터 제거

언제든지 필터를 제거할 수 있습니다. 필터를 제거하면 다음에 고급 분석 영역을 방문할 때 필터가 표시되지 않습니다.

>[!TIP]
>
>키보드의 키를 사용하여 기존 필터로 이동하고 제거할 수도 있습니다.\
>자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md) 문서의 [키보드 단축키](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 섹션을 참조하십시오.

필터를 제거하려면 다음 작업을 수행하십시오.

{{step1-to-analytics}}

1. 프로젝트 필드 또는 사용자 지정 양식 필터를 제거하려면 **작업** 영역에 남아 있습니다.

   또는

   팀 필터를 제거하려면 왼쪽 패널에서 **사람**&#x200B;을(를) 선택하십시오.

1. 원하는 필터를 찾은 다음 **X**&#x200B;을(를) 클릭하여 제거합니다.

   ![제거](assets/remove-filter-350x213.png)

   필터가 더 이상 활성화되지 않으며 다시 추가하지 않으면 표시되지 않습니다.
