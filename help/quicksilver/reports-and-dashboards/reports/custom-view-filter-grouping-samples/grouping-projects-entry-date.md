---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 입력 날짜별 프로젝트'
description: 이 사용자 정의 프로젝트 그룹에서는 시작 날짜 값으로 그룹화된 프로젝트를 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 그룹화: 입력 날짜별 프로젝트

이 사용자 정의 프로젝트 그룹에서는 시작 날짜 값으로 그룹화된 프로젝트를 표시할 수 있습니다.

각 그룹에는 시작 일자가 다음 범위 내에 있는 프로젝트가 표시됩니다.

* 지난 30일
* 30-60일
* 60일 이상

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

## 입력 날짜별로 프로젝트 그룹화

이 그룹화를 적용하려면:

1. 기존 프로젝트 보고서로 이동하거나 새 프로젝트 보고서를 만듭니다.\
   보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.
1. **보고서 동작** > **편집**&#x200B;을 클릭합니다.
1. **그룹화** 탭에서 **그룹화 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **그룹화 기준** 영역에서 텍스트를 제거합니다.
1. 텍스트를 다음 코드로 바꿉니다.

   group.0.linkedname=direct
group.0.name=프로젝트 시작
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))&lt;=30,&quot;최근 30일&quot;,IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&amp;&amp;ABS(DATEDIFF({entryDate},$$TODAY))&lt;=60,&quot;30-60일&quot;,&quot;60일 이상&quot;)
group.0.valueformat=atDateAsMonthString
textmode=true

1. **완료** > **그룹화 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
