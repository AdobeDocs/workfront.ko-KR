---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 에 배열 매핑 [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion의 모듈 필드에 배열을 매핑할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 에 배열 매핑 [!DNL Adobe Workfront Fusion]

배열은 다음을 포함할 수 있는 특수 유형의 항목입니다.

* 하나 이상의 텍스트 값(단순 배열)
* 같은 유형의 컬렉션 하나 이상(복잡한 배열)

>[!INFO]
>
>**예:** 다음 [!UICONTROL 이메일 보기] 모듈은 모든 전자 메일에 대한 일련의 첨부 파일을 반환합니다. 모든 첨부 파일은 이름, 콘텐츠, 크기 등을 포함할 수 있는 컬렉션을 나타냅니다.

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

## 배열 매핑

1. 대상 필드에 있는 버튼을 클릭합니다.

   >[!INFO]
   >
   >  **예:** 위의 예를 보려면 [!UICONTROL 첨부 파일 추가] 버튼입니다.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 표시되는 상자에 품목을 입력합니다.

   패널을 사용하면 다른 유형의 항목과 동일한 방법으로 필드를 매핑할 수 있습니다. 각 항목을 별도로 채우지 않고 다른 배열을 대상 필드에 매핑하려면 [!UICONTROL 맵] 버튼을 클릭합니다. 이 경우 두 배열(소스 어레이와 타겟 배열)의 구조가 동일한지 확인합니다.

   배열에 원하는 개수의 항목을 추가할 수 있습니다.

반복기를 사용하여 배열을 개별 번들로 나눌 수 있습니다. 자세한 내용은 [[!UICONTROL 반복기] 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
