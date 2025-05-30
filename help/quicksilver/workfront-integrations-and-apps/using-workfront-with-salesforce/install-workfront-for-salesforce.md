---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: ' [!DNL Salesforce]용  [!DNL Adobe Workfront] 설치'
description: ' [!DNL Salesforce] AppExchange에서 앱을 사용하기 전에 설치하려면 AppExchange 마켓플레이스에서 앱을 사용하기 전에 Salesforce용 설치 [!DNL Workfront] 를 참조하십시오.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: b088c305cbd16aea1b6b79a9f3a9c5ac326cd0b8
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# [!DNL Adobe Workfront for Salesforce] 설치

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>[!DNL Salesforce AppExchange]에서 앱을 사용하기 전에 설치하려면 [설치 [!DNL Workfront for Salesforce] 를 참조하여  [!DNL AppExchange] 마켓플레이스](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)에서 앱을 사용할 수 있습니다.

[!DNL Salesforce] 및 [!DNL Adobe Workfront] 관리자는 [!DNL Workfront for Salesforce]을(를) 설치하여 [!DNL Salesforce] 사용자가 Salesforce를 종료하지 않고 [!DNL Workfront]개의 요청을 제출하고 프로젝트를 자동으로 만들 수 있습니다.

[!DNL Workfront for Salesforce]을(를) 설치하여 예상할 수 있는 사항에 대한 일반적인 이해는 [[!DNL Adobe Workfront for Salesforce] 개요](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md)를 참조하십시오.

