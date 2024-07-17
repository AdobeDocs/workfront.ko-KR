---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe] Workfront Fusion에서 배열 매핑'
description: Adobe Workfront Fusion의 모듈 필드에 배열을 매핑할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 배열 매핑

배열은 다음을 포함할 수 있는 특수한 유형의 항목입니다.

* 하나 이상의 텍스트 값(단순 배열)
* 동일한 유형의 컬렉션 하나 이상(복잡한 배열)

>[!INFO]
>
>**예:** [!UICONTROL 전자 메일 보기] 모듈은 모든 전자 메일에 대한 첨부 파일 배열을 반환합니다. 모든 첨부 파일은 이름, 콘텐츠, 크기 등을 포함할 수 있는 컬렉션을 나타냅니다.

자세한 내용은 [항목 데이터 형식 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)을 참조하세요.

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

## 배열 매핑

1. 대상 필드에 있는 버튼을 클릭합니다.

   >[!INFO]
   >
   >  **예:** 위 예제의 경우 전자 메일의 [!UICONTROL 첨부 파일 추가] 단추를 클릭합니다.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 표시되는 상자에 항목을 입력합니다.

   패널을 사용하면 다른 유형의 항목과 동일한 방식으로 필드를 매핑할 수 있습니다. 각 항목을 따로 채우지 않고 다른 배열을 대상 필드에 매핑하려면 [!UICONTROL 맵] 단추를 사용합니다. 이 경우 두 배열(소스 배열과 타겟 배열)의 구조가 동일해야 합니다.

   배열에 항목을 원하는 수만큼 추가할 수 있습니다.

반복기를 사용하여 배열을 개별 번들로 나눌 수 있습니다. 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)의 [[!UICONTROL 반복자] 모듈을 참조하십시오.
