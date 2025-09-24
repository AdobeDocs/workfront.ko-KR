---
product-area: projects;templates
navigation-topic: manage-projects
title: 프로젝트를 템플릿으로 저장
description: 프로젝트를 프로젝트 수준에서 템플릿으로 저장하면 사용자가 UI에서 를 확인할 수 있습니다. 이 링크에는 보다 심층적인 (단계별) 다른 문서가 있습니다. 이 기능은 프로젝트와 템플릿 영역 모두에 있어야 합니다.)
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# 프로젝트를 템플릿으로 저장

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<!--
<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

프로젝트가 나중에 다시 시작될 경우 기존 프로젝트에서 템플릿을 만들 수 있습니다. 그런 다음 템플릿을 다시 사용하여 유사한 정보를 포함하거나 기존 프로젝트와 동일한 타임라인 또는 할당을 공유할 수 있는 향후 프로젝트를 만들 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준 </p>
   또는 
   <p>현재: 플랜 </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기 </p> <p>프로젝트를 템플릿으로 저장한 후 템플릿에 대한 관리 권한을 받습니다</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트를 템플릿으로 저장

<!--
Saving a project as a template differs in the Production and the Preview environments. 

### Save a project as a template in the Production environment


1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/qs-more-icon-on-an-object.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td>Use the drop-down list to select any custom forms to attach to the template. If any custom forms have already been associated with the project, all of the data fields from those custom forms are displayed.<br>You can include up to 10 custom forms on a single template.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Manage Forms** to remove or reorder the forms. For information about how to remove and reorder custom forms on the template, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Click **Next Step.**
1. In the **Options** section, select the checkbox beside any information you want to clear from the template.

   ![](assets/save-as-template-options-step-350x109.png)

1. Click **Next Step.**
1. In the **Exclude** section, select any tasks that you want to exclude from the project.

   ![](assets/save-as-template-exclude-350x205.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates and can either be attached to an existing project or used to create a new one.


<div class="preview">

### Save a project as a template in the Preview environment

-->

1. 템플릿으로 저장할 프로젝트로 이동합니다.
1. **자세히** 메뉴 ![자세히 아이콘](assets/qs-more-icon-on-an-object.png)을 클릭한 다음 **템플릿으로 저장**&#x200B;을 클릭합니다.
1. **템플릿으로 저장** 섹션에서 템플릿에 대해 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 이름</td> 
      <td>템플릿 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>템플릿에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>다음 옵션 중에서 선택합니다.</p> 
       <ul> 
        <li> <p><strong>예</strong>: 다른 사용자가 템플릿을 찾아 프로젝트에 첨부할 수 있습니다.</p> </li> 
        <li><strong>아니요</strong>: 다른 사용자가 템플릿을 찾을 수 없어 프로젝트에 첨부할 수 없습니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td>드롭다운 목록을 사용하여 템플릿에 첨부할 사용자 정의 양식을 선택합니다. 사용자 정의 양식이 이미 프로젝트와 연결된 경우 해당 사용자 정의 양식의 모든 데이터 필드가 표시됩니다.<br>한 서식 파일에 최대 10개의 사용자 정의 양식을 포함할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 양식을 제거하거나 순서를 변경하려면 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.

   양식 순서를 변경하려면 올바른 순서로 양식 순서를 끌어서 놓습니다.
양식을 제거하려면 양식을 선택한 다음 **제거**&#x200B;를 클릭합니다. 선택한 양식을 제거하려면 **취소**&#x200B;를 클릭하십시오.

   ![템플릿으로 저장 상자의 사용자 정의 양식 영역](assets/custom-forms-ara-in-save-as-template-box.png)

1. 필요한 경우 첨부된 사용자 정의 양식의 정보를 업데이트합니다. 정보가 템플릿으로 전송됩니다.

1. 왼쪽 패널에서 **옵션**&#x200B;을 클릭한 다음 템플릿에 전송할 정보 옆의 확인란을 선택합니다. 선택 취소된 항목은 템플릿으로 전송되지 않습니다. 기본적으로 모든 옵션이 선택 해제됩니다.

   ![템플릿으로 저장 상자의 옵션 영역](assets/options-area-in-save-as-template-box.png)

1. 왼쪽 패널에서 **제외**&#x200B;를 클릭한 다음 프로젝트에서 제외할 작업을 선택하십시오. 기본적으로 모든 작업이 선택 해제됩니다.

   ![템플릿으로 저장 상자에서 영역 제외](assets/exclude-area-save-as-template-box.png)

1. 화면 오른쪽 상단의 **완료 및 템플릿 저장**&#x200B;을 클릭합니다.

   이제 템플릿이 사용 가능한 템플릿 목록에 표시되며 기존 프로젝트에 첨부하거나 새 템플릿을 만드는 데 사용할 수 있습니다.

