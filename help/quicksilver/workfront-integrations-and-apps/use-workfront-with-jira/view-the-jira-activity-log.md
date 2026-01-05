---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira 활동 로그 보기
description: ' [!DNL Jira] 관리자는  [!DNL Adobe Workfront] 에서 [!DNL Jira]  사이의 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 작업 로그에서 볼 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 5%

---

# [!UICONTROL [!DNL Jira] 작업 로그 보기]

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Jira용 Workfront 통합을 사용할 수 없습니다.
>
>Jira와 조직의 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Jira용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Jira 소프트웨어 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)을 참조하십시오.

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

[!DNL Jira] 관리자는 [!DNL Adobe Workfront]활동 로그[!DNL Jira]에서 [!UICONTROL 에서 &#x200B;] 사이의 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 볼 수 있습니다.

활동 로그에서 최대 500개의 항목을 볼 수 있으며 가장 최근 항목으로 시작하여 나열됩니다.

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

+++

## 전제 조건

[!DNL Workfront]과(와) [!DNL Jira] 사이의 항목을 연결하려면 먼저

* [!DNL Workfront for Jira] 설치

  [!DNL Workfront for Jira] 설치에 대한 지침은 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)를 참조하십시오.

## [!UICONTROL [!DNL Jira] 작업 로그]에 액세스:

1. 시스템 관리자로 Jira에 로그인합니다.
1. 주 **[!UICONTROL 메뉴에서]**&#x200B;설정[!DNL Jira]을 클릭합니다.
1. **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.

1. **[!DNL Workfront]** 추가 기능을 확장합니다.
1. **[!UICONTROL 구성]**&#x200B;을 클릭합니다.
1. 시스템 관리자로 [!DNL Workfront]에 로그인합니다.
1. **[!UICONTROL 활동 로그]** 탭을 선택합니다.

   항목을 생성하거나 두 응용 프로그램 간의 필드를 동기화하는 동안 발생한 예외 및 오류에 대한 정보를 봅니다.

   로그에는 다음 필드가 포함되어 있습니다.

   * 발생 날짜
   * Jira의 사용자 이름
   * Jira 문제 번호
   * 발생한 오류에 대한 간단한 설명입니다.
