---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 회사 만들기 및 편집
description: ' [!DNL Adobe Workfront] 에 회사를 추가하여 재무 계획, 보고 목적으로 사용하고 개체에 대한 사용 권한을 정의하며 정보를 기밀로 유지할 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 5d7cc28ebb1c7d7401a60ef4fc383fc90ed20631
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# 회사 만들기 및 편집

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있으며 프로덕션에 단계적으로 롤아웃할 때 릴리스됩니다.</span>

회사는 조직, 조직 내 부서 또는 함께 일하는 클라이언트를 나타낼 수 있는 [!DNL Adobe Workfront]의 조직 단위입니다. [!DNL Workfront]에 회사를 추가하여 재무 계획, 보고 목적으로 사용하고 개체에 대한 사용 권한을 정의하며 정보를 기밀로 유지할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 패키지</p> </td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스</p> </td> 
   <td><p>[!UICONTROL 계획]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템에서 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다.</p> </li> 
     <li> <p>회사 관리에 대한 관리 액세스 권한으로, 시스템에서 모든 회사를 편집할 수 있습니다.</p> </li> 
    </ul> <p><b>참고</b>:  
     <ul> 
      <li> <p>그룹 관리자로 할당된 모든 그룹과 연결된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>[!DNL Workfront] 시스템에서 사용자를 추가하고 제거하려면 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. </p> </li> 
        <li> <p>액세스 수준의 <b>[!UICONTROL 사용자]</b> 설정이 <b>[!UICONTROL 편집]</b> 액세스로 구성되었으며, <b>[!UICONTROL 만들기]</b>와(과) <b>[!UICONTROL 사용자 관리]</b> <b>에서 두 개의 </b>[!UICONTROL 사용자 관리]<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p> <img src="assets/access-req-users.png"> </p> <p>이 두 옵션 중 <b>[!UICONTROL 사용자 관리자(그룹 사용자)]</b>이(가) 활성화된 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 회사에 사용자를 추가하면 얻을 수 있는 이점 {#benefits-of-adding-users-to-a-company}

* 사용자를 부하 직원과 연결하여 회사의 조직도를 작성할 수 있습니다. 동일한 회사의 사용자만 해당 회사의 다른 사용자에 대한 직접 보고서로 추가할 수 있습니다.
* 프로젝트 관리자는 동일한 회사 내에서 사용 가능한 리소스를 식별할 수 있습니다.
* 다음 설정 중 하나 또는 모두를 선택하여 회사 간에 정보를 비공개로 유지할 수 있습니다.

   * 동일한 회사의 사용자가 서로의 요청을 볼 수 있습니다.

     [!DNL Workfront] 관리자가 사용자 회사를 기반으로 요청에 유사한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) 문서의 [모두를 위한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 섹션을 참조하십시오.

     그룹 관리자가 사용자 회사를 기반으로 요청에 유사한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

   * 사용자는 회사와 연결된 요청 대기열만 볼 수 있습니다. 요청 대기열의 가시성을 제한하는 방법에 대한 자세한 내용은 [요청 대기열에 대한 액세스 권한 제공](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md)을 참조하십시오.
   * 사용자가 회사 또는 회사 및 기본 회사의 사용자만 보도록 제한할 수 있습니다. 사용자 개인 정보 보호에 대한 기본 회사 기능에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.
   * 사용자는 회사 사용자만 항목에 대한 업데이트를 볼 수 있도록 제한할 수 있습니다. 회사 업데이트에 대한 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## [!DNL Workfront]에서 회사 만들기 또는 편집 {#create-or-edit-a-company-in-workfront}

추가할 수 있는 회사 수에는 제한이 없습니다. 그러나 너무 많은 단편화가 작업 항목에 대한 사용자의 가시성을 방해할 수 있으므로 오브젝트 권한과 관련하여 발생할 수 있는 문제로 인해 사용하는 회사 수를 제한하는 것이 좋습니다.

기본적으로 [!DNL Workfront]의 인스턴스와 연결된 회사는 [!DNL Workfront] 시스템에 이미 만들어져 있으며 조직의 기본 회사입니다. 고객명과 같은 이름을 가지고 있습니다. [!DNL Workfront]에서 고객 정보에 대한 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.

회사를 추가하거나 편집하려면:

{{step-1-to-setup}}

1. **[!UICONTROL 회사]**&#x200B;를 클릭합니다.

   회사 목록이 표시됩니다.

1. 회사를 추가하려면 **[!UICONTROL 새 회사]**&#x200B;를 클릭하세요.

   또는

   기존 회사를 편집하는 경우 회사를 선택한 다음 회사 목록 맨 위에 있는 **[!UICONTROL 편집]** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

1. **기본 정보** 섹션에서 다음 정보를 업데이트하십시오.

   * **회사 이름** <span class="preview"> 또는 **이름**</span>: 회사의 이름을 입력하십시오.
   * **활성 상태임**: 이 옵션을 활성화하면 사용자가 회사를 찾아 만들고 편집한 프로젝트에 첨부할 수 있습니다. 비활성 회사는 프로젝트에 연결할 수 없습니다. 이 옵션은 기본적으로 활성화되어 있습니다.
   * **기본 회사입니다** <span class="preview">또는 **기본 회사입니다**</span>: 회사를 조직의 기본 회사로 할당합니다. 기본 회사는 일반적으로 대부분의 사용자가 근무하는 Workfront 계정을 나타냅니다.

     1차 회사로 지정된 회사가 한 개 있거나 한 개도 없을 수 있지만, 여러 개의 회사를 1차 회사로 지정할 수는 없습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 및 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

     >[!NOTE]
     >
     >액세스 수준을 수정하여 사용자를 주 회사 또는 관련 회사와 주 회사에서만 다른 사용자를 볼 수 있도록 제한할 수 있습니다. 기본 회사가 사용자의 액세스 수준으로 작동하는 방법에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 및 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

   * **그룹**: 회사와 거래하는 그룹이 있으면 여기에 그룹 이름을 추가할 수 있습니다. 이 기능은 그룹이 거래하는 모든 회사에 대해 보고하고 관리해야 하는 그룹 관리자에게 유용합니다.

     이 회사와 함께 작업할 그룹을 연결하지 않으면 그룹 관리자는 액세스 수준의 회사에 대한 관리 액세스 권한이 없으면 회사에 액세스할 수 없습니다. 이 액세스 권한 부여 방법에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

     그룹 이름을 입력한 다음 표시될 때 선택합니다.

     회사에 그룹을 할당하면 해당 그룹의 그룹 관리자는 회사에 대한 관리 액세스 권한을 갖게 됩니다. 자세한 내용은 이 문서에서 [그룹 관리자 및 회사](#group-administrators-and-companies)를 참조하십시오.

   * **회사 구성원**: 회사에 기존 사용자를 추가합니다. 이렇게 하면 이러한 사용자를 이 회사와 연결하게 됩니다.

     사용자 이름을 입력한 다음 표시될 때 선택합니다.

     한 회사에 연결하는 사용자 수에는 제한이 없지만 사용자는 두 개 이상의 회사에 연결할 수 없습니다.

1. **사용자 지정 Forms** 섹션에서 사용자 지정 양식을 추가하거나 업데이트합니다.

   Workfront에서 사용할 수 없는 필드를 회사에 추가하려는 경우 사용자 정의 양식을 작성하여 회사에 연결할 수 있습니다.

   드롭다운 메뉴에서 이 양식을 선택하여 회사에 첨부할 수 있습니다. 활성 사용자 정의 양식만 메뉴에 나열됩니다.

   >[!NOTE]
   >
   >외부 조회 필드 및 Workfront 기본 필드와 같은 고급 사용자 정의 양식 기능은 회사 편집 대화 상자가 아닌 세부 정보 페이지에서 회사 레코드를 열 때만 사용할 수 있습니다. 회사 목록에서 회사 이름을 클릭하여 세부 정보를 엽니다.

   사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. (조건부) 회사를 만드는 경우 **[!UICONTROL 회사 만들기]** <span class="preview">또는 **저장**&#x200B;을 클릭합니다.</span>

   또는

   기존 회사를 편집하는 경우 **[!UICONTROL 변경 내용 저장]** <span class="preview"> 또는 **저장**&#x200B;을 클릭합니다.</span>

## 회사 삭제

{{step-1-to-setup}}

1. **[!UICONTROL 회사]**&#x200B;를 클릭합니다.

   회사 목록이 표시됩니다.

1. 삭제할 회사 옆에 있는 확인란을 클릭한 다음 페이지 상단 근처에 있는 삭제 아이콘 ![삭제 아이콘](assets/delete-icon.png)을 클릭합니다.
1. 기본 회사로 설정되어 있거나 다른 오브젝트에서 사용 중인 회사를 삭제하는 경우 삭제할 회사를 바꿀 회사를 선택합니다. 선택한 회사가 기본 회사가 되거나 회사가 지정된 오브젝트에서 삭제된 회사를 바꿉니다.
1. **삭제**&#x200B;를 클릭합니다.

## 회사 멤버십 관리

기존 회사의 멤버십 관리에 대한 자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)를 참조하십시오.

## 청구 요금 관리

회사 수준의 청구 요율 재정의에 대한 자세한 내용은 [회사 수준의 작업 역할 청구 요율 재정의](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)를 참조하십시오.

## 회사와의 오브젝트 공유 개요

[회사에 사용자를 추가하는 이점](#benefits-of-adding-users-to-a-company) 섹션에 설명된 대로 특정 권한은 회사와 연결된 사용자에게 제공됩니다. 이러한 권한 외에도 사용자가 [!DNL Workfront]의 개체를 보거나, 제공하거나, 편집할 수 있는 권한을 회사 사용자와 공유할 수 있습니다.

한 번에 한 명의 개별 사용자와 오브젝트를 공유하지 않고 전체 회사와 공유할 수 있습니다. 회사의 각 사용자는 해당 객체에 대해 동일한 권한을 갖습니다.

개체 공유에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

## 그룹 관리자 및 회사 {#group-administrators-and-companies}

[!DNL Workfront] 관리자가 회사에 그룹을 할당하면 그룹의 그룹 관리자는 [!UICONTROL 설정]에서 회사에 대한 [!UICONTROL 관리] 액세스 권한을 갖게 됩니다. 여기에는 [!UICONTROL 설정]의 [!UICONTROL 회사] 페이지에 대한 액세스 권한이 포함되어 있습니다. 이 페이지에서 해당 그룹과 연결된 회사를 확인하고 관리할 수 있습니다.

[!UICONTROL 회사] 페이지에 대한 이 액세스 권한으로 그룹 관리자는 회사에 그룹을 할당할 수 있지만 그룹 관리자가 만든 회사여야 합니다. 그룹 관리자의 액세스 수준이 회사에 대한 관리 액세스 권한으로 구성되지 않은 경우 그룹 관리자가 회사를 만들 때 [!UICONTROL 그룹] 필드가 필요합니다. 해당 <span class="preview">별표</span> 또는 굵은 제목은 다음을 나타냅니다.

<span class="preview">미리 보기 환경의 샘플 이미지:</span>
![그룹이 필요한 새 회사 대화 상자](assets/group-admin-add-company-group-required.png)

프로덕션 환경의 샘플 이미지:
![회사에는 그룹이 필요합니다](assets/group-admin-add-company.png)

사용자가 액세스 수준의 회사에 대한 관리 액세스 권한을 얻는 방법에 대한 자세한 내용은 [특정 영역에 대한 사용자 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

[!UICONTROL 설정] 영역에서 회사를 관리하는 방법에 대한 자세한 내용은 이 문서의 [회사 만들기 또는 편집 [!DNL Workfront]](#create-or-edit-a-company-in-workfront)을 참조하십시오.

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
