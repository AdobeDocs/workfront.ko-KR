---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에 템플릿 첨부
description: 프로젝트의 초기 생성 단계 동안 또는 템플릿이 생성된 후에 프로젝트에 템플릿을 첨부할 수 있습니다.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 5%

---

# 프로젝트에 템플릿 첨부

프로젝트의 초기 생성 단계 동안 또는 템플릿이 생성된 후에 프로젝트에 템플릿을 첨부할 수 있습니다.

템플릿을 사용하여 프로젝트를 만드는 방법에 대한 자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](../../../manage-work/projects/create-projects/create-project-from-template.md).

## 액세스 요구 사항

이 문서에 설명된 단계를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집 </p> <p>프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>.</p> <p>템플릿에 대한 액세스 보기</p> <p>템플릿 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">템플릿 공유</a>. </p> <p>템플릿 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 대한 액세스 권한 부여</a>.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>. </p> <p>템플릿에 대한 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

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

프로젝트 페이지나 프로젝트 목록 또는 보고서에서 Workfront의 프로젝트에 템플릿을 첨부할 수 있습니다.

1. 템플릿을 첨부할 프로젝트로 이동하고 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png) 프로젝트 이름의 오른쪽에 있습니다.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   또는

   프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택한 다음 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png) 를 클릭합니다.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. 클릭 **템플릿 첨부**.

   템플릿 첨부 상자가 표시됩니다.

1. 에 첨부할 템플릿의 이름을 입력합니다 **검색 템플릿** 필드를 클릭한 다음 목록이 표시되면 클릭합니다.

   또는

   에서 템플릿 이름을 클릭합니다 **기타 템플릿** 영역.

   템플릿에 대한 다음 정보가 포함된 템플릿의 미리 보기가 오른쪽에 표시됩니다.

   * 기간
   * 소유자
   * 최상위 수준의 작업 수(처음 세 개의 최상위 작업 목록 포함)
   * 총 작업 수
   * 첨부된 사용자 지정 양식의 이름

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (선택 사항) **즐겨찾기** 아이콘 ![](assets/favorites-icon-small.png) 즐겨찾기로 표시하려면 템플릿 이름의 왼쪽에 있는 를 클릭합니다. 즐겨찾기 목록에서 템플릿을 이동합니다.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (선택 사항) **즐겨찾기** 아이콘 ![](assets/favorites-icon-selected.png) 즐겨찾기 목록에서 제거하려면 다시 선택합니다.
1. 클릭 **사용자 지정 및 첨부**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. 템플릿을 첨부하기 전에 다음 섹션에서 정보를 업데이트합니다. 또는 **템플릿 첨부** 언제든지):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">작업 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래에서 선택한 템플릿 작업을 프로젝트로 가져옵니다. 제외할 템플릿 작업은 선택 취소합니다. </td> 
      <td>프로젝트에 첨부하기 전에 템플릿에서 제외할 모든 작업의 선택을 취소합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 템플릿의 전임 작업으로 사용할 프로젝트 작업을 선택하십시오.</td> 
      <td> <p>프로젝트 작업 목록을 표시하려면 필드를 클릭합니다. 템플릿 작업을 시작하기 전에 완료하려는 프로젝트 작업을 선택합니다. 또는 템플릿을 연결한 후 이 단계를 건너뛰고 프로젝트 내에서 관계를 설정할 수 있습니다. </p> <p> 을(를) 선택합니다 <strong>종속성 유형</strong>, <strong>지연</strong> 선행 사용자를 원하는 경우 <strong>강제 적용</strong> 아님 아님 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 템플릿의 상위 작업으로 사용할 프로젝트 작업을 선택하십시오.</td> 
      <td> 모든 템플릿 작업의 상위 작업으로 지정할 프로젝트 작업을 선택합니다. 선택하지 않으면 모든 템플릿 작업이 현재 프로젝트 작업 끝에 나타납니다. 템플릿이 첨부된 후 이 단계를 건너뛰고 프로젝트에서 작업을 이동할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">옵션 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래 선택된 항목이 프로젝트로 전송됩니다. 제외하려면 선택을 취소하십시오.</td> 
      <td> <p>템플릿에 첨부하기 전에 지우고자 하는 정보 옆의 확인란을 선택 취소합니다. 이 정보는 템플릿에서 프로젝트로 전송되지 않습니다. 각 필드에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">프로젝트에 템플릿 첨부 개요</a>. </p> <p>중요 사항: 확인 <strong>큐 속성 및 문제 설정</strong> 상자에 있는 템플릿의 큐 세부 정보 를 프로젝트의 큐 세부 정보로 덮어씁니다. 이 경우 템플릿의 라우팅 규칙, 큐 항목 및 주제 그룹이 프로젝트의 항목에 추가됩니다. <br>프로젝트가 요청 큐로 설정되고 프로젝트에 첨부하는 템플릿이 요청 큐로 설정되지 않은 경우, 프로젝트를 나갈 경우 프로젝트의 큐 정보는 제거됩니다 <strong>큐 속성 및 문제 설정</strong> 확인란을 선택합니다. <br>을 선택 취소하는 경우 <strong>큐 속성 및 문제 설정</strong> 이 상자에서 프로젝트의 모든 큐 설정 설정이 유지되며 템플릿의 큐 설정 설정이 첨부되지 않습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">사용자 지정 Forms 섹션</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 Forms</td> 
      <td> <p>사용자 지정 양식이 템플릿에 연결되면 왼쪽 패널에 해당 이름이 표시됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 사용자 지정 양식에서 정보를 업데이트합니다. 이 정보는 프로젝트로 전송됩니다.

   >[!TIP]
   >
   >* 템플릿의 사용자 지정 양식에 빈 필수 필드가 포함되어 있으면 이 단계를 수행해야 합니다.
   >* 템플릿 사용자 지정 양식의 필드가 이미 프로젝트에 있고 정보를 포함하는 경우 프로젝트에 이미 정보가 유지됩니다. 템플릿을 첨부하는 동안에는 편집할 수 없습니다.


