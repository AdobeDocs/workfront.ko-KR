---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Google Workspace에서  [!DNL Adobe Workfront] 알림 세부 정보 관리
description: Google Workspace에서 Adobe [!DNL Workfront] 이(가) 보낸 알림 이메일을 열면 받은 편지함에서 관련 작업 항목 세부 정보를 보고 응답할 수 있습니다. 요청 승인과 같은 작업을 사용할 수 있는 경우 Workfront for Google Workspace에서 직접 이러한 작업을 수행할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 알림 세부 정보 관리

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 다음 Google Workspace용 Workfront 기능은 **2026년 2월 28일** 이후에 사용할 수 없습니다.
>
>* Workfront 내에서 Google Workspace 기능 액세스
>
>* Gmail 또는 Google Calendar 사이트 패널에서 Workfront 작업 보기 및 관리
>
>조직의 Google Workspace 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Google Workspace용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Gmail 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) 및 [Google 달력 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)을 참조하십시오.

[!DNL Google Workspace]에서 [!DNL Adobe Workfront]이(가) 보낸 알림 전자 메일을 열면 연결된 작업 항목 세부 정보를 보고 [!UICONTROL 받은 편지함]에서 나가지 않고 응답할 수 있습니다. 요청 승인과 같은 작업을 사용할 수 있는 경우 [!DNL Workfront for Google Workspace]에서 직접 수행할 수 있습니다.

>[!NOTE]
>
> [!DNL Workfront for Google Workspace]은(는) [!DNL Workfront]에서 받을 수 있는 거의 모든 유형의 전자 메일 알림을 지원합니다(약 120개의 다른 유형). [!UICONTROL 에서 보낸 &#x200B;]일별 요약[!DNL Workfront] 전자 메일이 [!DNL Workfront for Google Workspace]에 표시되지 않습니다. [!DNL Workfront] 전자 메일 알림 유형에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

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
   <td> <p>표준</p><p>작업 이상</p>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Google Workspace]에서 알림 세부 정보를 관리하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Google Workspace] 설치\
   지침은 [설치 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)를 참조하십시오.

## [!DNL Adobe Workfront]에서 [!DNL Google Workspace] 알림 세부 정보 관리

1. [!DNL Workfront for Google Workspace] 패널이 표시되지 않으면 페이지의 오른쪽 끝에 있는 [!DNL Workfront] 추가 기능 사이드바에서 ![&#x200B; 아이콘 &#x200B;](assets/wf-lion-icon.png)Workfront 아이콘[!DNL Google Workspace]을 클릭하십시오.
1. [!DNL Google Workspace]에서 [!DNL Workfront] 알림 전자 메일을 엽니다.
1. 패널 상단 근처에 표시되면 **[!UICONTROL 모든 업데이트 보기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 세부 정보]**&#x200B;를 클릭합니다.
1. 사용 가능한 옵션을 클릭합니다.

   표시되는 옵션은 연 이메일 알림 유형과 관련이 있습니다. 예를 들어 작업을 승인하라는 이메일 알림인 경우 **[!UICONTROL 작업]** 또는 **[!UICONTROL 완료]**&#x200B;와 같은 옵션 대신 **[!UICONTROL 승인]** 및 **[!UICONTROL 거부]**&#x200B;이 표시됩니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>이메일 알림 유형</th> 
      <th>액션</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>작업 또는 문제</td> 
      <td><strong>[!UICONTROL 승인]</strong>, <strong>[!UICONTROL 거부]</strong>, <strong>[!UICONTROL 승인]</strong> 액세스, <strong>[!UICONTROL 무시]</strong> 액세스 요청, <strong>[!UICONTROL 작업]</strong> 또는 옵션을 클릭하여 <strong>[!UICONTROL 완료]</strong>임을 나타냅니다.</td> 
     </tr> 
     <tr> 
      <td>프로젝트</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access 또는 <strong>[!UICONTROL Ignore]</strong> access 요청</td> 
     </tr> 
     <tr> 
      <td>문서</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access 또는 <strong>[!UICONTROL Ignore]</strong> access 요청</td> 
     </tr> 
     <tr> 
      <td>업데이트 </td> 
      <td> <p>새 업데이트 또는 <strong>[!UICONTROL 회신]</strong>을(를) <strong>[!UICONTROL Post]</strong>해야 하는 컨텍스트를 갖도록 항목에 대한 전체 업데이트 목록의 일부를 봅니다. <strong>[!UICONTROL 알림]</strong>을(를) 클릭하여 특정 사용자에게 회신에 대해 경고할 수 있습니다. </p> <p>자세한 내용은 <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">[!DNL Adobe Workfront]에서 [!DNL Google Workspace]</a> 업데이트 알림에 회신 을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td>승인 요청</td> 
      <td><strong>[!UICONTROL Approve]</strong> 또는 <strong>[!UICONTROL Reject]</strong>(다른 옵션을 클릭하여 마음을 바꿀 수 있음), 다운로드, 소유자 보기 또는 참조 번호 보기</td> 
     </tr> 
     <tr> 
      <td>프로젝트 상태 변경</td> 
      <td> 사용자 정의 양식을 포함하여 프로젝트에 대한 현재 모든 정보를 봅니다. </td> 
     </tr> 
    </tbody> 
   </table>
