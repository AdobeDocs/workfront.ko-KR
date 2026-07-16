---
content-type: release-notes
title: Adobe Workfront Planning의 2026년 3분기 릴리스 활동
description: 2026년 3분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 847c38fe006ca5f1170e4b28c9b0a2c61c5c77fa
workflow-type: tm+mt
source-wordcount: '3109'
ht-degree: 0%

---

# Adobe Workfront Planning의 2026년 3분기 릴리스 활동

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

이 문서에서는 2026년 3분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록을 보려면 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.


## 액세스 수준에 대한 새 라이선스 유형 필드

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 7월 16일
>[!BADGE 일정 해제]{type=Neutral}


액세스 수준 상자에서 다음과 같은 필드를 변경했습니다.

* 액세스 수준 상자의 라이선스 유형 필드 이름을 워크플로 라이선스 유형으로 변경했습니다. 이 레이블 재지정에는 기능 변경 사항이 없습니다.

  자세한 내용은 [사용자 지정 액세스 수준 만들기 및 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

* Workfront Planning 패키지도 구입한 고객의 경우 Workfront Planning에 사용자 라이센스를 설명하기 위해 새 Planning 라이센스 유형 필드를 추가했습니다.
동일한 수의 Workflow 및 Planning 라이선스를 구입한 고객은 다음 라이선스 유형을 사용할 수 있습니다.

   * 계획 수립 표준
   * 계획 수립 참여자
   * 없음

>[!NOTE]
>
>Workflow와 Planning 간에 혼합된 라이센스 조합을 사용자에게 지정할 수 있지만 Planning Standard 라이센스를 얻으려면 사용자에게 유료 Workflow 라이센스가 있어야 합니다.
>
>예를 들어 Planning Standard 라이선스는 Workflow Contributor 사용자에게 할당할 수 없습니다. 이제 Workflow Light 라이선스가 있는 사용자에게 Planning에 표준 라이선스를 부여하여 작업 공간 및 콘텐츠를 관리할 수 있습니다. 이전에는 Planning 데이터에 대한 보기 전용 액세스 권한만 가질 수 있었습니다.
>
>신규 고객은 Planning 및 Workflow 라이센스를 다른 수량으로 구매하여 모든 조합과 함께 사용할 수 있습니다. 이 시나리오에서는 계획 기여자 라이선스 유형을 사용할 수 없습니다.

자세한 내용은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.

## Snowflake에서 Workfront Planning에 대한 자동 액세스 제어

>[!IMPORTANT]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 7월 16일
>[!BADGE 일정 해제]{type=Neutral}


이 릴리스에서는 Workfront Data Connect의 일부로 Snowflake의 Workfront Planning 데이터에 대한 권한 기반의 자동 액세스 관리를 도입했습니다.

보안 뷰 생성을 계획 테이블로 확장하여 다운스트림 액세스 제어에 필요한 기반을 구축하고 권한 기반 부여를 가능하게 합니다.

이를 기반으로 하는 리더 계정 프로비저닝은 이제 생성 시 TMS 권한을 확인하고 Planning 데이터베이스에 자동으로 부여를 적용 또는 보류하여 정확한지 확인합니다.

이 개선 사항 이전에는 Workfront에서만 사용할 수 있었습니다.

업데이트에는 다음 기능이 포함됩니다.

* 자동화된 일별 작업은 기존 고객에 대한 자격 변경 사항을 감지합니다.
* 새 작업은 권한을 기반으로 액세스 권한을 부여, 취소 또는 보존합니다.
* 프로비저닝, 계정 생성 및 지속적인 자격 변경 전반에 걸친 전체 라이프사이클 적용 범위.

[Workfront Data Connect 데이터 사전](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) 문서는 릴리스 날짜 이후에 업데이트됩니다.


## 레코드에 대한 기본 권한 설정

>[!NOTE]
>
>미리 보기: 2026년 7월 7일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 Workspace 관리자는 각 레코드 유형에 대해 기본 권한 규칙(열기 또는 제한됨)을 설정할 수 있으므로 수동으로 조작하지 않아도 새로 만든 레코드가 자동으로 보호됩니다.

제한을 선택하면 레코드 생성자와 특별히 선택한 사용자, 그룹, 팀, 역할 또는 회사만 레코드를 편집할 수 있으며 그 외의 모든 사용자는 보기 전용 액세스 권한을 유지합니다.

이 규칙은 레코드 생성 방법(새 레코드 단추, 요청 양식, API, Fusion 자동화 사용 또는 AI Assistant 사용)에 관계없이 새 레코드에 자동으로 적용됩니다. 규칙 변경 사항은 앞으로 작성된 레코드에만 영향을 주고 기존 레코드에는 영향을 주지 않습니다.

레코드가 만들어지더라도 향후 레코드에 대한 기본 규칙에 영향을 주지 않고 해당 권한을 독립적으로 업데이트할 수 있습니다.

자세한 내용은 [레코드에 대한 기본 권한 설정](/help/quicksilver/planning/access/set-default-record-permissions.md)을 참조하십시오.

## 타임라인 보기를 위한 스윔레인 그룹화 레이아웃

>[!NOTE]
>
>미리 보기: 2026년 7월 7일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 그룹화된 타임라인 보기는 수평 밴드를 스크롤하는 대신 고정된 왼쪽 헤더 열로 렌더링하여 스윔레인 레이아웃을 지원합니다. 이 그룹화 유형은 현재 스택 그룹화에 추가됩니다.

중첩된 그룹화 수준은 들여쓴 하위 열로 표시되며 각 레인 내의 레코드는 하위 스택되어 정렬됩니다.

그룹화된 보기에서 레코드를 끌어다 놓아 해당 정보와 날짜를 원활하게 업데이트할 수 있습니다.

보기를 보는 모든 사용자는 적용된 그룹화를 볼 수 있습니다.

자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.


## 글로벌 검색 상자의 최근에 방문한 항목

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 6월 30일
>[!BADGE 일정 해제]{type=Neutral}

이제 Planning의 글로벌 검색 상자는 가장 최근의 검색을 기억합니다. 즉, 마지막으로 방문한 7개의 작업 공간, 레코드 유형 및 보기는 명확하게 레이블이 지정된 전용 섹션에 표시되므로 쿼리를 다시 실행하지 않고도 빠르게 액세스할 수 있습니다.

최근 결과는 현재 권한을 준수하며 가장 최근 항목 목록은 라이브 검색 결과와 시각적으로 구별됩니다. 이전과 같이 Planning 랜딩 페이지나 모든 페이지에서 키보드 조합을 사용하여 검색에 액세스할 수 있습니다.

자세한 내용은 [Workspace 개요](/help/quicksilver/planning/architecture/workspaces-overview.md)를 참조하십시오.


## 캔버스 대시보드의 통화 계획 필드 지원

>[!NOTE]
>
>미리 보기: 2026년 6월 25일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 캔버스 대시보드의 테이블, KPI 및 차트 보고서에 통화 계획 필드를 포함할 수 있습니다.

이 개선 이전에는 통화 필드가 캔버스 대시보드에서 지원되지 않았습니다.

자세한 내용은 [캔버스 대시보드의 통화 필드 사용](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)을 참조하세요.

## 행 색상 컨트롤 인터페이스 개선

>[!NOTE]
>
>미리 보기: 2026년 6월 22일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

표 보기에서 행 색상 컨트롤의 모양과 느낌을 업데이트했습니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

## 선택 및 사용자 유형 필드에 대한 기본 선택 항목 추가

>[!NOTE]
>
>미리 보기: 2026년 6월 18일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 단일, 다중 선택 필드 또는 사람 유형 필드를 만들 때 이러한 필드의 기본값을 표시할 수 있습니다. 필드가 레코드에 표시될 때 기본값이 항상 적용됩니다.

필드를 저장한 후 필드의 기본 설정을 변경할 수 있습니다. 레코드 작업 시 필드의 기본값을 바꿀 수 있습니다.

자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

## 테이블 보기의 인터페이스 개선 사항

>[!NOTE]
>
>미리 보기: 2026년 6월 11일
>프로덕션 빠른 릴리스: 2026년 7월 15일
>모두를 위한 프로덕션: 2026년 7월 16일

Workfront Planning의 다음 영역에 대한 테이블 보기의 모양과 느낌을 업데이트했습니다.

* 모든 레코드 유형 페이지

* 프로젝트를 제외한 연결된 모든 레코드 유형 페이지

일부 탐색 변경 및 디자인 개선 사항 외에도 이 업데이트에서는 다음과 같은 사항이 개선되었습니다.

* SUM, AVG, MAX, MIN과 같은 집계기를 사용하여 숫자, 통화, 백분율 및 일부 공식 필드를 요약하는 테이블 하단의 집계 행 추가.

* 날짜 필드를 추가할 때 형식 유형이 줄어들고 더 간단한 날짜 형식입니다.

* 날짜 필드를 추가할 때 프로필의 시간대에 관계없이 모든 사용자가 볼 수 있는 시간대를 선택하는 기능.

* 깔끔한 디자인을 위해 행 번호 지정 제거

* 마우스로 행을 가리키면 표시되는 대신 영구 행 선택 상자

* 가독성을 높이기 위한 지속적인 열 구분선

* 열 헤더에서 정렬할 때 보다 간단한 정렬 환경

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.


## 이제 GenStudio for Performance Marketing 브랜드를 Planning 요청 양식에 추가할 수 있습니다.

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 6월 5일
>Adobe GenStudio for Performance Marketing이 있는 Adobe Workfront Planning 고객만 사용할 수 있습니다.
>[!BADGE 일정 해제]{type=Neutral}


이제 요청 제출로 시작하는 캠페인에 브랜드를 추가할 수 있도록 브랜드 연결 레코드 필드를 계획 요청 양식에 추가할 수 있습니다.

계획 레코드 유형이 GenStudio 브랜드 레코드 유형과 연결된 경우 계획 레코드 유형과 연결된 계획 요청 양식에 연결된 브랜드 필드를 추가할 수 있습니다.

자세한 내용은 [Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.


## 새 샘플 작업 공간 탭이 Planning 랜딩 페이지에 추가됨

>[!NOTE]
>
>미리 보기: 2026년 6월 1일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일


모범 사례 작업 영역의 예를 볼 수 있는 Planning 랜딩 영역에 샘플 작업 영역 탭을 추가했습니다. 작업 영역을 편집할 수 없습니다. Workspace 관리자는 샘플 작업 공간에서 보기를 수정할 수 있습니다. 이 탭은 Standard 및 System Administrator 사용자에게 표시됩니다.

샘플 작업 영역을 예로 보고 다중 작업 영역 템플릿 번들을 사용하여 해당 템플릿을 사용하는 작업 영역을 만들고, 편집하고, 공유하는 것이 좋습니다.  템플릿 번들에는 샘플 작업 공간 탭과 동일한 작업 공간이 포함되어 있습니다.

자세한 내용은 [작업 영역 개요](/help/quicksilver/planning/architecture/workspaces-overview.md)를 참조하십시오.

>[!NOTE]
>
>템플릿 번들에서 작업 공간 만들기는 Workflow Prime 또는 Ultimate 패키지의 조직에서만 사용할 수 있습니다.

## Workfront Planning API 버전 2

>[!NOTE]
>
>모든 고객이 사용 가능: 2026년 5월 28일
>[!BADGE 일정 해제]{type=Neutral}

이제 Workfront Planning API의 버전 2를 사용할 수 있으며 버전 1의 기능을 크게 확장합니다.

다음 개선 사항이 버전 2에 포함되어 있습니다.

* 프로그래밍 방식으로 작업 공간, 레코드 형식 및 필드를 만들고, 업데이트하고, 삭제합니다.

* 레코드를 완전히 관리합니다.
* URL 구조, 오류 처리, 페이지 매김, 필터링 및 사용 권한 개선.
* PATCH을 통한 부분 업데이트 포함
* 대량 레코드 작업을 포함합니다.

버전 1은 계속 사용할 수 있지만 버전 2를 사용하는 것으로 전환하는 것이 좋습니다.

>[!NOTE]
>
>Fusion용 Workfront Planning 커넥터가 API 버전 2로 업데이트되지 않았으며 추가 공지가 있을 때까지 버전 1을 계속 사용합니다.

자세한 내용은 [Adobe Workfront Planning API 기본 사항](/help/quicksilver/planning/general/planning-api-basics.md)을 참조하십시오.

Workfront Planning API 사양은 [Workfront Planning API](https://developer.adobe.com/wf-planning/) 개발자 설명서를 참조하십시오.

## 레코드에 대한 권한 부여

>[!NOTE]
>
>미리 보기: 2026년 5월 28일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일


이제 개별 레코드 권한을 조정하여 레코드 종류 내에서 관리할 수 있는 사용자를 제어할 수 있습니다.

기본적으로 사용자는 작업 영역 및 레코드 유형에서 레코드 권한을 상속합니다. 이제 특정 레코드에 대해 상속된 권한을 재정의하여 사용자 하위 집합에 대한 보기 또는 관리 액세스 권한을 부여할 수 있습니다. 권한 무시는 개별 레코드에 적용되거나 여러 레코드에서 일괄적으로 업데이트될 수 있습니다.

<!-- 
Laurel asked for this to be replaced with the above: 

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 
-->

>[!NOTE]
>
>* 사용자의 레코드 수준 권한은 해당 레코드 유형 권한을 초과할 수 없습니다. 예를 들어 레코드 유형에 대한 보기 액세스 권한이 있는 사용자에게 해당 유형의 개별 레코드에 대한 관리 액세스 권한을 부여할 수 없습니다.
>* 현재 레코드에서 사용자의 권한을 제거할 수 없습니다. 레코드 종류에 대해 적어도 보기 액세스 권한이 있는 모든 사용자는 해당 형식의 모든 레코드를 볼 수 있습니다.

자세한 내용은 [레코드 공유](/help/quicksilver/planning/access/share-records.md)를 참조하세요.

## 간소화된 글로벌 레코드 유형 추가

>[!NOTE]
>
>미리 보기: 2026년 5월 28일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

클릭을 줄이고 필요한 레코드 유형을 빠르게 찾을 수 있도록 글로벌 레코드 유형을 다른 작업 공간에 추가할 때 더 빠르고 직관적으로 사용할 수 있도록 레코드를 추가할 수 있는 환경을 개선했습니다.

기존 레코드 유형에서 레코드를 추가하도록 선택하면 이제 사용 가능한 모든 글로벌 레코드 유형 목록이 즉시 표시됩니다.

이 화면에서 직접 하나 이상의 글로벌 레코드 유형을 선택하고 동시에 추가할 수 있습니다.

자세한 내용은 [다른 작업 영역에서 기존 레코드 형식 추가](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)를 참조하십시오.

## 이제 모든 Designer Planning 고객이 Beta에서 Workfront Planning을 사용할 수 있습니다.

>[!NOTE]
>
>미리 보기: 2026년 5월 28일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일
>[!BADGE Beta]{type=Neutral}에서

이제 AI에서 제공하는 Adobe Planning Designer을 사용하여 작업 공간 및 데이터 구조를 쉽게 구성할 수 있습니다. Planning Designer은 작업 공간 생성 및 구성에서 필드 및 공식 정의, 레코드 관리, 변경 내용 검토 및 사용자 정의 보기 작성에 이르기까지 모든 작업을 지원합니다.

Planning Designer은 직접 사용하든 AI Assistant를 통해 사용하든 상관없이 구조화되고 연결된 정보를 구축하고 유지할 수 있는 유연하고 강력한 환경을 제공합니다.

Workfront 관리자는 설정의 시스템 환경설정 영역에서 Planning Designer의 가용성을 관리할 수 있습니다.

자세한 내용은 [Adobe Workfront Planning Designer 시작](/help/quicksilver/planning/general/planning-ai-designer.md)을 참조하십시오.


## Planning에서 AEM Assets으로 메타데이터 동기화

>[!NOTE]
>
>모두를 위한 미리 보기 및 프로덕션: 2026년 5월 28일
>Adobe GenStudio for Performance Marketing 및 Adobe Experience Manager이 있는 Adobe Workfront Planning 고객만 사용할 수 있습니다.
>[!BADGE 일정 해제]{type=Neutral}

데이터 무결성을 향상시키기 위해 GenStudio for Performance Marketing이 Workfront Planning에서 GenStudio 레코드 유형에 연결되어 있을 때 AEM Assets 레코드 유형과 AEM Assets 간에 매끄러운 메타데이터 동기화를 릴리스했습니다.

AEM Assets에 연결할 수 있는 GenStudio for Performance Marketing 레코드 유형은 Campaign, Product, Persona, Region 및 Channel입니다.

Workfront Planning에서 GenStudio 레코드 유형에 추가된 정보는 AEM에 있는 AEM 자산의 개별 캠페인 탭에 표시됩니다. 해당 캠페인에 대한 제품, 사용자, 지역 및 채널에 대한 정보도 읽기 전용 모드로 해당 탭에 표시됩니다.

이번 릴리스를 통해 주요 메타데이터는 두 플랫폼 모두에서 일관되며 실시간에 가까운 업데이트를 반영하므로 수동 조정이 줄어듭니다.

자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.

## Planning에서 AEM 컨텐츠 조각으로 메타데이터 동기화

>[!NOTE]
>
>모두를 위한 미리 보기 및 프로덕션: 2026년 5월 28일
>Adobe GenStudio for Performance Marketing 및 Adobe Experience Manager이 있는 Adobe Workfront Planning 고객만 사용할 수 있습니다.
>[!BADGE 일정 해제]{type=Neutral}

데이터 무결성을 향상시키기 위해 컨텐츠 조각이 GenStudio for Performance Marketing 캠페인에 연결될 때 GenStudio 작업 영역의 Planning 레코드 유형과 AEM 컨텐츠 조각 간의 매끄러운 메타데이터 동기화를 릴리스했습니다.

이제 GenStudio 캠페인 정보가 AEM에 있는 콘텐츠 조각의 메타데이터 탭에 표시됩니다.  해당 캠페인에 대한 제품, 사용자, 지역 및 채널에 대한 정보도 읽기 전용 모드로 해당 탭에 표시됩니다.

이번 릴리스를 통해 주요 메타데이터는 두 플랫폼 모두에서 일관되며 실시간에 가까운 업데이트를 반영하므로 수동 조정이 줄어듭니다.

자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.


## 목록 보기 업데이트

>[!NOTE]
>
>미리 보기: 2026년 5월 27일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

키보드 탐색 및 기타 개선 사항을 포함하도록 목록 보기의 여러 필드 유형이 업데이트되었습니다.

다중, 단일 선택 및 할당자 필드는 이제 목록 보기에서 키보드 탐색을 제공합니다.

* 키보드의 위쪽 및 아래쪽 화살표를 사용하여 사람 목록을 이동합니다.

* 스페이스바를 눌러 사용자를 선택하거나 선택한 사용자를 제거합니다.

목록 보기의 단일 및 다중 선택 필드에서 다음을 수행합니다.

* 결과를 찾을 수 없을 때 편집기에서 직접 새 옵션을 추가할 수 있습니다. 일부 목록에서는 이 기능을 사용할 수 없습니다.

* 이제 키보드에서 필드 상호 작용에 액세스할 수 있습니다. 여기에는 위쪽 및 아래쪽 화살표를 사용한 태그, 검색 옵션, 목록 간의 탐색이 포함됩니다. 스페이스 바를 눌러 항목을 선택하거나 선택한 항목을 제거합니다.

자동 완성 및 외부 조회 필드와 같은 참조 필드에 몇 가지 인터페이스 개선 사항이 수신되었습니다.

또한 사용 가능한 경우 열을 끌어서 놓는 경험이 시각적으로 개선되었습니다.

자세한 내용은 [Adobe Workfront Planning에서 목록 보기 관리](/help/quicksilver/planning/views/manage-the-list-view.md)를 참조하십시오.

## Workfront 참조 필드는 Planning 연결에 대한 조회 필드로 활성화됩니다

>[!NOTE]
>
>미리 보기: 2026년 5월 27일
>프로덕션 빠른 릴리스: 2026년 6월 11일\
>모두를 위한 프로덕션: 2026년 7월 16일

이제 Planning 레코드 유형을 Workfront 개체 유형으로 연결할 때 Workfront 참조 필드를 조회 필드로 추가할 수 있습니다.

예를 들어 프로젝트 객체의 Portfolio, 프로그램, 그룹 또는 회사 정보를 Planning에서 캠페인의 프로젝트 연결 필드에 추가할 수 있습니다.

자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 타임라인 보기 분류 기능에 대한 새 필터

>[!NOTE]
>
>미리 보기: 2026년 5월 27일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 레코드 분류에 포함된 개체와 일치하는 조건을 기준으로 타임라인 보기에서 정보를 필터링할 수 있습니다.

이 개선 이전에는 타임라인 보기의 기본 레코드에 대한 필터만 적용할 수 있었습니다.

자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

## 편집되고 삭제된 필드가 요청 양식에 영향을 준다는 새로운 표시

>[!NOTE]
>
>미리 보기: 2026년 5월 27일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

편집하거나 삭제하는 레코드 필드가 해당 필드를 포함하는 요청 양식에 영향을 줄 수 있다는 미리 알림을 추가했습니다. 이제 영향을 받는 양식을 검토하고 필드에 적용할 변경 사항이 기존 정보에 영향을 주지 않는지 확인할 수 있습니다.

자세한 내용은 [필드 설정 편집](/help/quicksilver/planning/fields/edit-fields.md)을 참조하세요.

## 제출된 Planning 요청 편집

>[!NOTE]
>
>미리 보기: 2026년 5월 27일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 Planning 요청을 제출한 후 요청에서 레코드가 생성되기 전에 편집할 수 있습니다.

다음 사용자는 제출된 요청을 편집할 수 있습니다.

* 요청 작성자
* 요청이 제출된 작업 공간의 Workspace 관리자
* 시스템 관리자

이 개선 사항 이전에는 제출된 요청을 편집할 수 없었습니다.

자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## AEM 컨텐츠 조각에 대한 새 미리보기 창

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 5월 14일
>[!BADGE 일정 해제]{type=Neutral}

Workfront Planning 레코드에 연결된 AEM 컨텐츠 조각으로 작업할 때 가시성을 높이기 위해 Workfront Planning의 조각에 대한 정보를 표시하는 미리보기 창을 추가했습니다.

이 기능은 이전에 AEM 에셋에서 사용할 수 있었으며 이제 콘텐츠 조각에 추가되었습니다.

자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

## 이제 조회 필드를 Workfront Planning의 AEM 컨텐츠 조각에 사용할 수 있습니다.

>[!NOTE]
>
>모든 고객을 위한 미리보기 및 프로덕션: 2026년 5월 14일
>Adobe Experience Manager이 있는 Adobe Workfront Planning 고객만 사용할 수 있습니다.
>[!BADGE 일정 해제]{type=Neutral}

이제 Planning 레코드 유형을 AEM 컨텐츠 조각에 연결할 때 다음 조회 필드를 추가할 수 있습니다.

* 생성한 사람
* 생성된 위치
* 수정한 사람
* 수정된 위치

이 개선 이전에는 조회 필드를 AEM 에셋 및 폴더에만 사용할 수 있었습니다.

자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.



## 레코드의 세부 정보 페이지에 대한 사용자 지정 보기

>[!NOTE]
>
>미리 보기: 2026년 5월 14일
>프로덕션 빠른 릴리스: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

레코드의 세부 정보 페이지에서 정보를 시각화할 수 있는 유연성을 높이기 위해 이 페이지에 대한 사용자 지정 보기를 만드는 기능이 도입되었습니다.

이제 모든 레코드 필드 또는 테이블 보기에 표시되는 필드만 포함하는 이미 빌드된 두 개의 세부 정보 페이지 보기를 추가할 수 있을 뿐만 아니라 레코드의 세부 정보 페이지에 대한 사용자 지정 보기를 만들 수도 있습니다. 만든 보기는 레코드에 액세스할 수 있는 모든 사용자가 볼 수 있습니다.

이 업데이트는 **모든 필드 표시** 설정을 제거하고 사용자 지정 세부 정보 보기로 대체합니다.

자세한 내용은 [레코드 페이지 관리](/help/quicksilver/planning/records/manage-the-record-page.md)를 참조하십시오.

## 프로젝트에 연결된 레코드 페이지에 그룹화 추가

>[!NOTE]
>
>미리 보기: 2026년 5월 14일\
>프로덕션 fast: 2026년 6월 11일
>모두를 위한 프로덕션: 2026년 7월 16일

이제 Workfront Planning에 있는 레코드의 연결된 레코드 프로젝트 페이지에서 정보를 그룹화할 수 있습니다. 이 기능이 향상되기 전에는 이 영역에 존재하지 않았습니다.

자세한 내용은 [목록 보기 관리](/help/quicksilver/planning/views/manage-the-list-view.md)를 참조하십시오.

