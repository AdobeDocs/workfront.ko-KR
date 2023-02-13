---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion의 시나리오 실행 흐름
description: 이 문서에서는 시나리오의 실행 방법과 데이터를 통해 이동하는 방법을 설명합니다. 또한 처리된 데이터에 대한 정보를 찾을 수 있는 위치와 그 정보를 읽는 방법을 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]

이 문서에서는 시나리오의 실행 방법과 데이터를 통해 이동하는 방법을 설명합니다. 또한 처리된 데이터에 대한 정보를 찾을 수 있는 위치와 그 정보를 읽는 방법을 설명합니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오 실행 흐름

시나리오가 올바로 설정되고 활성화되면 정의된 일정에 따라 실행됩니다.

시나리오가 시작되면, 첫 번째 모듈이 감시하도록 설정된 이벤트에 응답합니다. 번들(데이터)을 반환하면 이 번들은 다음 모듈에 전달되고 시나리오가 계속 진행되어 연속되는 각 모듈을 하나씩 전달합니다.

번들 프로세스가 모든 모듈에서 올바르게 처리되면 시나리오는 에 설명된 대로 시나리오 세부 영역에서 성공으로 표시됩니다. [의 시나리오 세부 사항 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 시나리오 설정에 대한 자세한 내용은 [의 기본 시나리오 설정 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 시나리오 활성화에 대한 자세한 내용은 [에서 시나리오 활성화 또는 비활성화 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 시나리오 예약에 대한 자세한 내용은 [에서 시나리오 예약 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 모듈에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md).

### 예: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]

>[!INFO]
>
>**예:** 에서 들어오는 요청을 감시하는 시나리오에서 [!DNL Workfront] 그런 다음 [!DNL Workfront] 프로젝트, 데이터는 다음과 같이 흐릅니다.
>
>첫 번째 모듈에서 수행하는 시나리오의 첫 번째 단계는 요청을 감시하는 것입니다. 들어오는 각 요청은 하나의 번들로 간주됩니다. 모듈이 번들을 찾지 않고 실행되는 경우 시나리오는 첫 번째 모듈 후에 종료됩니다.
>
>첫 번째 모듈이 번들을 반환하는 경우 번들이 시나리오의 나머지 부분을 통과합니다. 이 예에서 나머지 시나리오는 요청을 프로젝트로 변환하는 두 번째 모듈과 마지막 모듈로 구성됩니다.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 예: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한]

>[!INFO]
>
>**예:** 시나리오에서 [!DNL Adobe Workfront] 그리고 를 의 폴더로 보냅니다. [!DNL Dropbox], 데이터는 다음과 같이 흐릅니다.
>
>첫 번째 모듈에서 수행한 시나리오의 첫 번째 단계는 번들(문서)을 확인하는 것입니다. 이 예에서 모듈은 의 번들을 관찰합니다 [!DNL Workfront]. 번들을 반환하지 않으면 시나리오는 첫 번째 모듈 후에 종료됩니다.
>
>번들이 반환되면 번들이 시나리오의 나머지 부분을 전달합니다. 이 예에서 나머지 시나리오는 번들을 로 업로드하는 두 번째 모듈과 마지막 모듈로 구성됩니다 [!DNL Dropbox] 폴더를 입력합니다.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>첫 번째 모듈에서 여러 번들을 반환하면 첫 번째 번들이 업로드됩니다 [!DNL Dropbox] 두 번째 번들을 업로드하기 전에. 그런 다음 두 번째 번들이 업로드되고, 그 다음 세 번째 번들이 업로드됩니다.

## 처리된 번들에 대한 정보

각 모듈의 경우 번들은 다음 모듈로 이동하거나 최종 대상에 도달하기 전에 4단계 프로세스를 거칩니다. 4단계 프로세스는 초기화, 작업, 커밋/롤백 및 완료입니다. 이를 트랜잭션 처리라고 하며, 모듈에서 데이터가 처리되는 방식을 설명하는 데 도움이 됩니다.

시나리오 실행이 완료되면 각 모듈에 수행된 작업 수를 보여주는 아이콘이 표시됩니다. 이 아이콘을 클릭하여 처리된 번들에 대한 세부 정보를 위에 설명된 형식으로 표시할 수 있습니다. 사용된 모듈 설정과 어느 모듈에서 반환한 번들을 확인할 수 있습니다.

![](assets/info-processed-bundles-350x396.png)

모듈이 다음과 같은 입력 정보를 받았습니다.

* 변환된 이미지
* 이미지를 업로드할 폴더 선택
* 의 원래 이름 [!DNL Facebook] 이미지

처리 후 모듈이 다음 출력 정보를 반환했습니다.

* 에 의해 지정된 이미지 ID [!DNL Dropbox]
* 인 전체 경로 [!DNL Dropbox] [!DNL Workfront Fusion] 파일을 업로드했습니다.

위의 정보는 드롭다운 상자에 표시된 대로 각 번들에 대해 별도로 캡처됩니다 [!UICONTROL 작업 1] 및 [!UICONTROL 작업 2] 아래에 표시됩니다.

트랜잭션 처리에 대한 자세한 내용은 [시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 시나리오를 실행하는 동안 오류가 발생했습니다.

시나리오 실행 중에 오류가 발생할 수 있습니다. 예를 들어 [!DNL Dropbox] 모듈 설정에서 대상 폴더로 설정한 폴더는 오류 메시지와 함께 종료됩니다. 오류를 처리하는 방법에 대한 자세한 내용은 [에서 처리 중 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
