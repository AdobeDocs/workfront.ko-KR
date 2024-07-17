---
title: 'Adobe Workfront 계획 모범 사례'
description: 마케팅 운영 리더로서 Adobe Workfront Planning을 사용하여 모든 팀의 마케팅 라이프사이클 전반에서 작업을 구성할 수 있습니다. 다음은 Workfront Planning을 시작할 때 권장하는 몇 가지 모범 사례입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Adobe Workfront 계획 모범 사례

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

마케팅 운영 리더로서 Adobe Workfront Planning을 사용하여 모든 팀의 마케팅 라이프사이클 전반에서 작업을 구성할 수 있습니다.

이 문서에서는 Workfront Planning을 시작할 때 권장하는 몇 가지 모범 사례를 문서화합니다.

## Workfront 계획이란?

Workfront Planning 모듈은 서로 다르지만 연결되어 있는 세 가지 Workfront 기능 중 하나로, 함께 기록 마케팅 시스템을 만듭니다. 세 가지 기능은 다음과 같습니다.

* **계획**: Workfront 계획에 포함된 새로운 고급 기능입니다.

* **워크플로**: 현재 Workfront에서 사용하는 공동 작업 관리 기능(프로젝트 관리, 리소스 관리 등)

* **자동화 및 통합**: Workfront Fusion에서 제공하는 포괄적인 통합 및 자동화 기능입니다.

Workfront Planning은 사용자 정의가 용이합니다. Workfront Planning 용어 및 주요 개념에 대한 자세한 내용은 [Adobe Workfront Planning 개요](/help/quicksilver/planning/general/planning-overview.md)를 참조하십시오.

## Workfront Planning을 설정하기 전에 해야 할 질문

Workfront Planning 용어 및 아키텍처를 숙지한 후에는 새 환경 설정을 시작할 수 있습니다.

Planning을 설정할 때 자문할 수 있는 질문은 다음과 같습니다.

* **더 큰 조직 그룹에 작업 영역을 사용하시겠습니까? 아니면 사람들이 개인 항목을 설정하도록 권장해야 합니까?**

  여러분은 두 가지 모두에 좋은 사용이 있다는 것을 알게 될 것이다. 작업 영역이 너무 많으면 관리하기 어려워지고 워크플로우가 너무 많이 조각날 수 있으므로 사용하지 않는 것이 좋습니다.

  >[!TIP]
  >
  >    하나의 Workfront 인스턴스에 1,000개의 작업 공간이 있을 수 있습니다.

* **각 작업 영역에서 어떤 사용자 지정 레코드 유형을 만들어야 합니까?**

  레코드 유형은 Workfront의 오브젝트 유형과 같습니다. 워크플로우에 대해 생각하고 어떤 레코드 유형(작업 오브젝트, 사람 오브젝트, 분류 등)을 결정하십시오. 각 워크플로우에는 다음이 필요할 수 있습니다.

  자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

