---
title: 삭제된 개체의 할당이 할당자 보고서에 예기치 않게 나타납니다.
description: 삭제된 개체의 할당이 할당자 보고서에 예기치 않게 나타납니다.
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# 삭제된 개체의 할당이 할당자 보고서에 예기치 않게 나타납니다.

## 문제

할당이 있는 객체를 삭제하면 객체와 할당이 모두 삭제됩니다. 그러나 그 할당이 여전히 일부 보고서에 나타날 수도 있습니다.

예를 들어 사용자에게 할당된 작업을 삭제하면 사용자에게 할당된 할당도 삭제됩니다. 그러나 나중에 할당자로 필터링된 작업 보고서를 해당 사용자가 지정한 상태로 실행하면 해당 작업이 휴지통에 있는 경우 보고서에 삭제된 작업이 계속 표시됩니다.

## 원인

이는 휴지통의 아키텍처 제한 사항 때문입니다. 현재 이 문제를 해결하기 위한 로드맵에 대한 계획은 없습니다. 이것은 건축적 재설계가 필요하기 때문입니다.
