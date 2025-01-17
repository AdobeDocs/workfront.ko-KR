---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 모듈 유형
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 모듈 유형

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [모듈 개요](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!UICONTROL Adobe Workfront Fusion]은 작업 모듈, 검색 모듈, 트리거 모듈, 집계 및 반복기의 5가지 모듈 유형을 구분합니다. 집계기 및 반복기는 고급 시나리오용입니다.

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
   <td>이 문서에 설명된 기능을 사용하려면 조직에서 Adobe Workfront Fusion과 Adobe Workfront을 구매해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 작업 모듈

작업 모듈은 가장 일반적인 모듈 유형입니다. 일반적인 작업 모듈은 단일 번들을 반환한 다음 처리를 위해 다음 모듈로 전달합니다.

트리거 모듈과 달리 작업 모듈은 시나리오의 시작, 중간 또는 끝에 배치할 수 있습니다. 시나리오에는 작업 모듈을 무제한으로 포함할 수 있습니다.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 파일 업로드]**&#x200B;가 [!DNL Workfront]에 파일을 보내고 해당 식별자를 반환합니다.
>* **[!UICONTROL 이미지] > [!UICONTROL 크기 조정]**&#x200B;은(는) 이미지를 받고 지정된 치수로 크기를 조정한 다음 크기 조정된 이미지를 다음 작업에 전달합니다.

작업 유형에는 만들기, 읽기, 업데이트 및 삭제의 네 가지 하위 유형이 있습니다. 업데이트 하위 유형을 사용하면 다음 세 가지 작업을 수행할 수 있습니다.

* **필드의 내용을 지웁니다**. 이 작업은 필드의 내용이 키워드를 지우는 것으로 평가될 때 수행됩니다(*empty*&#x200B;과 혼동하지 않도록 함).

  ![](assets/erase-content-of-field.png)

* **필드의 내용을 변경하지 않고 둡니다**. 이 작업은 필드가 비어 있거나 필드의 내용이 비어 있는 것으로 평가될 때(JSON에서 null을 통해 표시됨) 발생합니다.

  ![](assets/leave-content-field-unchanged-350x231.png)

* **필드의 내용을 바꿉니다**. 이 작업은 상술한 두 가지 경우 이외의 모든 경우에 발생합니다.

>[!NOTE]
>
>* 매핑 패널에 `erase` 키워드가 표시되지 않으면 모듈이 업데이트 모듈이 아니거나 앱에 대한 최신 사양으로 업데이트되지 않은 것입니다.
>* &quot;[!UICONTROL Empty]&quot;은(는) 필드 콘텐츠를 변경하지 않습니다. 필드를 지워야 하는 경우 다음 공식을 사용할 수 있습니다.
>
>![](assets/formula-ifempty-name-erase.png)
>
>현재 필드의 내용이 비어 있는 것으로 평가될 때 필드를 변경하지 않고 그대로 둘 수 없습니다.

## 모듈 검색

일반 검색은 0개, 1개 또는 그 이상의 번들을 반환한 다음 처리를 위해 다음 모듈로 전달합니다.

시나리오의 시작, 중간 또는 끝에 검색을 배치할 수 있습니다.

시나리오에는 검색을 무제한으로 포함할 수 있습니다.

>[!INFO]
>
>**예:**
>
>**[!DNL Workfront]> [!UICONTROL 관련 레코드 읽기]**&#x200B;는 지정한 검색 쿼리와 일치하는 레코드를 읽습니다(특정 상위 개체).

## 트리거 모듈

트리거는 지정된 서비스가 변경되면 번들을 생성합니다. 새 레코드 만들기, 레코드 삭제, 레코드 업데이트 등이 변경 내용이 될 수 있습니다.

모든 트리거는 0개, 1개 또는 그 이상의 번들을 반환한 다음 처리를 위해 다음 모듈로 전달될 수 있습니다.

트리거는 시나리오의 시작 위치에만 배치할 수 있습니다.

각 시나리오에는 하나의 트리거만 포함될 수 있습니다.

[!DNL Workfront Fusion]은(는) 두 가지 유형의 트리거인 폴링 트리거와 인스턴트 트리거를 구별합니다.

### 폴링 트리거

폴링은 이전 실행 이후 변경 사항이 없더라도 주어진 서비스를 정기적으로 폴링합니다. 폴링 트리거가 포함된 시나리오를 정기적으로 실행하도록 예약하는 것이 좋습니다. *변경*&#x200B;이 있는 경우 트리거는 변경에 대한 정보가 포함된 번들을 반환합니다. *변경*&#x200B;이 없으면 트리거에서 번들을 출력하지 않습니다. 시나리오를 예약하는 방법에 대한 지침은 [다음 위치에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하십시오.

폴링 트리거를 사용하면 Epoch 패널을 통해 출력할 첫 번째 번들을 선택할 수 있습니다. 트리거를 저장하거나 트리거 설정을 변경하면 패널이 자동으로 표시됩니다. 자세한 내용은 [트리거 모듈이 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md)에서 시작되는 위치 선택을 참조하십시오.

>[!NOTE]
>
>에포크 패널에서 수행한 설정은 모듈의 첫 번째 실행에만 영향을 줍니다. 모듈이 실행되면 마지막으로 출력된 번들을 기억하고 Epoch 패널을 통해 설정된 설정을 무효화합니다.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 레코드 보기]**&#x200B;에서 시나리오가 마지막으로 실행된 이후 새로 추가된 파일을 반환합니다.
>
>* **[!DNL Google Sheets]> [!UICONTROL 행 보기]**&#x200B;는 시나리오가 마지막으로 실행된 이후 사용자가 추가한 새 행을 반환합니다.

