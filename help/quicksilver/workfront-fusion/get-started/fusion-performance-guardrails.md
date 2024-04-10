---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 시나리오,성능
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion 성능 보호 기능
description: Adobe Workfront Fusion에는 Adobe Workfront 라이센스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 00ef33666bebe434739056cb38c3dff24285d682
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] 성능 보호

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 을(를) 필요로 합니다. [!DNL Adobe Workfront Fusion] 에 더해진 라이센스 [!DNL Adobe Workfront license].

작업 자동화는 신속한 처리가 필요하므로 [!DNL Adobe Workfront Fusion] 높은 성능을 제공하도록 설계되었습니다. 오래 실행되는 시나리오는 작업의 속도를 저하시킬 수 있으므로 [!DNL Workfront Fusion] 실행 시간, 데이터 크기 및 기타 시나리오 매개 변수를 제한하는 성능 보존 가드레일 사용. [!DNL Workfront Fusion] 디자이너는 이러한 가드레일을 인식하고 이를 디자인 사례에 통합해야 합니다.

## 브라우저

Workfront Fusion은 Chrome 기반 브라우저만 지원합니다.

## 시나리오

* 기본 시나리오 실행 시간 제한: **40분**. 실행이 이 시간 초과에 도달하면, [!DNL Workfront Fusion] 시나리오에 따라 다음 주기 또는 작업 후 시나리오 실행을 중단합니다. 이렇게 하면 40분 제한에 도달한 직후 시나리오가 중지됩니다
* 시나리오 블루프린트의 최대 크기는 다음과 같습니다. **5MB**, 하지만 시나리오 크기를 다음 범위 아래로 유지하는 것이 좋습니다. **3MB**.

  많은 수의 필드로 데이터를 생성하거나 업데이트하는 앱 모듈로 인해 매우 큰 블루프린트가 발생할 수 있습니다.

   * 사용 시 [!DNL Workfront] 앱에서 사용 사례를 만들거나 업데이트하는 데 필요한 필드만 선택하십시오.
   * 다른 앱을 사용하는 경우 사용자 지정 API 모듈을 사용하여 필드가 많은 레코드 유형과 상호 작용합니다.

* 시나리오에는 모듈 수에 대한 제한이 없지만 모듈이 150개를 초과하는 시나리오는 의 성능에 부정적인 영향을 줍니다. [!DNL Workfront Fusion] 시스템. 이러한 이유로 150개 이상의 모듈로 시나리오를 만드는 것은 권장되지 않습니다.

## 작업

* 기본 작업 시간 제한은 일반적으로 입니다. **40초**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 파일

* 파일에 대한 Fusion의 총 처리 용량은 다음과 같습니다. **1GB**. 제한은 총 메모리 비용을 기준으로 합니다. 모든 작업이 그 비용에 기여한다. 400MB의 단일 파일을 다운로드하여 업로드하는 경우 파일 용량에 대한 총 비용은 800MB가 됩니다.

## 서버 메모리 사용

* 단일 실행에 대한 서버 메모리 사용량은 다음으로 제한됩니다. **1GB**.

  대용량 파일 또는 복잡한 모듈과 같은 많은 요인은 예측하거나 제어하기 어려운 방식으로 서버 메모리 사용에 영향을 줄 수 있습니다. 이 때문에 시나리오가 다른 모든 성능 보호 기능을 따르는 경우에도 시나리오 실행이 1GB 메모리 제한을 초과할 수 있습니다. 메모리 제한을 초과하면 실행이 실패합니다.

## 웹후크

* 페이로드의 기본 최대 크기는 입니다. **5MB**.
* 웹후크는 다음으로 제한됩니다. **초당 요청 100개**. 이 한도에 도달하면 Workfront Fusion에서 429([!UICONTROL 요청이 너무 많음]) 상태.
* [!DNL Workfront Fusion] 30일 동안 webhook 페이로드를 저장합니다. 받은 후 30일 이상 지난 후 Webhook 페이로드에 액세스하면 오류가 발생합니다.&quot;[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot;
* 다음 중 하나가 적용되는 경우 웹후크는 자동으로 비활성화됩니다.

   * 웹후크가 5일 이상 어떤 시나리오에도 연결되지 않았습니다.
   * 웹후크는 30일 이상 비활성 상태인 비활성 시나리오에서만 사용됩니다.

* 비활성화된 웹후크는 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태인 경우 자동으로 삭제 및 등록 취소됩니다.

## 실행 기록

* 실행 기록 로그의 크기는 다음과 같이 제한됩니다. **100MB**. 실행 기록이 이 크기를 초과하면 처음 100MB만 표시됩니다.

## 재시도

Break 모듈을 사용하고 Retry 지시문을 지정할 때 시나리오가 2분 기간 내에 10번 연속적으로 실패하면 시나리오가 자동으로 비활성화됩니다.

