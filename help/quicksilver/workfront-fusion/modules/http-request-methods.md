---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]
description: 모듈에서 API 호출을 구성할 때 HTTP 요청 메서드에 대한 필드를 입력해야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]

모듈에서 API 호출을 구성할 때 HTTP 요청 메서드에 대한 필드를 입력해야 합니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## HTTP 메서드

다음 HTTP 메서드 중 하나를 사용합니다.

* **[!UICONTROL GET]**: 매개 변수를 기반으로 웹 서버에서 데이터를 검색합니다. [!UICONTROL GET] 지정된 리소스의 표시를 요청하고 [!UICONTROL 200 OK] 성공하면 요청된 콘텐츠가 포함된 응답 메시지를 반환합니다.
* **[!UICONTROL POST]**: 매개 변수를 기반으로 웹 서버에 데이터를 보냅니다. [!UICONTROL POST] 요청에는 파일 업로드와 같은 작업이 포함됩니다. 다중 [!UICONTROL POST]1개의 결과와는 다른 결과를 초래할 수 있습니다 [!UICONTROL POST], 실수로 여러 개를 전송하는 것에 대해 주의 [!UICONTROL POST]s. 다음과 같은 경우 [!UICONTROL POST] 이(가) 성공하면 [!UICONTROL 200 OK] 응답 메시지.
* **[!UICONTROL PUT]**: 매개 변수를 기반으로 웹 서버의 위치로 데이터를 보냅니다. [!UICONTROL PUT] 요청에는 파일 업로드와 같은 작업이 포함됩니다. 의 차이점 [!UICONTROL PUT] 및 [!UICONTROL POST] PUT은 idempotent입니다. 즉, 하나의 성공적인 결과로 [!UICONTROL PUT] 는 동일한 수와 같습니다 [!UICONTROL PUT]s. PUT이 성공하면 200개의 응답 메시지(일반적으로 201개 또는 204개)를 받게 됩니다.
* **[!UICONTROL PATCH]**: (일부 API 호출 모듈에는 사용할 수 없음) 매개 변수를 기반으로 웹 서버의 리소스에 부분 수정 사항을 적용합니다. [!UICONTROL PATCH] 는 idempotent가 아닙니다. 즉, 여러 개의 결과가 [!UICONTROL PATCH]그것은 의도하지 않은 결과를 초래할 수 있다. 다음과 같은 경우 [!UICONTROL PATCH] 에 성공하면 200개의 응답 메시지(일반적으로 204개)를 받게 됩니다.
* **[!UICONTROL DELETE]**: 매개 변수를 기반으로 웹 서버에서 지정된 리소스를 삭제합니다(리소스가 있는 경우). 다음과 같은 경우 [!UICONTROL DELETE] 이(가) 성공하면 200 OK 응답 메시지를 받게 됩니다.
