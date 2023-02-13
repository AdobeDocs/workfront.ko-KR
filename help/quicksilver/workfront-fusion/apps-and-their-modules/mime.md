---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME 모듈
description: Adobe Workfront Fusion에서 MIME 유형을 사용할 수 있습니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형 텍스트/html인 파일은 MIME 유형 이미지/jpeg의 파일과 다르게 브라우저에서 처리됩니다. MIME 유형은 운영 체제 및 하드웨어에 관계없이 작동합니다.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] 모듈

Adobe Workfront Fusion에서 MIME 유형을 사용할 수 있습니다. MIME(Multipurpose Internet Mail Extension) 유형은 소프트웨어가 인터넷에서 공유되는 서로 다른 유형의 데이터를 식별할 수 있도록 하는 레이블입니다. 웹 서버와 브라우저는 MIME 유형을 사용하여 파일로 수행할 작업을 결정합니다. 예를 들어 MIME 유형을 갖는 파일입니다 `text/html` 은 MIME 유형을 사용하는 파일과 다르게 브라우저에서 처리됩니다 `image/jpeg`. MIME 유형은 운영 체제 및 하드웨어에 관계없이 작동합니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] 모듈 및 해당 필드

### [!UICONTROL MIME 유형 가져오기]

이 변압기 모듈은 지정된 이름, 경로 또는 확장과 연결된 MIME 유형을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL File]</td> 
   <td> <p>MIME 유형을 결정할 파일을 입력하거나 매핑하십시오. </p> <p>다음을 사용하여 파일을 입력할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 경로]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL 파일 이름]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL File Extension]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 파일 확장명 가져오기]

이 변압기 모듈은 지정된 MIME 유형에 대한 원래 파일 확장명을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME 유형]</td> 
   <td> <p>파일 확장자를 결정할 MIME 유형을 입력하거나 매핑하십시오. </p> </td> 
  </tr> 
 </tbody> 
</table>
