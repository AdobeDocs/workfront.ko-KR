---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 모듈 유형
description: 'Adobe Workfront Fusion은 다음 다섯 가지 유형의 모듈을 구별합니다. 작업 모듈, 검색 모듈, 트리거 모듈, 누적 및 반복기 누적 및 반복자는 고급 시나리오에 사용됩니다.'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# 모듈 유형

A[!UICONTROL Adobe Workfront Fusion] 다음 다섯 가지 유형의 모듈을 구별합니다. 작업 모듈, 검색 모듈, 트리거 모듈, 누적 및 반복기 누적 및 반복자는 고급 시나리오에 사용됩니다.

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
   <td>이 문서에 설명된 기능을 사용하려면 조직이 Adobe Workfront Fusion과 Adobe Workfront을 구입해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 작업 모듈

작업 모듈은 가장 일반적인 모듈 유형입니다. 일반적인 작업 모듈은 단일 번들을 반환하고, 이 번들은 처리를 위해 다음 모듈로 전달됩니다.

트리거 모듈과 달리 작업 모듈은 시나리오의 시작, 중간 또는 끝에 배치할 수 있습니다. 시나리오에는 무제한의 작업 모듈이 포함될 수 있습니다.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 파일 업로드]** 에 파일 보내기 [!DNL Workfront] 및에서 해당 식별자를 반환합니다.
>* **[!UICONTROL 이미지] > [!UICONTROL 크기 조정]** 이미지를 받고, 지정된 차원으로 크기를 조정하고, 크기를 조정한 이미지를 다음 작업에 전달합니다.


작업 유형에는 네 가지 하위 유형이 있습니다. 작성, 읽기, 업데이트 및 삭제 업데이트 하위 유형은 다음 세 가지 작업을 활성화합니다.

* **필드의 컨텐츠 지우기**. 이 작업은 필드의 내용이 키워드 지우기(와 혼동하지 않도록)로 평가될 때 발생합니다 *비어 있음*).

   ![](assets/erase-content-of-field.png)

* **필드의 내용을 변경하지 않고 그대로 둡니다**. 이 작업은 필드가 비어 있거나 필드의 컨텐츠가 비어 있다고 평가될 때(JSON에서 null을 통해 표시됨) 발생합니다.

   ![](assets/leave-content-field-unchanged-350x231.png)

* **필드의 컨텐츠 바꾸기**. 이 작업은 위에서 설명한 두 가지 이외의 다른 모든 경우에 수행됩니다.

>[!NOTE]
>
>* 이 표시되지 않으면 `erase` 매핑 패널에서 키워드가 업데이트되었거나 모듈이 앱에 대한 최신 사양으로 업데이트되지 않았습니다.
>* &quot;[!UICONTROL Empty]필드 내용은 변경되지 않습니다. 필드를 지워야 하는 경우 다음 공식을 사용할 수 있습니다.
>
>![](assets/formula-ifempty-name-erase.png)
>
>콘텐츠를 빈 것으로 평가할 때 필드를 변경하지 않는 상태로 두는 것은 현재 사용할 수 없습니다.

## 검색 모듈

일반적인 검색은 0이나 1개 이상의 번들을 반환한 다음 처리를 위해 다음 모듈로 전달합니다.

시나리오의 시작, 중간 또는 끝에 검색을 배치할 수 있습니다.

시나리오에는 검색 횟수가 무제한으로 포함될 수 있습니다.

>[!INFO]
>
>**예:**
>
>**[!DNL Workfront]> [!UICONTROL 관련 레코드 읽기]**  지정한 검색 쿼리와 일치하는 레코드를 특정 상위 개체에서 읽습니다

## 트리거 모듈

지정된 서비스에서 변경된 경우 트리거가 번들을 생성합니다. 변경 사항은 새 레코드 작성, 레코드 삭제, 레코드 업데이트 등이 될 수 있습니다.

모든 트리거는 0개, 1개 이상의 번들을 반환한 다음 처리를 위해 다음 모듈에 전달할 수 있습니다.

트리거는 시나리오 시작 부분에만 배치할 수 있습니다.

