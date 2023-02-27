---
content-type: api
navigation-topic: general-api
title: API 예제 스크립트
description: FAPI 예 스크립트
author: Becky
feature: Workfront API
exl-id: 76c5eca6-be82-4331-9da9-9943e0bda669
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# API 예제 스크립트

## Adobe Workfront API 예

다음은 Workfront RESTful API와 상호 작용하는 데 사용되는 다양한 프로그래밍 언어의 예입니다. 각 예제는 다음 작업을 수행합니다.

* 연결 설정
* 로그인한 사용자 정보 검색
* 프로젝트 쿼리
* 프로젝트 만들기
* 프로젝트를 검색합니다
* 프로젝트 업데이트
* 프로젝트 삭제
* 로그아웃

Workfront의 Github 페이지에서 다음 예를 다운로드할 수 있습니다.  [https://github.com/Workfront](https://github.com/Workfront)

저장소에서 예를 찾으려면 를 입력합니다 `example` 로 **저장소 찾기...** 상자.

>[!NOTE]
>
>API의 모든 사용은 프로덕션 환경에서 실행하기 전에 Workfront의 베타 환경에서 테스트해야 합니다. 고객이 On-Demand 소프트웨어에 부담이 된다고 합리적으로 생각하는 프로세스에 API를 사용하는 경우(즉, 프로세스가 다른 고객에 대한 소프트웨어 성능에 실질적 부정적인 영향을 주고 있음) Workfront은 고객이 해당 프로세스를 중단하도록 요청할 수 있는 권한을 보유하며, 고객이 준수하지 않고 문제가 계속되면 Workfront은 프로세스를 종료할 수 있는 권한을 보유합니다.

>[!IMPORTANT]
>
>본 소프트웨어는 상품성, 특정 목적 적합성 및 비침해에 대한 보증을 포함하되 이에 국한되지 않으며 명시적이든 묵시적이든 어떠한 종류의 보증도 없이 &quot;있는 그대로&quot; 제공됩니다. 어떠한 경우에도 저작자 또는 저작권 보유자는 소프트웨어와 관련되었거나 무관한 또는 기타 소프트웨어 취급 중 계약, 불법 행위 또는 기타 어떠한 방법으로든 발생한 클레임, 손해 또는 기타 책임에 대해 책임을 지지 않습니다.