### 인스턴트 트리거

인스턴트 트리거를 사용하면 서비스에서 [!DNL Workfront Fusion]변경&#x200B;*에 대해 즉시 알릴 수 있습니다.* 즉시 트리거가 포함된 시나리오를 즉시 실행하도록 예약하는 것이 좋습니다. 지침은 [Adobe Workfront Fusion에서 시나리오 예약](../../workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하십시오. 들어오는 데이터를 처리하는 방법에 대한 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)의 [인스턴트 트리거(웹후크)도 참조하십시오.

>[!INFO]
>
>**예:**
>
>* **[!DNL Workfront]> [!UICONTROL 이벤트 보기]**&#x200B;는 작업 만들기와 같은 특정 유형의 이벤트가 Workfront에서 발생할 때 정보를 반환합니다.
>* **[!DNL Google Sheets]> [!UICONTROL 변경 내용 보기]**&#x200B;는 셀이 업데이트될 때마다 정보를 반환합니다.

## 집계자

취합기는 여러 번들을 하나의 단일 번들로 누적하는 모듈 유형입니다.

모든 집계는 하나의 번들만 반환하며, 그런 다음 추가적인 처리를 위해 다음 모듈로 전달됩니다.

집계자는 시나리오 중간에만 배치할 수 있습니다.

시나리오에는 무제한의 집계자가 포함될 수 있습니다.

>[!INFO]
>
>**예:**
>
>* **[!UICONTROL 보관] > [!UICONTROL 보관 만들기]** 받은 파일을 zip 보관 파일로 압축합니다.
>* **[!UICONTROL CSV] > [!UICONTROL CSV로 집계]**&#x200B;이(가) CSV 파일의 여러 문자열을 단일 행으로 병합합니다
>* **[!UICONTROL 도구] > [!UICONTROL 텍스트 집계]**&#x200B;는 여러 문자열을 하나의 문자열로 결합합니다

자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)의 [집계 모듈을 참조하십시오.

## 반복기

반복자는 배열을 여러 개의 개별 번들로 분할하는 모듈 유형입니다.

모든 반복기는 하나 이상의 번들을 반환한 다음, 처리를 위해 다음 모듈로 전달합니다.

반복기는 시나리오 중간에만 배치할 수 있습니다.

시나리오에는 반복기를 무제한으로 포함할 수 있습니다.

>[!INFO]
>
>**예:**
>
>**[!UICONTROL 전자 메일] > [!UICONTROL 첨부 파일 검색]**&#x200B;은(는) 첨부 파일 배열을 개별 번들로 나눕니다

자세한 내용은 [반복자 모듈 in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) 및 [배열 매핑 in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md)을 참조하십시오.
