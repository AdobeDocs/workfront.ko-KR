---
title: 2026년 4분기 보고 개선 사항
description: 2026년 4분기 보고 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 3%

---

# 2026년 4분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 4분기 릴리스의 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)를 참조하십시오.

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

## 캔버스 대시보드의 승인 유형 필드

>[!NOTE]
>
>모두를 위한 프로덕션: 2026년 8월 28일
>[!BADGE 일정 해제]{type=Neutral}

이제 승인 엔터티에 **승인 유형** 필드가 포함되어 있으므로 사용자가 증명 승인, 문서 버전 승인, 접수 승인 및 기타 승인 종류를 구분할 수 있습니다.

## 캔버스 대시보드의 승인 용어 업데이트

>[!NOTE]
>
>모두를 위한 프로덕션: 2026년 8월 28일
>[!BADGE 일정 해제]{type=Neutral}

보다 명확하게 하기 위해 문서 및 작업 승인을 위해 캔버스 대시보드에 사용된 다음 필드 이름의 이름이 변경되었습니다.

| 이전 이름 | 새 이름 |
| --- | --- |
| 문서 승인 | 승인 |
| 문서 승인 단계 | 승인 단계 |
| 문서 승인 단계 참가자 | 승인 단계 참가자 |
| 승인 진행 | 작업 승인 프로세스 |
| 승인 단계 | 작업 승인 단계 |
| 승인자 상태 | 작업 승인자 상태 |
| 승인 대기 중 | 작업 승인 대기 중 |

이 변경 사항은 현재 보고서의 작동 방식에 영향을 주지 않습니다.

## 캔버스 대시보드의 피벗 테이블 보고서

>[!NOTE]
>
>미리 보기: 2026년 8월 27일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

캔버스 대시보드의 새로운 피벗 테이블 보고서 유형은 정확하고 완전한 롤업으로 데이터를 집계합니다. 카운트, 합계 및 평균과 같은 지표를 대시보드에서 직접 작성한 다음 모든 합계 뒤의 기본 레코드를 드릴다운할 수 있습니다.

자세한 내용은 [캔버스 대시보드에 피벗 테이블 보고서 작성](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md)을 참조하세요.

## 예약된 보고서에 대한 종료 일자 적용

>[!NOTE]
>
>미리 보기: 2026년 8월 13일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

이제 예약된 보고서를 무기한 게재하지 않도록 하려면 종료 날짜가 필요합니다. 종료 날짜가 지난 일정은 자동으로 비활성화됩니다.

기존 일정은 종료 날짜를 업데이트해 신뢰성을 높이고 불필요한 시스템 사용량을 줄였다. 또한 Workfront에서는 종료 날짜가 가까워지면 보고서 예약 주기를 관리하는 데 도움이 되는 추가 가시성 및 경고를 제공합니다.

자세한 내용은 [자동 보고서 배달 예약](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)을 참조하세요.

## 기본 참조 필드는 목록 및 보고서에 사용할 수 있습니다

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일

이제 Workfront의 목록 및 보고서에 네이티브 참조 필드를 추가할 수 있습니다.

네이티브 참조 필드는 사용자 지정 필드입니다. 필드가 오브젝트에 첨부된 사용자 정의 양식에 있는 경우 필드는 오브젝트 데이터에서 채워집니다. 예를 들어 필드가 설명 필드를 참조하고 프로젝트에 첨부된 사용자 정의 양식에 있는 경우 프로젝트 설명을 가져옵니다. (데이터가 없는 경우 필드에 &quot;N/A&quot;가 표시될 수 있습니다.)

지원되는 네이티브 필드 목록을 포함하여 네이티브 참조 필드를 만드는 방법에 대한 자세한 내용은 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
보고서에 필드를 추가하는 방법에 대한 자세한 내용은 [사용자 지정 보고서 만들기](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

## 기존 목록 및 보고서의 다중 선택 필드 값에 대한 일관된 순서

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일

이제 다중 선택 사용자 정의 필드에 대해 선택한 옵션이 레거시 목록 및 보고서에 일관되고 예측 가능한 순서로 표시됩니다. 필드 순서는 사용자 정의 양식에서 필드를 정렬하는 방법에 따라 결정됩니다.

![사용자 정의 양식 필드 순서가 목록 또는 보고서에서 선택한 값의 순서와 일치합니다](assets/new-field-order-multi-select.png)

이전에는 선택한 옵션이 선택한 순서로 표시되었거나 일관되지 않은 순서로 표시되었으므로 행을 스캔하고 비교하기가 더 어려워졌습니다.

참고: 필드에서 텍스트 모드를 사용하는 경우 새 정렬이 적용되지 않습니다.
