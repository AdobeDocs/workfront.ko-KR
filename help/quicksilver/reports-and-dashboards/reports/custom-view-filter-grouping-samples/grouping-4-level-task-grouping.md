---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화'
description: 이 작업 그룹화는 4가지 수준의 그룹화를 제공합니다. 이 경우 작업은 Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태별로 그룹화됩니다. 표준 인터페이스를 사용하여 최대 3개의 그룹화 수준만 가질 수 있습니다. 네 번째 수준을 추가하려면 텍스트 모드를 사용해야 합니다. 보고서를 동시에 4개 이상의 기준으로 그룹화할 수 없습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 그룹화: Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화

<!--Audited: 10/2024-->

이 작업 그룹화는 4가지 수준의 그룹화를 제공합니다. 이 경우 작업은 Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태별로 그룹화됩니다. 표준 인터페이스를 사용하여 최대 3개의 그룹화 수준만 가질 수 있습니다. 네 번째 수준을 추가하려면 텍스트 모드를 사용해야 합니다. 보고서를 동시에 4개 이상의 기준으로 그룹화할 수 없습니다.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화 만들기

이 그룹화를 적용하려면:

1. 작업 목록으로 이동합니다.
1. **그룹화** 드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **보고서 그룹화** 영역에서 텍스트를 제거합니다.
1. 표시되는 상자의 텍스트를 다음 코드로 바꿉니다.
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio 소유자<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=프로그램 소유자<br>group.1.notime=false<br>group.1.valuefield=project:program:소유자:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgroupingparsedmethod=nested(project).owner(name)<br>group.2.namekey=projecterkey mm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. **완료**&#x200B;를 클릭한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
