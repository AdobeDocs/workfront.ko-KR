---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront for Jira] 구성'
description: ' [!DNL Adobe Workfront for Jira] 을(를) 사용하여  [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '2470'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Jira] 구성

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Jira용 Workfront 통합을 사용할 수 없습니다.
>
>Jira와 조직의 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Jira용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Jira 소프트웨어 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)을 참조하십시오.

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

[!DNL Adobe Workfront for Jira]을(를) 사용하여 [!DNL Jira] 및 [!DNL Workfront] 시스템을 통합할 수 있습니다.

추가 기능을 설치한 후 [!DNL Jira]개의 작업 항목을 만들 때 [!DNL Workfront]개의 문제를 자동으로 만드는 워크플로를 정의할 수 있습니다. 두 응용 프로그램의 항목이 연결되고 일부 정보는 두 시스템에서 자동으로 업데이트됩니다.

[!DNL Workfront] 및 [!DNL Jira]의 모든 사용자가 이 통합을 통해 혜택을 받을 수 있습니다. 가장 많이 사용하는 시스템에 대한 라이선스만 있으면 되고 두 시스템 모두에 대한 라이선스는 필요하지 않습니다.

이 추가 기능은 [!UICONTROL &#x200B; 소프트웨어의 &#x200B;]Server[!UICONTROL &#x200B; 및 &#x200B;]OnDemand[!UICONTROL (또는 &#x200B;]Cloud[!DNL Jira]) 버전 모두에서 사용할 수 있습니다.

현재 [!DNL Jira]에서 지원하는 [!DNL Workfront for Jira] 버전 목록은 [[!DNL Workfront for Jira]의 ](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) [!DNL Atlassian Marketplace]을(를) 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] 플랜]</td> 
   <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: [!UICONTROL Pro] 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard] </p>
       <p>또는</p> 
       <p>현재: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 [!DNL Jira] 및 [!DNL Workfront]에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 사용하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Workfront for Jira]을(를) 구성하기 전에 다음을 수행해야 합니다.

* [!DNL Workfront for Jira] 설치.
[!DNL Workfront for Jira] 설치에 대한 지침은 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)를 참조하십시오.

## [!DNL Workfront for Jira] 구성

[!DNL Workfront for Jira]을(를) 구성하여 다음을 수행할 수 있습니다.

* [!DNL Jira]개 항목을 만들 때 [!DNL Workfront]개 항목을 만들 트리거를 정의합니다.
* [!DNL Jira]과(와) [!DNL Workfront] 사이에 연결된 항목 간에 동기화할 필드를 지정하십시오.

