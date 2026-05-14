---
title: 2026년 3분기 보고 개선 사항
description: 2026년 3분기 보고 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# 2026년 3분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

## 캔버스 대시보드 보고서의 데이터 정확도 개선

>[!NOTE]
>
>미리 보기: 2026년 5월 14일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일
>
>Canvas Dashboards는 현재 베타 버전입니다.

이제 캔버스 대시보드는 필터나 필드가 관련 레코드를 교차할 때 중복 행을 방지하기 위해 보고서 쿼리를 구조화하므로 카운트, 합계 및 기타 합계는 정확한 값을 반환합니다.

이전에는 관련 레코드 간의 조인으로 각 관련 레코드에 대해 상위 레코드를 한 번 반복할 수 있었습니다. 예를 들어 특정 사용자에게 할당된 작업으로 필터링된 프로젝트 보고서에서 각 프로젝트는 일치하는 모든 작업에 대해 한 번씩 반복됩니다. 프로젝트 예산을 합산한 KPI는 올바른 $1,250 대신 $6,000을 표시할 수 있습니다.

캔버스 대시보드 인터페이스에는 변경 사항이 없습니다. 기존 보고서는 이 릴리스 이후 정확한 데이터를 자동으로 반환합니다.
