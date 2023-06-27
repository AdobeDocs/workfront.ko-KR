---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]
description: 모듈에서 API 호출을 구성할 때는 HTTP 요청 메서드에 대한 필드를 채워야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]

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

## HTTP 메서드

다음 HTTP 메서드 중 하나를 사용합니다.

* **[!UICONTROL GET]**: 매개 변수를 기반으로 웹 서버에서 데이터를 검색합니다. [!UICONTROL GET] 지정된 리소스의 표현을 요청하고 [!UICONTROL 200개] 성공하면 요청된 콘텐츠가 포함된 응답 메시지입니다.
* **[!UICONTROL POST]**: 매개 변수를 기반으로 웹 서버에 데이터를 전송합니다. [!UICONTROL POST] 요청에는 파일 업로드와 같은 작업이 포함됩니다. 복수 [!UICONTROL POST]s는 단일 결과와 다른 결과를 초래할 수 있습니다. [!UICONTROL POST], 따라서 의도하지 않게 다중 전송에 주의하십시오 [!UICONTROL POST]s. 인 경우 [!UICONTROL POST] 성공하면 다음을 받게 됩니다. [!UICONTROL 200개] 응답 메시지.
* **[!UICONTROL PUT]**: 매개 변수를 기반으로 웹 서버의 위치에 데이터를 전송합니다. [!UICONTROL PUT] 요청에는 파일 업로드와 같은 작업이 포함됩니다. 의 차이점 [!UICONTROL PUT] 및 [!UICONTROL POST] 이 PUT은 idempotent이며, 이것은 하나의 성공의 결과를 의미합니다 [!UICONTROL PUT] 은(는) 많은 와(과) 동일합니다. [!UICONTROL PUT]s. PUT이 성공하면 200 응답 메시지(일반적으로 201 또는 204)를 받습니다.
* **[!UICONTROL PATCH]**: (일부 API 호출 모듈에 사용할 수 없음) 매개 변수를 기반으로 웹 서버의 리소스에 부분 수정 사항을 적용합니다. [!UICONTROL PATCH] 은 idempotent가 아닙니다. 즉, 여러 개의 결과가 [!UICONTROL PATCH]의 의도하지 않은 결과가 발생할 수 있습니다. 다음과 같은 경우 [!UICONTROL PATCH] 성공하면 200개의 응답 메시지(일반적으로 204개)를 받게 됩니다.
* **[!UICONTROL DELETE]**: 매개 변수를 기반으로 웹 서버에서 지정된 리소스를 삭제합니다(리소스가 있는 경우). 다음과 같은 경우 [!UICONTROL DELETE] 성공하면 200 OK 응답 메시지가 표시됩니다.
