---
title: Adobe Workfront Planning 객체 제한 사항 개요
description: Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 1%

---


<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning 객체 제한 사항 개요

{{planning-important-intro}}


Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.

다음 표는 Workfront Planning에서 생성할 수 있는 객체 수에 대한 제한을 보여 줍니다. 다음 단계의 개발로 넘어감에 따라 제한 사항이 변경될 수 있습니다.

| Adobe Workfront Planning 개체 | 제한 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 하나의 Workfront 인스턴스에 대한 작업 공간 수 | 제한 없음* |
| 하나의 작업 영역에 대한 섹션 수 | 50 |
| 하나의 작업 영역에 대한 레코드 유형 수 | 1,000(모든 섹션의 레코드 유형과 작업 영역 템플릿을 사용할 때 생성된 레코드 유형 포함) |
| 하나의 레코드 유형에 대한 레코드 수 | 25,000 |
| 하나의 작업 영역에 대한 레코드 수 | 계획 계획이 있는 고객의 경우 25,000명 <br>계획 플러스 계획이 있는 고객의 경우 500,000명 |
| Workfront Planning 유형 인스턴스 하나에 대한 총 레코드 수 | 계획 계획이 있는 고객의 경우 50만 개, 계획 플러스 계획이 있는 고객의 경우 <br>2만 개 |
| 하나의 레코드 유형 또는 분류법에 대한 필드 수 | 500 |
| 텍스트 필드의 문자 수 | 1,000자 |
| 레코드 종류 표에 붙여 넣을 수 있는 파일 크기 | 1MB |
| 레코드 유형 테이블에 대한 API를 통해 가져올 수 있는 파일의 크기입니다. | 1.5MB |
| API 요청을 수행할 수 있는 속도입니다 | 분당 요청 200개 |
| 한 사용자가 하나의 레코드 유형에 대해 만들 수 있는 보기 수 | 10 |

*작업 영역은 관리하기 어려워질 수 있으며 워크플로우가 너무 많이 조각날 수 있으므로 너무 많이 사용하지 않는 것이 좋습니다.

Workfront Planning 가격 및 패키징에 대한 자세한 내용은 [Adobe Workfront 가격 및 패키징](https://business.adobe.com/products/workfront/pricing.html)을 참조하십시오.

<!--
****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

