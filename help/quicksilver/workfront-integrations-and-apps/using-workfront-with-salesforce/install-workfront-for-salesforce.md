---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 설치 [!DNL Adobe Workfront] 대상 [!DNL Salesforce]
description: 에서 앱을 사용하기 전에 설치하려면 다음을 수행하십시오. [!DNL Salesforce] AppExchange, 설치 참조 [!DNL Workfront] AppExchange 마켓플레이스에서 사용할 수 있게 되기 전의 Salesforce용.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: c0e7340e2bf650b6f9931ae12aee07c5f7d5292b
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# 설치 [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>에서 앱을 사용하기 전에 설치하려면 다음을 수행하십시오. [!DNL Salesforce AppExchange], 참조 [설치 중 [!DNL Workfront for Salesforce] 에서 사용할 수 있게 되기 전에 [!DNL AppExchange] 마켓플레이스](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

로서의 [!DNL Salesforce] 및 [!DNL Adobe Workfront] 관리자, 다음을 설치할 수 있습니다 [!DNL Workfront for Salesforce] 허용 [!DNL Salesforce] 제출할 사용자 [!DNL Workfront] Salesforce를 종료하지 않고 프로젝트를 요청하고 자동으로 만듭니다.

를 설치하여 기대할 수 있는 사항에 대한 일반적인 이해를 위해 [!DNL Workfront for Salesforce], 참조 [[!DNL Adobe Workfront for Salesforce] 개요](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [설치 및 사용을 위한 사전 요구 사항 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [설치 중 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 설치 및 사용을 위한 사전 요구 사항 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 다음 항목이 있어야 합니다. [!DNL Salesforce] 앱을 설치하기 위해 시스템 관리자 계정에 액세스할 수 있는 인스턴스입니다.
* 다음 항목이 있어야 합니다. [!DNL Workfront] 통합을 구성하기 위해 시스템 관리자 계정에 액세스할 수 있는 인스턴스가 추가되었습니다.
* [!UICONTROL Salesforce] 사용자에게 다음이 있어야 함: [!DNL Workfront] 계정 관리:

   * 만들기 [!DNL Workfront] 의 요청 [!DNL Salesforce]
   * 보기 [!DNL Workfront] Salesforce의 요청 또는 프로젝트

## 설치 중 [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

다음이어야 합니다: [!DNL Salesforce] 및 a [!DNL Workfront] 설치 및 구성할 시스템 관리자 [!DNL Workfront for Salesforce].

다음 하위 섹션에서는 설치 방법을 설명합니다 [!DNL Workfront] 에 대한 [!DNL Salesforce] 프로덕션 환경. 동일한 단계에 따라 설치할 수 있습니다 [!DNL Workfront] 에 대한 [!DNL Salesforce] 샌드박스 환경.

* [설치 중 [!DNL Workfront for Salesforce] 에서 사용할 수 있게 되기 전에 [!DNL AppExchange] 마켓플레이스](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [설치 중 [!DNL Workfront for Salesforce] 다음에서 [!DNL Salesforce Classic] 프레임워크](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [설치 중 [!DNL Workfront for Salesforce] 다음에서 [!DNL Salesforce Lightning Experience] 프레임워크](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 설치 중 [!DNL Workfront for Salesforce] 에서 사용할 수 있게 되기 전에 [!DNL AppExchange] 마켓플레이스 {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 다음에서 사용할 수 있습니다. [!DNL Salesforce AppExchange] 곧.

앱을 사용하기 전에 설치하려면:

1. 프로덕션 환경에서 로 이동합니다.

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   샌드박스 환경에서

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >이러한 페이지에 액세스하려면 Salesforce에 로그인해야 합니다.

1. 다음 확인: **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]** 상자.

   로딩 화면이 표시됩니다. 설치하는 데 시간이 걸릴 수 있습니다.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되는 시점입니다.

1. 다음으로 이동 **[!UICONTROL 설정]** > **[!UICONTROL 보안] 컨트롤** > **[!UICONTROL 원격 사이트 설정]**.
1. (조건부) 목록에서 Workfront 를 선택합니다.

   또는

   다음 항목이 표시되지 않으면 [!DNL Workfront] 다음에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, 클릭 **[!UICONTROL 새 원격 사이트]**.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**.

   예를 들어, *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**.

   예를 들어, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스 및 **[!UICONTROL WorkfrontOpportunities]** 및 **[!UICONTROL Workfront 계정]** [!UICONTROL Visualforce] 사용자 환경에서 페이지가 생성되었습니다.

   [!DNL Salesforce] 을(를) 추가하면 사용자는 앱을 사용할 수 있습니다. [!DNL Workfront] 섹션에 추가 [!UICONTROL 영업 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃입니다.\
   사용자를 위한 Workfront 섹션 구성에 대한 자세한 내용은 [Salesforce 사용자를 위한 Adobe Workfront 섹션 구성](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 설치 중 [!DNL Workfront] 대상 [!DNL Salesforce] 다음에서 [!DNL Salesforce Classic] 프레임워크

1. 에 로그인 [!DNL Salesforce] 시스템 관리자입니다.
1. 다음으로 이동 **설정.**
1. 다음에서 **빌드** 섹션, 클릭 **AppExchange 마켓플레이스**.

1. 다음에서 **AppExchange 앱 검색** 상자, 유형 **Workfront**.

1. Workfront 앱을 찾으면 클릭한 다음 **지금 받기**.
1. 클릭 **[!UICONTROL 프로덕션에 설치]** 을(를) 설치하려면 [!DNL Workfront] 의 앱 [!DNL Salesforce] 프로덕션 환경. (권장)
1. 사용 약관을 읽고 동의한 후 **[!UICONTROL 약관을 읽고 동의합니다.]** 필드.
1. 클릭 **[!UICONTROL 확인 및 설치]**.
1. 선택 **[!UICONTROL 모든 사용자용 설치]** (권장) 을 클릭하고 **[!UICONTROL 설치]**.

1. (조건부) 서드파티 액세스를 승인할지 묻는 메시지가 표시되면 다음을 선택해야 합니다 **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 계속]**.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되는 시점입니다.

   다음 [!DNL Workfront] 앱은에 나열되어 있습니다. **[!UICONTROL 설치된 패키지]**.


1. 다음으로 이동 **[!UICONTROL 설정>보안 제어>원격 사이트 설정]**.
1. (조건부) 다음 메시지가 표시되지 않는 경우 [!DNL Workfront] 다음에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, 클릭 **[!UICONTROL 새 원격 사이트]**.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**.
예를 들어, *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**.
예를 들어, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스. 다음 **[!UICONTROL WorkfrontOpportunities]** 및 **[!UICONTROL Workfront 계정]** [!UICONTROL Visualforce] 귀하의 환경에서 페이지가 작성되었습니다.\
   [!DNL Salesforce] 을(를) 추가할 때까지 사용자는 아직 앱을 사용할 수 없습니다. [!DNL Workfront] 섹션에 추가 [!UICONTROL 영업 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃입니다.\
   구성에 대한 자세한 내용은 [!DNL Workfront] 사용자 섹션은 다음을 참조하십시오. [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 설치 중 [!DNL Workfront for Salesforce] 다음에서 [!DNL Salesforce Lightning Experience] 프레임워크

1. 에 로그인 [!DNL Salesforce] 시스템 관리자입니다.
1. 다음을 클릭합니다. **[!UICONTROL 설정] 아이콘**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]**.

1. 다음에서 **[!UICONTROL 플랫폼 도구]** 섹션, 확장 **[!UICONTROL 앱].**

1. 클릭 **[!DNL AppExchange Marketplace]**.
1. 다음에서 **[!UICONTROL 검색 [!DNL AppExchange] 앱]** 상자, 유형 **[!DNL Workfront]**.

1. Workfront 앱을 찾으면 클릭한 다음 **지금 받기**.
1. 클릭 **[!UICONTROL 로그인 화면 열기]**.\
   다음으로 로그인해야 합니다. [!DNL Workfront] 관리자 계정 [!DNL Salesforce].

1. 클릭 **[!UICONTROL 허용]**.
1. 다음에서 **[!UICONTROL 이 조직에 설치]** 상자, 클릭 **[!UICONTROL 여기에 설치]** 설치하려면 [!DNL Workfront] (으)로 [!DNL Salesforce] 프로덕션 환경. (권장)

1. 사용 약관을 읽고 동의한 후 **[!UICONTROL 약관을 읽고 동의합니다.]** 필드.
1. 클릭 **[!UICONTROL 확인 및 설치]**.
1. 선택 **[!UICONTROL 모든 사용자용 설치]** (권장) 을 클릭하고 **[!UICONTROL 설치]**.

1. (조건부) 서드파티 액세스를 승인할지 묻는 메시지가 표시되면 다음을 선택해야 합니다 **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 계속]**.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되는 시점입니다.

   다음 [!DNL Workfront] 앱은에 나열되어 있습니다. **[!UICONTROL 설치된 패키지]**.

1. 다음으로 이동 **[!UICONTROL 설정].**
1. 다음에서 **[!UICONTROL 설정]** 섹션, 확장 **[!UICONTROL 보안].**

1. 클릭 **[!UICONTROL 원격 사이트 설정]**.
1. (조건부) 다음 메시지가 표시되지 않는 경우 [!DNL Workfront] 다음에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, 클릭 **[!UICONTROL 새 원격 사이트]**.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 이름]**.
예를 들어, *[!DNL Workfront]*.

1. (조건부) 사이트를 추가하는 경우 **[!UICONTROL 원격 사이트 URL]**.
예를 들어, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스 및 **[!DNL Workfront]** 이제 구성 요소가 환경에 추가됩니다.

   [!UICONTROL Salesforce] 사용자는 [!DNL Workfront] 앱을 추가한 후 [!DNL Workfront] 섹션에 추가 [!UICONTROL 영업 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃입니다.\
   구성에 대한 자세한 내용은 [!DNL Workfront] 사용자 섹션은 다음을 참조하십시오. [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
