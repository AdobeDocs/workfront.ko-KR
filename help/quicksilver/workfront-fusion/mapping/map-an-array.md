---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 에서 배열 매핑 [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion의 모듈 필드에 배열을 매핑할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 에서 배열 매핑 [!DNL Adobe Workfront Fusion]

배열은 다음을 포함할 수 있는 특수한 유형의 항목입니다.

* 하나 이상의 텍스트 값(단순 배열)
* 동일한 유형의 컬렉션 하나 이상(복잡한 배열)

>[!INFO]
>
>**예:** 다음 [!UICONTROL 이메일 보기] 모듈은 모든 이메일에 대한 첨부 파일 배열을 반환합니다. 모든 첨부 파일은 이름, 콘텐츠, 크기 등을 포함할 수 있는 컬렉션을 나타냅니다.

자세한 내용은 [의 항목 데이터 유형 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## 배열 매핑

1. 대상 필드에 있는 버튼을 클릭합니다.

   >[!INFO]
   >
   >  **예:** 위의 예에서는 [!UICONTROL 첨부 파일 추가] 이메일 버튼.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 표시되는 상자에 항목을 입력합니다.

   패널을 사용하면 다른 유형의 항목과 동일한 방식으로 필드를 매핑할 수 있습니다. 각 항목을 별도로 채우지 않고 다른 배열을 대상 필드에 매핑하려면 [!UICONTROL 맵] 단추를 클릭합니다. 이 경우 두 배열(소스 배열과 타겟 배열)의 구조가 동일해야 합니다.

   배열에 항목을 원하는 수만큼 추가할 수 있습니다.

반복기를 사용하여 배열을 개별 번들로 나눌 수 있습니다. 자세한 내용은 [[!UICONTROL 반복자] 의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
