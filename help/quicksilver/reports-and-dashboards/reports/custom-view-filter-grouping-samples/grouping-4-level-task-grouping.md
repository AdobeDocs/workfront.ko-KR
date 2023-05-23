---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화'
description: 이 작업 그룹화는 4가지 수준의 그룹화를 제공합니다. 이 경우 작업은 Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태별로 그룹화됩니다. 표준 인터페이스를 사용하여 최대 3개의 그룹화 수준만 가질 수 있습니다. 네 번째 수준을 추가하려면 텍스트 모드를 사용해야 합니다. 보고서를 동시에 4개 이상의 기준으로 그룹화할 수 없습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 그룹화: Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화

이 작업 그룹화는 4가지 수준의 그룹화를 제공합니다. 이 경우 작업은 Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태별로 그룹화됩니다. 표준 인터페이스를 사용하여 최대 3개의 그룹화 수준만 가질 수 있습니다. 네 번째 수준을 추가하려면 텍스트 모드를 사용해야 합니다. 보고서를 동시에 4개 이상의 기준으로 그룹화할 수 없습니다.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>그룹화 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 그룹화 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Portfolio 소유자, 프로그램 소유자, 프로젝트 소유자 및 프로젝트 상태에 대한 4단계 작업 그룹화 만들기

이 그룹화를 적용하려면:

1. 작업 목록으로 이동합니다.
1. 다음에서 **그룹화** 드롭다운 메뉴에서 다음을 선택합니다. **새 그룹화**.

1. 클릭&#x200B;**텍스트 모드로 전환**.
1. 에서 텍스트 제거 **보고서 그룹화** 영역입니다.
1. 텍스트를 다음 코드로 바꿉니다.

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio 소유자<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgroupingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. 클릭 **그룹화 저장**.
