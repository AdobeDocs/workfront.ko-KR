---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: ' [!DNL Adobe Workfront] 사용자를 위한  [!DNL Salesforce] 섹션 구성'
description: Salesforce용  [!DNL Adobe Workfront] 관리자  [!DNL Workfront] 를 설치한 후 Salesforce의 Opportunity 및 Account 페이지 레이아웃에 새 섹션에 추가하여 사용자에게 제공할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 사용자에 대한 [!DNL Salesforce] 섹션 구성

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Salesforce용 Workfront 통합을 사용할 수 없습니다.
>
>조직의 Salesforce 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Salesforce용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Salesforce 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)을 참조하십시오.

[!DNL Adobe Workfront] 관리자로서 [!DNL Salesforce]용 [!DNL Workfront]을(를) 설치한 후 새 섹션에서 [!UICONTROL 기회] 및 [!UICONTROL 계정]에 추가하여 사용자가 사용할 수 있도록 설정할 수 있습니다.
[!UICONTROL Salesforce]의 페이지 레이아웃.

[!DNL Workfront for Salesforce] 설치에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)를 참조하십시오.

사용자가 [!DNL Workfront] 및 [!DNL Classic] 프레임워크 모두에서 [!DNL Lightning Experience]을(를) 사용할 수 있게 하려면 [!DNL WorkfrontOpportunities] 및 [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] 페이지를 각각 [!UICONTROL Opportunity] 및 [!UICONTROL Accounts] 페이지 레이아웃에 추가해야 합니다.



## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>플랜</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* 시스템 관리자 계정에 액세스할 수 있는 [!DNL Salesforce] 인스턴스가 있어야 합니다.
* 시스템 관리자 계정에 액세스할 수 있는 [!DNL Workfront] 인스턴스가 있어야 합니다.

## [!DNL Workfront] 프레임워크에서 [!DNL Salesforce Classic] 섹션 구성

1. [!DNL Salesforce]에 Workfront 관리자로 로그인합니다.
1. **[!UICONTROL 설정].**&#x200B;을 클릭합니다.
1. **[!UICONTROL 빌드]** 섹션에서 **[!UICONTROL 사용자 지정].**&#x200B;을 확장합니다.

1. **[!UICONTROL 기회]**&#x200B;를 확장한 다음 **[!UICONTROL 페이지 레이아웃]**&#x200B;을 클릭하여 [!DNL Workfront] 섹션을 기회에 추가합니다.

   또는

   **[!UICONTROL 계정]**&#x200B;을 확장한 다음 **[!UICONTROL 페이지 레이아웃]**&#x200B;을 클릭하여 [!DNL Workfront] 섹션을 계정에 추가합니다.
.

1. 기존 레이아웃에서 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

   또는

   새 레이아웃을 추가하려면 **[!UICONTROL 새로 만들기]**&#x200B;를 클릭하세요.

1. (선택 사항) **[!UICONTROL Section]** 구성 요소를 레이아웃으로 끌어서 원하는 위치에 놓습니다.\

1. (선택 사항) 새 섹션의 이름을 지정합니다.

   이 섹션의 이름을 **[!DNL Workfront]**&#x200B;로 지정하는 것이 좋습니다.

1. (선택 사항) 새 섹션에 대해 원하는 **[!UICONTROL 레이아웃]** 및 **[!UICONTROL 탭 키 순서]**&#x200B;를 지정합니다.

   **[!UICONTROL 섹션에 대해]** 1열[!DNL Workfront] 레이아웃을 선택하는 것이 좋습니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 레이아웃]** 영역에서 **[!UICONTROL Visualforce 페이지].**&#x200B;를 클릭합니다.

1. **[!UICONTROL WorkfrontOpportunities]** 구성 요소를 **[!UICONTROL Opportunities]** 레이아웃의 새 섹션으로 끌어다 놓습니다.

   또는

   **[!UICONTROL WorkfrontAccounts]** 구성 요소를 **[!UICONTROL Account]** 레이아웃의 새 섹션으로 끌어다 놓습니다.\

1. 새로 추가된 구성 요소의 오른쪽 상단에 있는 **[!UICONTROL 속성]** 아이콘을 클릭합니다.\