* [ [!DNL Workfront for Salesforce]을(를) 설치 및 사용하기 위한 필수 구성 요소](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [ [!DNL Workfront for Salesforce] 설치 중](#installing-workfrontfor-salesforce)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서에 설명된 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront for Salesforce]을(를) 설치 및 사용하기 위한 필수 구성 요소 {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 앱을 설치하려면 시스템 관리자 계정에 액세스할 수 있는 [!DNL Salesforce] 인스턴스가 있어야 합니다.
* 통합을 구성하려면 시스템 관리자 계정에 액세스할 수 있는 [!DNL Workfront] 인스턴스가 있어야 합니다.
* [!UICONTROL Salesforce] 사용자가 [!DNL Workfront] 계정을 가지고 있어야 다음 작업을 수행할 수 있습니다.

   * [!DNL Salesforce]에서 [!DNL Workfront]개 요청 만들기
   * Salesforce에서 [!DNL Workfront]개의 요청 또는 프로젝트 보기

## [!DNL Workfront for Salesforce] 설치 중 {#installing-workfront-for-salesforce}

[!DNL Workfront for Salesforce]을(를) 설치하고 구성하려면 [!DNL Salesforce] 및 [!DNL Workfront] 시스템 관리자여야 합니다.

다음 하위 섹션에서는 [!DNL Salesforce] 프로덕션 환경에 [!DNL Workfront]을(를) 설치하는 방법을 설명합니다. 동일한 단계에 따라 [!DNL Salesforce] 샌드박스 환경에 [!DNL Workfront]을(를) 설치할 수 있습니다.

* [ [!DNL AppExchange] 마켓플레이스에서 사용할 수 있게 되기 전에  [!DNL Workfront for Salesforce] 설치](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [ [!DNL Salesforce Classic] 프레임워크에  [!DNL Workfront for Salesforce] 을(를) 설치하는 중](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [ [!DNL Salesforce Lightning Experience] 프레임워크에  [!DNL Workfront for Salesforce] 을(를) 설치하는 중](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### [!DNL AppExchange] 마켓플레이스에서 [!DNL Workfront for Salesforce]을(를) 사용하려면 먼저 설치 {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce]은(는) 곧 [!DNL Salesforce AppExchange]에서 사용할 수 있습니다.

앱을 사용하기 전에 설치하려면:

1. 프로덕션 환경에서 로 이동합니다.

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   샌드박스 환경에서

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >이러한 페이지에 액세스하려면 Salesforce에 로그인해야 합니다.

1. **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]** 상자를 선택합니다.

   로딩 화면이 표시됩니다. 설치하는 데 시간이 걸릴 수 있습니다.

1. 설치가 완료되면 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 보안] 제어** > **[!UICONTROL 원격 사이트 설정]**(으)로 이동합니다.
1. (조건부) 목록에서 Workfront 를 선택합니다.

   또는

   **[!UICONTROL 모든 원격 사이트]** 목록에 [!DNL Workfront] URL이 표시되지 않으면 **[!UICONTROL 새 원격 사이트]**&#x200B;를 클릭합니다.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**&#x200B;을(를) 지정하십시오.

   예: *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**&#x200B;을(를) 지정하십시오.

   예: *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   [!DNL Workfront] 앱이 이제 [!DNL Salesforce] 인스턴스에 설치되고 **[!UICONTROL WorkfrontOpportunities]** 및 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 페이지가 환경에 만들어졌습니다.

   [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃에 [!DNL Workfront] 섹션을 추가하면 [!DNL Salesforce] 사용자가 앱을 사용할 수 있습니다.\
   사용자를 위한 Workfront 섹션 구성에 대한 자세한 내용은 [Salesforce 사용자를 위한 Adobe Workfront 섹션 구성](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)을 참조하십시오.

### [!DNL Salesforce Classic] 프레임워크에서 [!DNL Salesforce]에 대해 [!DNL Workfront]을(를) 설치하는 중

1. 시스템 관리자로 [!DNL Salesforce]에 로그인합니다.
1. **설정으로 이동**
1. **빌드** 섹션에서 **AppExchange 마켓플레이스**&#x200B;를 클릭합니다.

1. **AppExchange 앱 검색** 상자에 **Workfront**&#x200B;을 입력하십시오.

1. Workfront 앱을 찾으면 클릭한 다음 **지금 가져오기**&#x200B;를 클릭합니다.
1. [!DNL Salesforce] 프로덕션 환경에 [!DNL Workfront] 앱을 설치하려면 **[!UICONTROL 프로덕션에 설치]**&#x200B;를 클릭하십시오. (권장)
1. 사용 약관을 읽고 동의한 후에는 **[!UICONTROL 사용 약관을 읽고 동의합니다]** 필드를 사용하도록 설정하십시오.
1. **[!UICONTROL 확인 및 설치]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 모든 사용자에 대해 설치]**(권장)를 선택한 다음 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.

1. (조건부) 서드파티 액세스를 승인할지 묻는 메시지가 표시되면 **[!UICONTROL 예, 이러한 서드파티 웹 사이트에 대한 액세스 권한 부여]**&#x200B;를 선택한 다음 **[!UICONTROL 계속]**&#x200B;을 클릭해야 합니다.

1. 설치가 완료되면 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

   [!DNL Workfront] 앱은 **[!UICONTROL 설치된 패키지]** 아래에 나열됩니다.


1. **[!UICONTROL 설정>보안 컨트롤>원격 사이트 설정]**(으)로 이동합니다.
1. (조건부) **[!UICONTROL 모든 원격 사이트]** 목록에 [!DNL Workfront] URL이 표시되지 않으면 **[!UICONTROL 새 원격 사이트]**&#x200B;를 클릭합니다.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**&#x200B;을(를) 지정하십시오.
예: *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**&#x200B;을(를) 지정하십시오.
예: *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   [!DNL Workfront] 앱이 이제 [!DNL Salesforce] 인스턴스에 설치되었습니다. **[!UICONTROL WorkfrontOpportunities]** 및 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 페이지가 환경에 만들어졌습니다.\
   [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃에 [!DNL Workfront] 섹션을 추가할 때까지 [!DNL Salesforce] 사용자가 아직 앱을 사용할 수 없습니다.\
   사용자의 [!DNL Workfront] 섹션 구성에 대한 자세한 내용은 [사용자 [!DNL Salesforce] 의  [!DNL Adobe Workfront] 섹션 구성](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)을 참조하십시오.

### [!DNL Salesforce Lightning Experience] 프레임워크에 [!DNL Workfront for Salesforce]을(를) 설치하는 중

1. 시스템 관리자로 [!DNL Salesforce]에 로그인합니다.
1. **[!UICONTROL 설정] 아이콘**&#x200B;을 클릭한 다음 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 플랫폼 도구]** 섹션에서 **[!UICONTROL 앱].**&#x200B;을 확장합니다.

1. **[!DNL AppExchange Marketplace]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL 앱 [!DNL AppExchange]개 검색]** 상자에 **[!DNL Workfront]**&#x200B;을(를) 입력하십시오.

1. Workfront 앱을 찾으면 클릭한 다음 **지금 가져오기**&#x200B;를 클릭합니다.
1. **[!UICONTROL 로그인 화면 열기]**&#x200B;를 클릭합니다.\
   [!DNL Salesforce]의 [!DNL Workfront] 관리자 계정으로 로그인해야 합니다.

1. **[!UICONTROL 허용]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 이 조직에 설치]** 상자에서 **[!UICONTROL 여기 설치]**&#x200B;를 클릭하여 [!DNL Salesforce] 프로덕션 환경에 [!DNL Workfront]을(를) 설치합니다. (권장)

1. 사용 약관을 읽고 동의한 후에는 **[!UICONTROL 사용 약관을 읽고 동의합니다]** 필드를 사용하도록 설정하십시오.
1. **[!UICONTROL 확인 및 설치]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 모든 사용자에 대해 설치]**(권장)를 선택한 다음 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.

1. (조건부) 서드파티 액세스를 승인할지 묻는 메시지가 표시되면 **[!UICONTROL 예, 이러한 서드파티 웹 사이트에 대한 액세스 권한 부여]**&#x200B;를 선택한 다음 **[!UICONTROL 계속]**&#x200B;을 클릭해야 합니다.

1. 설치가 완료되면 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

   [!DNL Workfront] 앱은 **[!UICONTROL 설치된 패키지]** 아래에 나열됩니다.

1. **[!UICONTROL 설치].**(으)로 이동
1. **[!UICONTROL 설정]** 섹션에서 **[!UICONTROL 보안].**&#x200B;을 확장합니다.

1. **[!UICONTROL 원격 사이트 설정]**&#x200B;을 클릭합니다.
1. (조건부) **[!UICONTROL 모든 원격 사이트]** 목록에 [!DNL Workfront] URL이 표시되지 않으면 **[!UICONTROL 새 원격 사이트]**&#x200B;를 클릭합니다.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**&#x200B;을(를) 지정하십시오.
예: *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**&#x200B;을(를) 지정하십시오.
예: *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 [!DNL Workfront] 앱이 [!DNL Salesforce] 인스턴스에 설치되고 **[!DNL Workfront]** 구성 요소가 환경에 추가됩니다.

   [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃에 [!DNL Workfront] 섹션을 추가하면 [!UICONTROL Salesforce] 사용자가 [!DNL Workfront] 앱을 사용할 수 있습니다.\
   사용자의 [!DNL Workfront] 섹션 구성에 대한 자세한 내용은 [사용자 [!DNL Salesforce] 의  [!DNL Adobe Workfront] 섹션 구성](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)을 참조하십시오.

## Salesforce용 Workfront 통합에 대한 권한 구성

### `workfront_business`에 대한 권한

1. **설정** > **보안** > **신뢰할 수 있는 URL**&#x200B;로 이동합니다.
1. 목록에서 `workfront_business`을(를) 선택합니다.
1. **편집**&#x200B;을 클릭합니다.
1. CSP 지시문에서 다음 옵션을 확인합니다.

   * connect-src(스크립트)
   * font-src(글꼴)
   * frame-src (iframe 콘텐츠)
   * img-src (이미지)
   * media-src(오디오 및 비디오)
   * style-src(스타일시트)

1. **저장**&#x200B;을 클릭합니다.


### workfront_session 권한

1. **설정** > **보안** > **신뢰할 수 있는 URL**&#x200B;로 이동합니다.
1. 목록에서 `workfront_session`을(를) 선택합니다.
1. **편집**&#x200B;을 클릭합니다.
1. CSP 지시문에서 다음 옵션을 확인합니다.

   * connect-src(스크립트)
   * font-src(글꼴)
   * frame-src (iframe 콘텐츠)
   * img-src (이미지)
   * media-src(오디오 및 비디오)
   * style-src(스타일시트)

1. **저장**&#x200B;을 클릭합니다.

