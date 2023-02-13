---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 만들기 및 관리
description: 로서의 [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리자 액세스 권한이 있는 사용자는 사용자에게 지정할 수 있는 작업 역할을 만들고 해당 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 작업 역할 만들기 및 관리

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

로서의 [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리자 액세스 권한이 있는 사용자는 사용자에게 지정할 수 있는 작업 역할을 만들고 해당 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다. 의 관리 액세스에 대한 자세한 내용 [!DNL Workfront]를 참조하십시오. [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 역할에 대한 관리자 액세스</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 역할 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 을 클릭합니다&#x200B;. **[!UICONTROL 작업 역할].**
1. 클릭 **[!UICONTROL 새 작업 역할].**
1. 다음을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>작업 역할의 이름을 지정합니다. 이 이름은 [!DNL Workfront] 여기서 [!UICONTROL 작업 역할] 필드가 표시됩니다. </p> <p>팁: 작업 역할 이름은 최대 255자를 포함할 수 있습니다. 그러나 더 긴 이름은 [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL이 활성화되어 있음]</span> </td> 
      <td> 
       <ul> 
        <li> <p>선택 <b>[!UICONTROL Yes]</b> 역할을 활성화하여 [!DNL Workfront] 사용자, 작업 항목 등과 연결되어야 합니다. </p> </li> 
        <li> <p>선택 <b>[!UICONTROL No]</b>, 역할을 비활성화하고 사용자, 작업 항목 등에 할당할 수 없도록 하려면 . </p> </li> 
       </ul> <p><span>작업 역할 비활성화에 대한 자세한 내용은</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">작업 역할 비활성화</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>역할에 대한 고유한 내용을 나타내는 설명을 입력합니다. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 기본 통화]</span> </td> 
      <td> <p><span>Workfront 관리자가 [!UICONTROL 설정] 영역에 설정한 [!UICONTROL 기본 통화]입니다. 자세한 내용은</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a> .</p> <p>팁: <span>작업 역할 수준에서 [!UICONTROL 기본 통화]를 편집할 수 없습니다. 이 필드는 흐리게 표시되어 시스템에 대한 기본 통화가 무엇인지에 대한 미리 알림 역할을 합니다.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost/Hr.]</td> 
      <td>작업 역할의 시간당 비용입니다. 이 값은 역할과 연관된 태스크 및 문제의 계획 및 실제 원가, 궁극적으로 프로젝트의 계획 및 실제 원가를 계산합니다. <span>[!UICONTROL 기본 통화]를 사용하여 환율을 입력합니다.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Bill/ Hr.] </td> 
      <td>작업 역할의 시간당 청구 비율입니다. 이 값은 역할과 연관된 태스크 및 문제의 계획 및 실제 수익 및 프로젝트의 계획 및 실제 수익을 계산합니다. [!UICONTROL 기본 통화]를 사용하여 환율을 입력합니다. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td> 
       <div> 
        <p>이 작업 역할과 연결된 통화를 선택합니다. 이 통화는 [!DNL Workfront] 이 작업 역할과 연관된 비용 및 수익을 계산하는 데 사용됩니다. </p> 
        <p><span>이는 사용자가 설정한 [!UICONTROL 기본 통화]와 다릅니다 [!DNL Workfront] 관리자는 [!UICONTROL 설정] 영역에서 사용할 수 있으며, 프로젝트와 연결된 통화와 다를 수 있습니다.</span> </p> 
        <p>팁: 시스템의 [!UICONTROL 환율] 영역에서 사용할 수 있는 통화만 이 필드에서 사용할 수 있습니다.</p> 
       </div> <p><span>에서 [!UICONTROL 기본 통화] 설정에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오.</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>.</p> <p><span>프로젝트 통화 변경에 대한 자세한 내용은</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">프로젝트 통화 변경</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 통화 비용/시간 대체]</span> </td> 
      <td> 
       <div> 
        <p>선택한 [!UICONTROL Override Currency]를 사용하는 작업 역할의 시간당 비용입니다. [!DNL Workfront] 이 값을 사용하여 작업 역할과 연관된 작업 및 문제의 계획 및 실제 비용을 계산합니다. </p> 
        <p><span>위에 지정된 [!UICONTROL Override Currency]에 환율을 입력합니다. [!UICONTROL 기본 통화]를 사용할 때 이 작업 역할에 대한 비용/시간 비율도 업데이트됩니다.</span> </p> 
        <p>방법 [!DNL Workfront] 비용 계산 을 참조하십시오. <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> 
       </div> <p>팁: 이미 연관된 비용/시간 비율이 있는 기존 작업 역할을 업데이트할 때 [!DNL Workfront] 시스템의 전환율을 기반으로 [!UICONTROL 재정의 통화] 비율을 계산합니다. [!UICONTROL 대체 통화 비용/시간]을 업데이트하면 작업 역할의 비용/시간도 자동으로 업데이트됩니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
      <td> 
       <div> 
        <p>선택한 [!UICONTROL Override Currency]를 사용하는 작업 역할의 시간당 청구 비율입니다. [!DNL Workfront] 이 값을 사용하여 작업 역할과 연관된 작업 및 문제의 계획 및 실제 매출액을 계산합니다. </p> 
        <p><span>위에 지정된 [!UICONTROL Override Currency]에 환율을 입력합니다. [!UICONTROL 기본 통화]를 사용할 때 이 작업 역할에 대한 청구/시간 비율도 업데이트됩니다.</span> </p> 
        <p>방법 [!DNL Workfront] 매출 계산 을 참조하십시오. <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</p> 
       </div> <p>팁: 이미 연관된 청구/시간 비율이 있는 기존 작업 역할을 갱신할 때, [!DNL Workfront] 시스템의 전환율을 기반으로 대체 통화 환율을 계산합니다. 대체 통화 청구/시간을 갱신하면 작업 역할의 청구/시간도 자동으로 업데이트됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >작업 역할은 리소스 관리의 필수적인 부분입니다. 자원 계획 도구를 사용하려면 작업 역할에 비용 및 과금이 연관되어 있어야 합니다. 자세한 내용은 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. 클릭 **[!UICONTROL 작업 역할 만들기]**. 이제 작업 역할을 작업, 문제, 승인 또는 작업 템플릿에 할당하거나 레이아웃 템플릿 또는 다른 개체를 이 역할과 공유할 수 있습니다. 의 모든 작업 역할 사용에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). 작업 역할 삭제에 대한 자세한 내용은 [작업 역할 삭제](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
