---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 반복자 모듈
description: 반복자 모듈은 배열을 일련의 번들로 변환하는 특별한 유형의 모듈입니다. 각 배열 항목은 별도의 번들로 출력됩니다.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL 반복자] 의 모듈 [!DNL Adobe Workfront Fusion]

An [!UICONTROL 반복자] 모듈은 배열을 일련의 번들로 변환하는 특별한 유형의 모듈입니다. 각 배열 항목은 별도의 번들로 출력됩니다.

자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md) 및 [Adobe Workfront Fusion에서 배열 매핑](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>이 문서에 설명된 기능을 사용하려면 조직에서 Adobe Workfront Fusion과 Adobe Workfront을 구매해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 반복자] 모듈 구성

을(를) 설정했습니다. [!UICONTROL 반복자] 다른 모듈을 설정하는 것과 동일한 모듈입니다. 다음 [!UICONTROL 배열] 필드에는 변환하거나 별도의 번들로 분할할 배열이 포함됩니다.

![](assets/set-up-iterator-350x190.jpg)

자세한 내용은 [Adobe Workfront Fusion에서 모듈 설정 구성](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**예:**
>
>* 아래 시나리오는 첨부 파일이 있는 전자 메일을 검색하고 첨부 파일을 선택한 파일에 단일 파일로 저장하는 방법을 보여 줍니다 [!DNL Dropbox] 폴더를 삭제합니다.
>
>   이메일에는 여러 첨부 파일이 포함될 수 있습니다. 다음 [!UICONTROL 반복자] 첫 번째 모듈 뒤에 삽입된 모듈을 사용하면 각 첨부 파일을 개별적으로 처리할 수 있습니다. 다음 [!UICONTROL 반복자] 모듈은 첨부 파일의 배열을 단일 번들로 분할합니다. 그러면 첨부 파일이 한 개씩 있는 각 번들이 선택한 항목에 한 번에 하나씩 저장됩니다 [!DNL Dropbox] 폴더를 삭제합니다. 다음 [!UICONTROL 반복자] 모듈 설정이 위에 표시되어 있습니다. [!UICONTROL 배열] 필드는 다음을 포함해야 합니다. `Attachments` 배열입니다.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* 귀하의 편의를 위해, 많은 [!DNL Workfront Fusion] 특별 제공되는 앱 [!UICONTROL 반복자] 간소화된 설정이 있는 모듈입니다. 예를 들어 [!UICONTROL 이메일] 앱에 특수 항목 포함 [!UICONTROL 반복자] 모듈 [!UICONTROL 이메일] > [!UICONTROL 첨부 파일 반복] 일반과 같은 결과가 나올 것이다 [!UICONTROL 반복자] 모듈.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## 문제 해결: 매핑 패널에 매핑 가능한 항목이 표시되지 않음 [!UICONTROL 반복자] 모듈

다음의 경우 [!UICONTROL 반복자] 모듈에는 배열 항목의 구조에 대한 정보가 없으며 다음 모듈의 매핑 패널에 있습니다. [!UICONTROL 반복자] 모듈은 아래에 2개의 항목만 표시합니다. [!UICONTROL 반복자] 모듈 :`Total number of bundles` 및 `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

각 모듈은 다음 모듈의 매핑 패널에 이러한 항목이 올바르게 표시될 수 있도록 출력하는 항목에 대한 정보를 제공할 책임이 있기 때문입니다. 그러나 경우에 따라 여러 모듈이 이 정보를 제공하지 못할 수 있습니다(예: ). [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 또는 [!UICONTROL 웹훅] > [!UICONTROL 사용자 지정 웹후크] 누락된 데이터 구조가 있는 모듈.

해결 방법은 시나리오를 수동으로 실행하여 모듈이 출력하는 항목에 대해 학습하도록 하여 다음 모듈에 정보를 제공할 수 있도록 하는 것입니다.

예를 들어 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 다음과 같이 데이터 구조가 없는 모듈:

![](assets/json-parse-json-350x285.png)

그리고 다음을 연결하면 [!UICONTROL 반복자] 이 경우 모듈의 출력을 의 설정 패널에 있는 배열 필드에 매핑할 수 없습니다 [!UICONTROL 반복자] 모듈 :

![](assets/connect-iterator-module-350x146.png)

이 문제를 해결하려면 시나리오 편집기에서 시나리오를 수동으로 시작합니다. 다음 작업 이후에 모듈의 연결을 끊을 수 있습니다. [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 흐름이 더 이상 진행되지 않도록 하는 모듈입니다. 또는 다음을 마우스 오른쪽 단추로 클릭할 수 있습니다. [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 모듈 및 선택 **[!UICONTROL 이 모듈만 실행]** 컨텍스트 메뉴에서 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 모듈.

다음의 경우 [!UICONTROL JSON] > [!UICONTROL JSON 구문 분석] 를 실행하고 출력한 항목에 대해 학습한 후 이 정보를 반복자 모듈을 포함한 모든 후속 모듈에 제공합니다. 그러면 반복자 설정의 매핑 패널에 다음 항목이 표시됩니다.

![](assets/mapping-panel-displays-items-350x131.png)

또한 모듈 뒤에 연결된 모듈의 매핑 패널도 [!UICONTROL 반복자] 모듈은 배열의 항목에 포함된 항목을 표시합니다.

![](assets/items-contained-in-array-350x156.png)

모듈의 매핑 패널에서 일부 항목을 볼 수 없는 경우, 시나리오를 한 번 실행하여 모든 모듈이 출력하는 항목에 대해 학습하고 이 정보를 다음 모듈에 제공합니다.
