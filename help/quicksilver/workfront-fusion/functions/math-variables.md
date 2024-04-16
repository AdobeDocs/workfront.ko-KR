---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 의 수학 변수 [!DNL Adobe Workfront Fusion]
description: 다음 수학 변수는 [!DNL Adobe Workfront Fusion mapping] 패널.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 3%

---

# 의 수학 변수 [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td>  
   <td> <p>임의</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td>  
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td>  
   <td> 
   <p>현재: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p> 
   <p>또는</p> 
   <p>레거시: 모두 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">제품</td>  
   <td> 
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 플랜: [!DNL Workfront Fusion] 포함됩니다.</li></ul> 
   <p>또는</p> 
   <p>현재: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## pi

수학 기호 $\pi$를 나타냅니다.

## [!UICONTROL random]

범위에서 부동 소수점 의사 난수를 반환합니다. [`0`,`1`] (포함) `0`, 그러나 아님 `1`).

다음 수식을 사용하여 범위에서 정수 의사 난수를 생성합니다 [`min`,`max`] (둘 다 포함) `min` 및 `max`):

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
