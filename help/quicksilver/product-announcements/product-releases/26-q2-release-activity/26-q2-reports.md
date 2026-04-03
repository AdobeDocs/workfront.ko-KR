---
title: 2026년 2분기 보고 개선 사항
description: 2026년 2분기 보고 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 1a37ff7e4e4b60ac23b0edde6b60258ed508e90b
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 2026년 2분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 2분기 릴리스의 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 2분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 2분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)를 참조하십시오.

## 예약된 보고서 게재가 이제 링크 기반 이메일을 지원합니다.

>[!NOTE]
>
>미리 보기: 2026년 4월 3일
>프로덕션 빠른 릴리스: 2026년 4월 15일
>모두를 위한 프로덕션: 2026년 4월 16일

이제 Workfront에 예약된 보고서에 대한 새로운 링크 게재 유형이 포함됩니다. 이 옵션은 파일을 생성하여 첨부하는 대신 Workfront의 보고서에 대한 직접 링크가 포함된 이메일을 보내어 수신자가 애플리케이션에서 최신 데이터를 볼 수 있도록 합니다.

링크 옵션은 이제 새로 생성된 예약된 보고서 게재 규칙의 기본 게재 유형이며 기존 파일 기반 형식(HTML, PDF, Excel 및 TSV)은 계속 사용할 수 있습니다.

이 변경 사항으로 보고서 게재 이메일의 모양새도 업데이트했습니다.

자세한 내용은 [자동 보고서 배달 예약](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)을 참조하세요.

## 캔버스 대시보드에서 특정 사용자로 보고서 실행

>[!NOTE]
>
>미리 보기: 2026년 4월 2일
>프로덕션 빠른 릴리스: 2026년 4월 15일
>모두를 위한 프로덕션: 2026년 4월 16일
>
>Canvas Dashboards는 현재 베타 버전입니다.

이제 캔버스 대시보드에서 보고서를 구성하여 특정 사용자로 실행할 수 있습니다. 활성화되면 보고서는 뷰어의 권한 대신 선택한 사용자의 액세스 권한에 따라 데이터를 표시합니다.

이를 통해 Planning 작업 공간, 레코드 유형 또는 권한 부여 설정에 대한 액세스가 다른 경우에도 대시보드 뷰어 전체에서 보다 일관되고 안정적인 데이터를 얻을 수 있습니다.

자세한 내용은 [캔버스 대시보드에 KPI 보고서 빌드](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [캔버스 대시보드에 차트 보고서 빌드](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) 또는 [캔버스 대시보드에 테이블 보고서 빌드](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md)를 참조하십시오.

## Data Connect 연결을 위한 새 인증 옵션

>[!NOTE]
>
>미리 보기: 2026년 3월 12일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

이제 RSA 키 또는 PAT(Programmatic Access Tokens) 연결을 사용하여 Data Connect를 인증할 수 있으므로 기존 사용자 이름/암호 자격 증명에 보다 안전하고 유연한 대안을 추가할 수 있습니다.

이러한 새로운 옵션을 통해 조직은 사용자 기반 로그인 방법에 의존하지 않고 Power BI, Tableau 및 기타 타사 BI 도구에서 안정적인 연결을 유지할 수 있습니다.

>[!IMPORTANT]
>
>2026년 6월에 다단계 인증(MFA)을 사용하려면 사용자 이름/암호 자격 증명이 필요합니다. Data Connect에서 인증 프로세스에서 MFA에서 작동하지 않는 서드파티 시각화 도구, 데이터 프로세서 및 스크립트로 데이터를 로드하는 데 사용되는 서비스 사용자 계정의 경우 RSA 또는 PAT 기반 인증으로 전환하는 것이 좋습니다.

## 보고서를 작성할 때 표시되는 사용자 정의 필드 레이블

>[!NOTE]
>
>미리 보기: 2026년 2월 26일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

이제 사용자 지정 필드 레이블이 보고서 작성 도구의 필드 이름과 개체 앞에 표시되므로 필드를 더 쉽게 찾을 수 있습니다. 목록에서 필터, 보기 및 그룹화를 정의할 때도 필드 레이블이 표시됩니다.

사용자 정의 필드 레이블은 시스템 인터페이스용이며, 필드 이름은 API 및 백엔드 스토리지 용도로 자주 사용되며, 필드를 찾을 때 그다지 유용하지 않을 수 있습니다.

자세한 내용은 [사용자 지정 보고서 만들기](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

## 공유 가능한 보고서 폴더

>[!NOTE]
>
>미리 보기: 2026년 2월 26일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

이제 공유 가능한 보고서 폴더를 사용하여 보고서를 구성하고 공유할 수 있습니다. 이 새로운 기능은 대량의 보고서를 관리하는 팀이 확장 가능하고 일관된 액세스 제어를 유지하는 데 도움이 됩니다.

* **구성된 폴더 구조를 만듭니다**: 시스템 관리자는 최상위 수준의 폴더를 만들 수 있으며, 관리 액세스 권한이 있는 사용자는 최대 4단계의 하위 폴더를 만들 수 있습니다.
* **세부 권한 컨트롤**: 다음 두 가지 권한 수준으로 폴더를 공유합니다.
   * 보기: 사용자는 보고서를 열고 폴더를 공유할 수 있습니다
   * 관리: 사용자는 폴더 세부 사항을 편집하고, 항목을 추가/제거하고, 폴더 내의 모든 보고서에 대한 관리 액세스 권한을 자동으로 수신할 수 있습니다
* **상속된 사용 권한**: 사용 권한이 상위 폴더에서 폴더 트리 내의 모든 하위 폴더 및 보고서로 캐스케이드됩니다
* **향상된 목록 환경**: 공유 가능한 폴더를 사용하도록 설정하면 향상된 목록 환경에 액세스할 수 있습니다. 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.


자세한 내용은 [공유 가능한 보고서 폴더 사용](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md)을 참조하세요.

## 캔버스 대시보드의 차트 그룹화에 대한 날짜 레이블이 개선됨

>[!NOTE]
>
>미리 보기: 2026년 2월 26일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

>[!NOTE]
>
>Canvas Dashboards는 현재 베타 버전입니다.

데이터를 날짜별로 그룹화하는 차트에 이제 더 명확하고 읽기 쉬운 날짜 레이블이 표시됩니다. 이 업데이트를 통해 날짜 레이블은 선택한 그룹화 기준 옵션(예: 일, 주, 월 또는 년)에 따라 동적으로 조정되므로 차트를 쉽게 읽고 해석할 수 있습니다.

<table> <tbody> <tr> <td>Day</td> <td>전체 날짜를 표시합니다. 예: 2026/3/12</td> </tr> <tr> <td>주</td> <td>서식이 지정된 주 시작 날짜를 표시합니다. 예, 2026년 3월 8일</td> </tr> <tr> <td>Month</td> <td>월과 연도를 표시합니다. 예제 2026년 3월</td> </tr> <tr> <td>Year</td> <td>연도만 표시합니다. 예: 2026</td> </tr> </tbody> </table>

이전에는 차트 그룹화에 선택한 기간의 시작 일자가 항상 숫자 형식으로 표시되었습니다.
