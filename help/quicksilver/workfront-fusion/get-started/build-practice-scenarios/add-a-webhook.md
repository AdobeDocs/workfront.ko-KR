---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 기본 시나리오에 웹후크 추가
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 기본 시나리오에 웹후크 추가

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [기본 시나리오에 웹후크 추가](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

즉각적인 트리거라고도 하는 웹후크는 주어진 일정이 아닌 변경이 있을 때마다 시나리오를 시작할 수 있는 특정 종류의 트리거 모듈입니다.

이 예에서는 요청이 특정 대기열에 제출되는 즉시 시나리오를 시작하기 위해 웹후크를 추가합니다. 그런 다음 시나리오에서는 해당 요청을 프로젝트로 전환합니다.

이 예제에서는 [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)에서 만든 시나리오를 수정합니다.

## 전제 조건

이 절차를 수행하기 전에 [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)에 설명된 시나리오를 만들어야 합니다.

## Webhook 추가 및 구성

1. Convert 개체 모듈을 엽니다.
1. Issue ID 필드에서 검정색 ID 블록을 삭제합니다. 블록이 매핑된 모듈을 더 이상 사용할 수 없으므로 블록은 검정색입니다.
1. 첫 번째 모듈(이벤트 보기) 아래에서 ID 블록을 선택하여 두 번째 모듈에 매핑합니다.
1. **확인**&#x200B;을 클릭합니다.

### Webhook 모듈 추가

1. 시나리오 편집기에서 시나리오를 엽니다.
1. 첫 번째 모듈을 마우스 오른쪽 단추로 클릭하고 **모듈 삭제**&#x200B;를 선택합니다.

   모듈이 삭제되고 빈 자리 표시자가 남습니다.

1. 빈 모듈을 클릭하고 앱 목록에서 **Adobe Workfront**&#x200B;을(를) 선택합니다.
1. **이벤트 보기**&#x200B;를 선택합니다.
1. Webhook 필드 옆에 있는 **추가**&#x200B;를 클릭합니다.
1. 레코드 유형 필드에서 **문제**&#x200B;를 선택하면 모듈이 문제 변경을 트리거합니다.
1. 상태 필드에서 **새 상태**&#x200B;를 선택합니다. 이 예제에서는 다루지 않는 필터에 사용되는 필수 필드입니다.
1. 레코드 원본 필드에서 **새 레코드만**&#x200B;을(를) 선택합니다. 이렇게 하면 문제가 업데이트 또는 삭제될 때가 아니라 추가될 때 시나리오가 트리거될 수 있습니다.
1. 모듈 구성을 저장하려면 **저장**&#x200B;을 클릭하세요.
