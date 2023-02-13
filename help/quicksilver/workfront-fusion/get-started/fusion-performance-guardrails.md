---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 시나리오,성능
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion 성능 보호 기능
description: Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 성능 보호 기능

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 를 사용하려면 [!DNL Adobe Workfront Fusion] 라이센스 [!DNL Adobe Workfront license].

작업 자동화는 빠른 처리가 필요하므로 [!DNL Adobe Workfront Fusion] 고성능을 위해 설계되었습니다. 장시간 실행되는 시나리오는 작업 속도를 저하시킬 수 있으므로 Adobe는 이미 설계했습니다 [!DNL Workfront Fusion] 실행 시간, 데이터 크기 및 기타 시나리오 매개 변수를 제한하는 성능 유지 보호 기능을 사용할 수 있습니다. [!DNL Workfront Fusion] 디자이너는 이러한 가드 레일을 알고 디자인 행위에 통합할 수 있어야 합니다.

## 시나리오

* 기본 시나리오 실행 시간 제한은 다음과 같습니다 **40분**. 실행이 이 시간 초과에 도달하면, [!DNL Workfront Fusion] 시나리오에 따라 다음 주기 또는 작업 후 시나리오 실행을 중단합니다. 따라서 40분 제한에 도달한 직후 시나리오가 중단됩니다
* 시나리오 블루프린트의 최대 크기는 다음과 같습니다 **5MB**&#x200B;그러나 시나리오 크기를 다음 미만으로 유지하는 것이 좋습니다 **3MB**.

   필드가 많은 데이터를 만들거나 업데이트하는 앱 모듈은 매우 큰 청사진을 일으킬 수 있습니다.

   * 를 사용할 때 [!DNL Workfront] 앱은 만들기 또는 업데이트 사용 사례에 필요한 필드만 선택해야 합니다.
   * 다른 앱을 사용할 때 사용자 지정 API 모듈을 사용하여 필드가 많은 레코드 유형과 상호 작용합니다.

* 시나리오에 모듈 수에 대한 제한이 없지만 150개 이상의 모듈이 있는 시나리오는 성능에 부정적인 영향을 줍니다 [!DNL Workfront Fusion] 시스템. 따라서 150개 이상의 모듈이 있는 시나리오를 만들지 않는 것이 좋습니다.

## 작업

* 기본 작업 시간 제한은 일반적으로 **40초**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 파일

* Fusion의 파일 총 처리 용량은 **1GB**. 이 제한은 총 메모리 비용을 기준으로 합니다. 모든 작업이 그 비용에 기여합니다. 400MB의 단일 파일을 다운로드하여 업로드하면 파일 용량의 총 비용은 800MB가 됩니다.

## 서버 메모리 사용

* 단일 실행에 대한 서버 메모리 사용량은 다음으로 제한됩니다 **1GB**.

   대용량 파일 또는 복잡한 모듈과 같은 많은 요소는 예측하거나 제어하기 어려운 방식으로 서버 메모리 사용에 영향을 줄 수 있습니다. 따라서 시나리오가 다른 모든 성능 보호 기능을 수행하는 경우에도 시나리오 실행이 1GB 메모리 제한을 초과할 수 있습니다. 메모리 제한을 초과하면 실행이 실패합니다.

## Webhooks

* 페이로드의 기본 최대 크기는 다음과 같습니다 **5MB**.
* 웹 후크는 다음으로 제한됩니다 **초당 100개 요청**. 이 한도에 도달하면 Workfront Fusion에서 429([!UICONTROL 너무 많은 요청]) 상태.
* [!DNL Workfront Fusion] 는 30일 동안 웹 후크 페이로드를 저장합니다. 웹 후크 페이로드에 수신한 후 30일 이상 액세스하면 &quot; 오류가 발생합니다.[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot;
* 다음 중 하나가 적용되는 경우 웹 후크는 자동으로 비활성화됩니다.

   * 웹 후크가 5일 이상 시나리오에 연결되지 않았습니다
   * 웹 후크는 30일 이상 비활성 시나리오에서만 사용됩니다.

* 비활성화된 웹 후크는 모든 시나리오에 연결되어 있지 않고 30일 이상 비활성화된 상태에 있는 경우 자동으로 삭제되고 등록되지 않습니다.
