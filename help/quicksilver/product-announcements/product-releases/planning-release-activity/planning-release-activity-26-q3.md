---
content-type: release-notes
title: Adobe Workfront Planning의 2026년 3분기 릴리스 활동
description: 2026년 3분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 12552dfefc58a664c278598496097f1b30d3cf0e
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---

# Adobe Workfront Planning의 2026년 3분기 릴리스 활동

<!--take the next sentence out when we start listing features-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

이 문서에서는 2026년 3분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록을 보려면 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Workfront Planning API 버전 2

>[!NOTE]
>
>모든 고객이 사용 가능: 2026년 5월 28일>[!BADGE 일정 해제]{type=Neutral}

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
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

이제 개별 레코드 권한을 조정하여 레코드 종류 내에서 관리할 수 있는 사용자를 제어할 수 있습니다.

사용자는 기본적으로 작업 영역 및 레코드 유형에서 레코드 권한을 상속합니다. 레코드 유형 권한이 있는 선택 사용자만 특정 레코드에만 권한을 관리하려면 선택 레코드에 대해 상속된 권한을 비활성화하고 해당 사용자만 해당 레코드에 대한 관리 액세스 권한을 부여할 수 있습니다. 하나의 레코드에 대한 권한 또는 여러 레코드에 대한 권한을 동시에 일괄 조정할 수 있습니다.

사용자에게 다음과 같은 권한 수준을 부여할 수 있습니다.

* 보기
* 관리

>[!NOTE]
>
>* 사용자의 레코드 수준 권한은 해당 레코드 유형 권한을 초과할 수 없습니다. 예를 들어 레코드 유형에 대한 보기 액세스 권한이 있는 사용자에게 해당 유형의 개별 레코드에 대한 관리 액세스 권한을 부여할 수 없습니다.
>* 현재 레코드에서 사용자의 권한을 제거할 수 없습니다. 레코드 종류에 대해 적어도 보기 액세스 권한이 있는 모든 사용자는 해당 형식의 모든 레코드를 볼 수 있습니다.

자세한 내용은 [레코드 공유](/help/quicksilver/planning/access/share-records.md)를 참조하세요.

## 간소화된 글로벌 레코드 유형 추가

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

클릭을 줄이고 필요한 레코드 유형을 빠르게 찾을 수 있도록 글로벌 레코드 유형을 다른 작업 공간에 추가할 때 더 빠르고 직관적으로 사용할 수 있도록 레코드를 추가할 수 있는 환경을 개선했습니다.

기존 레코드 유형에서 레코드를 추가하도록 선택하면 이제 사용 가능한 모든 글로벌 레코드 유형 목록이 즉시 표시됩니다.

이 화면에서 직접 하나 이상의 글로벌 레코드 유형을 선택하고 동시에 추가할 수 있습니다.

자세한 내용은 [다른 작업 영역에서 기존 레코드 형식 추가](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)를 참조하십시오.


## Planning에서 AEM Assets으로 메타데이터 동기화

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 5월 28일>모두를 위한 프로덕션: 2026년 5월 28일>[!BADGE 일정 해제]{type=Neutral}

데이터 무결성을 향상시키기 위해 GenStudio for Performance Marketing이 Workfront Planning에서 GenStudio 레코드 유형에 연결되어 있을 때 AEM Assets 레코드 유형과 AEM Assets 간에 매끄러운 메타데이터 동기화를 릴리스했습니다.

AEM Assets에 연결할 수 있는 GenStudio for Performance Marketing 레코드 유형은 Campaign, Product, Persona, Region 및 Channel입니다.

Workfront Planning에서 GenStudio 레코드 유형에 추가된 정보는 AEM에 있는 AEM 자산의 개별 캠페인 탭에 표시됩니다. 해당 캠페인에 대한 제품, 사용자, 지역 및 채널에 대한 정보도 읽기 전용 모드로 해당 탭에 표시됩니다.

이번 릴리스를 통해 주요 메타데이터는 두 플랫폼 모두에서 일관되며 실시간에 가까운 업데이트를 반영하므로 수동 조정이 줄어듭니다.

자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.

## Planning에서 AEM 컨텐츠 조각으로 메타데이터 동기화

>[!NOTE]
>
>미리 보기: 2026년 5월 28일>프로덕션 빠른 릴리스: 2026년 5월 28일>모두를 위한 프로덕션: 2026년 5월 28일>[!BADGE 일정 해제]{type=Neutral}

데이터 무결성을 향상시키기 위해 컨텐츠 조각이 GenStudio for Performance Marketing 캠페인에 연결될 때 GenStudio 작업 영역의 Planning 레코드 유형과 AEM 컨텐츠 조각 간의 매끄러운 메타데이터 동기화를 릴리스했습니다.

