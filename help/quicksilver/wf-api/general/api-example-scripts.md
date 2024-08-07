---
content-type: api
navigation-topic: general-api
title: API 예제 스크립트
description: FAPI 예제 스크립트
author: Becky
feature: Workfront API
role: Developer
exl-id: 76c5eca6-be82-4331-9da9-9943e0bda669
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---


# API 예제 스크립트

## Adobe Workfront API 예

다음은 Workfront RESTful API와 상호 작용하는 데 사용되는 다양한 프로그래밍 언어의 예입니다. 각 예제는 다음 작업을 수행합니다.

* 연결 설정
* 로그인한 사용자 정보 검색
* 쿼리 프로젝트
* 프로젝트를 만듭니다.
* 프로젝트를 검색합니다.
* 프로젝트 업데이트
* 프로젝트를 삭제합니다.
* 로그아웃

Workfront의 Github 페이지에서 이러한 예를 다운로드할 수 있습니다.  [https://github.com/Workfront](https://github.com/Workfront)

저장소에서 예제를 찾으려면 **저장소 찾기..** 상자에 `example`을(를) 입력하십시오.

>[!NOTE]
>
>API의 모든 사용은 프로덕션 환경에서 실행하기 전에 Workfront의 Beta 환경에서 테스트해야 합니다. Workfront이 온디맨드 소프트웨어에 부담을 준다고 합리적으로 생각하는 프로세스에 고객이 API를 사용하는 경우(즉, 프로세스가 다른 고객을 위해 소프트웨어 성능에 중대한 부정적인 영향을 미치는 경우), Workfront은 고객에게 해당 프로세스를 중단하도록 요청할 수 있는 권한을 보유하며, 고객이 이에 따르지 않고 문제가 지속되는 경우 Workfront은 프로세스를 종료할 수 있는 권한을 보유합니다.

>[!IMPORTANT]
>
>본 소프트웨어는 상품성, 특정 목적에의 적합성 및 비침해에 대한 보증을 포함하되 이에 국한되지 않으며 명시적이든 묵시적이든 어떠한 종류의 보증도 없이 &quot;있는 그대로&quot; 제공됩니다. 어떠한 경우에도 작성자 또는 저작권 소유자는 계약, 불법 행위 또는 기타 어떠한 방법으로든 소프트웨어 또는 소프트웨어의 사용 또는 기타 거래로부터 또는 소프트웨어와 관련하여 발생하는 클레임, 손해 또는 기타 책임에 대해 책임을 지지 않습니다.
