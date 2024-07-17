---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: AI를 사용하여 모듈 생성
description: 텍스트 프롬프트를 입력하여 프롬프트에 구성된 HTTP 모듈을 만들 수 있습니다.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# AI를 사용하여 모듈 생성

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>이 기능은 아직 개발 초기 단계이므로 내부 Workfront 사용자만 사용할 수 있습니다.

AI를 사용하여 필요한 모듈을 설명하는 텍스트 프롬프트를 입력할 수 있습니다. 그런 다음 Fusion은 원하는 API의 올바른 끝점에 연결하는 HTTP 모듈을 생성합니다.

AI에서 생성된 모든 것과 마찬가지로 생성된 모듈을 두 번 확인하고 테스트하여 의도한 대로 작동하는지 확인하는 것이 좋습니다.

## 현재 지원되는 AI 모듈 애플리케이션

Fusion AI는 현재 다음 애플리케이션에 연결하는 모듈을 생성할 수 있습니다.

* Adobe Firefly
* Azure OpenAI
* Microsoft 그래프
* Adobe 마에스트로
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

1. 모듈을 추가하고 응용 프로그램 목록에서 **AI로 생성**&#x200B;을 선택합니다.

   또는

   시나리오 편집기의 빈 영역을 마우스 오른쪽 단추로 클릭한 다음 **AI로 생성**&#x200B;을 선택합니다.
1. 상자에 텍스트 프롬프트를 입력합니다.

   프롬프트에 대한 팁은 이 문서에서 [텍스트 프롬프트 작성 팁](#tips-for-creating-text-prompts)을 참조하십시오.
1. 애플리케이션에 대한 API 토큰을 모듈에 추가합니다.
1. 모듈을 확인하여 적절한 애플리케이션 및 작업에 맞게 구성된 것처럼 보이는지 확인합니다.
1. (조건부) 모듈이 시나리오에 첨부되지 않은 경우 해당 모듈로 드래그합니다.

생성된 모듈이 의도한 대로 작동하는지 확인하려면 모듈을 테스트하는 것이 좋습니다.

## 텍스트 프롬프트 작성 팁

텍스트 프롬프트에 최소한 다음 정보가 포함되어야 합니다.

* 연결 중인 응용 프로그램
* 수행할 작업입니다

>[!INFO]
>
>**예**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   여기에는 `Google Calendar` 응용 프로그램과 `Retrieve a list of my calendars` 작업이 포함됩니다.
>
>* `Retrieve popular songs from Spotify`
>
>   여기에는 `Spotify` 응용 프로그램과 `Retrieve popular songs` 작업이 포함됩니다.

텍스트 프롬프트를 생성할 때 다음 사항을 고려하십시오.

* 각 Fusion 모듈은 단일 작업을 수행하기 때문에 텍스트 프롬프트는 하나의 특정 작업을 설명해야 합니다.
* 직접적이고 간단한 언어를 사용하십시오.
* 모듈을 확인하고 테스트합니다. 예상대로 수행되지 않으면 프롬프트를 세분화하고 다시 시도하십시오.
