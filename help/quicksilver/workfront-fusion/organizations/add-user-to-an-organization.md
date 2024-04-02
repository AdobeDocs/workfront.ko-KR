---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion에서 조직에 사용자 추가
description: Adobe Workfront Fusion에서 조직에 사용자를 추가할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Adobe Workfront Fusion에서 조직에 사용자 추가

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 온보딩되지 않은 조직에만 적용됩니다. [!DNL Adobe Admin Console]. 조직이 로 온보딩된 경우 [!DNL Adobe Admin Console], 다음을 통해 이 작업을 수행해야 합니다. [!DNL Adobe Admin Console].
>
>에서 사용자 추가에 대한 지침:[!DNL  Adobe Admin Console]문서에서 &quot;사용자 세부 정보 편집&quot; 섹션을 참조하십시오 [개별적으로 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 또는 다음 사용자에게 문의 [!UICONTROL Adobe Admin Console] 관리자.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront Fusion/Adobe 비즈니스 플랫폼)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 
     <p>다음이어야 합니다: [!DNL Workfront Fusion] 조직의 관리자.</p>
     <p>다음이어야 합니다: [!DNL Workfront Fusion] 팀 관리자.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 조직에 사용자 추가


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

조직에 사용자를 추가하려면 사용자를 추가하려는 조직의 관리자여야 합니다. 역할에 대한 자세한 내용은 [에서 조직 역할 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

조직에 사용자를 추가하려면 다음 작업을 수행하십시오.

1. 다음으로 이동 **[!UICONTROL 조직]** 메뉴에서 사용자를 추가할 조직을 선택합니다.
1. 를 엽니다. **[!UICONTROL 사용자]** 대시보드의 탭입니다.
1. 클릭 **[!UICONTROL 새 사용자 초대]**&#x200B;을(를) 클릭하고 양식(이메일, 메시지, 역할)을 작성한 다음 을(를) 클릭하여 초대장을 보냅니다. **[!UICONTROL 보내기]**.

>[!NOTE]
>
>   
>표시되지 않는 경우 [!UICONTROL 새 사용자 초대] 버튼, 조직이 [!DNL Adobe Business Platform.]
>
>  에 온보딩된 조직에 사용자를 추가하는 방법에 대한 지침 [!DNL Adobe Business Platform], 참조 [에 사용자 추가 [!DNL Adobe Workfront Fusion] 다음을 통해 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

사용자는 초대를 수락할 수 있는 초대 이메일을 수신합니다.
