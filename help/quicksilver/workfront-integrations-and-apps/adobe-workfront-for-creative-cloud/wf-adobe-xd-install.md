---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: XD용 Adobe Workfront 설치 및 열기
description: Adobe 마켓플레이스에서 XD용 Adobe Workfront 플러그인을 설치할 수 있습니다.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: c21e1c1d8e45b7c6407e8741b31055bfed9f4717
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 2%

---

# [!DNL Adobe Workfront for XD] 설치 및 열기

Adobe 마켓플레이스에서 [!DNL Adobe Workfront for XD] 플러그인을 설치할 수 있습니다. 플러그인은 다음 언어를 지원합니다.

* 영어
* 프랑스어
* 독일어
* 이탈리아어
* 스페인어
* 포르투갈어
* 일본어
* 중국어 간체
* 중국어 번체
* 한국어

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package/td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Standard</p>
    <p>Work or higher</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td><p>[!DNL Adobe Creative Cloud] 라이선스 외에 [!DNL Workfront] 라이선스가 있어야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

* Workfront 플러그인을 설치하기 전에 [!DNL Adobe XD] 앱을 설치해야 합니다.

## 조직에 대한 [!DNL Adobe Workfront for XD] 플러그 인 설치

[!DNL Adobe Admin Console] 관리자인 경우 [!DNL Creative Cloud] 배포 패키지에 플러그인을 포함할 수 있습니다. 자세한 내용은 [패키지에 플러그인 포함](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html)을 참조하십시오.

[비디오 튜토리얼은 여기에서 봅니다](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console] 관리자는 사용자에게 배포할 플러그 인 전용 패키지를 만들 수도 있습니다. 자세한 내용은 [에서 사용자의  [!DNL Adobe Workfront] [!UICONTROL [!DNL Creative Cloud]] for [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)패키지 만들기를 참조하십시오.

## 개별적으로 [!DNL Adobe Workfront for XD] 플러그 인을 설치하십시오.

[!DNL Adobe Workfront for XD]에서 직접 [!DNL Adobe Exchange] 플러그인을 설치할 수 있습니다.

1. Adobe Exchange의 [XD용 Adobe Workfront 설치 페이지](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&workflow=share)&#x200B;(으)로 이동합니다.
1. 표시되는 대화 상자에서 **데스크톱 앱 [!DNL Adobe Creative Cloud] 열기**&#x200B;를 클릭합니다.
1. [!DNL Adobe XD] 플러그 인 관리자가 열리면 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.
1. 대화 상자에서 정보를 읽은 다음 **[!UICONTROL 확인]**&#x200B;을 클릭합니다.
1. 플러그인을 여는 방법에 대한 자세한 내용은 다음 섹션을 계속하십시오.

## [!DNL Adobe Workfront for XD] 플러그 인을 엽니다.

1. [!DNL Adobe XD] 열기

1. 새 파일을 만들거나 기존 파일을 엽니다.

1. 왼쪽 하단 모서리에서 **Plugins** 아이콘을 클릭합니다.

![XD 플러그 인 창](assets/xd-plugin-window-350x620.png)

1. **[!UICONTROL 플러그인 패널]**&#x200B;에서 **[!UICONTROL XD용 Adobe Workfront]**&#x200B;를 찾으십시오.

1. 플러그인에 로그인하는 방법에 대한 자세한 내용은 다음 섹션을 계속하십시오.

## [!DNL Adobe Workfront for XD]에 로그인

1. 플러그 인 패널이 열려 있는지 확인한 다음 **[!DNL Adobe Workfront for XD]**&#x200B;을(를) 클릭합니다.
1. 도메인을 입력한 다음 **[!UICONTROL 로그인]**&#x200B;을 클릭합니다. 브라우저 페이지가 열립니다.

   >[!TIP]
   >
   >* 도메인을 찾으려면 브라우저를 열고 [!DNL Workfront] 인스턴스로 이동한 다음 URL의 첫 부분을 복사합니다.\
   >![도메인 찾기](assets/domain-350x50.png)
   >
   >* Workfront 인스턴스가 Experience Cloud과 통합되고 도메인이 `experience.adobe.com`(으)로 시작하는 경우 관리자에게 Admin Console의 제품 > Workfront 아래에 있는 Workfront 도메인을 제공하도록 요청하십시오.

1. 브라우저에서 [!DNL Adobe] 자격 증명을 입력한 다음 **[!DNL Log in]**&#x200B;을(를) 클릭합니다. 회사에서 SSO(Single Sign-On)를 사용하는 경우, 로그인할 SSO 공급자의 페이지로 이동합니다.

   >[!NOTE]
   >
   >최근에 로그인한 경우 [!DNL Workfront] 자격 증명을 입력하라는 메시지가 표시되지 않을 수 있습니다.

1. 메시지에 따라 [!DNL Workfront]에 로그인합니다.

   >[!NOTE]
   >
   >* [!DNL Workfront]은(는) 사용자의 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 보안 표준인 OAuth 2.0을 사용하여 [!DNL Adobe Creative Cloud]에 연결합니다.

1. 로그인을 완료하려면 **[!UICONTROL 액세스 허용]**&#x200B;을 클릭하고 작업을 보려면 [!DNL Adobe XD]&#x200B;(으)로 돌아가세요.

### 로그인 오류 문제 해결

로그인하려고 할 때 **&quot;문제가 발생했습니다&quot; 오류가 표시됩니다.**


`experience.adobe.com`(으)로 시작하는 URL을 사용하여 플러그인에 로그인할 수 없습니다.

![로그인 오류](assets/plugin-log-in-error.png) ![도메인](assets/incorrect-domain.png)


이 문제를 해결하려면,

1. Adobe Workfront for XD 플러그인을 제거하고 다시 설치하여 도메인 및 오류를 지웁니다.

1. Workfront 도메인을 입력합니다. 도메인은 `company-name.my.workfront.com`이(가) 아닌 `experience.adobe.com`이어야 합니다.

Adobe 통합 경험을 사용하는 경우 Workfront 도메인을 찾으려면 다음으로 이동합니다.
