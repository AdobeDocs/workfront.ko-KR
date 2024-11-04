---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열에 있는 두 필드 간의 계산 결과 표시'
description: 열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 보기: 열에 있는 두 필드 간의 계산 결과를 표시합니다

<!--Audited: 11/2024-->

열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.

예를 들어 두 날짜 사이에 경과된 주 일수를 확인하려면 텍스트 모드 구문과 데이터 표현식을 사용하여 이 차이를 계산할 수 있습니다.\
예를 들어 작업의 계획된 완료 일자와 실제 완료 일자 간의 요일 차이를 계산하고 결과를 열에 표시할 수 있습니다.

이 계산에서 다른 두 일자(실제 시작, 실제 완료, 예상 시작, 예상 완료 등)를 사용할 수 있습니다.\
계산된 데이터 식에 대한 자세한 내용은 [계산된 데이터 식의 개요](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

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


## 열에 있는 두 필드 간의 계산 결과 표시

이 열을 작업 보기에 추가하려면 다음 작업을 수행하십시오.

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭합니다.

1. **열 추가**&#x200B;를 클릭한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (선택 사항) 그룹화에서 보기에 표시된 값을 집계하려면 [그룹화에 설명된 단계를 따릅니다. 그룹화에서 여러 계산된 값을 집계한 결과를 표시합니다](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
