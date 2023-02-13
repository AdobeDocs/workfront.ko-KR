---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 열에 있는 두 필드 사이의 계산 결과 표시'
description: 열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 보기: 열에 있는 두 필드 사이의 계산 결과 표시

열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.

예를 들어, 두 날짜 사이에 경과된 주 일수를 찾으려면 텍스트 모드 구문과 데이터 표현식을 사용하여 이 차이를 계산할 수 있습니다.\
예를 들어, 작업의 계획 완료 일자와 실제 완료 일자 간의 주 일자 차이를 계산하고 결과를 열에 표시할 수 있습니다.

이 계산에서 다른 두 일자(실제 시작, 실제 완료, 예상 시작, 예상 완료 등)를 사용할 수 있습니다.\
계산된 데이터 표현식에 대한 자세한 내용은 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

## 열에 있는 두 필드 사이의 계산 결과 표시

이 열을 작업 보기에 추가하려면 다음을 수행합니다.

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 클릭 **열 추가**, 그런 다음 **텍스트 모드로 전환**.

1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.
   <pre>displayname=주간 차이<br>textmode=true<br>valueexpression=WEEKDAYDIFF({planningCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (선택 사항) 그룹화된 보기에서 표시된 값을 집계하려면 [그룹화: 그룹화에서 여러 계산된 값을 합산한 결과 표시](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. 클릭 **저장**, 그런 다음 **보기 저장**.
