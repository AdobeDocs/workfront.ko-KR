---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 프로젝트 스폰서 수 시간'
description: 이 시간 그룹화는 시간이 기록되는 프로젝트의 스폰서별로 시간을 구성합니다. 시간 그룹화에 대한 표준 Report Builder 인터페이스는 프로젝트 스폰서 필드에 대한 매핑을 제공하지 않습니다. 이 필드에 액세스하려면 텍스트 모드 인터페이스를 사용해야 합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 그룹화: 프로젝트 스폰서 수 시간

이 시간 그룹화는 시간이 기록되는 프로젝트의 스폰서별로 시간을 구성합니다. 시간 그룹화에 대한 표준 Report Builder 인터페이스는 프로젝트 스폰서 필드에 대한 매핑을 제공하지 않습니다. 이 필드에 액세스하려면 텍스트 모드 인터페이스를 사용해야 합니다.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 몇 시간 동안 프로젝트 후원자별 그룹

이 그룹을 적용하려면

1. 시간 목록으로 이동합니다.
1. 에서 **그룹화** 드롭다운 메뉴에서 **새 그룹화**.

1. 클릭&#x200B;**텍스트 모드로 전환**.
1. 에서 텍스트 제거 **보고서 그룹화** 영역.

1. 텍스트를 다음 코드로 바꿉니다.

   <pre>group.0.linkedname=project:sponsor:이름<br>group.0.name=<br>group.0.valuefield=project:sponsor:이름<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. 클릭 **그룹화 저장**.
