---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe] Workfront Fusion의 고급 오류 처리'
description: 고급 오류 처리 기술에는 필터링 및 중첩이 포함됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 고급 오류 처리

고급 오류 처리 기술에는 필터링 및 중첩이 포함됩니다.

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

## 필터링

오류 처리기 경로에서 수행할 수 있는 필터링에는 두 가지가 있습니다.

* [오류 처리기 경로에 필터 추가](#adding-a-filter-to-the-error-handler-route)
* [오류 처리기 경로에 필터 뒤에 라우터 추가](#adding-a-router-followed-by-filters-to-the-error-handler)

### 오류 처리기 경로에 필터 추가

필터를 사용하여 오류 처리기 경로에 의해 처리되는 오류를 제어할 수 있습니다. 이를 통해 특정 유형의 오류만 처리할 수 있습니다. 오류가 필터를 통과하지 않으면 해당 모듈에 대해 정의된 오류 처리기 경로가 없는 것처럼 처리됩니다.

>[!INFO]
>
>**예:**
>
>![](assets/filter-error-handling-350x238.png)

### 오류 처리기에 필터 뒤에 [!UICONTROL 라우터]을(를) 추가하는 중

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>이 예제에서는 [!UICONTROL 폴더 만들기] 모듈(A)에서 오류가 발생하며, 이 모듈에는 일반 경로와 오류 처리기 경로가 있습니다. 후자의 라우터는 특정 유형의 오류(데이터 오류가 발생함)를 정의하는 필터가 있는 라우터와 다른 모든 오류에 대한 기본 경로인 라우터로 이어집니다. 첫 번째 경로는 모듈 A에서 다시 시작할 시나리오의 대체 값을 포함하는 [!UICONTROL Resume] 지시문으로 끝나며([!UICONTROL 폴더 만들기]), 두 번째 경로는 시나리오 실행을 즉시 중지하는 [!UICONTROL Rollback] 지시문으로 끝납니다.

다양한 오류 유형과 [!DNL Workfront Fusion]이(가) 오류 처리 및 평가를 수행하는 방법에 대한 자세한 내용은 [오류 처리 위치 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)를 참조하십시오.

### 예제 시나리오

이 예제 시나리오를 설정하여 오류 처리에 대해 이러한 필터가 작동하는 방식을 이해할 수 있습니다.

새 파일을 만드는 대신 기존 [!DNL Dropbox] 폴더를 사용하여 파일을 업로드하십시오.

[!DNL Dropbox]에 [!UICONTROL 폴더 만들기] 모듈을 사용하고 같은 이름의 폴더가 이미 있는 경우 모듈은 아래와 같이 데이터 오류를 발생시킵니다.

![](assets/dropbox-350x276.png)

전체 시나리오:

![](assets/dropbox-scenario-350x190.png)

1. [!UICONTROL 도구] > [!UICONTROL 변수 설정] 모듈에 폴더 이름이 있습니다.
1. [!UICONTROL HTTP] >[!UICONTROL 파일 가져오기] 모듈은 폴더에 업로드해야 하는 파일을 가져옵니다
1. [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈에서 같은 이름으로 매핑된 폴더가 이미 있는 경우 오류가 발생합니다
1. 오류 처리기 경로(투명 버블)에 오류를 필터링할 라우터가 포함되어 있습니다
1. 첫 번째 경로는 데이터 오류라는 지정된 유형의 오류에 대한 것입니다.

   1. 데이터 오류가 발생하고 오류 세부 정보가 필터를 통과할 경우 [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈에 있는 모든 파일/하위 폴더 나열]은(는) [!DNL Dropbox]의 모든 폴더를 나열합니다
   1. 다음 필터는 폴더 이름과 일치합니다
   1. [!UICONTROL Resume] 지시문은 기존 폴더의 폴더 ID와 폴더 경로를 지정하며 시나리오 실행은 [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈에서 다시 시작되지만 새 폴더를 만드는 대신 이번에는 [!UICONTROL Resume] 지시문의 값을 사용하여 다음 모듈로 이동하고 기존 폴더에 파일을 업로드합니다

1. 두 번째 경로는 다른 모든 오류에 대한 것이고 [!UICONTROL Rollback] 지시문으로 끝나므로 시나리오가 즉시 중지됩니다

다음은 5차 성명에 대한 자세한 설명입니다.

후속 모듈([!UICONTROL 아래 파일 업로드])에서 기존 폴더를 사용하려면 모듈에 오류 처리기 경로를 추가하고 다음에 나오는 [!UICONTROL Resume] 지시문 모듈에 매핑될 폴더 경로를 가져와야 합니다.

![](assets/add-error-handler-route-350x113.png)

첫 번째 경로의 필터는 이름이 같은 폴더가 이미 있을 때 나타나는 특정 오류(데이터 오류)만 처리하도록 설정됩니다.

![](assets/condition-350x327.png)

[!UICONTROL Dropbox] >[!UICONTROL 폴더에 있는 모든 파일 나열] 모듈이 대상 폴더에 있는 모든 폴더를 반환하도록 구성되었습니다. 다음 필터는 원래 만들려고 했던 필터만 전달합니다(폴더 이름은 33에 저장됨). 폴더 이름 항목):

![](assets/condition2-350x193.png)

결과적으로 [!UICONTROL Resume] 지시문은 폴더 경로를 실패한 모듈에 대한 출력으로 제공합니다. 폴더 ID는 &#39;[!UICONTROL 파일 업로드]&#39; 모듈에 필요하지 않으므로 비어 있습니다.

![](assets/flow-control-350x190.png)

## 중첩

모듈의 위치에 관계없이 라우터를 제외한 모든 모듈에서 오류 처리기 경로를 만들고 구현할 수 있습니다. 다른 모듈에 대해 만들어진 기존 오류 처리기 경로에 이미 속해 있는 모듈에 대한 오류 처리기 경로를 만들 수 있습니다.

다음은 중첩 오류 처리기 경로의 예입니다.

![](assets/nested-error-handling-route-350x174.png)

이 시나리오에서, 제2 오류 핸들러 경로는 제1 오류 핸들러 경로 아래에 중첩된다. 따라서 [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈 만들기]에서 오류가 발생하면 실행은 경로 1로 이동하고, [!UICONTROL 데이터 오류가 발생하면] 필터가 전달된 경우 다음 모듈이 실행되고, [!UICONTROL Dropbox] >[!UICONTROL 모든 파일/하위 폴더 목록]에서 오류가 발생하지 않으면 [!UICONTROL 다시 시작] 지시문 모듈이 실행됩니다.

그러나 이 [!DNL Dropbox] 모듈에서 오류가 발생하면 실행이 오류 처리기 Route 2로 이동하고 [!UICONTROL Ignore] 지시문으로 끝납니다. 이 경우 [!UICONTROL Resume 지시문] 모듈이 실행되지 않습니다.

이는 오류 처리기 필터링과 중첩의 조합입니다.

