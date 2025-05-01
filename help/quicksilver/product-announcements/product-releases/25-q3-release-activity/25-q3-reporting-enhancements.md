---
title: 2025년 3분기 보고 개선 사항
description: 2025년 3분기 프로젝트 개선 사항
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 2025년 3분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2025년 3분기 릴리스의 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2025년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2025년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)를 참조하십시오.

## 사용자 와일드카드는 필터링 시 더 이상 null 값이 포함된 결과를 반환하지 않습니다.

>[!NOTE]
>
>* 미리 보기: 2025년 4월 30일
>* 프로덕션 빠른 릴리스: 2025년 5월 15일
>* 모든 고객을 위한 프로덕션: 2025년 7월 17일

보고서를 필터링할 때 null 값을 제외하도록 사용자 와일드카드 동작을 업데이트했습니다. 이러한 변경 사항은 사용자가 올바르게 구성되지 않은 결과(null 결과)를 반환하는 대신 필터가 보다 정확한 결과를 생성하는 데 도움이 됩니다.

이전에는 사용자 와일드카드가 null 값을 생성하면 보고서에는 null 값도 포함된 모든 레코드가 표시됩니다.

이 변경 사항은 다음 와일드카드 필터에 적용됩니다.

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

