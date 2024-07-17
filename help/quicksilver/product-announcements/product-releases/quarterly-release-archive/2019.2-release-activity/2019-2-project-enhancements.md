---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2 프로젝트 개선 사항
description: 이 페이지에서는 2019.2 릴리스에 포함된 모든 프로젝트 개선 사항에 대해 설명합니다. 이 기능은 2019년 5월 20일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 2019.2 프로젝트 개선 사항

이 페이지에서는 2019.2 릴리스에 포함된 모든 프로젝트 개선 사항에 대해 설명합니다. 이 기능은 2019년 5월 20일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

2019.2의 모든 변경 사항 목록은 [2019.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md)를 참조하십시오.

## 상태를 사용자 지정할 때 더 빠르게 그룹 찾기

설정 영역의 상태 탭에 있는 드롭다운 메뉴는 이제 자동 완성 메뉴입니다. 이렇게 하면 시스템에서 그룹을 빠르게 검색하고 찾을 수 있으므로 상태를 보다 쉽게 사용자 지정할 수 있습니다.

이전에는 드롭다운 메뉴에 제한된 수의 그룹이 표시되었습니다. 원하는 그룹이 표시되지 않으면 설정 > 그룹으로 이동하여 특정 그룹을 찾아 그룹의 상태를 사용자 정의해야 합니다.

자세한 내용은 [상태 만들기 또는 편집](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

## 작업에 기본 사용자 지정 Forms 및 승인 프로세스 첨부

이제 프로젝트에 작업을 추가할 때 작업에 첨부할 기본 사용자 정의 양식 및 승인 프로세스를 구성할 수 있습니다. 프로젝트 수준에서 기본 설정을 구성할 수 있습니다.

프로젝트 수준의 작업에 대한 기본 사용자 정의 양식 및 승인 프로세스를 구성하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../../manage-work/projects/manage-projects/edit-projects.md) 문서의 &quot;작업&quot; 섹션을 참조하십시오.

## 작업 목록에 상위 작업의 전체 행을 굵게 표시

작업 목록에서 상위 작업이 포함된 행은 굵게 표시됩니다. 이 변경 사항은 작업 분류 구조 또는 작업 번호 순으로 목록을 오름차순으로 정렬할 때 표시됩니다.

## 작업 목록의 변경 내용 취소

작업 목록의 새 자동 저장 버튼을 사용하면 변경 사항을 자동으로 저장할지 또는 저장하기 전에 변경 사항의 영향을 표시할지를 선택할 수 있습니다. 이 설정은 작업 목록과 간트 차트 모두에 적용됩니다.

이 개선 이전에는 모든 변경 사항이 항상 자동으로 저장되었습니다.

작업 목록에서 작업을 편집하는 방법에 대한 자세한 내용은 [작업 편집](../../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

간트 차트에서 작업을 편집하는 방법에 대한 자세한 내용은 [작업 목록 간트 차트에서 정보 업데이트](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)를 참조하십시오.

## 새 목록의 새 열 너비 기본값

이제 Workfront에서는 각 열의 valueformat 정보에 따라 열의 너비를 자동으로 조정합니다. 예를 들어, 숫자를 표시하는 열이 설명 필드를 표시하는 열보다 넓습니다.

이 개선 이전에는 별도로 지정하지 않는 한 새 프로젝트 및 작업 보기의 열 너비가 100픽셀로 설정되었습니다.

열 너비에 대한 자세한 내용은 [열 너비 및 순서 수정](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)을 참조하십시오.

## 사용하지 않는 개체 비활성화

>[!NOTE]
>
>이 기능은 2019.2 미리보기 기간 동안 프로덕션 환경에 직접 릴리스되었습니다.

이제 더 이상 사용되지 않는 객체가 있는 경우 사용자가 해당 객체를 다른 객체와 연관시키지 못하도록 목록에서 숨기도록 비활성화할 수 있습니다.

이제 아래 오브젝트를 편집할 때 활성화 여부를 표시할 수 있습니다. 활성으로 설정된 객체는 드롭다운 메뉴와 앞에 입력 필드에 나타나며 다른 객체에 첨부할 수 있습니다. 활성으로 설정되지 않은 객체는 다른 객체에 첨부할 드롭다운 메뉴와 자동 입력 필드에 표시되지 않습니다.

* 승인 프로세스
* 회사
* 사용자 정의 양식
* 마일스톤 경로
* 포트폴리오
* 프로그램
* 템플릿

현재 사용되는 비활성화하는 모든 항목은 항상 그랬던 것처럼 계속 작동하며 제거되거나 차단되지 않습니다.

>[!IMPORTANT]
>
>Workfront API를 통해 이러한 개체를 만들 때 &quot;isActive&quot; 매개 변수의 기본값은 true입니다. 모든 개체에 대한 새 필드이며 API 버전 11 이전에 편집할 수 없습니다. 이 필드는 Portfolio의 기본값이 false인 경우를 제외하고 이전에 존재했습니다. API 버전 11부터 기본값이 true로 변경됩니다.

## 예약된 작업의 예산 비용(BCWS) 및 수행된 작업 비용(BCWP)을 보기에 표시

이제 프로젝트 및 작업 보기에 BCWS(예약된 작업의 예산 비용) 및 BCWP(수행된 작업의 예산 비용)를 표시할 수 있습니다.

이러한 프로젝트 성능 지표는 이전에 Workfront의 재무 계산에 사용되었지만, 이 개선 이전에는 시스템에 표시되지 않았습니다.

BCWS 계산에 대한 자세한 내용은 [BCWS(예약된 작업의 예산 비용) 계산](../../../../manage-work/projects/project-finances/calculate-bcws.md)을 참조하십시오.

BCWP 계산에 대한 자세한 내용은 [BCWP(수행된 작업의 예산 비용 계산)](../../../../manage-work/projects/project-finances/calculate-bcwp.md)을 참조하세요.