* **어떻게 레코드를 만들 수 있습니까? Planning에 추가해야 하는 레코드가 이미 포함된 외부 목록 또는 스프레드시트가 사용 가능합니까? 필요에 따라 레코드가 점차적으로 추가됩니까? 또는 Fusion 또는 사용자 지정 API 통합을 사용하여 가져오시겠습니까?**

  자세한 내용은 다음을 참조하십시오.

   * [레코드 만들기](/help/quicksilver/planning/records/create-records.md)
   * [Adobe Workfront Planning 모듈](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **레코드에 대해 어떤 필드를 만들어야 합니까?**

  자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

* **종속성을 표시하고 조직에 대한 원활한 워크플로를 만들기 위해 Workfront Planning 레코드 유형에 연결하는 데 필요한 Workfront 또는 AEM Assets 개체 유형은 무엇입니까?**

  자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

* **캠페인 스토리를 전달하는 데 필요한 마케팅 일정 및 보기는 무엇입니까? 원활한 공동 작업을 위해 이러한 보기를 사용할 수 있는 이해 당사자는 무엇입니까?**

  자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.


## Workfront 계획 모범 사례

이 섹션에는 Workfront Planning을 설정할 때의 몇 가지 작업 및 금지 사항, 모범 사례 지침이 나와 있습니다.

설정하는 객체나 영역에 따라 지침이 구성됩니다.

### 작업 영역

#### 작업 영역의 할 일과 할 일

* 조직 수준의 작업 공간 중 가장 낮은 볼륨을 위한 설계

  예를 들어 모든 마케팅에 대해 하나의 Workspace을 만들어 봅니다

* 정기적으로 작업 공간을 조정하십시오. 처음부터 새로 빌드하는 대신 기존 빌드를 수정할 수 있습니다.

* 운영 방식이 완전히 다른 팀을 위해 새 Workspace을 만들어야 합니다.

  &quot;제품 개발&quot; 작업 영역은 &quot;마케팅&quot; 작업 영역과 구별되어야 합니다

* 모든 사소한 것에 대해 고유한 작업 영역을 만들지 마십시오. 작업 공간은 조직 전체에 도움이 될 수 있고 개인 요청을 추적하는 개인 공간이 아닌 모든 사람이 워크플로우를 매핑하고 공동 작업을 수행할 수 있는 기록 시스템으로 생각하십시오.

* 조직 내의 각 팀 또는 프로세스에 대해 고유한 작업 영역을 만들지 마십시오.

  마케팅 조직은 가시성을 유지하고 글로벌 계획 수준에서 데이터를 롤업할 수 있도록 한 개의 작업 영역만 유지 관리하도록 노력해야 합니다.

  유사한 프로세스를 따르는 팀(예: EMEA 마케팅 및 APAC 마케팅)에 대해, 특히 이러한 팀이 일반적인 전략 캠페인으로 롤업하는 작업을 수행할 수 있는 유사 또는 중복 작업 영역을 만들지 마십시오.

#### 작업 영역 섹션은 어떻게 사용해야 합니까?

* 사용자가 운영 라이프사이클을 구성하는 방법을 이해하는 데 도움이 되는 섹션을 만들고 레이블을 지정합니다.

  예를 들어 캠페인, 전술 및 결과물을 배치하는 &quot;핵심 레코드&quot;라는 섹션을 만들 수 있습니다.

* &quot;좋아요&quot; 레코드 유형을 함께 그룹화합니다.

  지역, 국가 및 도시와 같은 레코드 유형을 포함하는 &quot;지역&quot;이라는 섹션을 만들 수 있습니다.

#### 작업 공간 권한을 관리하려면 어떻게 해야 합니까?

* 레코드 종류를 실수로 삭제하거나 불필요한 레코드 종류 및 필드를 만들지 않는 신뢰할 수 있는 사용자 그룹의 선택에 대한 액세스를 &quot;관리&quot;로 제한하지 마십시오.

  >[!TIP]
  >
  >Beta 프로그램 중에 많은 고객이 그룹 관리자에게 &quot;관리&quot; 액세스 권한을 부여할 것으로 생각한다는 사실을 알게 되었습니다.

* Standard 라이선스를 가진 사용자의 레이아웃 템플릿에 계획 영역을 추가하지 마십시오.

* 표준 라이선스가 있는 사용자가 개인 작업 공간을 만들 수 있도록 허용합니다. 이것은 그들에게 도구를 배우고 편안해질 수 있는 안전한 공간을 제공합니다. 이는 타인을 위한 경험을 어지럽히지 않으며 사용자의 개인 생산성을 향상시킬 수 있다.

  >[!TIP]
  >
  >    개인 작업 영역을 공유하지 않는 것이 좋습니다.


### 레코드 유형

#### 단일 또는 다중 선택 필드와 연결된 레코드 유형 비교

* 개체가 다른 여러 레코드 유형에서 사용될 경우 새 레코드 유형을 작성하십시오.

  예를 들어, 캠페인은 여러 Target 대상에 연결되어 있을 수 있으며, 전술은 단일 Target 대상에 연결되어 있을 수 있습니다.

* 개체를 조회할 때 유용할 수 있는 추가 메타데이터 값을 저장해야 하는 경우 새 레코드 유형을 작성하십시오.

  예를 들어 &quot;이메일&quot;과 같은 채널 레코드 유형에는 기본 메타데이터나 독립 실행형 &quot;결과물&quot; 레코드 유형에 대한 연결로서 지원 결과물 목록이 저장될 수 있습니다.

* 저장하는 데이터의 범위를 단일 레코드 종류로만 지정해야 하는 경우에는 새 레코드 종류를 추가하지 마십시오. 대신 선택 필드를 사용하십시오.

  예를 들어 캠페인 레코드 유형에는 특정 캠페인과 직접 연관된 경우에만 관련이 있는 캠페인 크기라는 단일 선택 필드가 있을 수 있습니다.

#### 레코드 유형에 레이블을 지정하려면 어떻게 해야 합니까?

&quot;캠페인&quot;과 같이 단일 구문 또는 명사를 나타내는 레코드 유형을 만들고 레이블을 지정합니다.

:no_entry_sign: 보기 레이어로 더 잘 표시되는 레코드 형식을 만들지 마십시오. 예를 들어 &quot;달력&quot;은 레코드 형식 자체가 아니라 레코드 보기이므로 레코드 형식에 적합하지 않습니다.

### 몇 개의 계층 구조를 만들어야 합니까?

보기

...

워크플로

...

### 필드 관리

기본 필드

연결할 때 이러한 레코드를 더 쉽게 찾고 &quot;선택&quot;할 수 있도록 하려면 고유한 기본 필드 값을 사용하십시오.

연결할 때 사용자는 기본 필드의 값을 검색하고 값이 고유하지 않으면 사용자는 선택할 값을 알 수 없습니다.

연결 선택기 메뉴를 사용할 때 기본 필드를 검색해야 하는 사용자에게 혼동을 줄 수 있으므로 고유하지 않은 값을 기본 필드로 사용하지 마십시오.



크리스 오닐로부터의 소식입니다.

Planning을 가장 잘 사용하는(또는 사용하지 않는) 사용 사례도 고려해야 할 사항 중 하나입니다. 예를 들어, 오늘 있었던 리소스 관리 논의



알리나의 노트:

ExL의 &quot;모범 사례&quot; 문서의 예: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346 의 Field Readiness에 대한 추가 정보