---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 설치 [!DNL Adobe Workfront] 대상 [!DNL Salesforce]
description: 앱에서 사용할 수 있게 되기 전에 앱을 설치하려면 다음을 수행하십시오. [!DNL Salesforce] AppExchange, 설치 를 참조하십시오 [!DNL Workfront] Salesforce용 을 사용 중인지 여부에 따라 AppExchange Marketplace에서 사용할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 254ffae14b21dbef19b8f6b66a1c11e348c85c85
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# 설치 [!DNL Adobe Workfront for Salesforce]

앱에서 사용할 수 있게 되기 전에 앱을 설치하려면 다음을 수행하십시오. [!DNL Salesforce AppExchange]를 참조하십시오. [설치 [!DNL Workfront for Salesforce] 다음에서 사용 가능 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

로서의 [!DNL Salesforce] 및 [!DNL Adobe Workfront] 관리자, 설치 [!DNL Workfront for Salesforce] 허용 [!DNL Salesforce] 사용자를 제출합니다. [!DNL Workfront] Salesforce를 종료하지 않고도 프로젝트를 요청 및 자동으로 만들 수 있습니다.

설치 시 얻을 수 있는 사항에 대한 일반적인 이해 [!DNL Workfront for Salesforce]를 참조하십시오. [[!DNL Adobe Workfront for Salesforce] 개요](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [설치 및 사용을 위한 사전 요구 사항 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [설치 [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## 액세스 요구 사항

이 문서에 설명된 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 설치 및 사용을 위한 사전 요구 사항 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 다음을 수행해야 합니다. [!DNL Salesforce] 앱을 설치하기 위해 시스템 관리자 계정에 액세스할 수 있는 인스턴스.
* 다음을 수행해야 합니다. [!DNL Workfront] 통합을 구성하기 위해 시스템 관리자 계정에 액세스할 수 있는 인스턴스
* [!UICONTROL Salesforce] 사용자에게 [!DNL Workfront] 계정을 사용하여

   * 만들기 [!DNL Workfront] 요청 [!DNL Salesforce] 또는
   * 보기 [!DNL Workfront] Salesforce의 요청 또는 프로젝트

## 설치 [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

넌 [!DNL Salesforce] 그리고 [!DNL Workfront] 시스템 관리자가 설치 및 구성 [!DNL Workfront for Salesforce].

다음 하위 섹션에서는 설치 방법을 설명합니다 [!DNL Workfront] 에 대해 [!DNL Salesforce] 프로덕션 환경. 같은 단계에 따라 설치할 수 있습니다 [!DNL Workfront] 에 대해 [!DNL Salesforce] 샌드박스 환경.

* [설치 [!DNL Workfront for Salesforce] 다음에서 사용 가능 [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [설치 [!DNL Workfront for Salesforce] 에서 [!DNL Salesforce Classic] 프레임워크](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [설치 [!DNL Workfront for Salesforce] 에서 [!DNL Salesforce Lightning Experience] 프레임워크](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### 설치 [!DNL Workfront for Salesforce] 다음에서 사용 가능 [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] 은 [!DNL Salesforce AppExchange] 곧.

앱을 사용하기 전에 설치하려면 다음을 수행하십시오.

1. 프로덕션 환경에서 다음 위치로 이동하십시오.

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

   샌드박스 환경에서 다음 위치로 이동합니다.

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

1. 을(를) 확인합니다. **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]** 상자.

   로드 화면이 표시되고 설치하는 데 시간이 걸릴 수 있습니다.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되면

1. 다음으로 이동 **[!UICONTROL 설정>보안 컨트롤>원격 사이트 설정]**.
1. (조건부) [!DNL Workfront] 에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, **[!UICONTROL 새 원격 사이트]**.

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 이름]**.

   For example, *[!DNL Workfront]*.

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 URL]**.

   예, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스 및 **[!UICONTROL WorkfrontOpportunity]** 및 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 페이지가 사용자 환경에서 생성되었습니다.

   [!DNL Salesforce] 사용자는 다음에 앱을 추가하면 [!DNL Workfront] 섹션에 있는 [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃.\
   사용자를 위한 Workfront 섹션 구성에 대한 자세한 내용은 [Salesforce 사용자에 대한 Adobe Workfront 섹션을 구성합니다](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 설치 [!DNL Workfront] 대상 [!DNL Salesforce] 에서 [!DNL Salesforce Classic] 프레임워크

1. 에 로그인합니다. [!DNL Salesforce] 시스템 관리자
1. 이동 **설정.**
1. 에서 **빌드** 섹션을 클릭합니다. **AppExchange 마켓플레이스**.

1. 에서 **검색 AppExchange 앱** 상자, 유형 **Workfront**.

1. 앱이 있을 때 앱을 클릭한 다음 **지금 가져오기**.
1. 클릭 **[!UICONTROL 프로덕션에 설치]** 를 설치하려면 [!DNL Workfront] 앱 [!DNL Salesforce] 프로덕션 환경. (권장)
1. 을(를) 선택합니다 **[!UICONTROL 사용 약관을 읽고 동의함]** 약관을 읽고 동의한 후의 필드입니다.
1. 클릭 **[!UICONTROL 확인 및 설치]**.
1. 선택 **[!UICONTROL 모든 사용자용 설치]** (권장), **[!UICONTROL 설치]**.

1. (조건부) 타사 액세스를 승인할지 묻는 경우 다음을 선택해야 합니다 **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]**&#x200B;를 클릭한 다음 **[!UICONTROL 계속]**.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되면

   다음 [!DNL Workfront] 앱은 아래에 나열됩니다. **[!UICONTROL 설치된 패키지]**.


1. 다음으로 이동 **[!UICONTROL 설정>보안 컨트롤>원격 사이트 설정]**.
1. (조건부) [!DNL Workfront] 에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, **[!UICONTROL 새 원격 사이트]**.\

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 이름]**.\
   For example, *[!DNL Workfront]*.

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 URL]**.\
   예, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스 및 **[!UICONTROL WorkfrontOpportunity]** 및 **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] 페이지가 사용자 환경에서 생성되었습니다.\
   [!DNL Salesforce] 사용자는 [!DNL Workfront] 섹션에 있는 [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃.\
   구성에 대한 자세한 내용은 [!DNL Workfront] 사용자에 대한 섹션을 참조하십시오. [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### 설치 [!DNL Workfront for Salesforce] 에서 [!DNL Salesforce Lightning Experience] 프레임워크

1. 에 로그인합니다. [!DNL Salesforce] 시스템 관리자
1. 을(를) 클릭합니다. **[!UICONTROL 설정] 아이콘**&#x200B;를 클릭한 다음 **[!UICONTROL 설정]**.

1. 에서 **[!UICONTROL 플랫폼 도구]** 섹션, 확장 **[!UICONTROL 앱].**

1. 클릭 **[!DNL AppExchange Marketplace]**.
1. 에서 **[!UICONTROL 검색 [!DNL AppExchange] 앱]** 상자, 유형 **[!DNL Workfront]**.

1. 앱이 있을 때 앱을 클릭한 다음 **[!UICONTROL 지금 가져오기]**.
1. 클릭 **[!UICONTROL 로그인 화면 열기]**.\
   귀하의 [!DNL Workfront] 관리자 계정 [!DNL Salesforce].

1. 클릭 **[!UICONTROL 허용]**.
1. 에서 **[!UICONTROL 이 조직에 설치]** 상자를 클릭하여 **[!UICONTROL 여기에 설치]** 를 설치합니다. [!DNL Workfront] 다음 위치에서 [!DNL Salesforce] 프로덕션 환경. (권장)

1. 을(를) 선택합니다 **[!UICONTROL 사용 약관을 읽고 동의함]** 약관을 읽고 동의한 후의 필드입니다.
1. 클릭 **[!UICONTROL 확인 및 설치]**.
1. 선택 **[!UICONTROL 모든 사용자용 설치]** (권장), **[!UICONTROL 설치]**.

1. (조건부) 타사 액세스를 승인할지 묻는 경우 다음을 선택해야 합니다 **[!UICONTROL 예, 이러한 타사 웹 사이트에 대한 액세스 권한 부여]**&#x200B;를 클릭한 다음 **[!UICONTROL 계속]**.

1. 클릭 **[!UICONTROL 완료]** 설치가 완료되면

   다음 [!DNL Workfront] 앱은 아래에 나열됩니다. **[!UICONTROL 설치된 패키지]**.

1. 다음으로 이동 **[!UICONTROL 설정].**
1. 에서 **[!UICONTROL 설정]** 섹션, &#x200B; 확장&#x200B;**[!UICONTROL 보안].**

1. 클릭 **[!UICONTROL 원격 사이트 설정]**.
1. (조건부) [!DNL Workfront] 에 나열된 URL **[!UICONTROL 모든 원격 사이트]** 목록, **[!UICONTROL 새 원격 사이트]**.

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 이름]**.

   For example, *[!DNL Workfront]*.

1. 을(를) 지정합니다. **[!UICONTROL 원격 사이트 URL]**.

   예, *yourDomain.my.workfront.com*.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   다음 [!DNL Workfront] 이제 앱이 [!DNL Salesforce] 인스턴스 및 **[!DNL Workfront]** 이제 구성 요소가 환경에 추가됩니다.

   [!UICONTROL Salesforce] 사용자는 [!DNL Workfront] 추가되면 앱 [!DNL Workfront] 섹션에 있는 [!UICONTROL 기회] 또는 [!UICONTROL 계정] 페이지 레이아웃.\
   구성에 대한 자세한 내용은 [!DNL Workfront] 사용자에 대한 섹션을 참조하십시오. [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
