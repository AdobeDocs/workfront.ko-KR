---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 의 고급 오류 처리 [!DNL Adobe] Workfront Fusion
description: 고급 오류 처리 기술에는 필터링 및 중첩이 포함됩니다.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 의 고급 오류 처리 [!DNL Adobe Workfront Fusion]

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

### 추가 [!UICONTROL 라우터] 뒤에 오류 처리기에 대한 필터가 옵니다.

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>이 예제에서 오류는 [!UICONTROL 폴더 만들기] 모듈 (A): 일반 경로와 오류 처리기 경로가 있습니다. 후자의 라우터는 특정 유형의 오류(데이터 오류가 발생함)를 정의하는 필터가 있는 라우터와 다른 모든 오류에 대한 기본 경로인 라우터로 이어집니다. 첫 번째 경로는 [!UICONTROL 다시 시작] 모듈 A에서 재개할 시나리오에 대한 대체 값을 포함하는 지시문([!UICONTROL 폴더 만들기]), 반면에 두 번째 경로는 [!UICONTROL 롤백] 시나리오 실행을 즉시 중지하는 지시문입니다.

다음을 참조하십시오 [에서 처리하는 동안 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 를 참조하십시오. [!DNL Workfront Fusion] 는 이러한 프로세스를 처리하고 평가합니다.

### 예제 시나리오

이 예제 시나리오를 설정하여 오류 처리에 대해 이러한 필터가 작동하는 방식을 이해할 수 있습니다.

기존 항목 사용 [!DNL Dropbox] 새 파일을 만드는 대신 파일을 업로드할 폴더

를 사용하는 경우 [!UICONTROL 폴더 만들기] 다음에 대한 모듈 [!DNL Dropbox] 이름이 같은 폴더가 이미 있으면 모듈은 아래와 같이 데이터 오류를 발생시킵니다.

![](assets/dropbox-350x276.png)

전체 시나리오:

![](assets/dropbox-scenario-350x190.png)

1. 다음 [!UICONTROL 도구] > [!UICONTROL 변수 설정] 모듈에 폴더 이름이 포함되어 있음
1. 다음 [!UICONTROL HTTP] >[!UICONTROL 파일 가져오기] 모듈이 폴더에 업로드해야 하는 파일을 가져옵니다.
1. 다음 [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈에 매핑된 폴더와 동일한 이름의 폴더가 이미 있는 경우 모듈에서 오류가 발생합니다
1. 오류 처리기 경로(투명 버블)에 오류를 필터링할 라우터가 포함되어 있습니다
1. 첫 번째 경로는 데이터 오류라는 지정된 유형의 오류에 대한 것입니다.

   1. 데이터 오류가 발생하고 오류 세부 정보가 필터를 통과하는 경우 [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈의 모든 파일/하위 폴더 나열] 의 모든 폴더를 나열합니다. [!DNL Dropbox]
   1. 다음 필터는 폴더 이름과 일치합니다
   1. 다음 [!UICONTROL 다시 시작] 디렉티브는 기존 폴더의 폴더 ID와 폴더 경로를 지정하며 [!UICONTROL Dropbox] >[!UICONTROL 폴더 만들기] 모듈이지만 새 폴더를 만들려고 하는 대신 이번에는 [!UICONTROL 다시 시작] 다음 모듈로 이동하고 기존 폴더에 파일을 업로드하는 지시문

1. 두 번째 경로는 다른 모든 오류에 대한 것으로, [!UICONTROL 롤백] 시나리오를 즉시 중지하는 지시문

다음은 5차 성명에 대한 자세한 설명입니다.

후속 모듈에서 기존 폴더를 사용하려면[!UICONTROL 파일 업로드] 아래 참조)에서 모듈에 오류 처리기 경로를 추가하고 매핑할 폴더 경로를 가져와야 합니다. [!UICONTROL 다시 시작] 다음 지시문 모듈:

![](assets/add-error-handler-route-350x113.png)

첫 번째 경로의 필터는 이름이 같은 폴더가 이미 있을 때 나타나는 특정 오류(데이터 오류)만 처리하도록 설정됩니다.

![](assets/condition-350x327.png)

다음 [!UICONTROL Dropbox] >[!UICONTROL 폴더의 모든 파일 나열] 대상 폴더의 모든 폴더를 반환하도록 모듈이 구성되어 있습니다. 다음 필터는 원래 만들려고 했던 필터만 전달합니다(폴더 이름은 33에 저장됨). 폴더 이름 항목):

![](assets/condition2-350x193.png)

결국, [!UICONTROL 다시 시작] 디렉티브는 폴더 경로를 실패한 모듈에 대한 출력으로 제공합니다. 폴더 ID는 &#39;에 필요하지 않으므로 비워 두었습니다.[!UICONTROL 파일 업로드]&#39; 모듈:

![](assets/flow-control-350x190.png)

## 중첩

모듈의 위치에 관계없이 라우터를 제외한 모든 모듈에서 오류 처리기 경로를 만들고 구현할 수 있습니다. 다른 모듈에 대해 만들어진 기존 오류 처리기 경로에 이미 속해 있는 모듈에 대한 오류 처리기 경로를 만들 수 있습니다.

다음은 중첩 오류 처리기 경로의 예입니다.

![](assets/nested-error-handling-route-350x174.png)

이 시나리오에서, 제2 오류 핸들러 경로는 제1 오류 핸들러 경로 아래에 중첩된다. 그렇다면 [!UICONTROL Dropbox] >[!UICONTROL 폴더 모듈 만들기] 오류가 발생하면 실행이 경로 1로 이동합니다. [!UICONTROL 데이터 오류 발생] 필터가 전달되고 다음 모듈이 실행되며 [!UICONTROL 다시 시작] 에서 오류가 발생하지 않는 경우 디렉티브 모듈 [!UICONTROL Dropbox] >[!UICONTROL 모든 파일/하위 폴더 나열] 폴더 모듈에 있습니다.

단, 이 작업에 오류가 발생하는 경우 [!DNL Dropbox] 그런 다음 실행이 오류 핸들러 경로 2로 이동하고 [!UICONTROL 무시] 지시문입니다. 다음 [!UICONTROL Resume 지시문] 이 경우에는 모듈이 실행되지 않습니다.

이는 오류 처리기 필터링과 중첩의 조합입니다.

