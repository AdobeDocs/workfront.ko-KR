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
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 1%

---

# 에 사용자 추가 [!DNL Adobe Workfront Fusion] 다음을 통해 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 로 온보딩된 조직에만 적용됩니다. [!DNL Adobe Admin Console].
>
>조직에서 아직 온보딩되지 않은 경우 [!DNL Adobe Admin Console], 참조 [에서 조직에 사용자 추가 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>조직이 로 온보딩되었는지 여부에 따라 다른 절차 목록 [!DNL Adobe Admin Console], 참조 [플랫폼 기반 관리의 차이점 ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

에 사용자를 추가할 수 있습니다. [!DNL Adobe Admin Console] 할당 대상 [!DNL Adobe Workfront Fusion]또는에서 기존 사용자를 할당합니다. [!DNL Adobe Admin Console] 끝 [!DNL Workfront Fusion].

비디오 설명 [!DNL Workfront Fusion] 다음에서 [!DNL Adobe Admin Console], 사용자 추가 방법을 포함하여 을 참조하십시오. [[!DNL Fusion] Adobe IMS에서](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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
   <tr> 
   <td role="rowheader">[!DNL Adobe] 관리자 권한</td> 
   <td>의 [!UICONTROL 제품 구성 관리자]여야 합니다. [!DNL Adobe] 조직에 대한 제품입니다.</td> 
  </tr>
  </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

&#42;&#42;다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 전제 조건

를 사용하기 전에 [!DNL Admin Console] 대상 [!DNL Workfront]에 콘솔로 초대하는 이메일이 전송됩니다.

1. 을(를) 처음 사용하는 경우 [!DNL Adobe] 이제 관리할 권한이 있다는 이메일이 전송되었습니다. [!DNL Adobe] 조직을 위한 소프트웨어 및 서비스를 만들려면 이메일의 버튼을 클릭하고 [!DNL Adobe] 계정 및 열기 [!DNL Admin Console].

   또는

   이미 Adobe 계정이 있는 경우 [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/).


## 에 새 사용자 추가 [!DNL Adobe Admin Console] 및 [!DNL Workfront Fusion]

1. 다음에서 [[!DNL Adobe Admin Console] 페이지](https://adminconsole.adobe.com/)를 선택하고 **[!UICONTROL 제품]** 맨 위 탐색 막대에서 탭을 선택한 다음 **[!DNL Workfront Fusion]** 제품 타일.

   ![Admin Console의 Fusion](assets/fusion-product-admin-console.png)

1. 표시되는 목록에서 사용자를 추가하려는 조직을 선택합니다.

   ![Admin Console의 Fusion 인스턴스](assets/fusion-instances-admin-console.png)

1. 표시되는 목록에서 **[!UICONTROL 제품 프로필]** 탭을 선택하고 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 링크를 클릭합니다.

   ![Workfront Fusion 제품 프로필](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 을(를) 변경하지 마십시오 [!UICONTROL 제품 프로필] 그 자체.

1. 포함 **[!UICONTROL 사용자]** 목록 위에서 선택한 탭을 클릭하고 **[!UICONTROL 사용자 추가]**.

1. 다음에서 **[!UICONTROL 이 제품 프로필에 사용자 추가]** 상자에서 추가하려는 사용자의 이메일 주소 또는 이름을 입력한 다음 표시되는 목록에서 사용자를 선택합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자는에서 생성됩니다. [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (선택 사항) 계속 [에서 사용자의 액세스 수준 변경 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Workfront Fusion에서 사용자의 액세스 수준 변경

### 사용자의 역할을 관리자로 변경

사용자에게 관리자 역할을 부여하는 작업은 [!DNL Adobe Admin Console].

1. 다음에서 [!DNL Workfront Fusion] [!UICONTROL 제품 프로필] 사용자를 추가한 페이지에서 **[!UICONTROL 관리자]** 탭.

1. 클릭 **[!UICONTROL 관리자 추가]**.

1. 다음에서 **[!UICONTROL 제품 프로필 관리자 추가]** 상자에서 추가하려는 사용자의 이메일 주소 또는 이름을 입력한 다음 표시되는 목록에서 사용자를 선택합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이 사용자는 이제 의 관리자입니다. [!DNL Workfront Fusion].

### 사용자의 역할을 다음으로 변경 [!UICONTROL 멤버], [!UICONTROL 회계사], 또는 [!UICONTROL 앱 개발자].

[!UICONTROL 멤버], [!UICONTROL 회계사], 및 [!UICONTROL 앱 개발자] 역할은 내에서 처리됩니다. [!DNL Workfront Fusion].

자세한 내용은 [사용자 역할 보기 또는 편집](../organizations/manage-fusion-users.md#view-or-edit-user-roles) 이 문서에서 [관리 [!DNL Adobe Workfront Fusion] 조직의 사용자](../organizations/manage-fusion-users.md)

## 에서 기존 사용자 할당 [!DNL Adobe Admin Console] 끝 [!DNL Workfront Fusion]

1. 문서의 &quot;사용자 세부 정보 편집&quot; 섹션에 설명된 대로 사용자 편집을 시작합니다 [개별적으로 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 다음에서 [!DNL Adobe Admin Console] 설명서를 참조하십시오.

1. 추가 **[!DNL Adobe Workfront Fusion]** (사용자에게 할당된 제품)
