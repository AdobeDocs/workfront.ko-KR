---
title: 레코드 유형 개요
description: 레코드 유형은 Adobe Workfront Planning 작업 영역의 기본 구성단위입니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# 레코드 유형 개요

{{planning-important-intro}}

객체 유형이 사전 정의된 Workfront과 달리 Adobe Workfront Planning에서는 고유한 객체 유형을 만들 수 있습니다.

예를 들어 Workfront에서 프로그램, Portfolio, 프로젝트, 작업 또는 문제의 객체 유형이 이미 생성되었습니다.

Workfront Planning 객체 유형을 &quot;레코드 유형&quot;이라고 하며 사용자가 만들 때만 존재합니다.

레코드 유형은 Workfront Planning 작업 영역의 기본 구성 요소이며, 워크플로우 및 기타 정보와 연결할 수 있도록 모든 레코드 유형을 만들어야 합니다.

레코드 유형은 작업 영역에서 구성됩니다.

작업 영역에 대한 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

## 레코드 유형 개요

Workfront Planning에서 조직의 요구 사항에 맞는 사용자 정의 레코드 유형을 만들 수 있습니다.

레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

* 템플릿에서 작업 공간을 만들면 다음 작업 공간 섹션에 레코드 유형이 생성됩니다.

   * **운영 레코드 종류**: 전략 계획, 이니셔티브 또는 계획된 작업을 나타내는 레코드 종류. 예를 들어 Campaign, Activity, Tactic, Opportunity 는 운영 레코드 유형입니다.
   * **분류**: 작업 레코드 형식에 대한 특성을 캡처하는 레코드 형식입니다. 예를 들어 지역, 주소, 대상은 분류법입니다.

  이러한 섹션의 이름을 바꾸거나 삭제하거나 더 많이 만들 수 있습니다.

* 처음부터 만든 작업공간에 레코드 유형을 만들면 작업공간에서 만든 모든 섹션에 레코드 유형을 배치할 수 있습니다.
* 레코드 유형을 만들면 사용자와 작업 공간에 액세스할 수 있는 권한을 부여한 사용자만 레코드 유형을 볼 수 있습니다.
* 작업 영역에 대한 레코드 유형을 만들려면 먼저 작업 영역을 만들어야 합니다.
* 한 작업 영역 또는 Workfront 인스턴스에서 가질 수 있는 레코드 종류의 수에 대한 제한 사항은 [Adobe Workfront Planning 개체 제한 사항 개요](/help/quicksilver/planning/general/limitations-overview.md)를 참조하십시오.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

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
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
