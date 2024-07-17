---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]의 HTTP 요청 메서드'
description: 모듈에서 API 호출을 구성할 때는 HTTP 요청 메서드에 대한 필드를 채워야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 HTTP 요청 메서드

모듈에서 API 호출을 구성할 때는 HTTP 요청 메서드에 대한 필드를 채워야 합니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
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

## HTTP 메서드

다음 HTTP 메서드 중 하나를 사용합니다.

* **[!UICONTROL GET]**: 매개 변수를 기반으로 웹 서버에서 데이터를 검색합니다. [!UICONTROL GET]이(가) 지정된 리소스의 표현을 요청하고 성공하면 요청된 콘텐츠와 함께 [!UICONTROL 200 OK] 응답 메시지를 받습니다.
* **[!UICONTROL POST]**: 매개 변수를 기반으로 웹 서버에 데이터를 보냅니다. [!UICONTROL POST] 요청에 파일 업로드와 같은 작업이 포함되어 있습니다. 여러 [!UICONTROL POST]은(는) 단일 [!UICONTROL POST]과(와) 다른 결과를 초래할 수 있으므로 실수로 여러 [!UICONTROL POST]을(를) 전송하는 것에 주의하십시오. [!UICONTROL POST]이 성공하면 [!UICONTROL 200 OK] 응답 메시지가 표시됩니다.
* **[!UICONTROL PUT]**: 매개 변수를 기반으로 웹 서버의 위치로 데이터를 보냅니다. [!UICONTROL PUT] 요청에 파일 업로드와 같은 작업이 포함되어 있습니다. [!UICONTROL PUT]과(와) [!UICONTROL POST]의 차이점은 PUT이 멱등 행렬이라는 것입니다. 즉, 하나의 성공적인 [!UICONTROL PUT]의 결과가 동일한 [!UICONTROL PUT]과(와) 동일합니다. PUT이 성공하면 200개의 응답 메시지(일반적으로 201 또는 204)를 받습니다.
* **[!UICONTROL PATCH]**: (일부 API 호출 모듈에는 사용할 수 없음) 매개 변수를 기반으로 웹 서버의 리소스에 부분 수정 사항을 적용합니다. [!UICONTROL PATCH]은(는) idempotent가 아닙니다. 즉, 여러 [!UICONTROL PATCH]의 결과가 의도하지 않은 결과를 초래할 수 있습니다. [!UICONTROL PATCH]이 성공하면 200개의 응답 메시지(보통 204개)를 받게 됩니다.
* **[!UICONTROL DELETE]**: 매개 변수를 기반으로 웹 서버에서 지정된 리소스를 삭제합니다(리소스가 있는 경우). [!UICONTROL DELETE]이 성공하면 200 OK 응답 메시지가 표시됩니다.
