---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 프로젝트 비율 분류 1'
description: 이 사용자 지정 프로젝트 그룹화에서는 완료율 값 범위별로 그룹화된 프로젝트를 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---

# 그룹화: 프로젝트 비율 분류 1

이 사용자 지정 프로젝트 그룹화에서는 완료율 값 범위별로 그룹화된 프로젝트를 표시할 수 있습니다.

다음 그룹화는 완료율 값을 기준으로 프로젝트를 다음 그룹 중 하나로 구성합니다.

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![percent_complete_breakdown_custom_project_grouping_25__increments.png](assets/percent-complete-breakdown-custom-350x56.png)

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

## 프로젝트 백분율 분류별로 그룹화

이 그룹을 적용하려면

1. 프로젝트 목록으로 이동합니다.
1. 에서 **그룹화** 드롭다운 메뉴에서 **새 그룹화**.

1. 클릭 **텍스트 모드로 전환**.
1. 상자에서 텍스트를 제거하고 사용 가능한 공간에 다음 코드를 붙여 넣습니다.
   <pre>group.0.linkedname=direct<br>group.0.name=백분율 분류<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0%",IF({percentComplete}&lt;=26,"0-25%",IF({percentComplete}&lt;=51,"25-50%",IF({percentComplete}&lt;=76,"50-75%",IF({percentComplete}&lt;1000,"75-99%",")%) %)<br>group.0.valueformat=string</pre>

1. 클릭 **그룹화 저장**.
