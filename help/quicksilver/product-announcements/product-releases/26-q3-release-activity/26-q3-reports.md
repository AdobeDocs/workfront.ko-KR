---
title: 2026년 3분기 보고 개선 사항
description: 2026년 3분기 보고 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 0c7265c477030137d14e95f42eaf67580589d70b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 2026년 3분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 3분기 릴리스의 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)를 참조하십시오.

## Snowflake에서 Workfront Planning에 대한 자동 액세스 제어

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 7월 16일일정 해제&rbrack;{type=Neutral}

이 릴리스에서는 Workfront Data Connect의 일부로 Snowflake의 Workfront Planning 데이터에 대한 권한 기반의 자동 액세스 관리를 도입했습니다.
보안 뷰 생성을 계획 테이블로 확장하여 다운스트림 액세스 제어에 필요한 기반을 구축하고 권한 기반 부여를 가능하게 합니다.이를 기반으로 하는 리더 계정 프로비저닝은 이제 생성 시 TMS 권한을 확인하고 Planning 데이터베이스에 자동으로 부여를 적용 또는 보류하여 정확한지 확인합니다.
이 개선 사항 이전에는 Workfront에서만 사용할 수 있었습니다.
업데이트에는 다음 기능이 포함됩니다. 

* 자동화된 일별 작업은 기존 고객에 대한 자격 변경 사항을 감지합니다.
* 새 작업은 권한을 기반으로 액세스 권한을 부여, 취소 또는 보존합니다.
* 프로비저닝, 계정 생성 및 지속적인 자격 변경 전반에 걸친 전체 라이프사이클 적용 범위.

[Workfront Data Connect 데이터 사전](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) 문서는 릴리스 날짜 이후에 업데이트됩니다.

## 새 오브젝트에 대한 사용자 정의 데이터 지원 추가

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 7월 7일일정 해제&rbrack;{type=Neutral}

2026년 2분기 중에 Workfront의 엔터프라이즈 작업 개선 사항을 지원하는 새 개체를 추가했습니다.현재 릴리스에서는 캔버스 대시보드의 여러 새 오브젝트에 대한 사용자 정의 데이터 지원도 추가하고 있습니다.

자세한 내용은 [캔버스 대시보드 개요](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md)를 참조하십시오.

## 캔버스 대시보드 프롬프트 기본값 및 사용자 환경 설정 지속성

>[!NOTE]
>
>미리 보기: 2026년 6월 25일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일

작업 필터 상태를 유지하여 대시보드와 레코드 간을 이동하는 사용자의 효율성을 개선하기 위해 대시보드 관리자는 이제 캔버스 대시보드에 대한 기본 프롬프트 값을 정의할 수 있습니다. 이러한 기본값은 모든 대시보드 뷰어에 자동으로 적용됩니다.

사용자가 프롬프트를 업데이트할 때 선택 사항이 저장되고 새로 고침, 다시 열기 또는 레코드로 이동한 후 복원됩니다.

관리자는 언제든지 대시보드의 기본 상태를 재설정할 수 있습니다. 세 점 메뉴를 통해 빠르게 기본값으로 되돌릴 수도 있습니다.

이 개선 이전에는 대시보드 프롬프트에 프롬프트 상태에 대한 구성 가능한 기본값이나 저장된 사용자 기본 설정이 없었습니다.

자세한 내용은 [캔버스 대시보드 필터링](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md)을 참조하십시오.

## 여러 Power BI IP 주소 범위를 Data Connect에 한 번에 추가합니다

>[!NOTE]
>
>미리보기: 해당 사항 없음프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

이제 Microsoft Power BI을 Workfront Data Connect에 연결하는 Workfront 관리자는 전체 지역의 Azure IP 주소 범위 세트를 허용 목록에 추가하다 IP에 한 번에 추가할 수 있습니다. 이제 **데이터 연결**&#x200B;의 **IP 범위** 탭에서 **새 IP 주소** 단추에 **Power BI IP 주소 블록 추가** 옵션이 포함되어 있습니다. 이 옵션은 Microsoft에서 게시한 Azure IP 범위 및 서비스 태그 JSON 파일의 Power BI 서비스 태그 항목을 붙여넣을 수 있는 대화 상자를 엽니다.

이 기능은 각 Power BI CIDR 블록을 한 번에 하나씩 추가하는 이전 워크플로우를 대체합니다. 이 작업은 수십 개의 주소 접두사를 게시하는 지역에서는 시간이 오래 걸립니다.

자세한 내용은 [Workfront Data Connect에 연결 설정](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)을 참조하십시오.


