---
product-area: projects;templates
navigation-topic: manage-projects
title: 프로젝트를 템플릿으로 저장
description: 프로젝트를 템플릿으로 저장"템플릿으로 저장"을 프로젝트 수준에서 사용할 수 있으므로 UI에서 볼 수 있습니다. 이 링크가 더 심층적인(단계별)링크라는 다른 문서가 있습니다. 이 기능은 프로젝트 및 템플릿 영역 모두에서 유지되어야 합니다.)"
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# 프로젝트를 템플릿으로 저장

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

나중에 프로젝트가 다시 수행된다고 결정하는 경우, 기존 프로젝트에서 템플릿을 만들 수 있습니다. 그런 다음 템플릿을 다시 사용하여 유사한 정보를 포함하거나 기존 프로젝트와 동일한 타임라인이나 지정을 공유할 수 있는 향후 프로젝트를 만들 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>템플릿에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기 이상 </p> <p>프로젝트를 템플릿으로 저장한 후 템플릿에 대한 관리 권한을 받게 됩니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트를 템플릿으로 저장

1. 템플릿으로 저장할 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png), 그런 다음 **템플릿으로 저장**.
1. 템플릿에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td>템플릿의 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>템플릿에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>다음 옵션 중에서 선택합니다.</p> 
       <ul> 
        <li> <p><strong>예</strong>: 다른 사용자는 템플릿을 찾아 프로젝트에 첨부할 수 있습니다.</p> </li> 
        <li><strong>아니요</strong>: 다른 사용자는 템플릿을 찾을 수 없으며 프로젝트에 첨부할 수 없습니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td>드롭다운 목록을 사용하여 템플릿에 첨부할 사용자 지정 양식을 선택합니다. 사용자 지정 양식이 이미 프로젝트와 연결되어 있는 경우 해당 사용자 지정 양식의 모든 데이터 필드가 표시됩니다.<br>단일 템플릿에 최대 10개의 사용자 지정 양식을 포함할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **Forms 관리** 양식을 제거하거나 재정렬하려면 다음을 수행하십시오. 템플릿에서 사용자 지정 양식을 제거하고 다시 정렬하는 방법에 대한 자세한 내용은 [사용자 지정 양식](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. 클릭 **다음 단계.**
1. 에서&#x200B;**옵션** 섹션에서 템플릿에서 지울 정보 옆의 확인란을 선택합니다.

   ![](assets/save-as-template-options-step-350x109.png)

1. 클릭 **다음 단계.**
1. 에서 **제외** 섹션에서 프로젝트에서 제외할 작업을 선택합니다.

   ![](assets/save-as-template-exclude-350x205.png)

1. 클릭 **템플릿 완료 및 저장.**

   이제 템플릿이 사용 가능한 템플릿 목록에 표시되고 기존 프로젝트에 첨부하거나 새 템플릿을 만드는 데 사용할 수 있습니다.
