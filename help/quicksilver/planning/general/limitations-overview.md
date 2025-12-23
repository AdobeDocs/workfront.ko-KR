---
title: Adobe Workfront Planning 객체 제한 사항 개요
description: Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 2%

---


<!--keep the 30 connection limit in yellow till Jan 2026-->

# Adobe Workfront Planning 객체 제한 사항 개요

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 프로덕션에 대한 월별 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}


Adobe Workfront Planning에는 인스턴스에서 생성할 수 있는 객체 수에 대한 제한이 있습니다. 제품 성능을 개선하고 Workfront Planning에 대한 경험을 개선하기 위해 오브젝트 제한이 적용됩니다.

다음 표는 Workfront Planning에서 생성할 수 있는 객체 수에 대한 제한을 보여 줍니다. 제한 사항은 변경될 수 있습니다.

| Adobe Workfront Planning 개체 | 제한 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 하나의 Workfront 인스턴스에 대한 작업 공간 수 | 무제한* |
| 하나의 작업 영역에 대한 섹션 수 | 50 |
| 하나의 작업 영역에 대한 레코드 유형 수 | 100(모든 섹션의 레코드 유형과 작업 공간 템플릿을 사용할 때 생성되는 레코드 유형 포함) |
| 하나의 레코드 유형에 대한 레코드 수 | 25,000 |
| 하나의 작업 영역에 대한 레코드 수 | 계획 선택: 25,000 <br> 계획 Prime: 500,000 <br> 계획 Ultimate: 1,000,000 |
| Workfront Planning 인스턴스 하나에 대한 총 레코드 수 | Planning 선택: 500,000 <br> Planning Prime: 2,000,000 <br> Planning Ultimate: 무제한 |
| 하나의 레코드 유형 또는 분류법에 대한 필드 수 | 500 |
| 한 줄 텍스트 필드의 문자 수 | 1,000자 |
| 단락 필드의 문자 수 | 10,000자 |
| 하나의 레코드 종류에 대한 단락 필드 수 | 20개 단락 필드 |
| 레코드 유형 테이블에서 정보를 가져오는 데 사용할 수 있는 파일 크기 | 1MB |
| API를 통해 레코드 유형 테이블의 정보를 가져오는 데 사용할 수 있는 파일 크기 | 1.5MB |
| API 요청을 수행할 수 있는 속도입니다 | 분당 요청 200개 |
| 한 사용자가 하나의 레코드 유형에 대해 만들 수 있는 보기 수 | 10 |
| 레코드 유형을 만들기 위해 가져올 수 있는 Excel 파일의 CSV 크기 | 5MB |
| CSV 또는 Excel 파일로 가져와 레코드 유형을 만들 수 있는 행 수 | 25,000 |
| CSV 또는 Excel 파일로 가져와 레코드 유형을 만들 수 있는 열 수 | 500 |
| 하나의 레코드 유형에 대한 공식 필드 수 | 20 |
| <span class="preview">하나의 레코드 형식에 대한 연결 필드 수</span> | <span class="preview">30</span> |
| 공식 필드 표현식의 문자 수 | 50,000 |
| Planning 객체를 공유할 수 있는 엔티티(사용자, 역할, 팀, 회사, 그룹) 수 | 100 |
| <span class="preview">계층 구조의 레코드 종류 수</span> | 4 |
| <span class="preview">작업 영역의 계층 구조 수</span> | 5 |
| <span class="preview">계층 구조 내에서 자식 레코드 형식의 레코드에 연결된 부모 레코드 형식의 레코드 수</span> | 10 |
| 다중 선택 연결 형식의 한 레코드에 연결된 레코드 수 <span class="preview">레코드 사이에 계층 구조가 구성되지 않음</span> | 500 |

*작업 영역은 관리하기 어려워질 수 있고 워크플로가 너무 많이 조각날 수 있으므로 너무 많이 사용하지 않는 것이 좋습니다.

Workfront Planning 가격 및 패키징에 대한 자세한 내용은 계정 관리자에게 문의하십시오.

<!--
****************KEEP THIS COMMENTED OUT:

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
