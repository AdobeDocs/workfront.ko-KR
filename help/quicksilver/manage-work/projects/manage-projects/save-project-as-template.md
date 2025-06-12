---
product-area: projects;templates
navigation-topic: manage-projects
title: 프로젝트를 템플릿으로 저장
description: 프로젝트를 템플릿으로 저장Save as a template at project level(프로젝트 수준에서 템플릿으로 저장)을 참조하십시오. 이 문서에는 보다 심층적인(단계별) 링크가 있습니다. 이 기능은 프로젝트와 템플릿 영역 모두에서 유지되어야 합니다.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 1%

---

# 프로젝트를 템플릿으로 저장

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기 릴리스부터 1주일 후에 모든 고객의 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다.

자세한 내용은 [인터페이스 현대화](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)를 참조하십시오.

</div>

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

프로젝트를 템플릿으로 저장하는 것은 프로덕션 및 미리보기 환경에서 다릅니다.

### 프로덕션 환경에서 프로젝트를 템플릿으로 저장

1. 템플릿으로 저장할 프로젝트로 이동합니다.
1. **자세히** 메뉴 ![자세히 아이콘](assets/qs-more-icon-on-an-object.png)을 클릭한 다음 **템플릿으로 저장**&#x200B;을 클릭합니다.
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
      <td>드롭다운 목록을 사용하여 템플릿에 첨부할 사용자 정의 양식을 선택합니다. 사용자 정의 양식이 이미 프로젝트와 연결된 경우 해당 사용자 정의 양식의 모든 데이터 필드가 표시됩니다.<br>한 서식 파일에 최대 10개의 사용자 정의 양식을 포함할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 양식을 제거하거나 순서를 변경하려면 **Forms 관리**&#x200B;를 클릭하십시오. 템플릿에서 사용자 정의 양식을 제거하고 순서를 변경하는 방법에 대한 자세한 내용은 [사용자 정의 양식](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)을 참조하십시오.

   ![](assets/save-as-template-first-step-350x159.png)

1. **다음 단계를 클릭합니다.**
1. **옵션** 섹션에서 템플릿에서 지우려는 정보 옆의 확인란을 선택합니다.

   ![](assets/save-as-template-options-step-350x109.png)

1. **다음 단계를 클릭합니다.**
1. **제외** 섹션에서 프로젝트에서 제외할 작업을 선택합니다.

   ![](assets/save-as-template-exclude-350x205.png)

1. **템플릿 완료 및 저장**&#x200B;을 클릭합니다.

   이제 템플릿이 사용 가능한 템플릿 목록에 표시되며 기존 프로젝트에 첨부하거나 새 템플릿을 만드는 데 사용할 수 있습니다.


<div class="preview">

### 미리보기 환경에서 프로젝트를 템플릿으로 저장

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

1. 왼쪽 패널 섹션에서 **옵션**&#x200B;을 클릭한 다음 템플릿에 전송할 정보 옆의 확인란을 선택합니다. 선택 취소된 항목은 템플릿으로 전송되지 않습니다. 기본적으로 모든 옵션이 선택 해제됩니다.

   ![템플릿으로 저장 상자의 옵션 영역](assets/options-area-in-save-as-template-box.png)

1. 왼쪽 패널에서 **제외**&#x200B;를 클릭한 다음 프로젝트에서 제외할 작업을 선택하십시오. 기본적으로 모든 작업이 선택 해제됩니다.

   ![템플릿으로 저장 상자에서 영역 제외](assets/exclude-area-save-as-template-box.png)

1. **템플릿 완료 및 저장**&#x200B;을 클릭합니다.

   이제 템플릿이 사용 가능한 템플릿 목록에 표시되며 기존 프로젝트에 첨부하거나 새 템플릿을 만드는 데 사용할 수 있습니다.

</span>