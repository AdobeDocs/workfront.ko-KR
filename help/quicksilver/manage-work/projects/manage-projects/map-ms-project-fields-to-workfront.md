---
product-area: projects
navigation-topic: manage-projects
title: Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑
description: Adobe Workfront 및 Microsoft Project의 프로젝트는 대부분 호환됩니다. 이 문서에서는 두 애플리케이션에서 가장 일반적인 프로젝트 필드가 서로 매핑되는 방식을 설명합니다.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑

Adobe Workfront 및 Microsoft Project의 프로젝트는 대부분 호환됩니다. 두 애플리케이션을 사용하여 다음을 수행할 수 있습니다.

* Microsoft 프로젝트에서 프로젝트를 내보내고 Workfront으로 가져오기
* Workfront에서 프로젝트를 내보내고 Microsoft 프로젝트로 가져옵니다. 

의 Microsoft 프로젝트에서 Workfront으로 프로젝트를 가져오는 방법에 대한 자세한 내용은 [Microsoft 프로젝트에서 프로젝트 가져오기](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)를 참조하십시오.

Workfront에서 프로젝트를 내보내어 Microsoft Project로 가져오는 방법에 대한 자세한 내용은 [Microsoft Project로 프로젝트 내보내기](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)를 참조하십시오.

이러한 데이터 가져오기를 수행할 때 정보가 한 애플리케이션에서 다른 애플리케이션으로 어떻게 변환되는지 이해하는 것이 중요합니다. 대부분의 경우 가져오기를 완료한 후 프로젝트를 수동으로 수정해야 합니다. 

## 필드 매핑 개요

>[!NOTE]
>
>계획된 일자가 두 시스템 간에 항상 일치하는 것은 아닙니다. 일정과 Workfront과 Microsoft Project 간의 시스템 환경 설정 차이를 통해 불일치를 해결할 수 있습니다. 이러한 날짜 불일치로 인해 노력, 기간 및 완료율의 차이가 발생할 수도 있습니다.

| **Microsoft 프로젝트 필드** | **Workfront 필드** |
|---|---|
| 프로젝트 제목 | 프로젝트 이름 |
| 시작 및 완료 날짜 | 계획된 시작 및 완료 일자 |
| 작업 이름 | 작업 이름 |
| 작업 기간 | 작업 계획 기간 |
| 작업 | 작업 계획 시간 |
| 작업 % 완료 | 작업 % 완료(작업 기간 기준) |
| 작업 작업 % 완료 | 작업 % 완료(작업의 계획된 시간 기준) |
| 예약된 시작 및 완료 | 계획된 시작 및 완료 일자 |
| 실제 시작 및 완료 | 실제 시작 및 완료 일자 |
| 리소스 이름 | 작업 할당 |
| 배정 단위 | 할당 할당 백분율 |
| 작업 메모 | 작업 설명 |
| 전임 작업 | 전임 작업 |

## 포함되지 않은 데이터 개요

Workfront으로 가져오거나 내보내지지 않는 프로젝트 필드가 많습니다.

이러한 필드에는 다음이 포함되지만 이에 국한되지 않습니다.

* 문서 첨부 파일
* 사용자 정의 필드(프로젝트 또는 작업 수준)
* Workfront 노트
* 문제
* 시작/완료 전임 작업 관계가 있는 작업의 음수 지연(작업이 지연 없이 가져옴)
* 할당
* 작업 제한

  >[!NOTE]
  >
  >제한 사항은 Microsoft Project와 Workfront 간에 매핑되지 않으므로 작업 간에 전임 작업 관계가 있는지 확인하십시오. 그렇지 않으면 가져온 프로젝트에서 작업의 계획된 시작 일자 및 계획된 완료 일자가 정확하지 않을 수 있습니다. 
