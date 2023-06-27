---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion의 라우터 모듈
description: 라우터 모듈을 사용하면 플로우를 여러 경로로 분기하고 각 경로 내의 데이터를 다르게 처리할 수 있습니다. 라우터 모듈이 번들을 수신하면 라우터가 라우터 모듈에 연결된 순서대로 연결된 각 경로로 전달합니다.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL 라우터] 의 모듈 [!DNL Adobe Workfront Fusion]

다음 [!UICONTROL 라우터] 모듈을 사용하면 플로우를 여러 경로로 분기하고 각 경로 내의 데이터를 다르게 처리할 수 있습니다. 한 번 [!UICONTROL 라우터] 모듈이 번들을 수신하고, 경로가 첨부된 순서대로 연결된 각 경로로 전달합니다. [!UICONTROL 라우터] 모듈.

>[!NOTE]
>
>* 경로의 순서를 확인하려면 [!UICONTROL 자동 정렬] 아이콘 - 위에서 아래로 순서에 따라 경로를 정렬합니다.
>
>  순서를 변경하려면 [!UICONTROL 라우터] 모듈을 지정한 다음 원하는 순서로 경로를 다시 연결합니다.
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

## 추가 [!UICONTROL 라우터] 시나리오에 대한 모듈

A [!UICONTROL 라우터] 다음 방법 중 하나로 시나리오에 추가할 수 있습니다.

* 을(를) 연결하려면 [!UICONTROL 라우터] 모듈 모듈 다음에 있는 모듈의 오른쪽 핸들을 클릭하고 입력을 시작합니다. **[!UICONTROL 라우터]** 을(를) 검색하려면 다음을 선택합니다 **[!UICONTROL 흐름 제어]** > **[!UICONTROL 라우터]** 표시되는 모듈 목록에 있습니다.

  ![](assets/connect-the-router-350x108.png)

* 을(를) 삽입하려면 [!UICONTROL 라우터] 모듈 두 모듈 사이에서 두 모듈을 연결하는 경로 아래의 렌치 아이콘을 클릭하고(또는 경로를 마우스 오른쪽 단추로 클릭) 를 선택합니다 **[!UICONTROL 라우터 추가]** 메뉴에서 삭제할 수 있습니다.

  ![](assets/insert-router-350x191.png)

* 다음을 삽입할 수 있습니다. [!UICONTROL 라우터] 모듈을 자동으로 추가합니다. 예를 들어, 아래 이미지에서 오른쪽 아래 모서리의 모듈을 왼쪽 위 모서리(오른쪽 위 모서리의 모듈에 이미 연결되어 있음)의 모듈에 연결하려면 오른쪽 아래 모듈의 왼쪽 핸들을 드래그하여 왼쪽 위 모듈에 놓습니다.

  ![](assets/insert-router-automatically-350x379.png)

## 필터

다음 경로 뒤에 필터를 배치할 수 있습니다. [!UICONTROL 라우터] 모듈을 사용하여 다른 경로에서 번들을 필터링할 수 있습니다.

1. 경로의 점 중 하나를 클릭합니다.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 다음에서 **[!UICONTROL 필터 설정]** 상자를 표시하고 조건을 추가한 다음 **[!UICONTROL 확인]** 필터 설정을 저장합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

자세한 내용은 [의 시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## 대체 경로

다음 이후 경로에서 필터 설정 [!UICONTROL 라우터] 모듈에는 다음과 같은 특별 옵션이 포함되어 있습니다. 대체 경로:

![](assets/fallback-route-350x260.png)

활성화된 경우 번들을 다음에서 계속 진행할 수 없는 경우 이 경로를 사용합니다. [!UICONTROL 라우터] 다른 경로의 필터에서 필터링되었으므로 다른 경로를 통해 모듈을 필터링합니다.

대체 경로는 내의 다른 화살표 기호와 구별됩니다. [!UICONTROL 라우터] 모듈:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

대체 경로의 일반적인 사용 사례는 다음 단계에서처럼 조건이 충족되면 한 경로에서 흐름을 계속 진행하고 그렇지 않으면 다른 경로에서 흐름을 계속 진행하는 것입니다.

1. 삽입 [!UICONTROL 라우터] 를 입력합니다.
1. 두 경로를 모두 [!UICONTROL 라우터] 모듈 을 참조하십시오.
1. 첫 번째 경로를 클릭하고 조건을 지정합니다.

   ![](assets/set-up-a-filter-2-350x242.png)

1. 두 번째 경로를 클릭하고 [!UICONTROL 대체 경로] 옵션:

   ![](assets/enable-fallback-route-option-350x238.png)
