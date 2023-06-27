---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 의 데이터 구조 [!DNL Adobe Workfront Fusion]
description: 데이터 구조는 Adobe Workfront Fusion으로 전송되는 데이터의 형식을 자세히 설명하는 문서입니다. 이 문서를 기반으로 시나리오 편집기는 어떤 모듈이 어떤 종류의 데이터를 반환하거나 수신하는지 파악할 수 있습니다. 데이터 구조 문서는 JSON, XML, CSV 및 기타 데이터와 같은 데이터 형식을 직렬화/구문 분석하는 데 가장 일반적으로 사용됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 의 데이터 구조 [!DNL Adobe Workfront Fusion]

데이터 구조는 전송되는 데이터의 형식을 자세히 설명하는 문서입니다 [!DNL Adobe Workfront Fusion]. 이 문서를 기반으로 시나리오 편집기는 어떤 모듈이 어떤 종류의 데이터를 반환하거나 수신하는지 파악할 수 있습니다. 데이터 구조 문서는 JSON, XML, CSV 및 기타 데이터와 같은 데이터 형식을 직렬화/구문 분석하는 데 가장 일반적으로 사용됩니다.

다음을 클릭하여 데이터 구조를 만들 수 있습니다. [!UICONTROL 새 데이터 구조 만들기] 의 단추 [!UICONTROL 데이터 구조 개요] 섹션에 있는 마지막 항목이 될 필요가 없습니다.

지원되는 데이터 유형은 다음에 설명되어 있습니다. [[!UICONTROL 모듈 유형]](../../workfront-fusion/modules/module-types.md) 기사.

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

## 데이터 구조 생성기

데이터 구조를 항상 만들 필요는 없습니다. 기본 제공 생성기의 템플릿을 사용하면 보다 쉽게 만들 수 있습니다. 데이터 샘플을 제공하면 생성기가 입력한 데이터 샘플을 기반으로 데이터 구조를 자동으로 만듭니다. 그런 다음 생성된 데이터 구조를 수동으로 수정할 수 있습니다.

![](assets/data-structure-generator-350x341.jpg)
