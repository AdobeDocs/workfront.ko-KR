---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 웹 서비스에서 웹 후크 받기
description: 웹 서비스가 현재 의 앱으로 구현되지 않은 경우 [!DNL Adobe Workfront Fusion]하지만 webhooks 전송을 지원하지만 사용자 지정 웹 후크 모듈을 인스턴트 트리거로 사용하여 시나리오에 서비스를 추가할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 웹 서비스에서 웹 후크 받기

웹 서비스가 현재 의 앱으로 구현되지 않은 경우 [!DNL Adobe Workfront Fusion]하지만 webhooks 전송을 지원하지만 사용자 지정 웹 후크 모듈을 인스턴트 트리거로 사용하여 시나리오에 서비스를 추가할 수 있습니다.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 웹 후크 받기

1. 추가 **[!UICONTROL Webhooks] >[!UICONTROL 사용자 정의 웹 후크]** 모듈에 대해 고려합니다.
1. 클릭 **[!UICONTROL 추가]**, 입력 **[!UICONTROL Webhook 이름]** 표시되는 상자에서 를 클릭합니다. **[!UICONTROL 저장]**.

1. 클릭 **[!UICONTROL 클립보드에 주소 복사]**&#x200B;를 클릭한 다음 **[!UICONTROL 확인]**.

1. 웹 서비스에 로그인하고 거기에서 다음을 수행합니다.

   1. 에서 [!UICONTROL 설정] 웹 서비스용 영역에서 웹 후크를 만듭니다.
   1. 3단계에서 클립보드에 복사한 주소를 붙여넣습니다.
   1. 웹 후크를 트리거할 이벤트를 선택합니다.

1. 에서 [!DNL Workfront Fusion] 시나리오에서 트리거할 이벤트 또는 이벤트를 지정합니다 [!UICONTROL 사용자 정의 웹 후크] 모듈.
1. 시나리오를 실행합니다.

   이벤트나 이벤트가 발생하면 [!UICONTROL 사용자 정의 웹 후크] 모듈 트리거와 시나리오가 실행됩니다.