>[!NOTE]
>
>* [!DNL Workfront for Jira] 환경에서 [!DNL Jira]을(를) 구성하면 모든 [!DNL Jira] 사용자에게 모든 [!DNL Workfront] 항목에 대한 [!DNL Jira] 오른쪽 패널이 표시됩니다. 패널에 [!DNL Workfront]에서 연결할 수 있는 항목에 대한 정보가 포함되어 있거나 [!DNL Workfront]개 항목이 [!DNL Jira]개 항목에 연결되어 있지 않도록 지정합니다.
>* [!DNL Jira Server] 설치를 사용하는 경우 Workfront 통합에 대한 트리거로 식별된 프로젝트와 관련된 문제만 Workfront 패널에 표시됩니다. [!DNL Workfront to Jira] 워크플로의 트리거 설정에 대한 자세한 내용은 [자동 연결 트리거 구성 [!DNL Jira] 과(와) [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)을(를) 참조하십시오.
>

[!DNL Workfront for Jira]을(를) 구성하려면:

1. [!DNL Jira]에 [!DNL Jira] 관리자로 로그인합니다.
1. 주 **[!UICONTROL 메뉴에서]**&#x200B;설정[!DNL Jira]을 클릭합니다.
1. **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.

1. **[!DNL Workfront]** 추가 기능을 확장합니다.
1. **[!UICONTROL 구성]**&#x200B;을 클릭합니다.
1. 메시지에 따라 [!DNL Workfront]에 로그인합니다.

   >[!NOTE]
   >
   >연결을 만들려면 `apiKey`Workfront[!UICONTROL 에 올바른 &#x200B;]이(가) 있어야 합니다.

   구성을 계속하려면 [!DNL Workfront]에 [!DNL Workfront] 관리자로 로그인해야 합니다.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront]은(는) 사용자의 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 표준인 OAuth 2.0을 사용하여 [!DNL Jira]에 연결합니다.
   >* [!DNL Workfront] 계정의 도메인을 입력하라는 메시지가 표시되면 *yourCompany&#39;sDomain.my.workfront.com* 형식을 사용하여 입력하세요. 회사의 도메인은 일반적으로 회사의 이름입니다.
   >* 향상된 인증은 [!DNL Workfront] 관리자가 이 통합에 사용하도록 설정할 때까지 사용할 수 없습니다.

1. Jira에서 **[!UICONTROL 트리거]** 탭을 선택하여 새 [!DNL Jira]개 항목이 생성될 때 [!DNL Workfront]개 항목의 자동 만들기를 구성하십시오.

   [!DNL Jira] 워크플로우에 대한 Workfront의 트리거 설정에 대한 자세한 내용은 [자동 연결 트리거 구성 [!DNL Jira] 과(와) [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)을(를) 참조하십시오.

1. 연결된 **[!UICONTROL 개 항목과]**&#x200B;개 항목 간의 필드 동기화를 구성하려면 [!DNL Jira]설정[!DNL Workfront] 탭을 선택하십시오.

   [!DNL Jira]과(와) [!DNL Workfront] 사이의 필드 동기화를 설정하는 방법에 대한 자세한 내용은 [과(와) [!DNL Jira] 과(와) [!DNL Workfront] 항목](#configure-field-synchronization-between-jira-and-workfront-items) 사이의 필드 동기화 구성 을 참조하십시오.

   >[!NOTE]
   >
   >두 응용 프로그램 간의 트리거 및 필드 동기화를 정의하면 작업 또는 문제를 만들 수 있는 [!DNL Workfront] 사용자가 [!DNL Jira]에 항목 만들기를 트리거할 수 있습니다. 사용자에게 [!DNL Jira] 라이선스가 없어도 사용자가 만드는 항목의 기준이 [!DNL Jira]의 트리거와 일치하는 경우 항목을 만들 수 있습니다. 또한 [!DNL Jira] 사용자는 [!DNL Jira] 항목에서 바로 작업을 시작할 수 있으며, [!DNL Workfront] 라이선스가 없어도 [!DNL Workfront]에서 업데이트를 볼 수 있습니다. [!DNL Workfront]의 모든 업데이트가 [!DNL Jira] 항목에도 표시됩니다.

1. (선택 사항) **[!UICONTROL 활동 로그]** 탭을 선택하여 통합 중에 발생했을 수 있는 오류를 검토합니다.

   [!UICONTROL 활동 로그]에 대한 자세한 내용은 [활동 로그 보기 [!DNL Jira] [!UICONTROL 를 참조하십시오]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## [!DNL Jira]과(와) [!DNL Workfront] 사이의 항목을 자동으로 연결하기 위한 트리거 구성

[!DNL Jira] 시스템 관리자는 [!DNL Jira]의 항목이 특정 기준을 만족할 때 [!DNL Workfront]에서 자동으로 문제를 만드는 트리거를 정의할 수 있습니다.

>[!NOTE]
>
>통합에서 [!DNL Jira]에 새 문제를 만드는 데 최대 10분이 걸릴 수 있습니다.

[!DNL Jira]개 항목이 생성될 때 [!DNL Workfront]개 항목 생성을 트리거하도록 구성할 때는 다음 사항을 고려하십시오.

* 통합은 단방향입니다. [!DNL Workfront]에서 만든 항목만 [!DNL Jira]에서 자동으로 만들도록 트리거할 수 있습니다. [!DNL Jira]에서 만든 항목을 [!DNL Workfront]에서 자동으로 만들도록 트리거할 수 없습니다.
* 가질 수 있는 트리거 수에 제한은 없습니다.
* [!DNL Workfront]에서 만든 항목이 두 개 이상의 트리거와 일치하는 경우 [!DNL Jira]에서 한 항목만 만들어집니다. 항목이 첫 번째 트리거에 따라 [!DNL Jira]에서 만들어집니다([!DNL Jira]에서 정의된 순서). 다른 모든 트리거는 무시됩니다.
* [!DNL Workfront]의 항목 하나만 Jira의 항목 하나에 연결할 수 있습니다. 한 개의 [!DNL Workfront] 항목을 여러 [!DNL Jira] 문제에 연결하거나 한 개의 [!DNL Jira] 문제를 여러 [!DNL Workfront] 항목에 연결할 수 없습니다.

[!DNL Jira]에서 항목을 자동으로 만들기 위한 트리거를 구성하려면 다음 작업을 수행하십시오.

1. 시스템 관리자로 [!DNL Jira]에 로그인합니다.
1. 주 **[!UICONTROL 메뉴에서]**&#x200B;설정[!DNL Jira]을 클릭합니다.
1. **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.
1. **[!DNL Workfront]** 추가 기능을 확장합니다.
1. **[!UICONTROL 구성]**&#x200B;을 클릭합니다.
1. 시스템 관리자로 [!DNL Workfront]에 로그인합니다.

   Jira에서 기본적으로 **[!UICONTROL 트리거]** 탭이 선택됩니다.

1. 새 트리거를 추가하려면 **[!UICONTROL 트리거 추가]**&#x200B;를 클릭하십시오.
1. **[!UICONTROL Workfront 팀/사용자/역할]** 필드에서 [!DNL Workfront] 팀, 사용자 또는 작업 역할의 이름을 지정한 다음 목록에 표시될 때 클릭하여 선택합니다.

   >[!NOTE]
   >
   >동일한 팀, 사용자 또는 역할에 여러 트리거를 사용할 수 없습니다.

   누군가가 작업 또는 문제를 만들어 이러한 엔터티 중 하나에 할당하면 [!DNL [!DNL Jira]]에서 문제가 자동으로 만들어집니다.

1. **[!UICONTROL [!DNL Jira]프로젝트]** 필드에서 [!DNL Jira] 프로젝트의 이름을 입력한 다음 목록에 표시될 때 클릭하여 선택합니다.

   [!DNL Jira] 문제가 만들어지면 여기에서 선택한 프로젝트에 배치됩니다.

1. 드롭다운 메뉴에서 **I[!UICONTROL 문제 유형]**&#x200B;을(를) 선택합니다.

   이는 [!DNL Jira]의 특정 프로젝트에 대한 설정에 따라 이 트리거의 조건이 충족될 때 [!DNL Jira]에서 만들어지는 문제 유형을 나타냅니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이 구성을 사용하면 [!DNL Workfront] 사용자가 지정된 트리거와 일치하는 항목을 만들 때마다 [!DNL Jira]에 새 문제가 만들어집니다.

## [!DNL Jira]과(와) [!DNL Workfront]개 항목 간의 필드 동기화 구성

[!DNL Jira] 관리자는 [!DNL Workfront]과(와) Jira 사이에 연결된 항목에 대해 자동으로 동기화할 필드를 정의할 수 있습니다. 특정 필드는 [!DNL Workfront]에서 [!DNL Jira] 항목으로 동기화되고 다른 필드는 Jira에서 Workfront으로 동기화됩니다.

두 애플리케이션 간에 연결된 항목에 대해 자동으로 동기화할 필드를 정의하려면

1. [!DNL Jira]에 Jira 관리자로 로그인합니다.
1. 주 **[!UICONTROL 메뉴에서]**&#x200B;설정[!DNL Jira]을 클릭합니다.
1. **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.
1. **[!DNL Workfront]** 추가 기능을 확장합니다.
1. **[!UICONTROL 구성]**&#x200B;을 클릭합니다.
1. [!DNL Workfront]에 Workfront 관리자로 로그인합니다.
1. Jira에서 **[!UICONTROL 설정]** 탭을 클릭합니다.
1. **[!UICONTROL Workfront에서 Jira로 동기화]** 섹션에서 Workfront에서 업데이트될 때 [!DNL Jira]에서 업데이트할 필드를 선택합니다.

   1. 필드가 동기화되는 다음 빈도 중 하나를 선택합니다.

      <table style="table-layout:auto">
         <tr>
              <td>만들 때 </td>
              <td>지정한 필드는 Workfront에서 항목을 만들 때 연결된 Workfront과 [!DNL Jira]개 항목 간에 동기화됩니다.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>지정한 필드는 Workfront에서 필드를 업데이트할 때 연결된 Workfront과 [!DNL Jira] 항목 간에 동기화됩니다. </td>
          </tr>
          <tr>
              <td>[!UICONTROL 사용 안 함]</td>
              <td>지정한 필드는 연결된 [!DNL Workfront]개 항목과 [!DNL Jira]개 항목 간에 동기화되지 않습니다. [!DNL Jira]에 필드가 [!DNL Workfront]에서 업데이트되었다는 표시가 없습니다. </td>
          </tr>
      </table>

   1. [!DNL Workfront]에서 [!DNL Jira]&#x200B;(으)로 필드를 동기화하려면 다음 중 하나를 선택하십시오.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 이름]</td>
         <td><p>[!DNL Workfront]의 작업 또는 문제 이름이 [!DNL Jira]에서 연결된 문제의 이름이 됩니다.</p><p>참고: [!DNL Jira]에서 새 항목을 자동으로 만들면 [!DNL Workfront] 이름이 이 필드를 여기에서 사용할 수 있는지 여부에 관계없이 항상 [!DNL Jira] 항목에 업데이트됩니다. [!DNL Jira] 항목이 [!DNL Workfront] 항목에 수동으로 연결된 경우 [!DNL Workfront]항상[!DNL Jira] 이 필드를 동기화하도록 선택하면 <strong> 항목의 이름이 </strong>에서만 업데이트됩니다. 항목을 수동 또는 자동으로 연결하는 방법에 대한 자세한 내용은 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">[!DNL Adobe Workfront]과(와) [!DNL Jira]</a> 사이의 항목 연결을 참조하십시오.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 설명]</td>
         <td>[!DNL Workfront]의 작업 또는 문제에 대한 설명이 [!DNL Jira]에서 연결된 문제에 대한 설명이 됩니다.</td>
        </tr>
        <tr>
         <td role="rowheader">문서</td>
         <td><p>[!DNL Workfront]의 작업 또는 문제에 첨부된 문서도 Jira에서 연결된 문제에 첨부됩니다. [!DNL Workfront]의 새 문서 버전이 별도의 문서로 Jira에 추가되고 Workfront에서 번호가 매겨진 버전을 나타내기 위해 <i>_v&lt;version number&gt;</i>와(과) 함께 추가됩니다. </p><p>예를 들어 [!DNL Workfront]에 있는 문서 이름이 <strong>주 광고</strong>이고 [!DNL Workfront]에 새 버전을 추가하면 새 버전이 [!DNL Jira]주 광고_v2<strong>라는 새 문서로 </strong>에 전송됩니다.</p><p>중요 사항: <p>문서를 동기화할 때는 다음 사항을 고려하십시오.</p>
           <ul>
            <li><p>5MB가 넘는 문서는 동기화되지 않습니다. 문서가 너무 커서 문서 동기화에 실패하면 오류가 활동 로그에 기록됩니다. </p><p>작업 로그에 대한 자세한 내용은 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira 작업 로그 보기</a>를 참조하십시오.</p></li>
            <li><p>외부 서버의 작업 및 문제에 연결된 문서는 [!DNL Jira] 항목으로 전송되지 않습니다. [!DNL Workfront]의 작업 또는 문제에 직접 업로드된 문서만 [!DNL Jira]의 연결된 문제로 전송됩니다.</p></li>
            <li><p>문서에서 증명을 만들려면 [!DNL Workfront]에 증명을 생성해야 합니다. </p><p>증명 생성에 대한 자세한 내용은 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">기존 문서에 대한 증명 만들기 </a>에서 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">문서에 대한 증명 만들기</a>를 참조하십시오.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 계획된 완료 일자]</td>
         <td><p>[!DNL Workfront]에 있는 작업 또는 문제의 [!UICONTROL 계획된 완료 일자]가 [!DNL Jira]에 연결된 문제의 [!UICONTROL 기한]이 됩니다.</p><p>참고: 이 값을 동기화하려면 <strong> 문제에 대해 </strong>[!UICONTROL 기한][!DNL Jira]을(를) 표시해야 합니다.</p></td>
        </tr>
       </tbody>
      </table>

1. **[!UICONTROL [!DNL Jira]에서[!DNL Workfront]]**(으)로 동기화 섹션에서 [!DNL Workfront]에 업데이트될 때 [!DNL Jira]에서 업데이트할 필드를 선택합니다.

   1. 필드가 동기화되는 다음 빈도 중 하나를 선택합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>지정한 필드는 [!DNL Workfront]에서 필드가 업데이트될 때 연결된 [!DNL Jira] 항목과 [!DNL Jira] 항목 간에 항상 동기화됩니다. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 사용 안 함]</td>
         <td><p>지정한 필드는 연결된 [!DNL Workfront]개 항목과 [!DNL Jira]개 항목 간에 동기화되지 않습니다. [!DNL Workfront]에 필드가 [!DNL Jira]에서 업데이트되었다는 표시가 없습니다. </p><p>참고: [안 함]을 선택하면 [!DNL Workfront] 문제의 왼쪽 [!DNL Jira] 패널에 있는 [!DNL Workfront]에서 [!DNL Jira] 필드를 수동으로 업데이트할 수 있습니다. 이러한 업데이트는 [!DNL Workfront] 및 [!DNL Jira]의 [!DNL Workfront]개 항목에만 표시되고 [!DNL Jira]개 항목에는 표시되지 않습니다.</p></td>
        </tr>
       </tbody>
      </table>

   1. [!DNL Jira]에서 [!DNL Workfront]&#x200B;(으)로 다음 필드 중 하나를 동기화하려면 선택하십시오.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 상태]</td>
         <td>[!DNL Jira]에서 문제의 [!UICONTROL 상태]가 [!DNL Workfront]에서 연결된 작업 또는 문제의 [!UICONTROL 상태]가 됩니다.<br>상태 [!DNL Workfront]에 대한 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>을 참조하세요.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 담당자]</td>
         <td><p>[!DNL Jira]에서 문제의 [!UICONTROL Assignee]이(가) [!DNL Workfront]에서 연결된 작업 또는 문제의 [!UICONTROL Assignee]이 됩니다.</p><p>중요: [!DNL Jira]의 항목을 [!DNL Workfront] 계정이 없는 사용자에게 할당하면 [!DNL Workfront]사용자에게 <strong> 계정이 없는 경우 [!DNL Workfront]에서 자동으로 사용자 만들기[!DNL Jira]가 [!DNL Workfront][!UICONTROL Always]</strong>(으)로 설정된 경우에만 통합에서 <strong>에서 새 활성 사용자를 만듭니다. </strong> 이 사용자는 [!DNL Workfront] 라이선스를 사용하지 않습니다. 활성 사용자를 [!DNL Workfront]의 작업 항목에 할당할 수 있지만 업데이트에 포함할 수 없습니다. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 첨부 파일]</td>
         <td>[!DNL Jira]의 문제 첨부 파일도 [!DNL Workfront]에서 연결된 작업 또는 문제에 첨부됩니다. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>[!DNL Jira] 문제에 대한 댓글이 [!UICONTROL Updates] 영역의 연결된 [!DNL Workfront] 항목에도 게시됩니다. 반대로 [!DNL Workfront] 작업 또는 문제에 대한 [!UICONTROL Updates] 영역에 게시된 댓글은 연결된 문제에 대한 [!DNL Jira]의 기본 댓글 스트림과 동기화됩니다. </p><p>기본적으로 <strong>[!UICONTROL Always]</strong>(으)로 설정됩니다. 여기에서 <strong>[!UICONTROL 사용 안 함]</strong>을(를) 선택한 경우에도 [!DNL Workfront] 또는 [!DNL Jira]의 연결된 항목에 수동으로 댓글을 게시할 수 있습니다.</p></td>
        </tr>
       </tbody>
      </table>

