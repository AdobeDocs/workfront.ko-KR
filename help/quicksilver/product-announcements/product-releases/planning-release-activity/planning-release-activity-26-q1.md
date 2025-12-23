---
content-type: release-notes
title: Adobe Workfront Planning의 2026년 1분기 릴리스 활동
description: 2026년 1분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: d956671b535d5c7a11d0fb17dc003a665a4f0597
workflow-type: tm+mt
source-wordcount: '1798'
ht-degree: 0%

---

# Adobe Workfront Planning의 2026년 1분기 릴리스 활동

이 문서에서는 2026년 1분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록을 보려면 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.

## 작업 영역에서 레코드 유형 계층 만들기

>[!NOTE]
>
>미리 보기: 2025년 12월 23일
>프로덕션 빠른 릴리스: 2026년 1월 14일
>모두를 위한 프로덕션: 2026년 1월 15일

이제 레코드 또는 개체 유형 간에 유연하지만 구조화된 계층을 정의할 수 있습니다.

계층은 레코드 유형 간의 연결입니다. 하나의 계층에서 최대 4개의 레코드 및 객체 유형을 연결할 수 있으며, 하나의 작업 영역에서 최대 5개의 계층을 사용할 수 있습니다. 계층의 첫 번째 레코드 유형은 첫 번째 부모입니다.

계층을 사용하여 작업을 구성하고 전략이 어떻게 실행되는지 시각화할 수 있습니다.

계층을 작성할 때 다음 사항을 고려하십시오.

* 계층 구조의 한 작업 영역과 Workfront 프로젝트에서 Planning 레코드 유형만 연결할 수 있습니다.
* 레코드 종류 또는 프로젝트는 동일한 작업 영역에서 하나의 상위 항목만 가질 수 있습니다.
* 레코드 유형은 여러 계층의 상위 유형이 될 수 있습니다.
* 연결 가능한 레코드 종류는 해당 작업 영역 이외의 작업 영역의 계층에서 사용할 수 없습니다.
* 글로벌 레코드 유형은 해당 유형이 생성되었거나 추가된 작업 영역에서만 계층에서 사용할 수 있습니다.

자세한 내용은 [계층 구조 및 이동 경로 개요](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)를 참조하십시오.

## 새 통합 이동 경로가 레코드 페이지에 추가됨

>[!NOTE]
>
>미리 보기: 2025년 12월 23일
>프로덕션 빠른 릴리스: 2026년 1월 14일
>모두를 위한 프로덕션: 2026년 1월 15일

레코드 유형 간에 계층을 만들면 해당 레코드 유형에 속하는 레코드에 대한 이동 경로를 생성합니다.

레코드 경로는 계층 구조에서 위치를 반영합니다. 계층을 만든 후에는 다른 상위 또는 하위 개체가 연결되는 것을 나타내는 레코드의 이동 경로를 페이지 맨 위에 볼 수 있습니다. 계층은 Workfront 및 Planning에서 일관됩니다.

예를 들어 프로젝트의 Planning 계층 구조가 Planning 경로에서 Planning 레코드 유형에 연결되어 있는 경우 Planning 계층을 보고, Workfront에서 포트폴리오 또는 프로그램과 같은 Workfront 객체 유형에 연결되어 있는 경우 해당 Workfront 계층을 볼 수 있습니다.

자세한 내용은 [계층 구조 및 이동 경로 개요](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)를 참조하십시오.


## 연결된 레코드 페이지 개선 사항

>[!NOTE]
>
>미리 보기: 2025년 12월 19일
>프로덕션 빠른 시간: 2026년 1월 14일
>모두를 위한 프로덕션: 2026년 1월 15일

연결된 레코드 페이지로 작업할 때 보다 유연하게 사용할 수 있도록 이 Workfront Planning 영역에서 보기 기능을 개선했습니다. 다음은 레코드의 연결된 레코드 페이지에서 향상된 기능입니다.

* 이제 레코드의 연결된 레코드 페이지에 타임라인 및 달력 보기를 추가할 수 있습니다.
* 이제 연결된 레코드 페이지에서 모든 보기를 공유할 수 있습니다. 이러한 페이지에서 공유되는 보기는 Workfront Planning의 다른 영역에서 공유하는 모든 사용자가 시스템 전체에 볼 수 있습니다. Planning의 다른 영역에서 공유되는 모든 보기는 공유된 동일한 사용자에 대해 연결된 레코드 페이지에도 표시됩니다.
* 각 레코드 또는 개체 유형당 연결된 레코드 페이지를 하나만 허용하는 제한 사항을 추가했습니다. 이 개선 이전에는 동일한 레코드 또는 개체 유형에 대해 여러 페이지를 추가할 수 있었습니다. 이제 연결된 하나의 레코드 페이지에서 동일한 레코드 종류에 대해 여러 보기를 사용할 수 있습니다.
* 테이블 보기의 맨 아래에 **새 행** 링크가 추가되었으며 연결된 레코드 페이지의 오른쪽 상단에 **레코드 연결** 단추가 있습니다. 개선 전에는 **새 행** 링크 및 **레코드 연결** 단추가 프로젝트에 연결된 페이지에만 있었습니다.

