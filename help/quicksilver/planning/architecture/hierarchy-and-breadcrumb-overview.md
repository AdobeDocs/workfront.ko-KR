---
title: 계층 구조 및 이동 경로 개요
description: 작업 영역의 레코드 유형 간에 여러 작업 영역 계층을 만들 수 있습니다.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# 계층 구조 및 이동 경로 개요

작업 영역 관리자는 레코드 유형과 Adobe Workfront Planning의 다른 객체 유형 간에 유연하지만 구조화된 계층을 정의할 수 있습니다.

계층은 레코드 유형 간의 연결입니다. 하나의 계층에서 최대 4개의 레코드 및 개체 유형을 연결할 수 있습니다.

계층 만들기에 대한 자세한 내용은 [작업 영역 계층 만들기](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)를 참조하십시오.

작업 공간에서 계층을 사용하면 다음과 같은 이점이 있습니다.

* 팀이 실제로 계획, 운영 및 제공하는 방법을 반영하는 방식으로 작업을 구성합니다.
* 사용자가 현재 위치, 레코드 종류가 연결되는 방식 및 전략의 실행 흐름을 시스템에서 위치를 나타내는 탐색 표시 집합을 참조하여 이해할 수 있도록 합니다.
* 더 나은 탐색을 제공하고 모든 워크플로우에서 명확성과 연속성을 만듭니다.
* 조직의 작동 방식에 맞는 흐름을 정의하여 모든 작업 단계에서 유연성과 일관성을 모두 지원합니다.

## 계층 작업 시 고려 사항

* 작업 영역 관리자는 하나의 작업 영역에 대해 여러 계층을 생성할 수 있습니다.
* 선택한 레코드 유형 간의 연결이 이미 있으면 시스템이 기존 연결을 재사용합니다.
* 연결이 없으면 Workfront에서 계층 설정의 일부로 연결을 자동으로 만듭니다.
* 다음은 계층 설정에 대한 규칙입니다.
   * 레코드 유형은 지정된 작업 영역에서 하나의 상위 레코드 유형만 가질 수 있습니다.

     예를 들어, [전략] 레코드 유형은 동일한 작업 영역에서 상위 레코드 유형으로 캠페인과 목표 레코드 유형을 모두 가질 수 없습니다.
   * 하나의 레코드를 여러 레코드 유형에 연결하거나 여러 레코드 유형을 여러 레코드 유형에 연결하면 같은 유형의 여러 상위 레코드에 연결할 수 있습니다.
예를 들어 전술 A는 캠페인 X와 캠페인 Y 모두에 속할 수 있습니다.
   * 레코드 종류는 여러 하위 레코드 종류에 연결할 수 있습니다.

     예를 들어 캠페인 레코드 유형은 전술, 테스트 및 기타 레코드 유형과 같은 다른 레코드 유형 여러 개에 대한 상위일 수 있습니다.
   * 계층에는 Planning 레코드 유형과 Workfront 객체 유형이 모두 포함될 수 있습니다.

     예를 들어 계획 전술 및 Workfront 프로젝트를 하위 항목으로 사용하는 캠페인 레코드 유형이 있을 수 있습니다.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * 글로벌 레코드 유형은 여러 계층 내의 여러 작업 영역에 나타날 수 있습니다. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Workfront 객체 유형은 여러 계층 및 다른 작업 공간에 표시될 수도 있습니다.
   * 글로벌 레코드 유형은 다른 작업 영역의 계층에 속할 수 없습니다.

     예를 들어 Campaign이 글로벌 레코드 유형이고 Workspace 1에 있는 계층의 일부인 경우 Workspace 2에 기존 레코드 유형으로 추가할 수 있지만 2에서는 계층의 일부가 될 수 없습니다. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * 연결된 레코드 유형에 해당 필드를 만들지 않는 연결이 있는 레코드 유형도 계층의 일부일 수 있습니다. 계층 설정 중에 생성된 새 연결은 기본적으로 연결된 레코드 유형에 해당 필드를 생성합니다.

## 이동 경로를 볼 때 고려 사항

레코드 유형 간에 계층을 만들면 해당 레코드 유형에 속하는 레코드에 대한 이동 경로를 생성합니다.

예를 들어 계층을 만들고 전술 및 프로그램과 캠페인, 프로젝트 순으로 연결한 경우 계층에 연결된 유형의 레코드로 이동하면 레코드가 배치된 위치를 계층 구조에서 볼 수 있습니다.

다음 사항을 고려하십시오.

* 레코드 유형이 여러 작업 공간의 여러 계층에 속하는 경우 레코드 페이지의 레코드 이동 경로에서 계층 간을 전환할 수 있습니다.
* 이동 경로는 Workfront 및 Planning에서 작동합니다.

  예를 들어 Planning 캠페인 및 전술, Workfront 포트폴리오 및 프로그램에도 연결된 프로젝트를 볼 때 이동 경로에서 Planning 및 Workfront 계층 간에 전환할 수 있습니다.

  자세한 내용은 [작업 영역 계층 만들기](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)를 참조하십시오.


