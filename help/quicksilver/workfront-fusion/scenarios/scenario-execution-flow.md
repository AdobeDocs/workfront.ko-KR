---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion의 시나리오 실행 흐름
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 시나리오 실행 흐름

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [시나리오 실행 흐름](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-flow.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

이 문서에서는 시나리오가 실행되는 방식과 이를 통해 데이터가 흐르는 방식을 설명합니다. 또한 처리된 데이터에 대한 정보를 찾을 수 있는 위치와 데이터 읽기 방법에 대해서도 설명합니다.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
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

## 시나리오 실행 흐름

시나리오가 올바로 설정되고 활성화되면 정의된 일정에 따라 실행됩니다.

시나리오가 시작되면 첫 번째 모듈이 관찰하도록 설정된 이벤트에 응답합니다. 번들(데이터)을 반환하는 경우 다음 모듈로 전달하고 시나리오가 계속되어 연속된 각 모듈을 하나씩 전달합니다.

모든 모듈에서 번들이 올바르게 처리되면 [시나리오 세부 정보  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)에서 설명한 대로 시나리오가 시나리오 세부 정보 영역에서 성공으로 표시됩니다.

* 시나리오 설정에 대한 자세한 내용은 [시나리오 편집기  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)을(를) 참조하십시오.
* 시나리오 활성화에 대한 자세한 내용은 [시나리오 활성화 또는 비활성화 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)를 참조하십시오.
* 시나리오 예약에 대한 자세한 내용은 [다음 위치에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하십시오.
* 모듈에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)을 참조하세요.

### 예: 작업 자동화용 [!UICONTROL [!DNL Workfront Fusion]]

>[!INFO]
>
>**예:** [!DNL Workfront]에서 들어오는 요청을 감시한 다음 [!DNL Workfront] 프로젝트로 변환하는 시나리오에서는 데이터가 다음과 같이 이동합니다.
>
>첫 번째 모듈에서 수행되는 시나리오의 첫 번째 단계는 요청을 감시하는 것입니다. 들어오는 각 요청은 하나의 번들로 간주됩니다. 번들을 찾지 못한 채 모듈이 실행되면 첫 번째 모듈 이후 시나리오가 종료됩니다.
>
>첫 번째 모듈이 번들을 반환하는 경우 번들은 나머지 시나리오를 통과합니다. 이 예에서 시나리오의 나머지 부분은 요청을 프로젝트로 변환하는 두 번째 및 마지막 모듈로 구성됩니다.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 예: 작업 자동화 및 통합용 [!UICONTROL [!DNL Workfront Fusion]]

>[!INFO]
>
>**예:** [!DNL Adobe Workfront]에서 문서를 다운로드하여 [!DNL Dropbox]의 폴더로 보내는 시나리오에서는 다음과 같이 데이터가 흐릅니다.
>
>첫 번째 모듈에서 수행되는 시나리오의 첫 번째 단계는 번들(문서)을 시청하는 것입니다. 이 예에서 모듈은 [!DNL Workfront]에서 번들을 감시합니다. 번들을 반환하지 않으면 첫 번째 모듈 이후에 시나리오가 종료됩니다.
>
>번들이 반환되면 번들은 나머지 시나리오를 통과합니다. 이 예제에서 나머지 시나리오는 두 번째 모듈과 마지막 모듈로 구성되어 번들을 [!DNL Dropbox] 폴더로 업로드합니다.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>첫 번째 모듈이 여러 번들을 반환하는 경우 두 번째 번들을 업로드하기 전에 첫 번째 번들이 [!DNL Dropbox]에 업로드됩니다. 그런 다음 두 번째 번들이 업로드되고, 세 번째 번들이 업로드되는 방식입니다.

## 처리된 번들에 대한 정보

각 모듈에 대해 번들은 다음 모듈로 이동하거나 최종 목적지에 도달하기 전에 4단계 프로세스를 거칩니다. 4단계 프로세스는 초기화, 작업, 커밋/롤백 및 완료입니다. 이를 거래 처리라고 하며 데이터가 모듈에서 처리된 방식을 설명하는 데 도움이 됩니다.

시나리오 실행이 완료되면 각 모듈에 수행된 작업 수를 표시하는 아이콘이 표시됩니다. 이 아이콘을 클릭하면 위에서 설명한 형식으로 처리된 번들에 대한 세부 정보가 표시됩니다. 사용된 모듈 설정과 해당 모듈에서 반환된 번들을 확인할 수 있습니다.

![](assets/info-processed-bundles-350x396.png)

모듈이 다음과 같은 입력 정보를 수신했습니다.

* 변환된 이미지
* 이미지를 업로드할 선택한 폴더
* [!DNL Facebook] 이미지의 원래 이름

처리 후 모듈은 다음 출력 정보를 반환했습니다.

* [!DNL Dropbox]이(가) 할당한 이미지 ID
* [!DNL Dropbox] [!DNL Workfront Fusion]에서 파일을 업로드한 전체 경로

위의 정보는 이미지의 드롭다운 상자 [!UICONTROL 작업 1] 및 [!UICONTROL 작업 2]에 표시된 대로 각 번들에 대해 별도로 캡처됩니다.

트랜잭션 처리에 대한 자세한 내용은 [시나리오 실행, 주기 및 단계  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)을(를) 참조하십시오.

## 시나리오를 실행하는 동안 오류가 발생했습니다.

시나리오 실행 중에 오류가 발생할 수 있습니다. 예를 들어 모듈 설정에서 대상 폴더로 설정한 [!DNL Dropbox] 폴더를 삭제하면 시나리오가 오류 메시지와 함께 종료됩니다. 오류를 처리하는 방법에 대한 자세한 내용은 [오류 처리 위치 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)를 참조하십시오.
