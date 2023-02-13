---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 데이터 구조 [!DNL Adobe Workfront Fusion]
description: 데이터 구조는 Adobe Workfront Fusion으로 전송되는 데이터의 형식을 자세히 설명하는 문서입니다. 이 문서를 기반으로 시나리오 편집기는 어떤 모듈이 어떤 종류의 데이터를 반환하거나 수신하는지 파악할 수 있습니다. 데이터 구조 문서는 JSON, XML, CSV 및 기타 데이터 형식을 직렬화/구문 분석하는 데 가장 일반적으로 사용됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 의 데이터 구조 [!DNL Adobe Workfront Fusion]

데이터 구조는 전송할 데이터의 형식을 자세히 설명하는 문서입니다 [!DNL Adobe Workfront Fusion]. 이 문서를 기반으로 시나리오 편집기는 어떤 모듈이 어떤 종류의 데이터를 반환하거나 수신하는지 파악할 수 있습니다. 데이터 구조 문서는 JSON, XML, CSV 및 기타 데이터 형식을 직렬화/구문 분석하는 데 가장 일반적으로 사용됩니다.

를 클릭하여 데이터 구조를 만들 수 있습니다 [!UICONTROL 새 데이터 구조 만들기] 단추 [!UICONTROL 데이터 구조 개요] 또는 데이터 구조 사양을 필요로 하는 모듈의 설정에서 참조할 수 있습니다.

지원되는 데이터 유형은 [[!UICONTROL 모듈 유형]](../../workfront-fusion/modules/module-types.md) 문서.

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

## 데이터 구조 생성기

데이터 구조를 항상 만들어야 하는 것은 아닙니다. 내장된 생성기의 템플릿을 사용하면 보다 손쉽게 작업할 수 있습니다. 데이터 샘플을 제공하면 입력한 데이터 샘플을 기반으로 데이터 구조가 자동으로 생성됩니다. 그런 다음 만든 데이터 구조를 수동으로 수정할 수 있습니다.

![](assets/data-structure-generator-350x341.jpg)
