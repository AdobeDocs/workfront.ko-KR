---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 개요
description: Blueprint는 기본 구성 요소를 제공하므로 고객과 함께 성장하는 작업 관리 시스템을 만들 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# 블루프린트 개요

Blueprint는 기본 구성 요소를 제공하므로 고객과 함께 성장하는 작업 관리 시스템을 만들 수 있습니다. 시스템 관리자는 Blueprint 카탈로그를 탐색하고 사용 가능한 프로젝트 템플릿을 설치할 수 있습니다. 다른 사용자는 카탈로그를 탐색하고 블루프린트 설치를 요청할 수 있습니다. 자세한 내용은 [블루프린트 카탈로그를 찾아보고 블루프린트 설치를 요청합니다](../../administration-and-setup/blueprints/browse-catalog.md).

각 블루프린트는 시스템에서 검증된 Best Practice를 신속하게 구현할 수 있도록 부서 및 특정 성숙도 수준을 대상으로 합니다. 아래 자세히 설명된 성숙도 수준은 블루프린트 카탈로그 카드 및 세부 정보에 표시됩니다.

**[!UICONTROL 관리]:** 관리 프로젝트 템플릿을 통해 활동 및 결과물을 표준 절차로서 완전히 수용하기 전에 새로운 비즈니스 프로세스를 채택할 수 있습니다. 여기에는 새 프로세스의 각 단계가 수행되도록 하는 작업이 포함됩니다.

**[!UICONTROL 통합]:** 통합 프로젝트 템플릿은 표준 운영 절차를 통해 비즈니스 기능이 지원된다고 가정합니다. 프로세스 기여자는 프로세스를 따르기 위해 완료해야 하는 단계 및 작업을 알고 있습니다. 이 프로세스를 지원하는 프로젝트 템플릿에는 보고 목적으로 필요한 이정표 및 기타 주요 결과물만 추적하는 작업이 거의 없습니다.

## 적합한 블루프린트 찾기

사용 사례, 만기 수준, 설치 상태별로 청사진을 찾아보고 카탈로그의 오른쪽에 있는 필터와 함께 입력할 수 있습니다. 관심 있는 블루프린트를 찾으면 세부 사항 페이지에서 세부 사항을 볼 수 있습니다.

### 블루프린트 유형

블루프린트 유형은 블루프린트에 포함된 사항을 보여줍니다. 유형이 카탈로그의 블루프린트 카드 하단에 나열됩니다. 블루프린트는 두 개 이상의 유형을 가질 수 있습니다.

다음 유형의 청사진을 사용할 수 있습니다.

* 프로젝트 템플릿: 프로젝트 템플릿과 연관된 표준 객체(작업, 문제, 역할 및 팀)와 해당 객체와 관련된 일부 기본 설정을 포함합니다. 자세한 내용은 [블루프린트 구성](../../administration-and-setup/blueprints/configure-template-package.md).
* 조직 구조: 조직의 구조와 연관된 객체(회사, 그룹, 역할 및 팀)를 포함합니다. 자세한 내용은 [블루프린트 구성](../../administration-and-setup/blueprints/configure-template-package.md).
* 대시보드: 구현 서비스와 같은 특정 사용 사례에 대해 하나 이상의 대시보드를 포함합니다.

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

현재 청사진을 검토하려면 다음을 참조하십시오 [사용 가능한 블루프린트 목록](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

###  세부 사항 보기

각 블루프린트에는 세부 사항 페이지가 포함되어 있습니다. 이 페이지에서 다음을 수행할 수 있습니다.

* 워크플로우 컨텐츠 요약 보기
* 블루프린트에 대한 간단한 요약 읽기
* 설치 기록 보기(클릭) **[!UICONTROL 자세한 내용은]** 블루프린트와 함께 설치된 개체의 전체 목록을 보려면
* 역할, 팀, 회사 및 그룹 설명 참조
* 프로젝트 템플릿과 같은 특정 블루프린트의 시각적 예를 참조하십시오(브라우저에서 전체 이미지를 미리 보거나 다운로드할 수 있음)

![[!UICONTROL 블루프린트 세부 사항] 페이지](assets/blueprint-details-page-2022.png)

## 블루프린트 설치

시스템 관리자는 프로덕션 환경 또는 샌드박스 환경에 직접 설치할 수 있습니다. 자세한 내용은 [블루프린트 설치](../../administration-and-setup/blueprints/blueprints-install.md) 또는 [블루프린트 구성](../../administration-and-setup/blueprints/configure-template-package.md).

설치 후 수행할 다음 작업에 대해 잘 모를 수 있습니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## 블루프린트 및 템플릿에 대한 추가 참고 사항

블루프린트는 의 프로젝트 템플릿 기능을 대체하지 않습니다 [!DNL Adobe Workfront]. 블루프린트는 새 템플릿을 더 빨리 만들어 보다 많은 작업을 에서 구성할 수 있는 방법입니다 [!DNL Workfront].

블루프린트를 복사하거나 편집할 수 없습니다. 그러나 블루프린트에서 솔루션을 설치하면 일반적인 방법으로 블루프린트에서 해당 레코드를 업데이트하는 것과 동일한 방식으로 프로젝트 템플릿, 작업 역할 또는 팀이 수정됩니다 [!DNL Workfront] 인터페이스. 또한 블루프린트를 설치하면 템플릿이 [!UICONTROL 템플릿] 영역 [!DNL Workfront] 원래 청사진은 [!UICONTROL 블루프린트] 영역. 필요에 따라 템플릿을 조정하기 전에 템플릿의 사본을 만들 필요가 없습니다.

블루프린트는 환경에 구성된 내용을 제거하거나 대체하지 않습니다. 새 템플릿을 만드는 블루프린트를 설치하여 기존 템플릿을 대체하려는 경우 템플릿에서 프로젝트를 작성하는 플래너 간의 혼동을 방지하기 위해 이전 버전을 비활성화하는 것이 좋습니다.
