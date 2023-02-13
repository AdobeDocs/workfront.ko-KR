---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Admin Console을 통해 Adobe Workfront Fusion에 사용자 추가
description: Adobe Admin Console에 사용자를 추가하고 Adobe Workfront Fusion에 할당하거나 Adobe Admin Console의 기존 사용자를 Workfront Fusion에 할당할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
hidefromtoc: true
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# 사용자 추가 대상 [!DNL Adobe Workfront Fusion] 사용 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 [!DNL Adobe Admin Console].
>
>조직에서 아직 [!DNL Adobe Admin Console]를 참조하십시오. [사용자를 의 조직에 추가 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>조직에서 [!DNL Adobe Admin Console]를 참조하십시오. [플랫폼 기반의 관리 차이점 ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

사용자를 [!DNL Adobe Admin Console] 그리고 그들을 [!DNL Adobe Workfront Fusion]또는 에서 기존 사용자를 할당합니다. [!DNL Adobe Admin Console] to [!DNL Workfront Fusion].

을 설명하는 비디오의 경우 [!DNL Workfront Fusion] 에서 [!DNL Adobe Admin Console]사용자를 추가하는 방법을 포함하여 다음을 참조하십시오. [[!DNL Fusion] 추가 정보](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion] </p> <p>작업 자동화를 위한 [!UICONTROL Workfront Fusion] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 관리자 권한</td> 
   <td>다음 [!UICONTROL 제품 구성 관리자]여야 합니다. [!DNL Adobe] 조직의 제품.</td> 
  </tr>
  </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

&#42;&#42;에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 전제 조건

를 사용하기 전에 [!DNL Admin Console] 대상 [!DNL Workfront]로 로그인하면 콘솔로 초대하는 이메일을 받게 됩니다.

1. 처음 사용하는 경우 [!DNL Adobe] 그리고 이제 관리할 관리 권한이 있음을 알리는 이메일을 수신했습니다 [!DNL Adobe] 조직의 소프트웨어 및 서비스에서 전자 메일의 버튼을 클릭하여 [!DNL Adobe] 계정을 열고 [!DNL Admin Console].

   또는

   이미 Adobe 계정이 있는 경우 [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/).


## 새 사용자를 [!DNL Adobe Admin Console] 및 [!DNL Workfront Fusion]

1. 에서 [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/)에서 을(를) 선택합니다. **[!UICONTROL 제품]** 위쪽 탐색 막대에서 탭을 선택하고 **[!DNL Workfront Fusion]** 제품 타일.

   ![Admin Console에서 융합](assets/fusion-product-admin-console.png)

1. 표시되는 목록에서 사용자를 추가할 조직을 선택합니다.

   ![Admin Console의 Fusion 인스턴스](assets/fusion-instances-admin-console.png)

1. 표시되는 목록에서 **[!UICONTROL 제품 프로필]** 탭을 선택한 다음 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 링크를 클릭합니다.

   ![Workfront Fusion 제품 프로필](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 을 변경하지 마십시오 [!UICONTROL 제품 프로필] 자체.

1. 사용 **[!UICONTROL 사용자]** 목록 위에 있는 탭을 클릭하고 **[!UICONTROL 사용자 추가]**.

1. 에서 **[!UICONTROL 이 제품 프로필에 사용자 추가]** 상자에 추가할 사용자의 이메일 주소나 이름을 입력한 다음 나타나는 목록에서 사용자를 선택합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자는에서 만들어집니다. [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (선택 사항) 계속 [에서 사용자의 액세스 수준 변경 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Workfront Fusion에서 사용자의 액세스 수준 변경

### 사용자의 역할을 관리자로 변경

사용자에게 관리자 역할을 부여하는 것은 [!DNL Adobe Admin Console].

1. 설정 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 사용자를 추가한 페이지에서 **[!UICONTROL 관리자]** 탭.

1. 클릭 **[!UICONTROL 관리자 추가]**.

1. 에서 **[!UICONTROL 제품 프로필 관리자 추가]** 상자에 추가할 사용자의 이메일 주소나 이름을 입력한 다음 나타나는 목록에서 사용자를 선택합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 이 사용자는 [!DNL Workfront Fusion].

### 사용자의 역할을 로 변경 [!UICONTROL 멤버], [!UICONTROL 회계사], 또는 [!UICONTROL 앱 개발자].

[!UICONTROL 멤버], [!UICONTROL 회계사], 및 [!UICONTROL 앱 개발자] 역할은 내에서 처리됨 [!DNL Workfront Fusion].

자세한 내용은 [사용자 역할 보기 또는 편집](../organizations/manage-fusion-users.md#view-or-edit-user-roles) 기사 [관리 [!DNL Adobe Workfront Fusion] 조직의 사용자](../organizations/manage-fusion-users.md)

## 에서 기존 사용자 할당 [!DNL Adobe Admin Console] to [!DNL Workfront Fusion]

1. 문서의 &quot;사용자 세부 사항 편집&quot; 섹션에 설명된 대로 사용자 편집을 시작합니다 [개별 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 에서 [!DNL Adobe Admin Console] 설명서.

1. 추가 **[!DNL Adobe Workfront Fusion]** 사용자에게 할당된 제품으로 마이그레이션합니다.