1. **[!UICONTROL 기타]** 섹션에서 연결된 항목 사이에 업데이트할 추가 필드를 선택합니다.

   1. 필드 수정 시 **[!UICONTROL Always]** 또는 **[!UICONTROL Never]** 업데이트를 지정한 필드가 [!DNL Jira] 또는 [!DNL Workfront]에서 업데이트되는지 여부를 결정하는 옵션을 선택하십시오.

   1. 다음 필드 및 업데이트 중에서 선택합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront]]의 오른쪽 패널에 [!DNL Jira] 사용자 지정 데이터를 복사합니다.</td>
         <td><p>[!DNL Workfront] 오른쪽 패널에 항목의 [!DNL Workfront] 사용자 지정 데이터를 표시합니다.</p><p>참고: 사용자 정의 양식 섹션은 [!DNL Workfront] 시스템 관리자의 액세스 수준으로 [!DNL Workfront] 오른쪽 패널에 표시됩니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront]]의 오른쪽 패널에 있는 [!DNL Jira] 복사 우선 순위</td>
         <td>[!DNL Workfront] 오른쪽 패널에 항목의 [!DNL Workfront] 우선 순위를 표시합니다.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront]의 기한 변경에 대해 [!DNL Jira] 업데이트 탭에 업데이트를 추가합니다.]</td>
         <td>연결된 [!DNL Workfront] 항목에서 [!UICONTROL 기한]이 변경되면 [!DNL Jira] 항목의 [!UICONTROL 업데이트] 탭에 주석을 추가합니다.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront] 사용자에게 [!DNL Jira] 계정이 없는 경우 [!DNL Workfront]에서 사용자를 자동으로 만듭니다.]</td>
         <td><p>다음과 같은 시나리오가 있습니다.</p>
          <ul>
           <li><strong>[!UICONTROL Always]</strong>을(를) 선택하면 [!DNL Jira] 계정이 없는 [!DNL Workfront] 사용자가 연결된 [!DNL Jira] 문제에 대해 다음 작업을 수행할 때마다 통합이 새 Workfront 사용자를 만들 수 있습니다.
            <ul>
             <li>[!DNL Jira] 문제에 할당됨</li>
             <li><p>[!DNL Jira] 문제에 시간을 기록합니다.</p><p>이 새 사용자는 [!DNL Workfront] 라이선스를 사용하지 않습니다. 기본 설정은 항상 입니다. [!DNL Workfront]에서 이러한 방식으로 만든 사용자의 이름에 "[!UICONTROL Jira]"가 추가되었습니다.</p></li>
            </ul></li>
           <li><strong>[!UICONTROL 사용 안 함]</strong>을(를) 선택하면 다음 상황이 발생합니다.
            <ul>
             <li>[!DNL Jira] 항목에서 [!DNL Workfront] 할당을 볼 수 없습니다. 이 경우 [!DNL Workfront]에서 수행된 할당만 [!DNL Workfront] 항목에 표시됩니다.</li>
             <li>[!DNL Jira] 계정이 없는 사용자가 연결된 [!DNL Workfront] 문제에 기록된 시간이 연결된 [!DNL Workfront] 항목으로 자동으로 전송되지 않습니다. [!DNL Workfront] 문제의 오른쪽 패널에 있는 [!DNL Jira] 항목에 시간을 계속 기록할 수 있습니다.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 사용자가 [!DNL Jira] 또는 [!DNL Workfront]의 항목에 대해 이 구성에 지정된 필드를 업데이트할 때마다 다른 응용 프로그램의 연결된 항목도 업데이트됩니다.