1. 클릭 **템플릿 첨부.**
1. 클릭 **첨부 파일 취소** 템플릿 첨부 중지

   또는

   첨부 파일에서 템플릿을 프로젝트에 추가할 수 있도록 합니다.

   템플릿을 첨부한 후에는 프로젝트를 편집하고 필요에 따라 작업, 정보 또는 설정을 조정할 수 있습니다.

1. (선택 사항) **프로젝트 세부 사항**, 그런 다음 **개요** 에서 첨부한 템플릿의 이름을 보려면 **프로젝트 관계** 영역.

   >[!TIP]
   >
   >프로젝트에 두 개 이상의 템플릿을 첨부하는 경우 먼저 첨부한 템플릿만 이 필드에 표시됩니다. 자세한 내용은 [기존 프로젝트에 여러 템플릿 첨부 및 템플릿 정보 보기](#attach-multiple-templates-to-an-existing-project-and-view-template-information) 섹션에 자세히 설명되어 있습니다.

1. (선택 사항) 템플릿을 첨부한 프로젝트에서 템플릿 정보를 제거합니다. 자세한 내용은 [프로젝트에서 템플릿 정보 제거](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## 기존 프로젝트에 여러 템플릿 첨부 및 템플릿 정보 보기 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

섹션에 설명된 단계에 따라 여러 템플릿을 동일한 프로젝트에 한 번에 하나씩 첨부할 수 있습니다 [기존 프로젝트에 템플릿 첨부](#attach-a-template-to-an-existing-project) 참조하십시오. 이렇게 하면 각 템플릿의 작업 및 기타 정보가 프로젝트에 추가됩니다.

>[!TIP]
>
>프로젝트에 여러 템플릿을 첨부하면 먼저 첨부한 템플릿만 프로젝트 세부 정보 영역에 표시됩니다.

프로젝트에 적용되는 템플릿을 이해하려면 다음을 수행하십시오.

1. 템플릿이 첨부된 프로젝트로 이동합니다.
1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 에서 프로젝트에 첨부된 템플릿의 이름을 찾습니다 **템플릿** 맨 아래 필드 **개요** 섹션 **프로젝트 관계** .

   ![](assets/nwe-template-info-on-project-350x356.png)

 

 
