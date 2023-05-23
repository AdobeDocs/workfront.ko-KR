---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열에 있는 두 필드 간의 계산 결과 표시'
description: 열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 보기: 열에 있는 두 필드 간의 계산 결과를 표시합니다

열에서 텍스트 모드를 사용하여 두 필드 간의 계산을 표시할 수 있습니다.

예를 들어 두 날짜 사이에 경과된 주 일수를 확인하려면 텍스트 모드 구문과 데이터 표현식을 사용하여 이 차이를 계산할 수 있습니다.\
예를 들어 작업의 계획된 완료 일자와 실제 완료 일자 간의 요일 차이를 계산하고 결과를 열에 표시할 수 있습니다.

이 계산에서 다른 두 일자(실제 시작, 실제 완료, 예상 시작, 예상 완료 등)를 사용할 수 있습니다.\
계산된 데이터 표현식에 대한 자세한 내용은 [계산된 데이터 표현식](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>보기 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 열에 있는 두 필드 간의 계산 결과 표시

이 열을 작업 보기에 추가하려면 다음 작업을 수행하십시오.

1. 작업 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기**.

1. 클릭 **열 추가**, 그런 다음 **텍스트 모드로 전환**.

1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 에서 찾은 텍스트 제거 **텍스트 모드** 확인란을 선택하고 다음 코드로 바꿉니다.
   <pre>displayname=요일 차이<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (선택 사항) 그룹화에서 보기에 표시된 값을 집계하려면 다음에 설명된 단계를 수행합니다 [그룹화: 그룹화에 있는 여러 계산된 값을 집계한 결과를 표시합니다.](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. 클릭 **저장**, 그런 다음 **보기 저장**.
