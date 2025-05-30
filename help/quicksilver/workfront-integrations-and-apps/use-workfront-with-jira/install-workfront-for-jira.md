---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Jira]용  [!DNL Adobe Workfront] 설치'
description: ' [!DNL Adobe Workfront] for [!DNL Jira] 을 사용하여  [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Jira] 설치

[!DNL Adobe Workfront for Jira]을(를) 사용하여 [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.

추가 기능을 설치한 후 [!DNL Workfront]개의 작업 항목을 만들 때 [!DNL Jira]개의 문제를 자동으로 만드는 워크플로를 정의할 수 있습니다. 두 응용 프로그램의 항목이 연결되고, 두 시스템에서 일부 정보가 자동으로 업데이트됩니다.

[!DNL Workfront] 및 [!DNL Jira]의 모든 사용자가 이 통합을 통해 혜택을 받을 수 있습니다. 가장 많이 사용하는 시스템에 대한 라이선스만 있으면 되고 두 시스템 모두에 대한 라이선스는 필요하지 않습니다.

이 추가 기능은 [!DNL Jira] 소프트웨어의 [!UICONTROL 서버] 및 [!UICONTROL OnDemand] (또는 [!UICONTROL 클라우드]) 버전에서 사용할 수 있습니다. [!DNL Jira] 소프트웨어의 [!DNL Data Center] 버전에서는 이 추가 기능을 사용할 수 없습니다.

현재 [!DNL Workfront for Jira]에서 지원하는 [!DNL Jira] 버전 목록은 Atlassian Marketplace에서 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview)을(를) 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> 
   <p>새로 만들기: 모두</p>
   <p>현재: [!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] 라이선스 개요</td> 
   <td> 
   <p>새로운 기능: 표준</p>
   <p>현재: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 [!DNL Jira] 및 [!DNL Workfront]에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 사용하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>[!DNL Workfront] 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Jira]에 대해 [!DNL Workfront] 설치

[!DNL Jira] OnDemand에 대해 [!DNL Workfront]을(를) 설치하는 것은 [!DNL Jira] 서버 인스턴스에 설치하는 것과 동일합니다.

[!DNL Workfront] 추가 기능을 설치하려면 [!DNL Jira] 관리자여야 합니다.

[!DNL Jira] 관리자가 아닌 경우 [!DNL Workfront] 추가 기능을 찾아 설치를 요청할 수 있습니다. 승인 및 설치를 위해 요청을 [!DNL Jira] 관리자에게 보냅니다.

[!DNL Jira] 응용 프로그램에 설치할 추가 기능을 요청하는 방법에 대한 자세한 내용은 [추가 기능에 대한 사용자 요청 관리](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)를 참조하십시오.

[!DNL Workfront for Jira]을(를) 설치하려면

1. [!DNL Jira]에 [!DNL Jira] 관리자로 로그인합니다.
1. [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview)에서 **[!DNL Workfront for Jira]** 추가 기능을 찾으십시오.

1. 설치하려면 **[!UICONTROL 지금 가져오기]**&#x200B;를 클릭하세요.

   설치가 완료되면 [!DNL Jira]에서 [!DNL Workfront]에 로그인하여 통합을 구성할 수 있습니다.

   자세한 내용은 [Jira용 Adobe Workfront 구성](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하십시오.

## [!DNL Jira Server] 설치 시 고려 사항

>[!NOTE]
>
>이러한 요구 사항은 [!DNL Jira] 소프트웨어의 [!UICONTROL OnDemand] ([!UICONTROL Cloud]) 버전에는 적용되지 않습니다.

두 [!DNL Jira] 환경에서 [!DNL Workfront] 추가 기능을 설치하는 것은 비슷하지만 [!DNL Jira Server] 설치를 사용하여 작업할 때는 다음 사항을 고려해야 합니다.

* [!DNL Jira]에서 추가 기능을 구성할 때 **[!DNL JIRA Base URL]** 필드에 지정된 주소가 개인 서버에서 [!DNL Jira]에 액세스하는 데 사용하는 URL과 다를 수 있습니다. **[!DNL JIRA Base URL]**&#x200B;은(는) NAT 또는 역방향 프록시 프로토콜을 사용하여 개인 서버에 공개적으로 액세스할 수 있는 주소여야 합니다. [!DNL Workfront]이(가) 이 주소에 액세스하여 서버에 요청할 수 있습니다.

* [!DNL Jira]과(와) [!DNL Workfront] 간의 통신을 보호하려면 SSL 암호화를 사용해야 합니다. SSL을 활성화할 때 인증 기관의 전체 SSL 인증서 스택이 있어야 합니다. 자체 서명된 인증서는 지원하지 않습니다.
* 회사 서버에서 [!DNL jira.workfront.com] 도메인에 액세스할 수 있는지 확인해야 합니다. [!DNL Workfront]에서 [!DNL Jira] 사이의 미들웨어 환경 역할을 하며 추가 기능을 작동하는 데 필요합니다.

  아웃바운드 및 인바운드 연결을 위해 다음 고정 IP 주소를 방화벽의 허용 목록에 추가하다에 추가해야 합니다.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  [!DNL Workfront]에서 최적의 기능을 위해 방화벽을 구성하는 방법에 대한 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.
