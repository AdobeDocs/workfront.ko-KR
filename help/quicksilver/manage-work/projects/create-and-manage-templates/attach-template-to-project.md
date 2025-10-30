---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에 템플릿 첨부
description: 프로젝트의 초기 생성 단계 또는 생성 후 프로젝트에 템플릿을 첨부할 수 있습니다.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 7fef704355fad677f2bdf40e630ea0146a9e1d58
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 5%

---

# 프로젝트에 템플릿 첨부

<!-- Audited: 10/2025 -->

프로젝트의 초기 생성 단계 또는 생성 후 프로젝트에 템플릿을 첨부할 수 있습니다.

템플릿을 사용하여 프로젝트를 만드는 방법에 대한 자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](../../../manage-work/projects/create-projects/create-project-from-template.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
    <p>플랜</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집 </p> <p>템플릿에 대한 액세스 보기</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>템플릿에 대한 권한 이상 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p>
   <p>Or</p>
   <p>Current: Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Share a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create and modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## 기존 프로젝트에 템플릿 첨부 {#attach-a-template-to-an-existing-project}

프로젝트 페이지나 프로젝트 목록 또는 보고서에서 프로젝트에 템플릿을 첨부할 수 있습니다.

{{step1-to-projects}}

1. **프로젝트** 페이지에서 템플릿을 첨부할 프로젝트를 선택합니다.

1. 프로젝트 이름의 오른쪽에 있는 **자세히** 아이콘 ![추가 드롭다운](assets/more-dropdown.png)을 클릭합니다.

   ![기타 아이콘](assets/qs-more-icon-on-an-object.png)

   또는

   프로젝트 목록 또는 보고서로 이동하여 프로젝트를 선택한 다음 목록 맨 위에 있는 **자세히** 아이콘 ![추가 드롭다운](assets/more-dropdown.png)을 클릭합니다.

   ![메뉴가 더 확장됨](assets/more-menu-expanded.png)

1. **템플릿 첨부**&#x200B;를 클릭합니다. **템플릿 첨부** 상자가 표시됩니다.

1. **템플릿 검색** 필드에 첨부할 템플릿 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   또는

   **기타 템플릿** 영역에서 템플릿 이름을 클릭합니다.

   템플릿에 대한 다음 정보가 포함된 템플릿 미리보기가 오른쪽에 표시됩니다.

   * 기간
   * 소유자
   * 최상위 작업 수(처음 3개의 최상위 작업 목록 포함)
   * 총 작업 수
   * 첨부된 사용자 정의 양식의 이름

   ![템플릿 상자 첨부](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (선택 사항) 템플릿 이름 오른쪽에 있는 **즐겨찾기** 아이콘 ![즐겨찾기 아이콘](assets/favorites-icon-small.png)을 클릭하여 즐겨찾기로 표시하고 **즐겨찾기** 목록으로 이동합니다.

1. (선택 사항) **즐겨찾기** 아이콘 ![즐겨찾기 아이콘](assets/favorites-icon-selected.png)을 다시 클릭하여 **즐겨찾기** 목록에서 제거하십시오.
1. **사용자 지정 및 첨부**&#x200B;를 클릭합니다. **템플릿 첨부** 사이드 패널이 열립니다.

1. (선택 사항) 다음 섹션에서 정보를 갱신합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">작업 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래에서 선택한 템플릿 작업을 프로젝트로 가져옵니다. 제외할 항목을 선택 취소합니다. </td> 
      <td>프로젝트에 첨부하기 전에 템플릿에서 제외할 작업을 선택 취소합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 템플릿의 전임 작업으로 사용할 프로젝트 작업을 선택하십시오.</td> 
      <td> <p>필드를 클릭하여 프로젝트 작업 목록을 표시한 다음 템플릿 작업을 시작하기 전에 완료해야 하는 작업을 선택합니다. 또는 템플릿을 첨부한 후 이 단계를 건너뛰고 프로젝트 내에서 관계를 설정할 수 있습니다. </p> <p> <strong>종속성 유형</strong>, <strong>지연 시간</strong> 정보를 선택하고 <strong>전임 작업 적용</strong> 확인란을 선택하여 전임 작업을 적용하려는 경우 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 템플릿의 상위 작업으로 사용할 프로젝트 작업을 선택하십시오.</td> 
      <td> 모든 템플릿 작업에 대해 상위 작업으로 지정할 프로젝트 작업을 선택합니다. 선택하지 않으면 모든 템플릿 작업이 현재 프로젝트 작업의 끝에 나타납니다. 템플릿을 첨부한 후 이 단계를 건너뛰고 프로젝트에서 작업을 이동할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">옵션 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래 선택된 항목이 프로젝트로 전송됩니다. 제외하려면 선택을 취소하십시오.</td> 
      <td> <p>프로젝트에 첨부하기 전에 템플릿에서 제외할 정보에 대한 확인란의 선택을 취소합니다. 각 필드에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">프로젝트에 템플릿을 첨부하는 개요</a>를 참조하십시오. </p> <p>중요: <strong>대기열 속성 및 문제 설정</strong> 상자를 선택하면 템플릿의 대기열 세부 정보가 프로젝트의 대기열 세부 정보를 덮어씁니다. 이 경우 템플릿의 라우팅 규칙, 대기열 주제 및 주제 그룹이 프로젝트의 그룹에 추가됩니다. <br>프로젝트가 요청 대기열로 설정되어 있고 프로젝트에 첨부한 템플릿이 요청 대기열로 설정되어 있지 않은 경우 <strong>대기열 속성 및 문제 설정</strong> 상자를 선택한 상태로 두면 프로젝트의 대기열 정보가 제거됩니다. <br><strong>대기열 속성 및 문제 설정</strong> 상자를 선택 취소하면 프로젝트의 모든 대기열 설정 설정이 유지되며 템플릿의 대기열 설정 설정은 첨부되지 않습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">사용자 지정 Forms 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 Forms</td> 
      <td> <p>사용자 정의 양식을 템플릿에 첨부하면 해당 이름이 왼쪽 패널에 표시됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 사용자 정의 양식의 정보를 업데이트합니다. 이 정보는 프로젝트로 전송됩니다.

   >[!TIP]
   >
   >* 템플릿의 사용자 정의 양식에 비어 있는 필수 필드가 포함된 경우 이 단계는 필수입니다.
   >* 템플릿 사용자 정의 양식의 필드가 프로젝트에 이미 있고 정보를 포함하는 경우 프로젝트에 이미 있는 정보가 유지됩니다. 템플릿을 첨부하는 동안에는 편집할 수 없습니다.

1. **템플릿 첨부**&#x200B;를 클릭합니다.
1. 템플릿 연결을 중지하려면 **첨부 취소**&#x200B;를 클릭하십시오.

   또는

   템플릿을 프로젝트에 추가하려면 첨부 파일을 완료하도록 허용합니다.

   템플릿을 첨부한 후에는 프로젝트를 편집하고 필요에 따라 작업, 정보 또는 설정을 조정할 수 있습니다.

1. (선택 사항) 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭한 다음 **개요**&#x200B;를 클릭하여 **프로젝트 관계** 영역에 첨부한 템플릿의 이름을 봅니다.

   >[!TIP]
   >
   >프로젝트에 템플릿을 두 개 이상 첨부하면 먼저 첨부한 템플릿만 이 필드에 표시됩니다. 자세한 내용은 이 문서의 [기존 프로젝트에 여러 템플릿 첨부 및 템플릿 정보 보기](#attach-multiple-templates-to-an-existing-project-and-view-template-information) 섹션을 참조하십시오.

1. (선택 사항) 템플릿을 첨부한 프로젝트에서 템플릿 정보를 제거합니다. 자세한 내용은 [프로젝트에서 템플릿 정보 제거](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md)를 참조하십시오.

## 기존 프로젝트에 여러 템플릿을 첨부하고 템플릿 정보 보기 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

이 문서의 [기존 프로젝트에 템플릿 첨부](#attach-a-template-to-an-existing-project) 섹션에 설명된 단계에 따라 동일한 프로젝트에 여러 템플릿을 한 번에 하나씩 첨부할 수 있습니다. 이렇게 하면 각 템플릿의 작업 및 기타 정보가 프로젝트에 추가됩니다.

>[!TIP]
>
>프로젝트에 여러 템플릿을 첨부할 때 먼저 첨부한 템플릿만 프로젝트 세부 정보 영역에 표시됩니다.

프로젝트에 적용되는 템플릿을 보려면 다음과 같이 하십시오.

{{step1-to-projects}}

1. **프로젝트** 페이지에서 서식 파일이 첨부된 프로젝트를 선택하십시오.

1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.

1. **프로젝트 관계** 아래 **개요** 섹션 아래쪽의 **템플릿** 필드에서 프로젝트에 첨부된 템플릿의 이름을 찾습니다.

   ![프로젝트에 대한 템플릿 정보](assets/nwe-template-info-on-project-350x356.png)


