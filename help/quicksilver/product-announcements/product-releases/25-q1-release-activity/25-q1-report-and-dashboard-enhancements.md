---
title: 2025년 1분기 보고서 및 대시보드 개선 사항
description: 2025년 1분기 보고서 및 대시보드 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3c0b4797-594c-44d0-b3ad-a64384b6c4a8
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 4%

---

# 2025년 1분기 보고서 및 대시보드 개선 사항

이 페이지에서는 미리보기 환경에 대한 2025년 1분기 릴리스의 모든 보고서 및 대시보드 개선 사항에 대해 설명합니다. 향상된 기능은 앞서 설명한 대로 프로덕션 환경에서 사용할 수 있습니다.

2025년 1분기 릴리스 주기의 현재 사용 가능한 모든 변경 사항에 대한 목록은 [2025년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)를 참조하십시오.

## 데이터 연결에서 사용할 수 있는 새 엔터티

>[!NOTE]
>
>미리보기 릴리스: 2025년 1월 15일, 모든 고객을 위한 프로덕션 릴리스: 2025년 1월 15일

Data Connect에서 다음 엔터티에 대한 지원을 추가했습니다.

* 프로젝트 팀 사용자
* 프로젝트 팀 사용자 역할
* 보고 가능한 예산 책정 시간
* 보고서 조회 통계 수
* 리소스 관리자
* 서식 있는 텍스트 메모

다음 에이전시별 엔티티에 대한 지원도 추가했습니다.

* 비즈니스 프로필
* 비즈니스 규칙
* 위치
* 비노동 리소스 범주
* 사용자 위치

자세한 내용은 [Workfront Data Connect 데이터 사전](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)을 참조하세요.

## 대시보드의 보고서, 외부 페이지 또는 일정 25개 제한

>[!NOTE]
>
>미리보기 릴리스: 2024년 12월 16일, 모든 고객을 위한 프로덕션 릴리스: 25.1 릴리스 포함(2025년 1월 16일)

대시보드 성능을 유지하기 위해 대시보드에 배치할 수 있는 보고서, 외부 페이지 또는 달력의 총 수에 대한 제한을 구현했습니다. 새 대시보드를 만들 때 최대 25개의 항목을 추가할 수 있습니다.

이 한도를 초과하는 기존 대시보드에는 최상위 25개 항목만 표시된다는 경고가 표시되며, 편집된 대시보드는 포함된 항목 수가 25개 이하로 줄어들 때까지 저장할 수 없습니다.

자세한 내용은 [대시보드 만들기](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하세요.

## 데이터 연결에 대한 첫 번째 판독기 계정 생성 단추

>[!NOTE]
>
>모든 고객을 위한 프로덕션 릴리스: 2024년 11월 14일

Data Connect에 처음 액세스하는 관리자에게는 이제 버튼 하나를 클릭하여 새 Snowflake 판독기 계정을 만들 수 있는 옵션이 제공됩니다. 이 프로세스는 완료하는 데 몇 분 정도 소요되지만 추가 작업은 필요하지 않습니다.

Data Connect 설정에 대한 자세한 내용은 [Snowflake의 Reader 계정 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)를 참조하십시오.
