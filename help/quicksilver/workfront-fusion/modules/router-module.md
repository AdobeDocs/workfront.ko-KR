---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 라우터 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 [!UICONTROL 라우터] 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [라우터 모듈 추가 및 경로 구성](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/router-module.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!UICONTROL 라우터] 모듈을 사용하면 흐름을 여러 경로로 분기하고 각 경로 내의 데이터를 다르게 처리할 수 있습니다. [!UICONTROL Router] 모듈이 번들을 받으면, [!UICONTROL Router] 모듈에 경로가 첨부된 순서대로 연결된 각 경로로 전달합니다.

>[!NOTE]
>
>* 경로의 순서를 확인하려면 [!UICONTROL 자동 정렬] 아이콘을 클릭하면 위쪽에서 아래쪽의 순서에 따라 경로가 정렬됩니다.
>
>  순서를 변경하려면 [!UICONTROL 라우터] 모듈을 제거하고 원하는 순서로 경로를 다시 연결하십시오.
>
>* 경로는 병렬로 처리되지 않고 순차적으로 처리됩니다. 이전 경로에서 완전히 처리될 때까지 번들이 다음 경로로 전송되지 않습니다.
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

## 시나리오에 [!UICONTROL 라우터] 모듈 추가 중

다음 방법 중 하나로 [!UICONTROL 라우터]를 시나리오에 추가할 수 있습니다.

* 모듈 뒤에 [!UICONTROL Router] 모듈을 연결하려면 모듈의 오른쪽 핸들을 클릭하고 **[!UICONTROL Router]**&#x200B;을(를) 입력하여 검색한 다음 표시되는 모듈 목록에서 **[!UICONTROL 흐름 제어]** > **[!UICONTROL Router]**&#x200B;을(를) 선택하십시오.

  ![](assets/connect-the-router-350x108.png)

* 두 모듈 사이에 [!UICONTROL 라우터] 모듈을 삽입하려면 두 모듈을 연결하는 경로 아래의 렌치 아이콘을 클릭하거나 경로를 마우스 오른쪽 단추로 클릭하고 메뉴에서 **[!UICONTROL 라우터 추가]**&#x200B;를 선택하십시오.

  ![](assets/insert-router-350x191.png)

* [!UICONTROL 라우터] 모듈을 자동으로 삽입할 수 있습니다. 예를 들어, 아래 이미지에서 오른쪽 아래 모서리의 모듈을 왼쪽 위 모서리(오른쪽 위 모서리의 모듈에 이미 연결되어 있음)의 모듈에 연결하려면 오른쪽 아래 모듈의 왼쪽 핸들을 드래그하여 왼쪽 위 모듈에 놓습니다.

  ![](assets/insert-router-automatically-350x379.png)

## 필터

[!UICONTROL Router] 모듈 뒤에 경로에 필터를 추가하여 다른 경로와 마찬가지로 번들을 필터링할 수 있습니다.

1. 경로의 점 중 하나를 클릭합니다.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 표시되는 **[!UICONTROL 필터 설정]** 상자에서 조건을 추가한 다음 **[!UICONTROL 확인]**&#x200B;을 클릭하여 필터 설정을 저장합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

자세한 내용은 [시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)를 참조하십시오.

## 대체 경로

[!UICONTROL 라우터] 모듈 이후의 경로에 대한 필터 설정에 다음과 같은 특별 옵션이 있습니다. 대체 경로:

![](assets/fallback-route-350x260.png)

활성화하면 다른 경로의 필터가 필터링하여 [!UICONTROL Router] 모듈에서 다른 경로를 통해 번들을 계속할 수 없는 경우에 이 경로를 사용합니다.

대체 경로는 [!UICONTROL 라우터] 모듈 내에서 다른 화살표 기호와 구분됩니다.

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

대체 경로의 일반적인 사용 사례는 다음 단계에서처럼 조건이 충족되면 한 경로에서 흐름을 계속 진행하고 그렇지 않으면 다른 경로에서 흐름을 계속 진행하는 것입니다.

1. 시나리오에 [!UICONTROL 라우터] 모듈을 삽입하십시오.
1. 두 경로를 [!UICONTROL 라우터] 모듈에 연결합니다.
1. 첫 번째 경로를 클릭하고 조건을 지정합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

1. 두 번째 경로를 클릭하고 [!UICONTROL 대체 경로] 옵션을 활성화하십시오.

   ![](assets/enable-fallback-route-option-350x238.png)
