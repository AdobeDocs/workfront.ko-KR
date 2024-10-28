---
content-type: reference
product-area: reporting;projects
keywords: 계산,집계,고급,보기
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 그룹화에 있는 여러 계산된 값을 집계한 결과를 표시합니다.'
description: 열에서 텍스트 모드를 사용하여 보고서나 목록 보기에서 두 필드 간의 계산을 표시할 수 있습니다. 각 행은 보고서나 목록의 각 객체에 대한 계산을 표시합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 그룹화: 그룹화에 있는 여러 계산된 값을 집계한 결과를 표시합니다.

<!--Audited: 10/2024-->

열에서 텍스트 모드를 사용하여 보고서나 목록 보기에서 두 필드 간의 계산을 표시할 수 있습니다. 각 행은 보고서나 목록의 각 객체에 대한 계산을 표시합니다.

예를 들어 작업 보고서의 각 작업에 대한 작업 균형이라는 세 번째 열에 실제 시간과 계획된 시간 간의 차이를 표시할 수 있습니다. 계산된 데이터 식에 대한 자세한 내용은 [계산된 데이터 식의 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

계산된 값을 포함하는 열의 `aggregator` 행에 계산을 추가하여 그룹화된 동일한 열에 있는 여러 계산된 보기 항목의 집계된 값을 표시할 수 있습니다. 예를 들어, 보고서 그룹이나 작업 균형 열의 목록에서 모든 작업의 작업 균형 시간을 집계(합계를 표시)할 수 있습니다. 이 문서에서는 이 작업을 수행하는 방법에 대해 설명합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹화에 여러 계산된 값을 집계한 결과 표시

1. 작업 보고서로 이동하여 **보고서 작업** > **편집**&#x200B;을 클릭하세요.
1. **그룹화** 탭에서 **그룹화 추가**&#x200B;를 클릭하고 **그룹화 기준** 필드에 **프로젝트 이름**&#x200B;을 입력한 다음 목록에 표시될 때 **프로젝트 > 이름**&#x200B;을 선택합니다.

1. **열(보기)** 탭에서 **열 추가**&#x200B;를 클릭하고 **이 열에 표시** 필드에 **계획된 시간**&#x200B;을 입력한 다음 목록에 표시될 때 선택합니다.

   >[!TIP]
   >
   >텍스트 모드에서 정보를 편집하기 전에 항상 표준 인터페이스를 사용하여 많은 정보를 추가하십시오. 계산하려는 정보에 가장 가깝거나 가장 많은 정보가 포함된 필드를 추가합니다.

1. **이 열을**(으)로 요약 필드에서 **합계**&#x200B;를 선택합니다.
1. 추가한 열에서 **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 상자의 텍스트를 다음 텍스트 모드 예제로 바꿉니다.

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >그룹화에서 집계된 값을 가져와서 계획된 시간과 실제 시간 필드 간의 집계된 차이를 표시하려면 `aggregator.valuefield` 줄에 동일한 방정식을 입력하십시오. 계획된 시간 열에 사용된 `aggregator.displayformat`은(는) 분을 시간으로 변환합니다. 계획된 시간 필드가 자리 표시자로 사용되었기 때문에 이 줄을 조정할 필요가 없습니다.
   >
   >
   >`aggregator.displayformat` 줄의 `minutesAsHoursString` 정의는 결과를 위해 `valueexpression`에 대해 수행한 대로 각 필드를 60으로 나눌 필요가 없음을 의미합니다. 이 `aggregator.valuefield=workRequired`에서 `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`이(가) 됩니다.
1. **완료**&#x200B;를 클릭합니다.
1. **저장+닫기**&#x200B;를 클릭합니다.
