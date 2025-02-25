---
title: 마일스톤 경로 만들기
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront 관리자는 시스템의 모든 프로젝트에 적용할 수 있는 마일스톤 경로를 만들 수 있습니다. 이 영역의 마일스톤 경로에 대한 변경 사항은 전체 Workfront 시스템에 영향을 줍니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: f3f33d870859408db5ec3dc306cf1d4209c126a3
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 3%

---

# 마일스톤 경로 만들기

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront 관리자는 시스템의 모든 프로젝트에 적용할 수 있는 마일스톤 경로를 만들 수 있습니다. 이 영역의 마일스톤 경로에 대한 변경 사항은 전체 Workfront 시스템에 영향을 줍니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 마일스톤 및 마일스톤 경로

프로젝트의 주요 작업을 사전 정의된 이정표와 연결할 수 있습니다. 이 기능은 프로젝트 진행 방식에 대한 높은 수준의 개요를 관리자 및 기타 이해 당사자에게 제공할 수 있습니다.

미리 정의된 모든 이정표의 합계를 이정표 경로라고 합니다.

이정표 경로를 구축하는 첫 번째 단계는 이정표 단계가 무엇인지 식별하고 이정표를 설정하는 것입니다. 마일스톤 경로를 여러 프로젝트에 연결할 수 있으므로 마일스톤 단계는 프로젝트의 일반 단계 또는 단계여야 합니다.

마일스톤 경로를 프로젝트와 연결하고 마일스톤을 작업에 연결하는 방법에 대한 자세한 내용은 [마일스톤과 작업 연결](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)을 참조하십시오.

## 마일스톤 경로 만들기

{{step-1-to-setup}}

1. **프로세스** > **마일스톤 경로**&#x200B;를 클릭합니다.
1. **새 마일스톤 경로**&#x200B;를 클릭합니다.
1. **기본 정보** 영역에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto">
    <tr>
      <td>마일스톤 경로 이름</td>
       <td>마일스톤 경로의 이름을 입력합니다.</td>
    </tr>
    <tr>
      <td>설명</td>
      <td>마일스톤 경로를 정의하는 설명을 입력합니다.</td>
    </tr>
    <tr>
       <td>활성화됨</td>
      <td>마일스톤 경로를 활성화하려면 이 확인란을 선택합니다. 다른 사용자는 프로젝트를 만들거나 편집할 때 이 경로를 찾아 프로젝트에 첨부할 수 있습니다. 비활성 마일스톤 경로는 프로젝트에 첨부할 수 없습니다. 이 기능은 기본적으로 활성화되어 있습니다.</td>
    </tr>
    <tr>
      <td>그룹</td>
      <td>이 그룹의 사용자가 이 마일스톤 경로를 보고 프로젝트에 적용할 수 있도록 하려면 나열된 그룹을 선택하십시오. 마일스톤 경로를 입력하는 사용자의 홈 그룹이 기본적으로 선택됩니다.</td>
    </tr>
   </table>

1. **마일스톤** 영역에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td>각 마일스톤의 수사적 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>이정표에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>마일스톤과 연결할 색상을 선택합니다. </p> <p>색상을 선택하지 않으면 마일스톤 경로에 사용되는 마지막 색상이 선택됩니다. 각 이정표에 대해 고유한 색상을 선택하는 것이 좋습니다. 색상은 시각적 및 보고 목적으로 사용됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **마일스톤 추가**&#x200B;를 클릭하고 경로가 완료될 때까지 필요에 따라 마일스톤을 계속 추가합니다.
1. 변경 내용을 저장하려면 **마일스톤 경로 만들기**&#x200B;를 클릭하세요.

   마일스톤 경로를 프로젝트와 연결할 준비가 되었습니다.

   마일스톤 경로를 프로젝트에 연결하고 마일스톤을 작업에 연결하는 방법에 대한 자세한 내용은 [마일스톤과 작업 연결](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)을 참조하세요.


## 보고서에서 마일스톤 경로 세부 정보 보기

프로젝트 보고서에서 마일스톤 경로의 세부 사항을 볼 수 있습니다.

마일스톤 경로를 프로젝트와 연결해야 프로젝트 보고서에서 해당 세부 사항을 볼 수 있습니다.

마일스톤 경로를 프로젝트에 연결하는 방법에 대한 자세한 내용은 [프로젝트 편집](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

{{step1-to-reports}}

1. **새 보고서**&#x200B;를 클릭한 다음 **프로젝트**&#x200B;를 클릭합니다.
1. **열 추가**&#x200B;를 클릭합니다.
1. **이 열에 표시** 영역에서 **마일스톤 경로**&#x200B;를 입력한 다음 표시될 때 **마일스톤 경로 이름**&#x200B;을 클릭하세요.
1. (선택 사항) **필터**&#x200B;를 클릭하고 보고서에 다음 필터를 추가합니다. **프로젝트 마일스톤 경로 ID가 비어 있지 않습니다**.

   필터는 보고서에 마일스톤 경로와 연결된 프로젝트만 표시하도록 합니다.

1. **저장 및 닫기**&#x200B;를 클릭합니다.
1. 보고서 이름을 추가한 다음 **적용**&#x200B;을 클릭합니다.

   프로젝트 보고서가 표시됩니다. 각 프로젝트와 연결된 마일스톤 경로가 보고서의 마지막 열에 표시됩니다.
1. 보고서의 마지막 열에서 마일스톤 경로 이름을 클릭합니다.

   마일스톤 경로의 세부 정보가 표시됩니다. 각 이정표에 대한 세부 정보도 표시됩니다.

   ![프로젝트 보고서의 마일스톤 경로 세부 정보](assets/milestone-details-from-project-report.png)

   <!--replace screen shot above with unshimming and mark it for Preview-->

1. (선택 사항) 프로젝트 보고서로 돌아가려면 **뒤로**&#x200B;를 클릭합니다.



