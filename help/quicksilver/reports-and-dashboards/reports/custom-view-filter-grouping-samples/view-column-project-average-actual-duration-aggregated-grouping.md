---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기 및 그룹화: 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시'
description: 프로젝트 보고서에 다음 열을 추가하여 그룹화에서 평균으로 집계된 실제 기간을 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 보기 및 그룹화: 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시

<!--Audited: 11/2024-->

프로젝트 보기에 다음 열을 추가하여 그룹화의 평균으로 집계된 실제 기간을 표시할 수 있습니다.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 그룹화의 평균으로 집계된 프로젝트 실제 기간 표시

이 열을 프로젝트 보기에 추가하려면 다음 작업을 수행하십시오.

1. 프로젝트 목록으로 이동합니다.
1. (필수) 프로젝트의 실제 기간에 대한 집계된 평균 값을 보려면 프로젝트 목록에 그룹이 추가되어 있어야 합니다.\
   그룹화 만들기에 대한 자세한 내용은 문서 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.
1. **보기** 드롭다운 메뉴를 확장하고 **보기 사용자 지정**&#x200B;을 선택합니다.
1. **열 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 모든 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 보기 이름을 업데이트한 다음 **보기 저장**&#x200B;을 클릭합니다.
