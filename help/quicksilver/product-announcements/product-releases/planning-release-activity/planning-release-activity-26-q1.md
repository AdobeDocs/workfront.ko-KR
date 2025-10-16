---
content-type: release-notes
title: Adobe Workfront Planning의 2026년 1분기 릴리스 활동
description: 2026년 1분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac079ad7cb4b696cb54ff5ad8ff34940d0d62913
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Adobe Workfront Planning의 2026년 1분기 릴리스 활동

이 문서에서는 2026년 1분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록을 보려면 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.


## 글로벌 레코드 유형 및 이를 다른 작업 공간에 기존 레코드 유형으로 추가하는 기능

>[!NOTE]
>
>미리 보기: 2025년 10월 16일
>&#x200B;>프로덕션 빠른 릴리스: 2025년 11월 13일
>&#x200B;>모두를 위한 프로덕션: 2026년 1월 15일

일반적인 워크플로우를 사용하여 여러 팀 조직을 위한 Workfront Planning을 구현할 때 각 팀의 작업 영역에 추가하여 작업을 캡처 및 관리할 수 있는 주요 레코드 유형(예: 캠페인 또는 결과물)에 대한 일관된 구조와 메타데이터를 정의해야 할 수 있습니다.

또한 중앙 수준으로 롤업하려면 각 팀의 작업이 필요할 수 있습니다.

이러한 워크플로우에서는 조직의 모든 사람을 모든 작업 공간에 추가할 필요 없이 팀이 작업을 일관되게 캡처하는 동시에 팀 간 가시성을 확보할 수 있습니다. 글로벌 레코드 유형을 사용하여 이를 수행할 수 있습니다.

이제 레코드 유형을 전역으로 지정하고 여러 작업 공간에서 사용할 수 있습니다. 사용자는 중앙 작업 영역에 이미 구성된 것과 동일한 필드 구조 및 연결을 사용할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [작업 영역 간 레코드 형식 개요](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [작업 영역 간 레코드 유형 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [다른 작업 영역에서 기존 레코드 유형 추가](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 하나의 레코드 종류에 대한 연결 필드의 새 제한

>[!NOTE]
>
>미리 보기: 2025년 10월 16일
>&#x200B;>프로덕션 빠른 릴리스: 2025년 11월 13일
>&#x200B;>모두를 위한 프로덕션: 2026년 1월 15일

각 레코드 유형에 대해 30개의 연결 필드 제한을 도입했습니다.

참고: 현재 조직에 하나의 레코드 종류에 대해 30개가 넘는 연결 필드가 있는 경우 30개를 초과하는 추가 필드를 유지할 수 있습니다. 그러나 한도를 초과하는 레코드 유형에는 더 많은 연결 필드를 추가할 수 없습니다. 앞으로 30개의 연결 필드에 대한 새로운 제한이 적용됩니다.

자세한 내용은 [연결된 레코드 종류 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하십시오.

## 선택 유형 필드 선택 사항에 대해 사용자에게 친숙한 값 설정

>[!NOTE]
>
>미리 보기: 2025년 10월 16일
>&#x200B;>프로덕션 빠른 릴리스: 2025년 11월 13일
>&#x200B;>모두를 위한 프로덕션: 2026년 1월 15일

단일 또는 다중 선택 필드에 필드 선택 사항을 추가하면 Workfront은 이제 각 선택 사항에 사용자에게 친숙한 고유한 값을 할당합니다. 이 개선 전에 Workfront에서는 API 호출 및 기타 통합에서 이해하고 사용하기 어려운 영숫자 ID를 생성했습니다.

이 개선 사항을 통해 다음 사항을 고려하십시오.

* 새 값이 새 필드 선택 사항에 추가됩니다. 기존 필드 선택 사항은 영숫자 ID를 유지합니다.

* 선택 값은 한 필드에 대해 고유하지만 다른 필드 간에 반복될 수 있습니다.

* 선택 항목의 이름을 변경해도 원래 값이 업데이트되지 않습니다.

* 선택 값은 소문자로 표시되며, 여러 단어 선택의 경우 밑줄로 구분됩니다. 동일한 필드에 다른 선택 이름으로 이미 사용된 레이블을 사용하는 경우 Workfront이 값에 순차적 번호를 추가합니다.

자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.