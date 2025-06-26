---
title: 2025년 3분기 보고 개선 사항
description: 2025년 3분기 프로젝트 개선 사항
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 2025년 3분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2025년 3분기 릴리스의 모든 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2025년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2025년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)를 참조하십시오.

## 향상된 보고서 전달 보안

* 미리 보기: 2025년 6월 26일
* 프로덕션: 2025년 6월 26일부터 2025년 7월 9일까지 단계적으로 롤아웃

Workfront 알림이 허용 목록에 추가하다에서 승인된 이메일 도메인으로만 전송되도록 예약된 보고서 배달을 개선했습니다.

이전에는 조직에서 이메일 도메인 Workfront 알림에 대한 제한을 정의한 경우 이메일이 추가되면 허용 목록에 추가하다에 대해 검사를 실행합니다.

허용 목록에 추가하다 이제 입력한 이메일이 이메일 주소를 준수하는지 확인하기 위해 이메일이 전송될 때 확인도 수행합니다. 이 개선된 검사는 사용자와 연결된 이메일 주소와 보고서 수신자 목록에 추가된 임시 이메일 모두에 적용됩니다.

자세한 내용은 [자동 보고서 배달 예약](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)을 참조하세요.


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
