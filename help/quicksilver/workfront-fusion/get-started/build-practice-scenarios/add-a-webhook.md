---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 기본 시나리오에 웹후크 추가
description: 즉각적인 트리거라고도 하는 웹후크는 주어진 일정이 아닌 변경이 있을 때마다 시나리오를 시작할 수 있는 특정 종류의 트리거 모듈입니다.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 의 기본 시나리오에 웹후크 추가 [!DNL Adobe Workfront Fusion]

즉각적인 트리거라고도 하는 웹후크는 주어진 일정이 아닌 변경이 있을 때마다 시나리오를 시작할 수 있는 특정 종류의 트리거 모듈입니다.

이 예에서는 요청이 특정 대기열에 제출되는 즉시 시나리오를 시작하기 위해 웹후크를 추가합니다. 그런 다음 시나리오에서는 해당 요청을 프로젝트로 전환합니다.

이 예는에서 생성된 시나리오를 수정합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 전제 조건

에 설명된 시나리오를 만들어야 합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 이 절차를 수행하기 전에.

## Webhook 추가 및 구성

1. Convert 개체 모듈을 엽니다.
1. Issue ID 필드에서 검정색 ID 블록을 삭제합니다. 블록이 매핑된 모듈을 더 이상 사용할 수 없으므로 블록은 검정색입니다.
1. 첫 번째 모듈(이벤트 보기) 아래에서 ID 블록을 선택하여 두 번째 모듈에 매핑합니다.
1. 클릭 **확인**.

### Webhook 모듈 추가

1. 시나리오 편집기에서 시나리오를 엽니다.
1. 첫 번째 모듈을 마우스 오른쪽 단추로 클릭하고 를 선택합니다. **모듈 삭제**.

   모듈이 삭제되고 빈 자리 표시자가 남습니다.

1. 빈 모듈을 클릭하고 다음을 선택합니다. **Adobe Workfront** 을 클릭합니다.
1. 선택 **이벤트 보기**.
1. 클릭 **추가** webhook 필드 옆에 있습니다.
1. 레코드 유형 필드에서 다음을 선택합니다. **문제**&#x200B;이 경우 모듈이 문제 변경을 트리거합니다.
1. 상태 필드에서 을(를) 선택합니다. **새 상태**. 이 예제에서는 다루지 않는 필터에 사용되는 필수 필드입니다.
1. 기록 원본 필드에서 을 선택합니다. **새 레코드만**. 이렇게 하면 문제가 업데이트 또는 삭제될 때가 아니라 추가될 때 시나리오가 트리거될 수 있습니다.
1. 클릭 **저장** 모듈 구성을 저장합니다.