## 문제 해결

### &quot;[!DNL Jira]찾을 수 없음[!UICONTROL &quot;으로 표시된 트리거 필드로 인해 &#x200B;]에서 항목을 만들 수 없습니다.

#### 문제

[!DNL Workfront for Jira] 응용 프로그램에 오류가 발생하면 [!DNL Workfront]에서 더 이상 문제가 발생하지 않도록 트리거를 사용하지 않도록 설정합니다. 이러한 트리거가 비활성화되면 &quot;[!UICONTROL 찾을 수 없음]&quot;으로 표시됩니다.

#### 솔루션

트리거를 비활성화한 오류를 찾습니다. [!DNL Workfront for Jira] [!UICONTROL 활동 로그]에서 오류를 찾을 수 있습니다.

이 동작의 가장 일반적인 원인은 오류 &quot;[!UICONTROL 필드 &#39;duedate&#39;를 설정할 수 없기 때문입니다. 적절한 화면이 아니거나 알 수 없습니다.]&quot;

이 오류는 &quot;[!UICONTROL 계획된 완료 일자]&quot;을(를) [!DNL Workfront]에서 [!DNL Jira]&#x200B;(으)로 동기화하려고 시도하고 있음을 의미합니다. 이렇게 하려면 [!DNL Jira] 개체에 &quot;[!UICONTROL 기한]&quot;이라는 필드가 있는지 확인해야 합니다. 이 필드가 없으면 [!DNL Workfront]이(가) [!DNL Workfront]에서 계획된 완료 일자를 동기화할 수 없으며 트리거를 사용할 수 없게 됩니다.

이 오류를 해결하려면 다음 중 하나를 시도해 보십시오.

* [!DNL Jira] 관리자에게 해당 [!DNL Jira] 개체가 기한 필드가 있는지 업데이트하도록 요청하십시오.
* Workfront [!DNL Workfront]설치[!UICONTROL &#x200B; 페이지에서 &#x200B;]의 계획된 완료 날짜에 대한 동기화를 사용하지 않도록 설정하십시오.
