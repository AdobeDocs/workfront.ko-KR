---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront] 용  [!DNL Jira]설치'
description: ' [!DNL Adobe Workfront] for [!DNL Jira] 을 사용하여  [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 3%

---

# [!DNL Adobe Workfront for Jira] 설치

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Jira용 Workfront 통합을 사용할 수 없습니다.
>
>Jira와 조직의 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Jira용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Jira 소프트웨어 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)을 참조하십시오.

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

[!DNL Adobe Workfront for Jira]을(를) 사용하여 [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.

추가 기능을 설치한 후 [!DNL Jira]개의 작업 항목을 만들 때 [!DNL Workfront]개의 문제를 자동으로 만드는 워크플로를 정의할 수 있습니다. 두 응용 프로그램의 항목이 연결되고, 두 시스템에서 일부 정보가 자동으로 업데이트됩니다.

[!DNL Workfront] 및 [!DNL Jira]의 모든 사용자가 이 통합을 통해 혜택을 받을 수 있습니다. 가장 많이 사용하는 시스템에 대한 라이선스만 있으면 되고 두 시스템 모두에 대한 라이선스는 필요하지 않습니다.

이 추가 기능은 [!UICONTROL &#x200B; 소프트웨어의 &#x200B;]서버[!UICONTROL &#x200B; 및 &#x200B;]OnDemand[!UICONTROL (또는 &#x200B;]클라우드[!DNL Jira]) 버전에서 사용할 수 있습니다. [!DNL Data Center] 소프트웨어의 [!DNL Jira] 버전에서는 이 추가 기능을 사용할 수 없습니다.

현재 [!DNL Jira]에서 지원하는 [!DNL Workfront for Jira] 버전 목록은 Atlassian Marketplace에서 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)을(를) 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준 </p>
       <p>플랜 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 Jira 및 Workfront에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++## [!DNL Workfront]용 [!DNL Jira] 설치

[!DNL Workfront] OnDemand에 대해 [!DNL Jira]을(를) 설치하는 것은 [!DNL Jira] 서버 인스턴스에 설치하는 것과 동일합니다.

[!DNL Jira] 추가 기능을 설치하려면 [!DNL Workfront] 관리자여야 합니다.

[!DNL Jira] 관리자가 아닌 경우 [!DNL Workfront] 추가 기능을 찾아 설치를 요청할 수 있습니다. 승인 및 설치를 위해 요청을 [!DNL Jira] 관리자에게 보냅니다.

[!DNL Jira] 응용 프로그램에 설치할 추가 기능을 요청하는 방법에 대한 자세한 내용은 [추가 기능에 대한 사용자 요청 관리](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)를 참조하십시오.

[!DNL Workfront for Jira]을(를) 설치하려면

1. [!DNL Jira]에 [!DNL Jira] 관리자로 로그인합니다.
1. **[!DNL Workfront for Jira]**&#x200B;[[!DNL Atlassian Marketplace]&#x200B;에서 &#x200B;](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) 추가 기능을 찾으십시오.

1. 설치하려면 **[!UICONTROL 지금 가져오기]**&#x200B;를 클릭하세요.

   설치가 완료되면 [!DNL Workfront]에서 [!DNL Jira]에 로그인하여 통합을 구성할 수 있습니다.

   자세한 내용은 [Jira용 Adobe Workfront 구성](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하십시오.

## [!DNL Jira Server] 설치 시 고려 사항

>[!NOTE]
>
>이러한 요구 사항은 [!UICONTROL &#x200B; 소프트웨어의 &#x200B;]OnDemand[!UICONTROL (]Cloud[!DNL Jira]) 버전에는 적용되지 않습니다.

두 [!DNL Workfront] 환경에서 [!DNL Jira] 추가 기능을 설치하는 것은 비슷하지만 [!DNL Jira Server] 설치를 사용하여 작업할 때는 다음 사항을 고려해야 합니다.

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
