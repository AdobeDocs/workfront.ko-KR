---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기 및 그룹화: 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시'
description: 프로젝트 보고서에 다음 열을 추가하여 그룹화에서 평균으로 집계된 실제 기간을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 보기 및 그룹화: 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시

프로젝트 보고서에 다음 열을 추가하여 그룹화에서 평균으로 집계된 실제 기간을 표시할 수 있습니다.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시

이 열을 프로젝트 보기에 추가하려면 다음 작업을 수행하십시오.

1. (권장) 최상의 결과를 얻고 실제 기간 의 집계된 평균 값을 보려면 프로젝트 목록 또는 보고서에 그룹화가 추가되어 있어야 합니다.\
   그룹화 만들기에 대한 자세한 내용은 문서 를 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 기존 프로젝트 보기로 이동합니다.
1. 보기 드롭다운 메뉴를 확장하고 을(를) 선택합니다. **보기 맞춤화**.
1. 클릭 **열 추가**.
1. 클릭 **텍스트 모드로 전환**.
1. 마우스를 위에 놓기 **이 열에 표시** 영역 및 클릭 **텍스트를 편집하려면 클릭**.

1. 텍스트 모드 상자에서 모든 텍스트를 제거하고 다음 코드로 대체합니다.

   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=프로젝트 실제 기간 <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinute <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. 클릭 **보기 저장**.
