---
title: 레코드 유형 및 분류 개요
description: 레코드 유형은 Maestro 작업 영역의 기본 구성 요소입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 유형 및 분류 개요

{{maestro-important-intro}}

오브젝트 유형이 사전 정의된 Workfront과 달리 Adobe Maestro에서는 나만의 오브젝트 유형을 만들 수 있습니다. 예를 들어 Workfront에서 프로그램, Portfolio, 프로젝트, 작업 또는 문제의 객체 유형이 이미 생성되었습니다.

Maestro 객체 유형을 &quot;레코드 유형&quot;이라고 합니다. 레코드 유형은 Maestro 작업 영역의 기본 구성 요소입니다. 작업 공간에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).

## 레코드 유형 개요

Maestro에서는 조직의 요구 사항에 맞는 사용자 정의 레코드 유형을 만들 수 있습니다.

* 다음은 Maestro 레코드 유형입니다.

   * [운영 레코드 유형](#operational-record-type): 전략 계획, 이니셔티브 또는 계획된 작업을 나타내는 레코드 유형입니다. 예를 들어 Campaign, Activity, Tactic, Opportunity 는 운영 레코드 유형이 될 수 있습니다.
   * [분류](#taxonomy): 작업 레코드 유형에 대한 속성을 캡처하는 레코드 유형입니다. 예를 들어 지역, 주소, 대상은 분류법일 수 있습니다.

* 레코드 유형을 만들면 사용자와 작업 공간에 액세스할 수 있는 권한을 부여한 사용자만 레코드 유형을 볼 수 있습니다.
* 작업 영역에 대한 레코드 유형을 만들려면 먼저 작업 영역을 만들어야 합니다.
* 한 작업 공간에 총 1,000개의 작업 레코드 유형과 분류를 사용할 수 있습니다. 여기에는 처음부터 만들거나 다른 시스템에서 가져오는 레코드 유형 또는 분류가 포함됩니다.

### 운영 레코드 유형{#operational-record-type}

작업 레코드 유형은 작업 관련 개체를 나타내는 Maestro 레코드 유형입니다.

![](assets/operational-record-type-blank.png)

레코드 유형을 만드는 방법을 포함하여 운영 레코드 유형에 대한 자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

### 분류{#taxonomy}

분류법은 작업 레코드 유형에 대한 속성을 캡처하는 레코드 유형입니다.

![](assets/taxonomy-record-type-blank.png)

분류 레코드 유형에 대한 자세한 내용은 [분류 체계 만들기](../architecture/create-a-taxonomy.md).

분류법을 만드는 것은 운영 레코드 유형을 만드는 것과 동일하지만 Maestro는 운영 레코드 유형과 분류 레코드 유형을 개념적으로 구분합니다. 분류 체계의 목적은 운영 기록 유형을 향상시키는 것입니다. 분류법은 작업 객체를 직접 나타내서는 안 됩니다.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

예를 들어 대상, 지역 또는 주소는 분류법 유형 레코드 유형일 수 있습니다.

자세한 내용은 [분류 체계 만들기](../architecture/create-a-taxonomy.md).

## 운영 레코드 유형과 분류 간의 유사점과 차이점

다음 테이블은 운영 레코드 유형과 분류 간의 일부 유사점과 차이점을 보여 줍니다.

| 레코드 유형 및 특성 | 운영 레코드 유형 | 분류 레코드 유형 |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| 작업 공간의 일부입니다 | ✓ 덧신 | ✓ 덧신 |
| 작업 영역 템플릿에서 자동으로 생성할 수 있습니다 | ✓ 덧신 | ✓ 덧신 |
| 처음부터 수동으로 만들 수 있습니다 | ✓ 덧신 | ✓ 덧신 |
| 외부 파일 또는 목록에서 정보를 복사하여 붙여 넣어 만들 수 있습니다 | ✓ 덧신 | ✓ 덧신 |
| Excel 또는 CSV 파일을 가져와서 만들 수 있습니다 | ✓ 덧신 |                     |
| 다른 응용 프로그램에서 개체 형식에 연결하여 읽기 전용 레코드 형식을 만들 수 있습니다 | ✓ 덧신 |                     |
| 작업 관련 객체를 나타냅니다. | ✓ 덧신 |                      |
| 작업 관련 객체에 대한 속성을 나타냅니다 |                         | ✓ 덧신 |
| 처음부터 만들 수 있습니다. | ✓ 덧신 | ✓ 덧신 |
| Excel 또는 CSV 파일을 가져와서 만들 수 있습니다 | ✓ 덧신 |                      |
| 다른 응용 프로그램의 개체에 레코드 형식을 연결할 수 있습니다 | ✓ 덧신 |                      |
| 다른 Maestro 레코드 유형에 연결할 수 있습니다. | ✓ 덧신 |                    |
| 테이블 보기에서 연결된 레코드를 볼 수 있습니다 | ✓ 덧신 | ✓ 덧신 |
| 연결된 레코드를 타임라인 보기에서 볼 수 있습니다 | ✓ 덧신 | ✓ 덧신 |
