---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Admin Console을 통해 Adobe Workfront Fusion에 사용자 추가
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 1%

---

# [!DNL Adobe Admin Console]을(를) 통해 [!DNL Adobe Workfront Fusion]에 사용자 추가

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [Adobe Admin Console을 통해 Adobe Workfront Fusion에 사용자 추가](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/add-fusion-users-admin-console.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 [!DNL Adobe Admin Console]에 온보딩된 조직에만 적용됩니다.
>
>조직이 아직 [!DNL Adobe Admin Console]에 온보딩되지 않은 경우 [조직에 사용자 추가 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md)를 참조하십시오.
>
>조직이 [!DNL Adobe Admin Console]에 온보딩되었는지 여부에 따라 다른 프로시저 목록을 보려면 [플랫폼 기반 관리 차이점([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md)을 참조하십시오.

[!DNL Adobe Admin Console]에 사용자를 추가하고 [!DNL Adobe Workfront Fusion]에 할당하거나 [!DNL Adobe Admin Console]의 기존 사용자를 [!DNL Workfront Fusion]에 할당할 수 있습니다.

사용자를 추가하는 방법을 포함하여 [!DNL Adobe Admin Console]의 [!DNL Workfront Fusion]에 대해 설명하는 비디오는 Adobe IMS에서 [[!DNL Fusion] 을(를) 참조하십시오](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
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
   <tr> 
   <td role="rowheader">[!DNL Adobe] 관리자 권한</td> 
   <td>조직의 [!DNL Adobe] 제품 중 [!UICONTROL 제품 구성 관리자]여야 합니다.</td> 
  </tr>
  </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

&#42;&#42;라이선스 [!DNL Adobe Workfront Fusion]에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.



## 전제 조건

[!DNL Workfront]에 대해 [!DNL Admin Console]을(를) 사용하기 전에 콘솔로 초대하는 전자 메일을 받아야 합니다.

1. [!DNL Adobe]을(를) 처음 사용하는 경우 조직의 [!DNL Adobe] 소프트웨어 및 서비스를 관리할 수 있는 관리 권한이 있다는 전자 메일을 받은 경우 전자 메일의 버튼을 클릭하여 [!DNL Adobe] 계정을 만들고 [!DNL Admin Console]을(를) 여십시오.

   또는

   이미 Adobe 계정이 있는 경우 [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/)(으)로 이동하십시오.


## [!DNL Adobe Admin Console] 및 [!DNL Workfront Fusion]에 새 사용자 추가

1. [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/)에서 위쪽 탐색 막대의 **[!UICONTROL 제품]** 탭을 선택한 다음 **[!DNL Workfront Fusion]** 제품 타일을 선택합니다.

   ![Admin Console의 Fusion](assets/fusion-product-admin-console.png)

1. 표시되는 목록에서 사용자를 추가하려는 조직을 선택합니다.

   ![Admin Console의 Fusion 인스턴스](assets/fusion-instances-admin-console.png)

1. **[!UICONTROL 제품 프로필]** 탭을 선택한 상태로 표시되는 목록에서 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 링크의 이름을 클릭합니다.

   ![Workfront Fusion 제품 프로필](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > [!UICONTROL 제품 프로필] 자체를 변경하지 마십시오.

1. 목록 위에 **[!UICONTROL 사용자]** 탭을 선택한 상태에서 **[!UICONTROL 사용자 추가]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 이 제품 프로필에 사용자 추가]** 상자에서 추가하려는 사용자의 전자 메일 주소 또는 이름을 입력한 다음 표시되는 목록에서 사용자를 선택하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자가 [!DNL Workfront Fusion]에서 만들어졌습니다.

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (선택 사항) [계속  [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)에서 사용자의 액세스 수준 변경

## Workfront Fusion에서 사용자의 액세스 수준 변경

### 사용자의 역할을 관리자로 변경

사용자에게 관리자 역할을 부여하는 작업은 [!DNL Adobe Admin Console]에서 수행해야 합니다.

1. 사용자를 추가한 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 페이지에서 **[!UICONTROL 관리자]** 탭을 선택합니다.

1. **[!UICONTROL 관리자 추가]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 제품 프로필 관리자 추가]** 상자에 추가할 사용자의 전자 메일 주소 또는 이름을 입력한 다음 표시되는 목록에서 사용자를 선택하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이 사용자는 현재 [!DNL Workfront Fusion]의 관리자입니다.

### 사용자의 역할을 [!UICONTROL 구성원], [!UICONTROL 회계사] 또는 [!UICONTROL 앱 개발자](으)로 변경합니다.

[!UICONTROL 구성원], [!UICONTROL 회계사] 및 [!UICONTROL 앱 개발자] 역할은 [!DNL Workfront Fusion] 내에서 처리됩니다.

자세한 내용은 [조직의 사용자 관리 [!DNL Adobe Workfront Fusion] 관리](../organizations/manage-fusion-users.md) 문서에서 [사용자 역할 보기 또는 편집](../organizations/manage-fusion-users.md#view-or-edit-user-roles)을 참조하십시오.

## [!DNL Adobe Admin Console]의 기존 사용자를 [!DNL Workfront Fusion]에 할당

Fusion에서 기존 사용자를 팀에 추가할 수 있습니다. 이 작업은 Fusion 내에서 처리됩니다.

자세한 내용은 Adobe Workfront Fusion의 조직 또는 팀에 사용자 추가 문서에서 [팀에 사용자 추가](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team)를 참조하십시오.
