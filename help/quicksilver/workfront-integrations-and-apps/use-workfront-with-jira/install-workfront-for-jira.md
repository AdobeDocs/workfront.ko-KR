---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 설치 [!DNL Adobe Workfront] 대상 [!DNL Jira]
description: 다음을 사용할 수 있습니다. [!DNL Adobe Workfront] 대상 [!DNL Jira] 를 [!DNL Jira] 및 [!DNL Workfront] 시스템.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 설치 [!DNL Adobe Workfront for Jira]

다음을 사용할 수 있습니다. [!DNL Adobe Workfront for Jira] 를 [!DNL Jira] 및 [!DNL Workfront] 시스템.

추가 기능을 설치한 후 다음을 만드는 워크플로를 정의할 수 있습니다. [!DNL Jira] 다음과 같은 경우 자동으로 문제 발생 [!DNL Workfront] 작업 항목이 만들어집니다. 두 응용 프로그램의 항목이 연결되고, 두 시스템에서 일부 정보가 자동으로 업데이트됩니다.

의 모든 사용자 [!DNL Workfront] 및 [!DNL Jira] 은 이 통합의 이점을 얻을 수 있습니다. 가장 많이 사용하는 시스템에 대한 라이선스만 있으면 되고 두 시스템 모두에 대한 라이선스는 필요하지 않습니다.

이 추가 기능은 [!UICONTROL 서버] 및 [!UICONTROL OnDemand] (또는 [!UICONTROL 클라우드]) 버전 [!DNL Jira] 소프트웨어. 이 추가 기능은 다음에 사용할 수 없습니다. [!DNL Data Center] 버전 [!DNL Jira] 소프트웨어.

의 목록 [!DNL Jira] 버전 [!DNL Workfront for Jira] 현재 지원됨, 참조 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 아틀라시안 마켓플레이스에서.

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
   <td> <p>시스템 관리자 액세스</p> <p>중요:에서 별도의 시스템 관리자 계정을 만드는 것이 좋습니다. [!DNL Jira] 및 [!DNL Workfront] 사용자에게 첨부할 수 있는 기존 통합 대신 이 통합 전용.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>다음이어야 합니다: [!DNL Workfront] 관리자.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 설치 [!DNL Workfront] 대상 [!DNL Jira]

설치 중 [!DNL Workfront] 대상 [!DNL Jira] OnDemand는 [!DNL Jira] 서버 인스턴스.

다음이어야 합니다: [!DNL Jira] 관리자를 사용하여 다음을 설치합니다. [!DNL Workfront] 추가 기능.

다음 대상이 아닌 경우: [!DNL Jira] 관리자, 다음을 찾아볼 수 있습니다. [!DNL Workfront] 기능을 추가하고 설치를 요청합니다. 요청이 (으)로 전송되었습니다. [!DNL Jira] 승인 및 설치 관리자.

에 추가 기능을 설치하도록 요청하는 방법에 대한 자세한 내용은 [!DNL Jira] 응용 프로그램, 참조 [추가 기능에 대한 사용자 요청 관리.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

설치하려면 [!DNL Workfront for Jira]:

1. 에 로그인 [!DNL Jira] as a [!DNL Jira] 관리자.
1. 다음 찾기 **[!DNL Workfront for Jira]** 의 추가 기능 [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. 클릭 **[!UICONTROL 지금 다운로드]** 설치.

   설치가 완료되면 다음 위치에 로그인할 수 있습니다 [!DNL Workfront] 출처: [!DNL Jira] 통합을 구성합니다.

   자세한 내용은 [Jira용 Adobe Workfront 구성](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 에 대한 고려 사항 [!DNL Jira Server] 설치

>[!NOTE]
>
>이러한 요구 사항은 다음에 적용되지 않습니다. [!UICONTROL OnDemand] ([!UICONTROL 클라우드]) 버전 [!DNL Jira] 소프트웨어.

를 설치하는 동안 [!DNL Workfront] 의 추가 기능 [!DNL Jira] 환경은 유사합니다. [!DNL Jira Server] 설치:

* 에서 추가 기능을 구성할 때 [!DNL Jira]에 지정된 주소 **[!DNL JIRA Base URL]** 필드는 액세스하는 데 사용하는 URL과 다를 수 있습니다. [!DNL Jira] 개인 서버에 있습니다. 다음 **[!DNL JIRA Base URL]** 는 NAT 또는 역방향 프록시 프로토콜을 사용하여 개인 서버에 연결된 공개적으로 액세스할 수 있는 주소여야 합니다. [!DNL Workfront] 서버에 요청할 수 있도록 액세스할 수 있습니다.

* 다음 사이에 통신을 보호하려면 SSL 암호화를 사용해야 합니다 [!DNL Jira] 및 [!DNL Workfront]. SSL을 활성화할 때 인증 기관의 전체 SSL 인증서 스택이 있어야 합니다. 자체 서명된 인증서는 지원하지 않습니다.
* 다음을 확인해야 합니다. [!DNL jira.workfront.com] 도메인은 회사 서버에서 액세스할 수 있습니다. 다음 사이에 미들웨어 환경 역할을 합니다 [!DNL Workfront] 및 [!DNL Jira] 추가 기능을 작동하려면 및 가 필요합니다.

  아웃바운드 및 인바운드 연결을 위해 다음 고정 IP 주소를 방화벽의 허용 목록에 추가하다에 추가해야 합니다.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  을(를) 통한 최적의 기능을 위해 방화벽을 구성하는 방법에 대한 자세한 내용 [!DNL Workfront], 참조 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
