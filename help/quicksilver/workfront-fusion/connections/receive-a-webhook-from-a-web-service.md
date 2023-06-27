---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 웹 서비스에서 웹후크 받기
description: 웹 서비스가 현재 의 앱으로 구현되지 않은 경우 [!DNL Adobe Workfront Fusion], 하지만 웹후크 전송을 지원하므로 사용자 지정 웹후크 모듈을 인스턴트 트리거로 사용하여 시나리오에 서비스를 추가할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 웹 서비스에서 웹후크 받기

웹 서비스가 현재 의 앱으로 구현되지 않은 경우 [!DNL Adobe Workfront Fusion], 하지만 웹후크 전송을 지원하므로 사용자 지정 웹후크 모듈을 인스턴트 트리거로 사용하여 시나리오에 서비스를 추가할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Webhook 받기

1. 추가 **[!UICONTROL 웹훅] >[!UICONTROL 사용자 지정 웹후크]** 을 시나리오에 연결합니다.
1. 클릭 **[!UICONTROL 추가]**, a 입력 **[!UICONTROL Webhook 이름]** 표시되는 상자에서 **[!UICONTROL 저장]**.

1. 클릭 **[!UICONTROL 클립보드에 주소 복사]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 확인]**.

1. 웹 서비스에 로그인하고 다음 작업을 수행합니다.

   1. 다음에서 [!UICONTROL 설정] 웹 서비스에 대한 영역에서 웹후크를 생성합니다.
   1. 3단계에서 클립보드로 복사한 주소를 붙여넣습니다.
   1. 웹후크를 트리거할 이벤트를 선택합니다.

1. 다음에서 [!DNL Workfront Fusion] 시나리오에서는 트리거할 이벤트를 지정합니다. [!UICONTROL 사용자 지정 웹후크] 모듈.
1. 시나리오를 실행합니다.

   이벤트 또는 이벤트가 발생하면 [!UICONTROL 사용자 지정 웹후크] 모듈이 트리거되고 시나리오가 실행됩니다.