## 캔버스 대시보드 목록 정렬

>[!NOTE]
>
>미리 보기: 2026년 6월 11일프로덕션 빠른 릴리스: 2026년 7월 15일모두를 위한 프로덕션: 2026년 7월 16일
>
>Canvas Dashboards는 현재 베타 버전입니다.

이제 **이름**, **설명**, **만든 사람** 또는 **만든 날짜** 열을 기준으로 캔버스 대시보드 목록을 정렬할 수 있습니다. 열 머리글을 클릭하여 해당 열을 기준으로 목록을 정렬한 다음, 동일한 머리글을 다시 클릭하여 정렬 방향을 반대로 바꿉니다. 기본적으로 목록은 A부터 Z까지 **이름**&#x200B;별로 정렬됩니다. 캔버스 대시보드 목록의 탭 간을 전환하면 정렬 순서가 유지됩니다.

자세한 내용은 [캔버스 대시보드 사용](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)을 참조하세요.

## 사용자 정의 공식의 실제 시간 변경

>[!NOTE]
>
>미리 보기: 2026년 6월 1일프로덕션 빠른 릴리스: 2026년 6월 1일모두를 위한 프로덕션: 2026년 6월 1일

2025년에 새 실제 시간 필드가 Workfront 데이터베이스에 `actualWorkRequiredDouble`(으)로 추가되었으며 기존 실제 시간 필드(`actualWorkRequired` in the database)가 이전 실제 시간으로 이름이 변경되었습니다. 자세한 내용은 [릴리스 정보](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md)를 참조하세요.

2026년 6월에 `actualWorkRequired`(기존 실제 시간)을 사용하는 기존 사용자 지정 수식이 `actualWorkRequiredDouble`(실제 시간)을(를) 대신 사용하도록 마이그레이션되었습니다. `actualWorkRequired`은(는) 더 이상 계산 및 수식에 사용할 수 없습니다.

또한 모든 보고서에서 `actualWorkRequiredDouble`을(를) 사용하는 것이 좋습니다.

필드를 바꿀 때 `actualWorkRequired`은(는) 값을 분 단위로 저장하는 반면 `actualWorkRequiredDouble`은(는) 값을 소수 자릿수로 시간 단위로 저장합니다.

실제 사용 시간에 대한 자세한 내용은 [실제 사용 시간 보기](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)를 참조하십시오.

## 캔버스 대시보드 보고서의 사용자 지정 통화 데이터 필드

>[!NOTE]
>
>미리 보기: 2026년 5월 28일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일

이제 캔버스 대시보드 보고서는 System Setup에서 여러 환율을 구성하는 경우를 포함하여 열, 필터, 그룹화 및 집계로서 사용자 지정 통화 데이터 필드를 지원합니다. 사용자 지정 통화 데이터 필드가 열 또는 합계로 표시되면 필드가 보고서 수준에서 잠겨 있지 않은 경우 값이 대시보드의 환율에 선택된 통화로 전환됩니다.

두 번째 환율 통화가 추가된 후 &quot;제한된 필드&quot; 메시지로 인해 이전에 실패한 보고서가 이제 렌더링됩니다. 복수 환율이 정의된 경우 계획 통화 필드는 제한된 상태로 유지됩니다.

자세한 내용은 [캔버스 대시보드의 통화 필드 사용](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)을 참조하세요.

## 캔버스 대시보드 보고서의 데이터 정확도 개선

>[!NOTE]
>
>미리 보기: 2026년 5월 14일프로덕션 빠른 릴리스: 2026년 6월 11일모두를 위한 프로덕션: 2026년 7월 16일
>
>Canvas Dashboards는 현재 베타 버전입니다.

이제 캔버스 대시보드는 필터나 필드가 관련 레코드를 교차할 때 중복 행을 방지하기 위해 보고서 쿼리를 구조화하므로 카운트, 합계 및 기타 합계는 정확한 값을 반환합니다.

이전에는 관련 레코드 간의 조인으로 각 관련 레코드에 대해 상위 레코드를 한 번 반복할 수 있었습니다. 예를 들어 특정 사용자에게 할당된 작업으로 필터링된 프로젝트 보고서에서 각 프로젝트는 일치하는 모든 작업에 대해 한 번씩 반복됩니다. 프로젝트 예산을 합산한 KPI는 올바른 $1,250 대신 $6,000을 표시할 수 있습니다.

캔버스 대시보드 인터페이스에는 변경 사항이 없습니다. 기존 보고서는 이 릴리스 이후 정확한 데이터를 자동으로 반환합니다.

