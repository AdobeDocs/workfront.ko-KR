---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion에서 조직에 사용자 추가
description: Adobe Workfront Fusion에서 조직에 사용자를 추가할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 5cdc438c6757d438b2c09796cf77e59dc19c45d9
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Adobe Workfront Fusion에서 조직 또는 팀에 사용자 추가

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 [!DNL Adobe Admin Console]에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 [!DNL Adobe Admin Console]에 온보딩된 경우 [!DNL Adobe Admin Console]을(를) 통해 이 작업을 수행해야 합니다.
>
>조직을 [!DNL  Adobe Admin Console](으)로 이동한 후 Adobe을 추가하는 방법과 통합 환경에 대한 지침은 [다음을 통해  [!DNL Adobe Workfront Fusion] 에 사용자 추가 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)를 참조하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 프로시저 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront Fusion/Adobe 비즈니스 플랫폼)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md)을 참조하십시오.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 
     <p>조직의 [!DNL Workfront Fusion] 관리자여야 합니다.</p>
     <p>팀의 [!DNL Workfront Fusion] 관리자여야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

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
>[!NOTE]
>
>조직이 현재 Adobe Admin Console으로 이동하는 중인 경우 Workfront에서 사용자를 관리(사용자 추가 또는 삭제)할 수 없습니다. 마이그레이션이 완료된 후 Adobe Admin Console에서 이러한 작업을 수행할 수 있습니다.

조직에 사용자를 추가하려면 사용자를 추가하려는 조직의 관리자여야 합니다. 역할에 대한 자세한 내용은 [조직 역할 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md)을 참조하세요.

조직에 사용자를 추가하려면 다음 작업을 수행하십시오.

1. 메뉴에서 **[!UICONTROL 조직]**(으)로 이동하고 사용자를 추가할 조직을 선택합니다.
1. 대시보드에서 **[!UICONTROL 사용자]** 탭을 엽니다.
1. **[!UICONTROL 새 사용자 초대]**&#x200B;를 클릭하고 **[!UICONTROL 보내기]**&#x200B;를 클릭하여 초대를 보냅니다.

   >[!NOTE]
   >
   >   
   >[!UICONTROL 새 사용자 초대] 단추가 표시되지 않으면 조직이 [!DNL Adobe Business Platform.]에 온보딩되었습니다.
   >
   >  [!DNL Adobe Business Platform]에 온보딩된 조직에 사용자를 추가하는 방법에 대한 지침은 [다음을 통해  [!DNL Adobe Workfront Fusion] 에 사용자 추가 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)를 참조하십시오.

1. 양식을 작성하십시오.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 전자 메일 주소]</td>
      <td>
        사용자의 이메일 주소 입력
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>
        <p>사용자의 전체 이름 입력</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 역할] </td>
      <td>사용자의 역할을 선택합니다. 역할에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">조직 및 팀 역할</a>을 참조하세요.</p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">팀</td>
      <td>사용자가 멤버로 활동할 팀을 모두 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">참고</td>
      <td>사용자에 대한 메모를 입력합니다. 이 메모는 사용자의 초대 이메일에 표시됩니다.</td>
    </tr>
  </tbody>
</table>

사용자는 초대를 수락할 수 있는 초대 이메일을 수신합니다.

## 팀에 사용자 추가

팀을 만들면 사용자가 팀에 할당됩니다. 기존 사용자를 팀에 추가해야 할 경우 팀의 사용자 페이지에서 추가할 수 있습니다.

팀에 사용자 추가는 해당 팀의 페이지에서 처리됩니다.

1. 왼쪽 패널에서 **조직**&#x200B;을 선택하고 조직 페이지의 **팀** 탭을 클릭한 다음 팀을 선택하여 사용자를 추가할 팀으로 이동합니다.

   또는

   다른 팀의 페이지에 있는 경우 페이지 상단의 팀 드롭다운을 클릭합니다.

1. 팀 페이지(페이지 맨 위에 팀 이름이 있음)에서 **사용자** 탭을 선택합니다.
1. 페이지에서 사용자를 찾습니다. 조직의 사용자는 팀의 구성원이 아니더라도 이 페이지에 표시됩니다.
1. 사용자 이름 오른쪽에 있는 **없음**&#x200B;을 클릭한 다음 팀에 부여할 역할을 선택하십시오.

사용자가 팀에 추가됩니다.