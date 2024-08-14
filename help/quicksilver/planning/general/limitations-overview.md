---
title: Adobe Workfront Planning 객체 제한 사항 개요
description: Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Adobe Workfront Planning 객체 제한 사항 개요

Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.

다음 표는 Workfront Planning에서 생성할 수 있는 객체 수에 대한 제한을 보여 줍니다. 다음 단계의 개발로 넘어감에 따라 제한 사항이 변경될 수 있습니다.

| Adobe Workfront Planning 개체 | 제한 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 하나의 Workfront 인스턴스에 대한 작업 공간 수 | 1,000 |
| 하나의 작업 영역에 대한 섹션 수 | 50 |
| 하나의 작업 영역에 대한 레코드 유형 수 | 1,000(모든 섹션의 레코드 유형과 작업 영역 템플릿을 사용할 때 생성된 레코드 유형 포함) |
| 하나의 레코드 유형에 대한 레코드 수 | 50,000 |
| 하나의 레코드 유형 또는 분류법에 대한 필드 수 | 500 |
| 텍스트 필드의 문자 수 | 1,000자 |
| 레코드 종류 표에 붙여 넣을 수 있는 파일 크기 | 1MB |
| 레코드 유형 테이블에 대한 API를 통해 가져올 수 있는 파일의 크기입니다. | 1.5MB |
| API 요청을 수행할 수 있는 속도입니다 | 분당 요청 200개 |
| 가져올 수 있는 Excel 파일의 CSV 크기* | 5MB |
| 한 사용자가 하나의 레코드 유형에 대해 만들 수 있는 보기 수 | 10 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*이 기능은 일시적으로 비활성화되었으며 나중에 사용할 수 있습니다.

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->