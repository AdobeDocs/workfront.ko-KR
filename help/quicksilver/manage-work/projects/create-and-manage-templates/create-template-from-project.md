---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에서 템플릿 만들기
description: 기존 프로젝트를 템플릿으로 저장할 때 템플릿을 만들 수 있습니다.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# 프로젝트에서 템플릿 만들기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

기존 프로젝트를 템플릿으로 저장할 때 템플릿을 만들 수 있습니다.

기존 프로젝트를 템플릿으로 저장한 후 새 템플릿을 사용하여 새 프로젝트를 만들 수 있습니다. 이를 통해 프로젝트 생성 프로세스를 간소화하고 신속하게 수행할 수 있습니다.

>[!NOTE]
>
>프로젝트를 템플릿으로 저장할 때 작업 및 프로젝트의 실제 날짜가 템플릿에 저장되지 않습니다.
>
>템플릿 및 해당 작업에는 실제 날짜가 없고, 작업이 시작될 수 있는 날짜(향후 프로젝트가 시작될 수 있는 날짜)와 작업이 완료되어야 하는 날짜가 표시됩니다. 템플릿을 사용하여 향후 프로젝트를 만들 때 프로젝트에 실제 날짜가 표시됩니다. 자세한 내용은 [프로젝트 만들기](../create-projects/create-project.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기 </p> <p>템플릿을 만든 후 템플릿에 대한 관리 권한을 받습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트에서 템플릿 만들기

1. 템플릿으로 저장할 프로젝트로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png), 그런 다음 **템플릿으로 저장**.
1. 템플릿에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
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
      <td>드롭다운 목록을 사용하여 템플릿에 첨부할 사용자 정의 양식을 선택합니다. 사용자 정의 양식이 이미 프로젝트와 연결된 경우 해당 사용자 정의 양식의 모든 데이터 필드가 표시됩니다.<br>단일 템플릿에 최대 10개의 사용자 정의 양식을 포함할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **Forms 관리** 을 클릭하여 양식을 제거하거나 순서를 변경합니다. 템플릿에서 사용자 정의 양식을 제거하고 순서를 변경하는 방법에 대한 자세한 내용은 [사용자 정의 양식](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. 클릭 **다음 단계.**
1. 다음에서&#x200B;**옵션** 섹션에서 템플릿에서 지우려는 정보 옆의 확인란을 선택합니다.

   ![](assets/save-as-template-options-step-350x109.png)

1. 클릭 **다음 단계.**
1. 다음에서 **제외** 섹션에서 프로젝트에서 제외할 작업을 선택합니다.

   ![](assets/save-as-template-exclude-350x205.png)

1. 클릭 **템플릿을 완료하고 저장합니다.**

   이제 템플릿이 사용 가능한 템플릿 목록에 표시되며 기존 프로젝트에 첨부하거나 새 템플릿을 만드는 데 사용할 수 있습니다.

 
