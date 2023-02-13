---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Adobe Workfront의 예산 리소스에 대한 액세스 필요
description: 특정 액세스 수준 설정과 작업 항목, 사용자, 작업 역할 및 팀에 대한 권한이 있을 때 볼 수 있는 액세스 권한이 있는 프로젝트의 리소스 계획에 대한 정보를 보고 관리할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Adobe Workfront의 예산 리소스에 대한 액세스 필요

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

회사에서 Resource Planning이 포함된 Adobe Workfront 라이센스를 구입한 경우 조회할 권한이 있는 프로젝트에 대한 리소스 예산 책정 정보를 볼 수 있습니다. 자원 계획자에서 예산 정보를 볼 수 있습니다.

Workfront에서 예산 책정 도구를 사용하기 위한 사전 요구 사항에 대한 자세한 내용은 다음을 참조하십시오 [리소스 계획 시작](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

자원 예산을 책정하려면 자원 풀을 관리하고 자원 계획 도구에서 비용 정보를 참조하며 회사 및 사용자에게 다음 액세스 권한이 있어야 합니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 
    <ul> 
     <li> <p>다음을 포함하는 액세스 수준에서 리소스 관리에 대한 액세스를 편집합니다.</p> 
      <ul> 
       <li> <p>프로젝트 우선순위 및 예산 시간을 편집할 수 있는 액세스 권한. </p> </li> 
       <li> <p>리소스 풀을 관리해야 하는 경우 리소스 풀을 관리하기 위한 액세스 권한</p> </li> 
      </ul> <p>리소스 관리 액세스 수준에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">리소스 관리에 대한 액세스 권한 부여</a>.</p> </li> 
     <li> <p>프로젝트 및 사용자에 대한 액세스를 편집합니다. </p> </li> 
     <li> <p> 비용별로 정보를 보거나 관리해야 하는 경우 액세스 레벨에서 재무 데이터에 대한 액세스를 편집합니다.</p> <p>재무 데이터 액세스 수준에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</p> </li> 
    </ul>

<p><b>메모</b> </p>

<p> 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 권한이 포함된 프로젝트의 권한을 관리합니다.</p> <p>프로젝트 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>프로젝트에 대한 재무 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">개체에 대한 재무 권한 공유</a></a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">개체에 대한 액세스 요청 </a>.</p>

<p><b>메모</b>

역할 뷰에서 자원 예산을 책정할 때 역할 아래에 나열된 하나 이상의 프로젝트에 대한 관리 권한보다 작으면 역할에 대해 시간, FTE 또는 비용을 예측할 수 없습니다. 관리 권한이 있는 프로젝트에만 예산을 지정할 수 있습니다.</p> </td>
</tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.
