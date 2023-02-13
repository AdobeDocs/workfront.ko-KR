---
product-area: projects;templates
navigation-topic: plan-a-project
title: 프로젝트 또는 템플릿에 대한 자원 관리자 지정
description: 프로젝트에 대한 자원 관리자를 지정하여 프로젝트의 자원 관리를 담당하는 사람을 표시할 수 있습니다.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# 프로젝트 또는 템플릿에 대한 자원 관리자 지정

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

프로젝트에 대한 자원 관리자를 지정하여 프로젝트의 자원 관리를 담당하는 사람을 표시할 수 있습니다. 정보 필드이며 리소스 관리 도구에 연결되어 있지 않습니다.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>프로젝트 및 템플릿에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 또는 템플릿에 대한 권한 관리</p>

<p><b>메모</b>

프로젝트나 템플릿에 리소스 관리자로 추가된 사용자는 프로젝트 또는 템플릿에 대한 관리 권한을 즉시 얻게 됩니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 리소스 관리자에 대한 고려 사항

>[!NOTE]
>
>리소스 관리자가 작업 역할이 아닙니다. 수동으로 업데이트할 수 있는 프로젝트 또는 템플릿에서 사용할 수 있는 필드입니다.

* 개별 프로젝트 또는 템플릿에 대해 최대 30명의 사용자를 리소스 관리자로 지정할 수 있습니다.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* 팀이나 그룹을 리소스 관리자로 지정할 수 없습니다. 사용자를 리소스 관리자로 지정할 수만 있습니다.

* 프로젝트 또는 템플릿에서 리소스 관리자로 지정하는 사용자는 자동으로 프로젝트 팀의 일부가 되지 않습니다.

   프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 관리](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* 프로젝트 또는 프로젝트 템플릿에 대해 자원 관리자를 지정할 수 있습니다. 프로젝트 템플리트에서 자원 관리자를 지정하면 템플리트에서 자원 관리자로 지정하는 모든 사용자는 해당 템플리트를 사용하여 생성된 모든 프로젝트에 대해 자동으로 자원 관리자가 됩니다.
* 다음 영역에서 리소스 관리자 필드를 볼 수 있습니다.

   * 이 문서에 설명된 대로 프로젝트를 편집할 때
   * 이 문서에 설명된 대로 템플릿을 편집할 때
   * 프로젝트 또는 템플릿 보고서를 작성할 때. 보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * 목록에 대한 프로젝트 또는 템플릿 보기를 만들거나 사용자 지정할 때. 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* 목록 또는 프로젝트 보기에 리소스 관리자 필드를 추가하고 인라인 편집을 사용하여 이 필드를 편집하여 여러 프로젝트 또는 템플릿에 리소스 관리자를 신속하게 추가하거나 제거할 수 있습니다.

## 프로젝트에 대한 자원 관리자 지정

1. 다음 중 하나를 수행합니다.

   * 단일 프로젝트에 리소스 관리자를 추가하려면, 하나 이상의 리소스 관리자를 지정할 프로젝트로 이동한 다음 **추가 메뉴** 프로젝트 이름 옆에 **편집 .**

   * 여러 프로젝트에 리소스 관리자를 동시에 추가하려면 프로젝트 목록으로 이동한 후 하나 이상의 리소스 관리자를 지정할 프로젝트를 선택한 다음 **편집**.

      기존 리소스 관리자는 편집 중인 프로젝트에서 제거되지 않습니다. 이러한 방식으로 추가하는 모든 사용자는 기존 리소스 관리자 외에도 프로젝트의 리소스 관리자로 추가됩니다.

   * 새 프로젝트에 리소스 관리자를 추가하려면 새 프로젝트 만들기를 시작합니다.

      프로젝트 만들기에 대한 내용은 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md).

1. 에서 **개요** 프로젝트 편집 대화 상자의 섹션에서 **리소스 관리자** 필드.
1. 프로젝트의 리소스 관리자로 추가하려는 사용자의 이름을 입력하고 목록에 이 이름이 표시되면 이름을 클릭합니다.

   이 단계를 반복하여 프로젝트에 대한 여러 리소스 관리자를 추가합니다.

1. 클릭 **변경 내용 저장**.

## 템플릿에 대한 자원 관리자 지정

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **템플릿**.

1. 다음 중 하나를 수행합니다.

   * 단일 템플릿에 리소스 관리자를 추가하려면 하나 이상의 리소스 관리자를 지정할 템플릿으로 이동한 다음 **추가 메뉴** 템플릿 이름 옆에 **편집 .**

   * 여러 템플릿에 리소스 관리자를 동시에 추가하려면 템플릿 목록으로 이동하여 하나 이상의 리소스 관리자를 지정할 템플릿을 선택한 다음 **편집**.

      기존 리소스 관리자는 편집 중인 템플릿에서 제거되지 않습니다. 이러한 방식으로 추가하는 모든 사용자는 기존 리소스 관리자 외에도 템플릿에 리소스 관리자로 추가됩니다.

   * 새 템플릿에 리소스 관리자를 추가하려면 **새 템플릿**&#x200B;를 클릭한 다음 **추가 메뉴** 템플릿 이름 옆에 **편집 .**

1. 에서 **개요** 섹션에서 **리소스 관리자** 필드.
1. 템플릿의 리소스 관리자로 추가할 사용자의 이름을 입력하고 목록에 이 이름이 표시되면 이름을 클릭합니다.

   템플릿에 여러 리소스 관리자를 추가하려면 이 단계를 반복합니다.

1. 클릭 **변경 내용 저장**.
