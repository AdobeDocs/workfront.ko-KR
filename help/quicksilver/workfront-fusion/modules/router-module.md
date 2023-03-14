---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 라우터 모듈
description: 라우터 모듈을 사용하면 흐름을 여러 경로로 분기하고 각 경로 내에서 데이터를 다르게 처리할 수 있습니다. 라우터 모듈이 번들을 수신하면 라우터 모듈에 연결된 각 라우트에 해당 경로가 연결된 순서대로 전달됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!UICONTROL 라우터] 모듈 [!DNL Adobe Workfront Fusion]

다음 [!UICONTROL 라우터] 모듈을 사용하면 여러 경로에 플로우를 분기하고 각 경로 내에서 데이터를 다르게 처리할 수 있습니다. 한 번 [!UICONTROL 라우터] 모듈이 번들을 수신하고, 연결된 각 경로들에 해당 경로가 연결된 순서대로 전달됩니다 [!UICONTROL 라우터] 모듈.

>[!NOTE]
>
>* 경로 순서를 확인하려면 [!UICONTROL 자동 정렬] 아이콘. 위에서 아래로 이동하는 순서에 따라 경로를 정렬합니다.
>
>  순서를 변경하려면 [!UICONTROL 라우터] 모듈 및 원하는 순서로 경로를 다시 연결합니다.
>
>* 경로는 평행이 아닌 순차적으로 처리됩니다. 이전 경로에 의해 번들이 완전히 처리될 때까지 다음 경로로 전송됩니다.
>




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

## 추가 [!UICONTROL 라우터] 시나리오 모듈

A [!UICONTROL 라우터] 다음 방법 중 하나로 시나리오에 추가할 수 있습니다.

* 연결을 원하는 경우 [!UICONTROL 라우터] 모듈 다음에 모듈의 오른쪽 핸들을 클릭하고 입력을 시작합니다 **[!UICONTROL 라우터]** 검색하려면 **[!UICONTROL 흐름 제어]** > **[!UICONTROL 라우터]** 를 클릭합니다.

   ![](assets/connect-the-router-350x108.png)

* 를 삽입하려면 [!UICONTROL 라우터] 두 모듈 사이의 모듈인 두 모듈을 연결하는 경로 아래의 공구모양 아이콘(또는 경로를 마우스 오른쪽 버튼으로 클릭)을 클릭하고 **[!UICONTROL 라우터 추가]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/insert-router-350x191.png)

* 을(를) 삽입할 수 있습니다 [!UICONTROL 라우터] 모듈 을 자동으로 검색합니다. 예를 들어, 아래 이미지에서 오른쪽 아래 모서리에 있는 모듈을 왼쪽 위 모서리에 있는 모듈(이미 오른쪽 위 모서리에 있는 모듈과 연결)과 연결하려면 오른쪽 아래 모듈의 왼쪽 핸들을 드래그하여 왼쪽 위 모듈에 놓습니다.

   ![](assets/insert-router-automatically-350x379.png)

## 필터

다음에 경로에 필터를 설정할 수 있습니다. [!UICONTROL 라우터] 다른 경로에서 번들을 필터링하는 모듈.

1. 경로에 있는 점 중 하나를 클릭합니다.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 에서 **[!UICONTROL 필터 설정]** 표시되는 상자에서 조건을 추가한 다음 를 클릭합니다 **[!UICONTROL 확인]** 필터 설정을 저장하려면 을 클릭합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

자세한 내용은 [의 시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## 대체 경로

다음 경로 이후의 경로에 필터 설정 [!UICONTROL 라우터] 모듈에는 다음과 같은 특수 옵션이 포함되어 있습니다. 대체 경로:

![](assets/fallback-route-350x260.png)

활성화되면 번들이 Marketing Cloud ID 클라이언트측 또는 Analytics Premium에서 계속 [!UICONTROL 라우터] 다른 경로의 필터가 해당 경로를 필터링했으므로 다른 경로를 통해 모듈합니다.

대체 경로는 [!UICONTROL 라우터] 모듈:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

대체 경로의 일반적인 사용 사례는 조건이 충족되는 경우 한 라우트와 그렇지 않은 경우 다른 라우트로 흐름을 계속 이동하는 것입니다.

1. 삽입 [!UICONTROL 라우터] 모듈의 수준을 제어합니다.
1. 두 경로를 [!UICONTROL 라우터] 모듈 .
1. 첫 번째 경로를 클릭하고 조건을 지정합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

1. 두 번째 경로를 클릭하고 [!UICONTROL 대체 경로] 옵션:

   ![](assets/enable-fallback-route-option-350x238.png)