각 시나리오에는 하나의 트리거만 포함할 수 있습니다.

[!DNL Workfront Fusion] 에서는 두 가지 트리거 유형을 구별합니다. 폴링 트리거 및 인스턴트 트리거입니다.

### 폴링 트리거

설문 조사는 이전 실행 이후 변경되지 않았더라도 주어진 서비스를 정기적으로 폴링합니다. 정기적으로 실행하도록 폴링 트리거가 포함된 시나리오를 예약하는 것이 좋습니다. 필요한 경우 *변경*&#x200B;를 반환하면 변경 사항에 대한 정보가 포함된 번들이 트리거에서 반환됩니다. 없는 경우 *변경*&#x200B;로 설정되면 트리거에서 번들을 출력하지 않습니다. 시나리오 예약에 대한 지침은 [에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

폴링 트리거를 사용하면 epoch 패널을 통해 출력해야 하는 첫 번째 번들을 선택할 수 있습니다. 트리거를 저장하거나 트리거 설정을 변경하면 패널이 자동으로 표시됩니다. 자세한 내용은 [트리거 모듈이 시작되는 위치 선택 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>epoch 패널에서 수행한 설정은 모듈의 첫 번째 실행에만 영향을 줍니다. 모듈이 실행되면 마지막으로 출력된 번들을 기억하고 epoch 패널을 통해 설정한 설정을 무시합니다.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 레코드 보기]** 시나리오가 마지막으로 실행된 이후 새로 추가된 파일을 반환합니다.
>
>* **[!DNL Google Sheets]> [!UICONTROL 보기 행]** 시나리오가 마지막으로 실행된 이후 사용자가 추가한 새 행 반환


### 인스턴트 트리거

인스턴트 트리거로 인해 서비스가 알림을 받을 수 있습니다 [!DNL Workfront Fusion] 정보 *변경* 즉시 작동합니다. 인스턴트 트리거가 포함된 시나리오를 예약하여 즉시 실행하는 것이 좋습니다. 자세한 내용은 [Adobe Workfront Fusion에서 시나리오 예약](../../workfront-fusion/scenarios/schedule-a-scenario.md). 참조 - [의 즉각적인 트리거(웹 후크) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) 수신 데이터 처리 방법에 대한 자세한 정보.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 이벤트 보기]** 작업 만들기와 같은 특정 유형의 이벤트가 Workfront에서 발생할 때 정보를 반환합니다.
>* **[!DNL Google Sheets]> [!UICONTROL 변경 사항 보기]** 셀이 업데이트될 때마다 정보를 반환합니다.


## 누적

누적 모듈은 여러 번들을 하나의 번들로 축적하는 모듈 유형입니다.

모든 누적 값은 한 번만 반환하고, 추가로 처리하기 위해 다음 모듈로 전달됩니다.

시나리오 중간에만 집계를 배치할 수 있습니다.

시나리오에는 무제한의 집계가 포함될 수 있습니다.

>[!INFO]
>
>**예:**
>
>* **[!UICONTROL 아카이브] > [!UICONTROL 아카이브 만들기]** 받은 파일을 zip 아카이브로 압축
>* **[!UICONTROL CSV] > [!UICONTROL CSV로 합계]** CSV 파일의 여러 문자열을 단일 행으로 병합합니다
>* **[!UICONTROL 도구] > [!UICONTROL 텍스트 누적]** 여러 문자열을 하나의 문자열로 결합합니다.


자세한 내용은 [의 누적 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 반복기

반복기는 배열을 여러 개의 개별 번들로 분할하는 모듈 유형입니다.

모든 반복기는 하나 이상의 번들을 반환한 다음 처리를 위해 다음 모듈로 전달합니다.

반복자를 시나리오 중간에만 배치할 수 있습니다.

시나리오에는 무제한의 반복자가 포함될 수 있습니다.

>[!INFO]
>
>**예:**
>
>**[!UICONTROL 이메일] > [!UICONTROL 첨부 파일 검색]** 일련의 첨부 파일을 별도의 번들로 나누기

자세한 내용은 [의 반복기 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) 및 [에 배열 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
