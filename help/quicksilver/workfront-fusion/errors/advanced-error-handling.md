---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 의 고급 오류 처리 [!DNL Adobe] Workfront Fusion
description: 고급 오류 처리 방법에는 필터링 및 중첩이 포함됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# 의 고급 오류 처리 [!DNL Adobe Workfront Fusion]

고급 오류 처리 방법에는 필터링 및 중첩이 포함됩니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 필터링

오류 처리기 경로에서 발생할 수 있는 두 가지 종류의 필터링이 있습니다.

* [오류 처리기 경로에 필터 추가](#adding-a-filter-to-the-error-handler-route)
* [오류 처리기 경로에 라우터를 추가하고 필터를 추가합니다.](#adding-a-router-followed-by-filters-to-the-error-handler)

### 오류 처리기 경로에 필터 추가

필터를 사용하여 오류 처리기 경로에서 처리하는 오류를 제어할 수 있습니다. 이를 통해 특정 유형의 오류만 처리할 수 있습니다. 오류가 필터를 통과하지 않으면 해당 모듈에 대해 정의된 오류 처리기 경로가 없는 것처럼 처리됩니다.

>[!INFO]
>
>**예:**
>
>![](assets/filter-error-handling-350x238.png)

### 추가 [!UICONTROL 라우터] 다음에 오류 처리기에 필터가 옵니다.

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>이 예제에서 오류는 [!UICONTROL 폴더 만들기] 모듈(A)에 대한 경로 및 오류 처리기 경로가 있습니다. 후자는 특정 유형의 오류(데이터 오류 발생)를 정의하는 필터가 있는 라우터와 다른 라우터가 있으며, 다른 라우터는 다른 모든 오류의 기본 경로입니다. 첫 번째 경로는 [!UICONTROL 다시 시작] 모듈 A에서 재개할 시나리오에 대한 대체 값을 포함하는 지시문입니다([!UICONTROL 폴더 만들기]로 끝나는 경우) [!UICONTROL 롤백] 시나리오 실행을 즉시 중지하는 지시문입니다.

자세한 내용은 [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 다양한 오류 유형 및 방법에 대한 자세한 정보 [!DNL Workfront Fusion] 처리 및 평가합니다.

### 예제 시나리오

이 예제 시나리오를 설정하여 오류 처리에 대해 이러한 필터가 작동하는 방식을 이해할 수 있습니다.

기존 [!DNL Dropbox] 새 파일을 만드는 대신 업로드하는 폴더

를 사용하는 경우 [!UICONTROL 폴더 만들기] 모듈 [!DNL Dropbox] 및 이름이 같은 폴더가 이미 있으면 모듈에 아래와 같이 데이터 오류가 발생합니다.

![](assets/dropbox-350x276.png)

전체 시나리오:

![](assets/dropbox-scenario-350x190.png)

1. 다음 [!UICONTROL 도구] > [!UICONTROL 변수 설정] 모듈에는 폴더 이름이 포함되어 있습니다.
1. 다음 [!UICONTROL HTTP] >[!UICONTROL 파일 가져오기] 모듈은 폴더에 업로드해야 하는 파일을 가져옵니다
1. 다음 [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈에 매핑된 폴더와 동일한 이름을 가진 폴더가 이미 있으면 모듈에 오류가 발생합니다
1. 오류 처리기 경로(투명한 버블)에 오류를 필터링할 라우터가 있습니다
1. 첫 번째 경로는 Data Error라는 지정된 유형의 오류에 대한 것입니다.

   1. 데이터 오류가 발생하고 오류 세부 정보가 필터를 통과하는 경우 [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈에 모든 파일/하위 폴더 나열] 의 [!DNL Dropbox]
   1. 후속 필터는 폴더 이름과 일치합니다
   1. 다음 [!UICONTROL 다시 시작] 지시문은 기존 폴더의 폴더 ID와 폴더 경로를 지정하고 시나리오 실행은 다음에서 재개됩니다 [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈 대신 새 폴더를 만들려 하지 않고 이번에는 [!UICONTROL 다시 시작] 다음 모듈로 이동하고 기존 폴더에 파일을 업로드하는 지시문

1. 두 번째 경로는 다른 모든 오류에 대한 경로이며 [!UICONTROL 롤백] 시나리오를 즉시 중지하는 지시문

아래는 5차 문구에 대한 상세한 설명이다.

후속 모듈에서 기존 폴더를 사용하려면[!UICONTROL 파일 업로드] 아래) 모듈에 오류 처리기 경로를 추가하고 폴더에 매핑할 폴더 경로를 가져와야 합니다. [!UICONTROL 다시 시작] 다음과 같은 지시문 모듈입니다.

![](assets/add-error-handler-route-350x113.png)

첫 번째 경로의 필터는 같은 이름의 폴더가 이미 있을 때 나타나는 특정 오류(데이터 오류)만 처리하도록 설정됩니다.

![](assets/condition-350x327.png)

다음 [!UICONTROL Dropbox] >[!UICONTROL 폴더에 있는 모든 파일 나열] 모듈이 대상 폴더의 모든 폴더를 반환하도록 구성되어 있습니다. 다음 필터는 원래 만들려 했던 필터만 전달합니다(폴더 이름은 33에 저장됩니다.). 폴더 이름 항목):

![](assets/condition2-350x193.png)

결국, [!UICONTROL 다시 시작] 지시문은 폴더 경로를 실패한 모듈의 출력으로 제공합니다. 폴더 ID는 &#39;[!UICONTROL 파일 업로드]&#39; 모듈:

![](assets/flow-control-350x190.png)

## 중첩

모듈의 위치에 관계없이 라우터를 제외한 모든 모듈에 오류 처리기 경로를 만들고 구현할 수 있습니다. 따라서 다른 모듈에 대해 생성된 기존 오류 처리기 경로의 일부인 모듈의 오류 처리기 경로를 만들 수 있습니다.

다음은 중첩 오류 처리기 경로의 예입니다.

![](assets/nested-error-handling-route-350x174.png)

이 시나리오에서는 두 번째 오류 처리기 경로가 첫 번째 오류 처리기 경로 아래에 중첩됩니다. 그러니까, [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈 만들기] 오류가 발생하면 가 [!UICONTROL 데이터 오류가 발생합니다] 필터가 전달되면 다음 모듈이 실행되고 그 다음에 [!UICONTROL 다시 시작] 오류가 발생하지 않는 경우 지시문 모듈 [!UICONTROL Dropbox] >[!UICONTROL 모든 파일/하위 폴더 나열] ( 폴더 모듈) 아래에 그룹화됩니다.

그러나 이와 함께 오류가 발생하는 경우 [!DNL Dropbox] 모듈을 호출한 다음, 실행이 오류 처리기 경로 2로 이동하여 [!UICONTROL 무시] 지시문 다음 [!UICONTROL Resume 지시문] 이 경우 모듈이 실행되지 않습니다.

이는 필터링 및 중첩 오류 처리기의 조합입니다.

