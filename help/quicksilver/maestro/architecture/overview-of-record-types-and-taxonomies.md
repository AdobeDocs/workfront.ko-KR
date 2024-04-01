---
title: 레코드 유형 개요
description: 레코드 유형은 Adobe Workfront Planning 작업 영역의 기본 구성단위입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 유형 개요

{{maestro-important-intro}}

객체 유형이 사전 정의된 Workfront과 달리 Adobe Workfront Planning에서는 고유한 객체 유형을 만들 수 있습니다. 예를 들어 Workfront에서 프로그램, Portfolio, 프로젝트, 작업 또는 문제의 객체 유형이 이미 생성되었습니다.

Workfront Planning 객체 유형을 &quot;레코드 유형&quot;이라고 하며, 모든 유형을 만들고 사용자 정의할 수 있습니다. 레코드 유형은 Workfront Planning 작업 영역의 기본 구성단위입니다. 작업 공간에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).

## 레코드 유형 개요

Workfront Planning에서 조직의 요구 사항에 맞는 사용자 정의 레코드 유형을 만들 수 있습니다.

* 템플릿에서 작업 공간을 만들면 다음 작업 공간 섹션에 레코드 유형이 생성됩니다.

   * [운영 레코드 유형](#operational-record-type): 전략 계획, 이니셔티브 또는 계획된 작업을 나타내는 레코드 유형입니다. 예를 들어 Campaign, Activity, Tactic, Opportunity 는 운영 레코드 유형이 될 수 있습니다.
   * [분류](#taxonomy): 작업 레코드 유형에 대한 속성을 캡처하는 레코드 유형입니다. 예를 들어 지역, 주소, 대상은 분류법일 수 있습니다.

* 처음부터 만든 작업공간에 레코드 유형을 만들면 작업공간에서 만든 모든 섹션에 레코드 유형을 배치할 수 있습니다.
* 레코드 유형을 만들면 사용자와 작업 공간에 액세스할 수 있는 권한을 부여한 사용자만 레코드 유형을 볼 수 있습니다.
* 작업 영역에 대한 레코드 유형을 만들려면 먼저 작업 영역을 만들어야 합니다.
* 작업 공간에 있는 섹션의 수에 관계없이 하나의 작업 공간에서 총 1,000개의 레코드 유형을 가질 수 있습니다. 여기에는 처음부터 만들거나 템플릿을 사용할 때 만드는 레코드 유형이 포함됩니다.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

![](assets/operational-record-type-blank.png)

For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

![](assets/taxonomy-record-type-blank.png)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->