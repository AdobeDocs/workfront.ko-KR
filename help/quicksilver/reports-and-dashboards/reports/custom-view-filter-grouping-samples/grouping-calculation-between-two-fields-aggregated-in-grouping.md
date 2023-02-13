---
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 그룹화''에서 여러 계산된 값을 합산한 결과 표시'
description: 열에서 텍스트 모드를 사용하여 보고서나 목록 보기에서 두 필드 사이의 계산을 표시할 수 있습니다. 각 행은 보고서나 목록의 각 객체에 대한 계산을 표시합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 그룹화: 그룹화에서 여러 계산된 값을 합산한 결과 표시

열에서 텍스트 모드를 사용하여 보고서나 목록 보기에서 두 필드 사이의 계산을 표시할 수 있습니다. 각 행은 보고서나 목록의 각 객체에 대한 계산을 표시합니다.

예를 들어, 작업 보고서의 각 작업에 대한 작업 밸런스라는 세 번째 열에 실제 시간과 계획 시간 간의 차이를 표시할 수 있습니다. 계산된 데이터 표현식에 대한 자세한 내용은 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

그룹에 계산을 추가하여 여러 계산된 뷰 항목의 합계값을 그룹핑의 동일한 열에 표시할 수 있습니다 `aggregator` 계산된 값이 들어 있는 열의 행입니다. 예를 들어, 보고서 그룹핑 또는 작업 잔액 열에 대한 목록의 모든 작업의 작업 잔액 시간 금액을 합계(합계 표시)할 수 있습니다. 이 문서에서는 이 작업을 수행하는 방법을 설명합니다.

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

## 그룹화에서 여러 계산된 값을 집계한 결과 표시

1. 작업 보고서로 이동하여 **보고서 작업** > **편집**.
1. 에서 **그룹화** 탭, **그룹화 추가**, 입력 시작 **프로젝트 이름** 에서 **보고서 그룹화** > **먼저** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

1. 에서 **열(보기)** 탭, **열 추가**&#x200B;를 입력한 다음 입력을 시작합니다. **계획 시간** 에서 **이 열에 표시** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

   >[!TIP]
   >
   >텍스트 모드에서 정보를 편집하기 전에 항상 표준 인터페이스를 사용하여 많은 정보를 추가합니다. 계산과 가장 가까운 정보이거나 들어 있는 필드를 추가하세요.

1. 에서 **다음 방법으로 이 열 요약** 필드, 선택 **합계**&#x200B;를 클릭한 다음 **완료**.
1. 클릭 **텍스트 모드로 전환** 을 입력합니다.
1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 바꾸기 `valuefield ` 그리고 `aggregator.valuefield` 다음 텍스트 모드 예에서 강조 표시된 줄이 있는 선:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >그룹핑에서 총괄된 값을 가져와서 계획된 시간과 실제 시간 필드 간의 총괄된 차이를 표시하려면 동일한 방정식을 `aggregator.valuefield` 줄. 다음 `aggregator.displayformat` 계획 시간 열에 사용되는 는 분을 시간으로 변환합니다. 계획 시간 필드가 자리 표시자로서 사용되었으므로 이 줄을 조정할 필요가 없습니다.
   >
   >
   >다음 `minutesAsHoursString` 의 정의 `aggregator.displayformat` 선은 각 필드에 대해 수행한 대로 각 필드를 60으로 나눌 필요가 없음을 의미합니다 `valueexpression` 참조하십시오. 이 `aggregator.valuefield=workRequired` 다음과 같이 바꿉니다. `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. 클릭 **저장+닫기**.
