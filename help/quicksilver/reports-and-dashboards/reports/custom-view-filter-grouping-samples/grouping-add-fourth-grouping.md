---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 목록에 네 번째 그룹화 추가'
description: 매트릭스 보고서에 4개의 그룹화를 포함할 수 있습니다. 행렬 보고서에 대한 자세한 내용은 행렬 보고서 만들기 를 참조하십시오.
author: Courtney
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---

# 그룹화: 목록에 네 번째 그룹화 추가

<!--Audited: 10/2024-->

매트릭스 보고서에 4개의 그룹화를 포함할 수 있습니다. 행렬 보고서에 대한 자세한 내용은 [행렬 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)를 참조하십시오.

표준 인터페이스를 통해 표준 보고서에는 3개의 그룹화만 있을 수 있습니다. 표준 보고서에 네 번째 그룹화를 추가하려면 텍스트 모드를 사용해야 합니다.

![Four_groupings_in_a_standard_report.png](assets/four-tier-grouping-for-tasks-350x239.png)

예를 들어 프로젝트 이름, 진행 상태 및 계획 완료 날짜별로 그룹화된 작업 보고서가 있을 수 있지만 할당 대상 이름별로 보고서를 그룹화하려는 경우도 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스</td> 
   <td> 
   <p>참여자 또는 필터 수정 요청 </p>
   <p>표준 또는 계획: 보고서 수정</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스를 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표에 있는 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 목록에 네 번째 그룹화 추가

네 번째 그룹화를 추가하려면 다음을 수행합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **보고서를 그룹화** 영역에서 텍스트를 제거합니다.
1. 표시되는 상자의 텍스트를 다음 코드로 바꿉니다.

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. **완료**&#x200B;를 클릭한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 그룹화 이름을 업데이트한 후 **그룹화 저장**&#x200B;을 클릭합니다.
