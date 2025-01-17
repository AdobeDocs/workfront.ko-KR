---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 시나리오,성능
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion 성능 보호 기능
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] 성능 보호

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [Adobe Workfront Fusion 성능 가드레일](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/fusion-performance-guardrails.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion]에는 [!DNL Adobe Workfront license] 외에 [!DNL Adobe Workfront Fusion] 라이선스가 필요합니다.

작업 자동화에는 빠른 처리가 필요하므로 [!DNL Adobe Workfront Fusion]은(는) 높은 성능을 제공하도록 설계되었습니다. 오래 실행되는 시나리오에서는 작업 속도가 느려질 수 있으므로 실행 시간, 데이터 크기 및 기타 시나리오 매개 변수를 제한하는 성능 보존 가드레일을 사용하여 [!DNL Workfront Fusion]을(를) 설계했습니다. [!DNL Workfront Fusion] 디자이너는 이러한 보호 기능을 인식하고 이를 디자인 작업에 통합해야 합니다.

## 브라우저

* Workfront Fusion은 Chrome 기반 브라우저만 지원합니다.

## 시나리오

* 기본 시나리오 실행 시간 제한은 **40분**&#x200B;입니다. 실행이 이 시간 제한에 도달하면 [!DNL Workfront Fusion]은(는) 시나리오에 따라 다음 주기나 작업 후 시나리오 실행을 중단합니다. 이렇게 하면 40분 제한에 도달한 직후 시나리오가 중지됩니다
* 시나리오 블루프린트의 최대 크기는 **5MB**&#x200B;이지만 시나리오 크기를 **3MB** 미만으로 유지하는 것이 좋습니다.

  많은 수의 필드로 데이터를 생성하거나 업데이트하는 앱 모듈로 인해 매우 큰 블루프린트가 발생할 수 있습니다.

   * [!DNL Workfront] 앱을 사용하는 경우 사용 사례를 만들거나 업데이트하는 데 필요한 필드만 선택하십시오.
   * 다른 앱을 사용하는 경우 사용자 지정 API 모듈을 사용하여 필드가 많은 레코드 유형과 상호 작용합니다.

* 시나리오에는 모듈 수에 대한 제한이 없지만 모듈이 150개를 초과하는 시나리오는 [!DNL Workfront Fusion] 시스템의 성능에 부정적인 영향을 줍니다. 이러한 이유로 150개 이상의 모듈로 시나리오를 만드는 것은 권장되지 않습니다.

## 작업

* 기본 작업 시간 제한은 일반적으로 **40초**&#x200B;입니다.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 파일

* 파일에 대한 Fusion의 총 처리 용량은 **1GB**&#x200B;입니다. 제한은 총 메모리 비용을 기준으로 합니다. 모든 작업이 그 비용에 기여한다. 400MB의 단일 파일을 다운로드하여 업로드하는 경우 파일 용량에 대한 총 비용은 800MB가 됩니다.
* Workfront Ultimate 플랜을 사용하는 조직은 1GB가 넘는 향상된 파일 처리에 액세스할 수 있습니다. Fusion 플랫폼은 단일 작업(예: 업로드 파일)에 대해 최대 15GB의 개별 파일을 지원할 수 있지만 데이터 전송에 영향을 주는 다른 요인이 있습니다. 단일 작업의 파일 크기 제한은 Fusion이 연결되는 웹 서비스에 따라 다릅니다. 데이터 전송은 단일 실행에 대한 총 처리입니다. 즉, 한 번의 실행으로 여러 가지 작업이 전체 데이터 전송에 기여합니다. Fusion은 실행 제한 40분에 도달할 때까지 파일을 처리합니다.

  자세한 내용은 [Adobe Workfront Fusion에서 대용량 파일 작업](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md)을 참조하십시오.


## 서버 메모리 사용

* 단일 실행에 대한 서버 메모리 사용량이 **1GB**(으)로 제한됩니다.

  대용량 파일 또는 복잡한 모듈과 같은 많은 요인은 예측하거나 제어하기 어려운 방식으로 서버 메모리 사용에 영향을 줄 수 있습니다. 이 때문에 시나리오가 다른 모든 성능 보호 기능을 따르는 경우에도 시나리오 실행이 1GB 메모리 제한을 초과할 수 있습니다. 메모리 제한을 초과하면 실행이 실패합니다.

## 웹후크

* 페이로드의 기본 최대 크기는 **5MB**&#x200B;입니다.
* Webhooks는 **초당 요청 100개로 제한됩니다**. 이 한도에 도달하면 Workfront Fusion에서 429([!UICONTROL 요청이 너무 많음]) 상태를 보냅니다.
* [!DNL Workfront Fusion]이(가) 30일 동안 webhook 페이로드를 저장합니다. 받은 후 30일 이상 지난 후 웹후크 페이로드에 액세스하면 &quot;[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot; 오류가 발생합니다.
* 다음 중 하나가 적용되는 경우 웹후크는 자동으로 비활성화됩니다.

   * 웹후크가 5일 이상 어떤 시나리오에도 연결되지 않았습니다.
   * 웹후크는 30일 이상 비활성 상태인 비활성 시나리오에서만 사용됩니다.

* 비활성화된 웹후크는 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태인 경우 자동으로 삭제 및 등록 취소됩니다.

## 실행 기록

* 실행 기록 로그의 크기는 **100MB**&#x200B;로 제한됩니다. 실행 기록이 이 크기를 초과하면 처음 100MB만 표시됩니다.
* 시나리오에 동시 실행이 여러 개 있는 경우. 시나리오 세부 정보 페이지의 실행 영역에는 5개의 실행만 표시됩니다. 5개 이상의 실행이 진행 중인 경우에도 마찬가지입니다.

## 불완전한 실행

* 불완전한 실행은 총 크기 **500MB**(으)로 제한됩니다. 500MB 제한에 도달하면 더 이상 완료되지 않은 실행이 저장되지 않습니다.

## 재시도

* Break 모듈을 사용하고 Retry 지시문을 지정할 때 시나리오가 2분 기간 내에 10번 연속적으로 실패하면 시나리오가 자동으로 비활성화됩니다.

