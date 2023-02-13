---
product-area: projects
navigation-topic: manage-projects
title: Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑
description: Adobe Workfront 및 Microsoft 프로젝트의 프로젝트는 대부분 호환됩니다. 이 문서에서는 두 응용 프로그램의 가장 일반적인 프로젝트 필드가 서로 매핑되는 방식을 설명합니다.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑

Adobe Workfront 및 Microsoft 프로젝트의 프로젝트는 대부분 호환됩니다. 두 응용 프로그램을 사용하여 다음을 수행할 수 있습니다.

* Microsoft 프로젝트에서 프로젝트를 내보내고 Workfront으로 가져옵니다
* Workfront에서 프로젝트를 내보내고 Microsoft Project로 가져옵니다. 

Microsoft Project에서 Workfront으로 프로젝트를 가져오는 방법에 대한 자세한 내용은 [Microsoft 프로젝트에서 프로젝트 가져오기](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

프로젝트를 Microsoft 프로젝트로 가져오기 위해 Workfront에서 프로젝트를 내보내는 방법에 대한 자세한 내용은 [Microsoft 프로젝트로 프로젝트 내보내기](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

이러한 데이터 가져오기를 수행할 때 정보가 한 애플리케이션에서 다른 애플리케이션으로 변환되는 방식을 이해하는 것이 중요합니다. 가져오기를 완료한 후 대부분의 경우 프로젝트를 수동으로 수정해야 합니다. 

## 필드 매핑 개요

>[!NOTE]
>
>계획된 날짜가 항상 두 시스템 간에 일치하지 않습니다. 불일치는 Workfront과 Microsoft 프로젝트 간의 시스템 환경 설정 일정과 차이를 통해 확인할 수 있습니다. 이러한 날짜 불일치로 인해 작업, 기간 및 완료율의 차이가 발생할 수도 있습니다.

| **Microsoft 프로젝트 필드** | **Workfront 필드** |
|---|---|
| 프로젝트 제목 | 프로젝트 이름 |
| 시작 및 완료 날짜 | 계획 시작 및 완료 일자 |
| 작업 이름 | 작업 이름 |
| 작업 기간 | 작업 계획 기간 |
| 작업 | 작업 계획 시간 |
| 작업 % 완료 | 작업 완료율(작업 기간 기준) |
| 작업 완료율 | 작업 % 완료(작업의 계획 시간 기준) |
| 예약된 시작 및 완료 | 계획 시작 및 완료 일자 |
| 실제 시작 및 완료 | 실제 시작 및 완료 일자 |
| 리소스 이름 | 작업 할당 |
| 배정 단위 | 발령 할당 퍼센트 |
| 작업 참고 | 작업 설명 |
| 전임 작업 | 전임 작업 |

## 포함되지 않은 데이터 개요

Workfront으로 가져오거나 내보내지 않는 프로젝트 필드가 많습니다.

이러한 필드는 다음과 같이 포함되지만 이에 국한되지 않습니다.

* 문서 첨부 파일
* 사용자 정의 필드(프로젝트 또는 작업 수준)
* Workfront 노트
* 문제
* 시작/완료 이전 관계(지연 없이 작업을 가져옵니다.)가 있는 작업의 음수 지연
* 할당
* 작업 제한

   >[!NOTE]
   제약 조건은 Microsoft 프로젝트와 Workfront 간에 매핑되지 않으므로 작업 간에 이전 관계가 있는지 확인하십시오. 그렇지 않으면, 가져온 프로젝트에서 작업의 계획 시작 및 계획 완료 일자가 정확하지 않을 수 있습니다. 