이제 GenStudio 캠페인 정보가 AEM에 있는 콘텐츠 조각의 메타데이터 탭에 표시됩니다.  해당 캠페인에 대한 제품, 사용자, 지역 및 채널에 대한 정보도 읽기 전용 모드로 해당 탭에 표시됩니다.

이번 릴리스를 통해 주요 메타데이터는 두 플랫폼 모두에서 일관되며 실시간에 가까운 업데이트를 반영하므로 수동 조정이 줄어듭니다.

자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.


## 목록 보기 업데이트

>[!NOTE]
>
>미리 보기: 2026년 5월 27일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

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
>미리 보기: 2026년 5월 27일>프로덕션 빠른 릴리스: 2026년 6월 11일\
>모두를 위한 프로덕션: 2026년 7월 16일

이제 Planning 레코드 유형을 Workfront 개체 유형으로 연결할 때 Workfront 참조 필드를 조회 필드로 추가할 수 있습니다.

예를 들어 프로젝트 객체의 Portfolio, 프로그램, 그룹 또는 회사 정보를 Planning에서 캠페인의 프로젝트 연결 필드에 추가할 수 있습니다.

자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 타임라인 보기 분류 기능에 대한 새 필터

>[!NOTE]
>
>미리 보기: 2026년 5월 27일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

이제 레코드 분류에 포함된 개체와 일치하는 조건을 기준으로 타임라인 보기에서 정보를 필터링할 수 있습니다.

이 개선 이전에는 타임라인 보기의 기본 레코드에 대한 필터만 적용할 수 있었습니다.

자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

## 편집되고 삭제된 필드가 요청 양식에 영향을 준다는 새로운 표시

>[!NOTE]
>
>미리 보기: 2026년 5월 27일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

편집하거나 삭제하는 레코드 필드가 해당 필드를 포함하는 요청 양식에 영향을 줄 수 있다는 미리 알림을 추가했습니다. 이제 영향을 받는 양식을 검토하고 필드에 적용할 변경 사항이 기존 정보에 영향을 주지 않는지 확인할 수 있습니다.

자세한 내용은 [필드 설정 편집](/help/quicksilver/planning/fields/edit-fields.md)을 참조하세요.

## 제출된 Planning 요청 편집

>[!NOTE]
>
>미리 보기: 2026년 5월 27일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

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
>미리 보기: 2026년 5월 14일>프로덕션 빠른 릴리스: 2026년 5월 14일>모두를 위한 프로덕션: 2026년 5월 14일>[!BADGE 일정 해제]{type=Neutral}

Workfront Planning 레코드에 연결된 AEM 컨텐츠 조각으로 작업할 때 가시성을 높이기 위해 Workfront Planning의 조각에 대한 정보를 표시하는 미리보기 창을 추가했습니다.

이 기능은 이전에 AEM 에셋에서 사용할 수 있었으며 이제 콘텐츠 조각에 추가되었습니다.

자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

## 이제 조회 필드를 Workfront Planning의 AEM 컨텐츠 조각에 사용할 수 있습니다.

>[!NOTE]
>
>미리 보기: 2026년 5월 14일>프로덕션 빠른 릴리스: 2026년 5월 14일>모두를 위한 프로덕션: 2026년 5월 14일>[!BADGE 일정 해제]{type=Neutral}

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
>미리 보기: 2026년 5월 14일>프로덕션 빠른 릴리스: 2026년 6월 11일>모두를 위한 프로덕션: 2026년 7월 16일

레코드의 세부 정보 페이지에서 정보를 시각화할 수 있는 유연성을 높이기 위해 이 페이지에 대한 사용자 지정 보기를 만드는 기능이 도입되었습니다.

이제 모든 레코드 필드 또는 테이블 보기에 표시되는 필드만 포함하는 이미 빌드된 두 개의 세부 정보 페이지 보기를 추가할 수 있을 뿐만 아니라 레코드의 세부 정보 페이지에 대한 사용자 지정 보기를 만들 수도 있습니다. 만든 보기는 레코드에 액세스할 수 있는 모든 사용자가 볼 수 있습니다.

이 업데이트는 **모든 필드 표시** 설정을 제거하고 사용자 지정 세부 정보 보기로 대체합니다.

자세한 내용은 [레코드 페이지 관리](/help/quicksilver/planning/records/manage-the-record-page.md)를 참조하십시오.

## 프로젝트에 연결된 레코드 페이지에 그룹화 추가

>[!NOTE]
>
>미리 보기: 2026년 5월 14일\
>제작 속도: 2026년 6월 11일>모두를 위한 제작: 2026년 7월 16일

이제 Workfront Planning에 있는 레코드의 연결된 레코드 프로젝트 페이지에서 정보를 그룹화할 수 있습니다. 이 기능이 향상되기 전에는 이 영역에 존재하지 않았습니다.

자세한 내용은 [목록 보기 관리](/help/quicksilver/planning/views/manage-the-list-view.md)를 참조하십시오.
