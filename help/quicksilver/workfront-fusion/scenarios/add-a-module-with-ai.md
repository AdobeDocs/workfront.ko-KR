---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: AI를 사용하여 시나리오 세그먼트 생성
description: 텍스트 프롬프트를 입력하여 프롬프트에 구성된 HTTP 모듈을 만들 수 있습니다.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 7013c8a88f047c5c8e769a4d7b71f2033c767b4a
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# AI를 사용하여 시나리오 세그먼트 생성

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>이 기능은 Beta에 있으므로 일부 Workfront 사용자만 사용할 수 있습니다.

AI를 사용하여 시나리오의 수행해야 할 작업을 설명하는 텍스트 프롬프트를 입력할 수 있습니다. 그런 다음 Fusion은 해당 작업을 수행하는 모듈을 생성하며, 이 모듈은 시나리오에서 사용할 수 있습니다.

AI에서 생성된 모든 것과 마찬가지로 생성된 모듈을 두 번 확인하고 테스트하여 의도한 대로 작동하는지 확인하는 것이 좋습니다.

## 현재 지원되는 AI 모듈 애플리케이션

Fusion AI는 현재 다음 애플리케이션에 연결하는 모듈을 생성할 수 있습니다.

* Adobe Firefly
* Azure OpenAI
* Microsoft 그래프
* Adobe Workfront 계획
* Adobe Analytics
* Adobe PDF 서비스
* Marketo Adobe
* Adobe Frame.io
* Dropbox
* NetSuite
* Google 캘린더
* 아틀라시안 지라
* GitLab
* 스포티파이
* Bitbucket
* 오픈에이아이
* Slack

## 모듈 생성

1. 모듈 추가를 시작하고 응용 프로그램 목록에서 **AI로 생성**&#x200B;을 선택합니다.

   또는

   시나리오 편집기 페이지 하단 근처에 있는 AI로 생성 아이콘 ![AI로 생성](assets/generate-with-ai-icon-beta.png)을 클릭합니다.

   해당 AI 지원 패널이 열립니다.
1. 상자에 텍스트 프롬프트를 입력합니다.

   프롬프트에 대한 팁은 이 문서에서 [텍스트 프롬프트 작성 팁](#tips-for-creating-text-prompts)을 참조하십시오.

   모듈 또는 모듈 세트가 생성됩니다.
1. (조건부) 필요한 경우 애플리케이션에 대한 API 토큰을 모듈에 추가합니다.
1. 모듈을 확인하여 적절한 애플리케이션 및 작업에 맞게 구성되었는지 확인합니다.
1. (조건부) 생성된 시나리오 섹션이 시나리오에 첨부되지 않은 경우 시나리오에 적절히 드래그합니다.

모듈을 테스트하여 의도한 대로 작동하는지 확인하는 것이 좋습니다.

## 텍스트 프롬프트 작성 팁

텍스트 프롬프트에 최소한 다음 정보가 포함되어야 합니다.

* 연결 중인 응용 프로그램
* 수행할 작업

>[!IMPORTANT]
>
>한 번에 두 개 이상의 모듈을 생성할 수 있지만 한 번에 한 애플리케이션에 대한 모듈만 생성할 수 있습니다.

>[!INFO]
>
>**예**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>여기에는 `Workfront Planning` 응용 프로그램과 `delete records` 작업이 포함됩니다. 이 프롬프트는 삭제할 각 레코드에 대해 하나씩, 세 개의 모듈을 만듭니다.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>여기에는 `Workfront Planning` 응용 프로그램과 `change campaign summary` 작업이 포함됩니다.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>여기에는 `Workfront Planning` 응용 프로그램과 `get field details` 작업이 포함됩니다.
>
>다음 예는 올바르지 않습니다.
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    이 예제는 두 개 이상의 애플리케이션을 포함하므로 올바르지 않습니다

텍스트 프롬프트를 생성할 때 다음 사항을 고려하십시오.

* 직접적이고 간단한 언어를 사용하십시오.
* 모듈을 확인하고 테스트합니다. 예상대로 수행되지 않으면 프롬프트를 세분화하고 다시 시도하십시오.