자세한 내용은 [레코드에 연결된 레코드 페이지 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.

## 연결된 레코드 프로젝트 페이지에서 보기 공유

>[!NOTE]
>
>미리 보기: 2025년 12월 18일
>프로덕션 빠른 릴리스: 2026년 1월 14일\
>모두를 위한 프로덕션: 2026년 1월 15일

필요한 정보를 더 쉽게 볼 수 있도록 프로젝트 연결 레코드 페이지에 보기를 공유하는 기능을 추가했습니다. 이제 다른 사용자, 팀 또는 그룹과 보기를 공유할 수 있습니다.

자세한 내용은 [레코드에 연결된 레코드 페이지 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.

## 현재 사용자 와일드카드를 프로젝트 연결 보기 필터에서 사용할 수 있음

>[!NOTE]
>
>미리 보기: 2025년 12월 18일
>프로덕션 빠른 릴리스: 2026년 1월 14일\
>모두를 위한 프로덕션: 2026년 1월 15일

사용자에게 적용되는 프로젝트 연결을 더 쉽게 필터링할 수 있도록 현재 사용자 와일드카드를 만들었습니다. 이제 필터링할 때 &quot;나(로그인한 사용자)&quot;를 선택할 수 있습니다. 그런 다음 필터는 요청 목록을 보고 있는 사용자에게 적용됩니다.

여러 사용자가 사용할 보기에 필터를 추가할 때 편리할 수 있습니다. 각 사용자에게 적용되는 필터 결과가 표시됩니다.

와일드카드는 값이 사용자인 필드에서 사용할 수 있습니다.

필터를 포함하여 프로젝트 연결 보기 구성에 대한 자세한 내용은 [레코드에 연결된 레코드 추가](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)를 참조하십시오.


## Workspace 기본 페이지 개선 사항

>[!NOTE]
>
>미리 보기: 2025년 12월 18일
>프로덕션 빠른 시간: 2026년 1월 14일
>모두를 위한 프로덕션: 2026년 1월 15일

Workfront Planning의 Workspaces 기본 페이지에 대해 다음과 같이 개선했습니다.

* 더욱 빠르고 동적인 스크롤 환경. 이는 조직에 많은 작업 공간이 있고 시스템 관리자를 위한 경우 특히 표시됩니다.

* 이제 이름별로 특정 작업 영역을 검색할 수 있는 검색 상자를 추가했습니다.

* **다른 작업 영역** 탭의 이름이 **모든 작업 영역**(으)로 변경되었으며 사용자가 만든 작업 영역을 포함하여 볼 수 있는 권한 이상이 있는 모든 작업 영역이 포함됩니다.

자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.


## GenStudio 작업 영역에서 기본적으로 제품 및 성향에 브랜드 연결 필드 추가

>[!NOTE]
>
>미리 보기: 2025년 12월 11일
>프로덕션 빠른 릴리스: 2025년 12월 11일
>모두를 위한 프로덕션: 2025년 12월 11일
>[!BADGE 일정 해제]{type=Neutral}

이제 GenStudio for Performance Marketing Brand와의 연결 필드가 Workfront Planning의 GenStudio 작업 영역에서 제품 및 가상 사용자 레코드 유형에 기본적으로 추가됩니다.

조직에 Workfront Planning과 Adobe GenStudio for Performance Marketing이 모두 있어야 합니다.

이 개선 이전에는 Brand Connection 필드를 제품 및 가상 사용자를 비롯한 모든 레코드 유형에 수동으로만 추가할 수 있었습니다. Brand GenStudio 레코드 유형을 Workfront Planning의 다른 레코드 유형에 수동으로 연결할 수 있습니다.

자세한 내용은 [Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.

## Planning에서 GenStudio for Performance Marketing 사용자의 권한 제거 제한

>[!NOTE]
>
>미리 보기: 2025년 12월 11일
>프로덕션 빠른 릴리스: 2025년 12월 11일
>모두를 위한 프로덕션: 2025년 12월 11일
>[!BADGE 일정 해제]{type=Neutral}

Workfront Planning 오브젝트에서 GenStudio for Performance Marketing 사용자의 권한을 제거할 수 없도록 하는 가드레일을 추가했습니다. 이러한 개선 사항으로 인해 Planning의 GenStudio 작업 영역에서 GenStudio 사용자를 더 이상 제거할 수 없으며, GenStudio 작업 영역의 레코드 유형에 GenStudio 사용자가 포함된 경우 해당 레코드 유형에 대해 상속된 권한을 비활성화할 수 없습니다. 이 개선 전에 Planning의 GenStudio 작업 영역에서 이러한 사용자를 제거하면 GenStudio의 레코드 유형에도 대한 권한이 상실됩니다.

조직에 Workfront Planning과 Adobe GenStudio for Performance Marketing이 모두 있어야 합니다.

자세한 내용은 [Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.


## 보조 작업 영역에서 글로벌 레코드 유형에 대한 보기의 공개 공유가 제거됨


>[!NOTE]
>
>미리 보기: 2025년 12월 3일
>프로덕션 빠른 릴리스: 2025년 12월 4일
>모두를 위한 프로덕션: 2026년 1월 15일


보조 작업 공간에서 글로벌 레코드에 대한 보기를 공유할 때 공개 공유 탭을 제거했습니다. 기존 글로벌 레코드 유형에서 다른 작업 영역에 추가된 글로벌 레코드 유형에서는 보기를 공개적으로 공유할 수 없습니다. 원래 작업 영역에서 글로벌 레코드 유형 보기를 공개적으로 공유할 수 있습니다.

자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.


## GenStudio for Performance Marketing 브랜드와 Workfront Planning 레코드 유형 연결

>[!NOTE]
>
>미리 보기: 2025년 11월 13일
>프로덕션 빠른 릴리스: 2025년 11월 13일
>모두를 위한 프로덕션: 2025년 11월 13일

이제 Workfront Planning 레코드 유형을 Adobe GenStudio for Performance Marketing의 브랜드와 연결할 수 있습니다. 조직에 Workfront Planning과 Adobe GenStudio for Performance Marketing이 모두 있어야 합니다.

자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.


## Planning 보기의 필터, 필드 및 행 색상 아이콘에서 새 필드 검색 상자

>[!NOTE]
>
>미리 보기: 2025년 11월 6일
>프로덕션 빠른 릴리스: 2025년 12월 11일
>모두를 위한 프로덕션: 2026년 1월 15일

이제 레코드 유형 보기에서 보기 요소를 작성할 때 특정 필드를 검색할 수 있습니다. 필터, 정렬, 그룹화하거나 필드 또는 행 색상을 구성할 때 검색 상자를 추가했습니다. 이 기능이 향상되기 전에는 사용 가능한 필드 목록을 스크롤하기만 하면 됩니다.

이 개선 사항은 모든 레코드 유형 보기에서 사용할 수 있습니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.


## 글로벌 레코드 유형 및 이를 다른 작업 공간에 기존 레코드 유형으로 추가하는 기능

>[!NOTE]
>
>미리 보기: 2025년 10월 16일
>프로덕션 빠른 릴리스: 2025년 11월 13일
>모두를 위한 프로덕션: 2026년 1월 15일

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
>프로덕션 빠른 릴리스: 2025년 11월 13일
>모두를 위한 프로덕션: 2026년 1월 15일

각 레코드 유형에 대해 30개의 연결 필드 제한을 도입했습니다.

참고: 현재 조직에 하나의 레코드 종류에 대해 30개가 넘는 연결 필드가 있는 경우 30개를 초과하는 추가 필드를 유지할 수 있습니다. 그러나 한도를 초과하는 레코드 유형에는 더 많은 연결 필드를 추가할 수 없습니다. 앞으로 30개의 연결 필드에 대한 새로운 제한이 적용됩니다.

자세한 내용은 [연결된 레코드 종류 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하십시오.

## 선택 유형 필드 선택 사항에 대해 사용자에게 친숙한 값 설정

>[!NOTE]
>
>미리 보기: 2025년 10월 16일
>프로덕션 빠른 릴리스: 2025년 11월 13일
>모두를 위한 프로덕션: 2026년 1월 15일

단일 또는 다중 선택 필드에 필드 선택 사항을 추가하면 Workfront은 이제 각 선택 사항에 사용자에게 친숙한 고유한 값을 할당합니다. 이 개선 전에 Workfront에서는 API 호출 및 기타 통합에서 이해하고 사용하기 어려운 영숫자 ID를 생성했습니다.

이 개선 사항을 통해 다음 사항을 고려하십시오.

* 새 값이 새 필드 선택 사항에 추가됩니다. 기존 필드 선택 사항은 영숫자 ID를 유지합니다.

* 선택 값은 한 필드에 대해 고유하지만 다른 필드 간에 반복될 수 있습니다.

* 선택 항목의 이름을 변경해도 원래 값이 업데이트되지 않습니다.

* 선택 값은 소문자로 표시되며, 여러 단어 선택의 경우 밑줄로 구분됩니다. 동일한 필드에 다른 선택 이름으로 이미 사용된 레이블을 사용하는 경우 Workfront이 값에 순차적 번호를 추가합니다.

자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.






