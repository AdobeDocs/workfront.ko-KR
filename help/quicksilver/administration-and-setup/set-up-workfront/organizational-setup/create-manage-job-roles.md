---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 만들기 및 관리
description: ' [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# 작업 역할 만들기 및 관리

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다. [!DNL Workfront]의 관리 액세스에 대한 자세한 내용은 [특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>
   <p>새로운 기능: [!UICONTROL Standard]</p>
   <p>또는</p>
   <p>현재: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>작업 역할에 대한 관리 액세스</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 역할 만들기

작업 역할을 생성하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL &#x200B;작업 역할].**&#x200B;을 클릭합니다.
1. **[!UICONTROL 새 작업 역할]을 클릭합니다.**
1. 다음을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td> <p>작업 역할의 이름을 나타냅니다. [!UICONTROL 작업 역할] 필드가 표시되는 [!DNL Workfront]의 모든 위치에 표시되는 이름입니다. </p> <p>팁: 작업 역할의 이름은 최대 255자를 포함할 수 있습니다. 그러나 [!DNL Workfront]의 특정 영역에서는 더 긴 이름이 잘릴 수 있습니다. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>역할에 대한 고유한 사항을 나타내는 역할에 대한 설명을 입력합니다. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 이 활성 상태입니다]</span> </td> 
      <td> 
       <ul> 
        <li> <p>역할을 활성화하여 [!DNL Workfront]의 모든 곳에서 사용할 수 있도록 하여 사용자, 작업 항목 등과 연결하려면 <b>[!UICONTROL 예]</b>를 선택하십시오. </p> </li> 
        <li> <p>역할을 비활성화하고 사용자, 작업 항목 등에 할당할 수 없도록 하려면 <b>[!UICONTROL No]</b>을(를) 선택하십시오. </p> </li> 
       </ul> <p><span>작업 역할 비활성화에 대한 자세한 내용은 </span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">작업 역할 비활성화</a>를 참조하십시오. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 기본 통화]</span> </td> 
      <td> <p><span>Workfront 관리자가 [!UICONTROL 설정] 영역에서 설정한 [!UICONTROL 기본 통화]입니다. 자세한 내용은 </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a> 을 참조하십시오.</p> <p>팁: <span>작업 역할 수준에서 [!UICONTROL 기본 통화]를 편집할 수 없습니다. 이 필드는 흐리게 표시되어 시스템의 기본 통화에 대한 미리 알림 역할을 합니다.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 비용 비율]</td> 
      <td><p>작업 역할의 시간당 비용입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 비용과 궁극적으로 프로젝트의 계획 및 실제 비용을 계산합니다. [!UICONTROL 기본 통화]를 사용하여 환율을 입력합니다.</p> 
      <p>날짜 유효 비용 요율을 보려면 <strong>[!UICONTROL 추가 요금]</strong>을(를) 클릭하십시오. 기간에 대한 비용/시간 값을 입력하고 필요에 따라 [!UICONTROL 시작 날짜] 및 [!UICONTROL 종료 날짜]를 지정합니다. 첫 번째 원가에는 시작 일자가 없고 마지막 원가에는 종료 일자가 없습니다.</p> <p>일부 날짜는 자동으로 추가됩니다. 예를 들어, 첫 번째 원가율에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 두 번째 원가율을 추가하면, 종료 일자가 2023년 4월 30일인 첫 번째 원가율에 추가되므로 공백이 없습니다.</p> <p>팁: 기존 작업 역할을 편집할 때 <strong>시작 날짜별로 정렬</strong>을 선택하여 요금 목록 맨 위에 가장 최근 시작 날짜를 표시할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 청구 요금] </td> 
      <td><p>작업 역할의 시간당 청구 요금입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 수익과 궁극적으로 프로젝트의 계획 및 실제 수익을 계산합니다. [!UICONTROL 기본 통화]를 사용하여 환율을 입력합니다.</p> <p>날짜 유효 청구 요금을 보려면 <strong>[!UICONTROL 추가 요금]</strong>을(를) 클릭하십시오. 해당 기간에 대한 청구/시간 값을 입력하고 필요에 따라 [!UICONTROL 시작 날짜] 및 [!UICONTROL 종료 날짜]를 지정합니다. 첫 번째 청구 요금에 시작 일자가 없고 마지막 청구 요금에 종료 일자가 없습니다.</p> <p>일부 날짜는 자동으로 추가됩니다. 예를 들어 첫 번째 청구 요금에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 두 번째 청구액을 추가한 경우, 간격이 없도록 종료 일자가 2023년 4월 30일인 첫 번째 청구 요금에 추가됩니다.</p> <p>팁: 기존 작업 역할을 편집할 때 <strong>시작 날짜별로 정렬</strong>을 선택하여 요금 목록 맨 위에 가장 최근 시작 날짜를 표시할 수 있습니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 통화 재정의]</span> </td> 
      <td>
        <p>이 작업 역할과 연결된 통화를 선택합니다. [!DNL Workfront]이(가) 이 작업 역할과 연결된 비용 및 수익을 계산하는 데 사용하는 통화입니다. </p> 
        <p><span>이는 [!DNL Workfront] 관리자가 [!UICONTROL Setup] 영역에서 설정한 [!UICONTROL 기본 통화]와 다르며 프로젝트와 관련된 통화와 다를 수 있습니다.</span> </p> 
        <p>팁: 시스템의 [!UICONTROL 환율] 영역에서 사용할 수 있는 통화만 이 필드에서 사용할 수 있습니다. 통화를 하나만 설정한 경우 이 필드가 표시되지 않습니다.</p> 
       <p><span>[!DNL Workfront]에서 [!UICONTROL 기본 통화] 설정에 대한 자세한 내용은 </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>을 참조하십시오.</p> <p><span>프로젝트 통화 변경에 대한 자세한 내용은 </span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">프로젝트 통화 변경</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 통화 비용 대체]</span> </td> 
      <td>
        <p>선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 비용입니다. [!DNL Workfront]은(는) 이 값을 사용하여 작업 역할과 관련된 작업 및 문제의 계획된 비용과 실제 비용을 계산합니다. </p> 
        <p><span>위에 지정된 [!UICONTROL Override Currency]에 환율을 입력합니다. [!UICONTROL 기본 통화]를 사용할 때 이 작업 역할의 비용률도 업데이트합니다.</span> </p> 
        <p>[!DNL Workfront]이(가) 비용을 계산하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>을 참조하십시오.</p> 
       <p>팁: 비용 환율이 이미 연결되어 있는 기존 작업 역할을 업데이트할 때 [!DNL Workfront]은(는) 시스템의 전환율을 기반으로 [!UICONTROL 통화 재정의] 환율을 계산합니다. [!UICONTROL 통화 대체 비용 비율]을 업데이트하면 작업 역할의 비용 비율도 자동으로 업데이트됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 통화 청구 요금 재정의]</span> </td> 
      <td>
        <p>선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 청구 요금입니다. [!DNL Workfront]은(는) 이 값을 사용하여 작업 역할과 관련된 작업 및 문제의 계획 및 실제 매출을 계산합니다. </p>
        <p><span>위에 지정된 [!UICONTROL Override Currency]에 환율을 입력합니다. 또한 [!UICONTROL 기본 통화]를 사용할 때 이 작업 역할에 대한 청구 요금이 업데이트됩니다.</span> </p>
        <p>[!DNL Workfront]이(가) 수익을 계산하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>를 참조하십시오.</p>
        <p>팁: 청구 요금이 이미 연결되어 있는 기존 작업 역할을 업데이트할 때 [!DNL Workfront]은(는) 시스템의 전환율을 기반으로 통화 재정의 요금을 계산합니다. 통화 대체 청구 단가를 갱신하면 작업 역할의 청구 단가도 자동으로 갱신됩니다. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >작업 역할은 리소스 관리의 필수적인 부분입니다. 자원 계획 도구를 사용하려면 작업 역할에 연관된 비용 및 청구 요금이 필요합니다. 자세한 내용은 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)을 참조하세요.

1. **[!UICONTROL 작업 역할 만들기]**&#x200B;를 클릭합니다. 이제 작업 역할을 작업, 문제, 승인에 할당하거나 레이아웃 템플릿 또는 다른 개체를 공유할 수 있습니다. [!DNL Workfront]의 모든 작업 역할 사용에 대한 자세한 내용은 [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)를 참조하십시오. 작업 역할 삭제에 대한 자세한 내용은 [작업 역할 삭제](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)를 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
