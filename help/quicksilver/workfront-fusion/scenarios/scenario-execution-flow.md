---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion의 시나리오 실행 흐름
description: 이 문서에서는 시나리오가 실행되는 방식과 이를 통해 데이터가 흐르는 방식을 설명합니다. 또한 처리된 데이터에 대한 정보를 찾을 수 있는 위치와 데이터 읽기 방법에 대해서도 설명합니다.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# 의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]

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
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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

## 시나리오 실행 흐름

시나리오가 올바로 설정되고 활성화되면 정의된 일정에 따라 실행됩니다.

시나리오가 시작되면 첫 번째 모듈이 관찰하도록 설정된 이벤트에 응답합니다. 번들(데이터)을 반환하는 경우 다음 모듈로 전달하고 시나리오가 계속되어 연속된 각 모듈을 하나씩 전달합니다.

번들이 모든 모듈에서 올바르게 처리되면에서 설명한 대로 시나리오가 시나리오 세부 사항 영역에서 성공으로 표시됩니다 [의 시나리오 세부 정보 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 시나리오 설정에 대한 자세한 내용은 [의 기본 시나리오 설정 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 시나리오 활성화에 대한 자세한 내용은 [에서 시나리오 활성화 또는 비활성화 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 시나리오 예약에 대한 자세한 내용은 [시나리오 예약 위치 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 모듈에 대한 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md).

### 예: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]

>[!INFO]
>
>**예:** 에서 수신 요청을 감시하는 시나리오에서 [!DNL Workfront] 그런 다음 로 변환합니다. [!DNL Workfront] 프로젝트, 데이터는 다음과 같이 흐릅니다.
>
>첫 번째 모듈에서 수행되는 시나리오의 첫 번째 단계는 요청을 감시하는 것입니다. 들어오는 각 요청은 하나의 번들로 간주됩니다. 번들을 찾지 못한 채 모듈이 실행되면 첫 번째 모듈 이후 시나리오가 종료됩니다.
>
>첫 번째 모듈이 번들을 반환하는 경우 번들은 나머지 시나리오를 통과합니다. 이 예에서 시나리오의 나머지 부분은 요청을 프로젝트로 변환하는 두 번째 및 마지막 모듈로 구성됩니다.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 예: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용]

>[!INFO]
>
>**예:** 에서 문서를 다운로드하는 시나리오에서 [!DNL Adobe Workfront] 다음 폴더에 해당 파일을 보냅니다: [!DNL Dropbox], 데이터는 다음과 같이 이동합니다.
>
>첫 번째 모듈에서 수행되는 시나리오의 첫 번째 단계는 번들(문서)을 시청하는 것입니다. 이 예에서 모듈은 의 번들을 감시합니다. [!DNL Workfront]. 번들을 반환하지 않으면 첫 번째 모듈 이후에 시나리오가 종료됩니다.
>
>번들이 반환되면 번들은 나머지 시나리오를 통과합니다. 이 예에서 시나리오의 나머지 부분은 번들을 로 업로드하는 두 번째 및 마지막 모듈로 구성됩니다. [!DNL Dropbox] 폴더를 삭제합니다.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>첫 번째 모듈이 여러 번들을 반환하는 경우 첫 번째 번들은 로 업로드됩니다. [!DNL Dropbox] 두 번째 번들을 업로드하기 전에. 그런 다음 두 번째 번들이 업로드되고, 세 번째 번들이 업로드되는 방식입니다.

## 처리된 번들에 대한 정보

각 모듈에 대해 번들은 다음 모듈로 이동하거나 최종 목적지에 도달하기 전에 4단계 프로세스를 거칩니다. 4단계 프로세스는 초기화, 작업, 커밋/롤백 및 완료입니다. 이를 거래 처리라고 하며 데이터가 모듈에서 처리된 방식을 설명하는 데 도움이 됩니다.

시나리오 실행이 완료되면 각 모듈에 수행된 작업 수를 표시하는 아이콘이 표시됩니다. 이 아이콘을 클릭하면 위에서 설명한 형식으로 처리된 번들에 대한 세부 정보가 표시됩니다. 사용된 모듈 설정과 해당 모듈에서 반환된 번들을 확인할 수 있습니다.

![](assets/info-processed-bundles-350x396.png)

모듈이 다음과 같은 입력 정보를 수신했습니다.

* 변환된 이미지
* 이미지를 업로드할 선택한 폴더
* 원래 이름 [!DNL Facebook] 이미지

처리 후 모듈은 다음 출력 정보를 반환했습니다.

* 이미지 ID 할당자: [!DNL Dropbox]
* 다음 위치에 있는 전체 경로 [!DNL Dropbox] [!DNL Workfront Fusion] 파일을 업로드했습니다.

위의 정보는 드롭다운 상자에서 표시된 대로 각 번들에 대해 별도로 캡처됩니다 [!UICONTROL 작업 1] 및 [!UICONTROL 작업 2] 을 클릭합니다.

트랜잭션 처리에 대한 자세한 내용은 [의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 시나리오를 실행하는 동안 오류가 발생했습니다.

시나리오 실행 중에 오류가 발생할 수 있습니다. 예를 들어 [!DNL Dropbox] 모듈 설정에서 대상 폴더로 설정한 폴더는 오류 메시지와 함께 종료됩니다. 오류를 처리하는 방법에 대한 자세한 내용은 [에서 처리하는 동안 오류 발생 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
