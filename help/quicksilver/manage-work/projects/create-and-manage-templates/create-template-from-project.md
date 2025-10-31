---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에서 템플릿 만들기
description: 기존 프로젝트를 템플릿으로 저장할 때 템플릿을 만들 수 있습니다.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# 프로젝트에서 템플릿 만들기

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

기존 프로젝트를 템플릿으로 저장할 때 템플릿을 만들 수 있습니다.

기존 프로젝트를 템플릿으로 저장한 후 새 템플릿을 사용하여 새 프로젝트를 만들 수 있습니다. 이를 통해 프로젝트 생성 프로세스를 간소화하고 신속하게 수행할 수 있습니다.

>[!NOTE]
>
>프로젝트를 템플릿으로 저장할 때 작업 및 프로젝트의 실제 날짜가 템플릿에 저장되지 않습니다.
>
>템플릿 및 해당 작업에는 실제 날짜가 없고, 작업이 시작될 수 있는 날짜(향후 프로젝트가 시작될 수 있는 날짜)와 작업이 완료되어야 하는 날짜가 표시됩니다. 템플릿을 사용하여 향후 프로젝트를 만들 때 프로젝트에 실제 날짜가 표시됩니다. 자세한 내용은 [프로젝트 만들기](../create-projects/create-project.md)를 참조하십시오.

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
   <td><p>표준</p> 
   <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>템플릿에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기 </p> <p>템플릿을 만든 후 템플릿에 대한 관리 권한을 받습니다</p></td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 프로젝트에서 템플릿 만들기

1. 템플릿으로 저장할 프로젝트로 이동합니다.
1. **자세히** 메뉴 ![자세히 아이콘](assets/more-icon.png)을 클릭한 다음 **템플릿으로 저장**&#x200B;을 클릭합니다.
1. 템플릿에 대해 다음 정보를 지정합니다.

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
    </tbody> 
   </table>

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. **사용자 정의 양식 추가** 필드를 클릭하고 사용자 정의 프로젝트 이름을 입력하거나 목록에서 선택하십시오.

   사용자 정의 양식이 이미 프로젝트와 연결된 경우 해당 사용자 정의 양식의 기존 필드 모든 정보가 양식에 표시됩니다.

   단일 템플릿에 최대 10개의 사용자 정의 양식을 포함할 수 있습니다.

1. 마우스를 양식 이름 위로 가져간 다음 클릭하여 새 위치에 끌어다 놓습니다.

   ![프로젝트를 서식 파일로 저장](assets/save-project-as-template-top-of-the-form.png)

1. 왼쪽 패널에서 **옵션**&#x200B;을 클릭한 다음 템플릿으로 전송할 필드 또는 항목을 선택합니다.

   기본적으로 모든 항목이 선택되어 있습니다. 선택 취소된 항목은 템플릿으로 전송되지 않습니다.

   ![템플릿으로 저장 옵션](assets/save-project-as-template-options-area.png)

1. 왼쪽 패널에서 **제외**&#x200B;를 클릭한 다음 프로젝트에서 제외할 작업을 선택하십시오.

   ![템플릿으로 저장 제외](assets/save-project-as-template-exclude-area.png)

1. **템플릿 완료 및 저장**&#x200B;을 클릭합니다.

   이제 사용 가능한 템플릿 목록에 템플릿이 표시됩니다. 사용자는 기존 프로젝트에 새 템플릿을 첨부하거나 이를 사용하여 프로젝트를 만들 수 있습니다.


