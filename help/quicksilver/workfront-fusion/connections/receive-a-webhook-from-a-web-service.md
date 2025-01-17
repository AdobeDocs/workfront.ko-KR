---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 웹 서비스에서 웹후크 받기
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 웹 서비스에서 웹후크 받기

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [커넥터 없이 웹 서비스에 대한 웹후크 구성](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

웹 서비스가 현재 [!DNL Adobe Workfront Fusion]에서 앱으로 구현되지 않았지만 웹후크 전송을 지원하는 경우 사용자 지정 웹후크 모듈을 인스턴트 트리거로 사용하여 시나리오에 서비스를 추가할 수 있습니다.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## Webhook 받기

1. 시나리오에 **[!UICONTROL Webhooks] >[!UICONTROL 사용자 지정 Webhook]** 모듈을 추가합니다.
1. **[!UICONTROL 추가]**&#x200B;를 클릭하고 표시되는 상자에 **[!UICONTROL Webhook 이름]**&#x200B;을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 클립보드에 주소 복사]**&#x200B;를 클릭한 다음 **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

1. 웹 서비스에 로그인하고 다음 작업을 수행합니다.

   1. 웹 서비스의 [!UICONTROL 설정] 영역에서 웹후크를 만듭니다.
   1. 3단계에서 클립보드로 복사한 주소를 붙여넣습니다.
   1. 웹후크를 트리거할 이벤트를 선택합니다.

1. [!DNL Workfront Fusion] 시나리오에서 [!UICONTROL 사용자 지정 Webhook] 모듈을 트리거할 이벤트를 지정합니다.
1. 시나리오를 실행합니다.

   이벤트가 발생하면 [!UICONTROL 사용자 지정 Webhook] 모듈이 트리거되고 시나리오가 실행됩니다.