1. 최적의 표시를 하려면 [!DNL Workfront Visualforce] 페이지에 대해 다음 속성을 지정하십시오.

   * **[!UICONTROL 너비(픽셀 또는 %)]**: 100%
   * **[!UICONTROL 높이(픽셀)]**: 600
   * **[!UICONTROL 스크롤 막대 표시]**&#x200B;를 선택합니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭합니다.
1. 레이아웃을 저장하려면 **[!UICONTROL 저장]**&#x200B;을 클릭하세요.

   이 레이아웃이 할당된 모든 사용자는 이제 [!DNL Workfront]기회[!UICONTROL &#x200B; 또는 &#x200B;]계정[!UICONTROL &#x200B; 개체에서 &#x200B;] 섹션을 볼 수 있습니다.

   [!DNL Workfront] 섹션에 [!DNL Workfront] 로그인 화면이 표시됩니다. [!DNL Workfront] 계정이 없는 경우 섹션을 축소할 수 있지만 레이아웃에서 제거할 수는 없습니다.

## [!DNL Workfront] 프레임워크에서 [!DNL Salesforce Lightning Experience] 섹션 구성

[!DNL Workfront] [!DNL Salesforce]기회[!UICONTROL &#x200B; 또는 계정의 레이아웃에 &#x200B;] 섹션을 추가할 수 있습니다.
[!DNL Salesforce Lightning Experience] 프레임워크에서 [!UICONTROL 설정] 영역에 액세스하거나 계정에서 액세스함
또는 [!UICONTROL Opportunity] 개체입니다.

* [&#x200B; [!DNL Workfront] 설정[!UICONTROL &#x200B; 수준에서 &#x200B;]섹션 구성](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [영업 기회 또는 계정 수준에서  [!DNL Workfront] 섹션 구성](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### [!DNL Workfront]설정[!UICONTROL &#x200B; 수준에서 &#x200B;] 섹션 구성 {#configure-the-workfront-section-at-the-setup-level}

1. 시스템 관리자로 [!DNL Salesforce]에 로그인합니다.
1. **[!UICONTROL 설정]** 아이콘을 클릭한 다음 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 개체 및 필드]**&#x200B;를 확장한 다음 **[!UICONTROL 개체 관리자]**&#x200B;를 클릭합니다.

1. 영업 기회의 레이아웃을 사용자 지정하려면 **[!UICONTROL 영업 기회]**&#x200B;를 클릭하십시오.

   또는

   계정의 레이아웃을 사용자 지정하려면 **[!UICONTROL 계정]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL 페이지 레이아웃]**&#x200B;을 클릭합니다.
1. 기존 페이지 레이아웃의 이름을 클릭하여 편집합니다.

   또는

   새 페이지 레이아웃을 만들려면 **[!UICONTROL 새로 만들기]**&#x200B;를 클릭하십시오.

1. 아래 [영업 기회 또는 계정 수준에서  [!DNL Workfront] 섹션 구성](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)을 계속합니다.

### 영업 기회 또는 계정 수준에서 [!DNL Workfront] 섹션 구성 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. 시스템 관리자로 [!DNL Salesforce]에 로그인합니다.
1. **[!UICONTROL 기회]** 또는 **[!UICONTROL 계정]**(으)로 이동합니다.

1. **[!UICONTROL 설정]** 아이콘을 클릭한 다음 **[!UICONTROL 페이지 편집]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 사용자 지정 관리]** 섹션을 확장합니다.
1. **[!DNL Workfront]**&#x200B;기회[!UICONTROL &#x200B; 또는 계정에 &#x200B;] 구성 요소를 끌어다 놓습니다.
페이지를 가리키도록 업데이트하는 중입니다.

   [!DNL Workfront] 섹션에 대해 레이아웃의 열 중 하나 대신 페이지의 전체 너비를 사용하는 것이 좋습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이 레이아웃이 할당된 모든 사용자는 이제 [!DNL Workfront]기회[!UICONTROL &#x200B; 또는 &#x200B;]계정[!UICONTROL &#x200B; 개체에서 &#x200B;] 섹션을 볼 수 있습니다.

   >[!NOTE]
   >
   >[!DNL Workfront] 섹션에 [!DNL Workfront] 로그인 화면이 표시됩니다. [!DNL Workfront] 계정이 없는 경우 섹션을 축소할 수 있지만 레이아웃에서 제거할 수는 없습니다. 사용자는 활성화한 인증 방법(향상된 인증 또는 SAML(Security Assertion Markup Language) URL)을 사용하여 로그인할 수 있습니다.

