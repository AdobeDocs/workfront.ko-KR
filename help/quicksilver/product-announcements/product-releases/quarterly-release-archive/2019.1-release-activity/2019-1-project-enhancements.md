---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 프로젝트 개선 사항
description: 이 페이지에서는 2019.1 릴리스에 포함된 모든 프로젝트 개선 사항에 대해 설명합니다. 이 기능은 현재 미리보기 환경에서 사용할 수 있습니다. 의 프로덕션 환경에서 사용할 수 있게 됩니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# 2019.1 프로젝트 개선 사항

이 페이지에서는 2019.1 릴리스에 포함된 모든 프로젝트 개선 사항에 대해 설명합니다. 이 기능은 현재 미리보기 환경에서 사용할 수 있습니다. 의 프로덕션 환경에서 사용할 수 있게 됩니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2019.1의 모든 변경 사항 목록은 &quot;2019.1 릴리스 활동 개요&quot;를 참조하십시오.

관리자용 **1&rbrace;**

* [휴지통에서 템플릿 복원](#restore-templates-from-the-recycle-bin)
* [홈의 날짜 필드에 대한 타임스탬프 표시](#show-timestamps-for-date-fields-in-home)
* [프로젝트 환경 설정에서 사용할 수 있는 모든 기간 유형](#all-duration-types-available-under-project-preferences)

**모든 사용자의 경우**

* [애자일 개선 사항](#agile-improvements)
* [목록에서 반복에 작업 및 문제 추가](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [간트 차트 내보내기를 위한 새로운 용지 크기](#new-paper-sizes-for-gantt-chart-export)
* [편집 모드에 있는 동안 간트 차트에서 대화 상자에 대한 액세스 제거됨](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [프로그램 또는 Portfolio의 프로젝트 목록 간트 차트에서 작업 정보 보기](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [템플릿의 작업 목록 간트 차트에 액세스](#access-the-task-list-gantt-chart-on-templates)
* [간트 차트에서 프로젝트 보기 이름이 변경됨](#renamed-the-project-view-on-the-gantt-chart)
* [작업 목록 간트 차트의 가상 시나리오](#what-if-scenarios-in-the-task-list-gantt-chart)
* [작업 목록 개선 사항](#task-list-improvements)
* [전체 화면에 목록 표시](#display-lists-in-full-screen)
* [추가 영역의 새 목록](#new-lists-in-additional-areas)
* [배달된 보고서를 XLSX 형식으로 보내기](#send-a-delivered-report-in-xlsx-format)
* [감사 로그 내보내기](#export-audit-logs)

## 휴지통에서 템플릿 복원 {#restore-templates-from-the-recycle-bin}

Workfront 관리자는 이제 휴지통에서 템플릿을 복원할 수 있습니다. 다른 삭제된 항목과 마찬가지로 템플릿을 삭제한 시간으로부터 최대 30일까지 복원할 수 있습니다.

자세한 내용은 &quot;삭제된 항목 복원&quot;을 참조하십시오.

## 홈의 날짜 필드에 대한 타임스탬프 표시 {#show-timestamps-for-date-fields-in-home}

이제 Workfront 관리자는 레이아웃 템플릿을 사용하여 작업 목록 및 달력에서 기한에 대한 타임스탬프를 표시하거나 숨기도록 선택할 수 있습니다. 기본적으로 타임스탬프는 템플릿 사용자와 비템플릿 사용자 모두에 대해 표시됩니다.

자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot; 문서의 &quot;홈 영역 사용자 정의&quot;를 참조하십시오.

## 프로젝트 환경 설정에서 사용할 수 있는 모든 기간 유형 {#all-duration-types-available-under-project-preferences}

설정 > 프로젝트 환경 설정에서 기본 작업 및 문제 기간 유형을 설정할 때 다음 옵션 중 하나를 사용할 수 있습니다.

단순

작업량 고정

계산된 할당

계산된 작업

이전에는 단순 또는 투입 고정 중 하나를 기본 기간 유형으로 설정한 경우 계산된 발령 및 계산된 작업을 선택할 수 없었습니다.

작업 및 문제 기간 유형 기본값 설정에 대한 자세한 내용은 &quot;작업 및 문제 환경 설정&quot;을 참조하십시오.

## 애자일 개선 사항 {#agile-improvements}

이제 애자일 도구에서 다음과 같은 개선 사항을 사용할 수 있습니다.

칸반

작업 목록 또는 보고서에서 칸반 보드에 작업 및 문제를 추가합니다.

이전에는 백로그에서만 Kanban 보드에 작업을 추가할 수 있었습니다. 문제를 추가할 수 없습니다.

칸반 보드를 팀의 개별 사용자별로 필터링합니다.

자세한 내용은 &quot;칸반 보드 사용&quot;을 참조하십시오.

Kanban 백로그에 대한 문제를 보고 관리합니다.

자세한 내용은 &quot;Kanban 보드 사용&quot;을 참조하십시오.

이전에는 Kanban 보드에서 문제를 추가하거나 관리할 수 없었습니다.

스크럼

팀의 개별 사용자별로 반복 스토리 보드를 필터링합니다.

자세한 내용은 &quot;스크럼 애자일 스토리 보드 사용&quot;을 참조하십시오.

이전에는 Kanban 또는 스크럼 보드에서 사용자별로 필터링할 수 없었습니다.

## 목록에서 반복에 작업 및 문제 추가 {#add-tasks-and-issues-from-a-list-to-an-iteration}

이제 작업 또는 문제 목록, 보고서 또는 대시보드를 사용하여 스토리를 반복에 추가할 수 있습니다. 여러 팀에 하나의 반복에 스토리를 할당하도록 할 수도 있습니다.

이전에는 작업 또는 문제 세부 정보 페이지에서만 반복에 스토리를 추가할 수 있었으며 팀이 만든 반복에만 스토리를 추가할 수 있었습니다.

자세한 내용은 &quot;애자일 반복 생성 및 관리&quot;를 참조하십시오.

## XLSX 형식으로 게재된 보고서 보내기 {#send-a-delivered-report-in-xlsx-format}

이제 다른 모든 현재 형식 외에도 MS Excel(.xlsx) 형식으로 보고서가 배달되도록 예약할 수 있습니다.

이전에는 다음 형식으로만 보고서를 제공할 수 있었습니다.

HTML

PDF

MS Excel (.xls)

TSV

보고서 배달 예약에 대한 자세한 내용은 &quot;보고서 배달 설정&quot;을 참조하십시오.

## 작업 목록 개선 사항 {#task-list-improvements}

[이 항목이 제거된 18.3 Beta 4 업데이트]

18.3 베타 4 릴리스 동안 잠시 제거한 후 새로 다시 디자인된 작업 목록이 다시 활성화되었습니다. 또한 원래 릴리스에 포함되지 않은 작업 목록에 다음과 같은 추가 기능을 도입했습니다.

한 작업을 인라인 편집할 때 마우스 오른쪽 버튼 클릭 메뉴를 기타 아이콘으로 바꾸기

여러 작업을 인라인 편집할 때 마우스 오른쪽 버튼 클릭 메뉴에서 사용할 수 있었던 옵션이 이제 작업 목록 맨 위에 표시된 아이콘으로 이동되었습니다.

기본적으로 작업 목록에는 2000개의 작업이 표시됩니다.

Workfront이 타임라인을 다시 계산할 때 날짜가 업데이트되는 작업 옆의 물음표가 회색 영역으로 바뀌었습니다.

인라인 작업 편집에 대한 자세한 내용은 &quot;작업 복사 및 복제&quot; 및 &quot;작업을 체인으로 전임 작업 관계 만들기&quot;를 참조하십시오.

프로젝트 타임라인 재계산에 대한 자세한 내용은 &quot;프로젝트에 대한 타임라인 재계산&quot;을 참조하십시오.

## 전체 화면으로 목록 표시 {#display-lists-in-full-screen}

프로젝트 또는 작업 목록이 화면 크기보다 클 경우 스크롤할 때 전체 브라우저 창에 목록이 자동으로 표시됩니다. 이렇게 하면 한 번에 표시되는 정보의 양이 늘어나며 목록을 쉽게 관리할 수 있습니다.

전체 화면에 다음 목록을 표시할 수 있습니다.

다음 탭 및 하위 탭의 프로젝트 목록입니다.

내가 진행 중인 프로젝트

내가 소유한 프로젝트

모든 프로젝트

Portfolio의 프로젝트 탭

프로그램의 프로젝트 탭

다음 탭의 작업 목록입니다.

프로젝트의 작업 탭

작업의 하위 작업 탭

목록에 개체를 표시하는 방법에 대한 자세한 내용은 &quot;목록의 항목 보기&quot;를 참조하십시오.

## 추가 영역의 새 목록 {#new-lists-in-additional-areas}

다음 영역에서 프로젝트 및 작업 목록의 성능을 개선하고 모양과 느낌을 개선했습니다.

프로젝트 영역의 Portfolio 및 프로그램 탭

작업 수준의 하위 작업 탭

이 개선 이전에는 다음 영역에서만 새 목록을 사용할 수 있었습니다.

프로젝트 영역의 프로젝트 탭

프로젝트 수준의 작업 탭

목록에 개체를 표시하는 방법에 대한 자세한 내용은 &quot;목록의 항목 보기&quot;를 참조하십시오.

## 프로그램 또는 Portfolio의 프로젝트 목록 간트 차트에서 작업 정보 보기 {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

이제 프로그램 또는 Portfolio 내의 프로젝트 목록 간트 차트에서 프로젝트 작업에 대한 정보를 볼 수 있습니다.

이전에는 프로젝트 탭의 프로젝트 목록 간트 차트에서만 작업에 대한 정보를 볼 수 있었습니다.

자세한 내용은 &quot;간트 차트에서 정보 보기&quot;를 참조하십시오.

## 작업 목록 간트 차트의 가상 시나리오 {#what-if-scenarios-in-the-task-list-gantt-chart}

이제 프로젝트의 작업이 간트 차트의 편집 모드로 표시될 때 다음 작업을 수행할 수 있습니다.

 작업 추가

작업 제거

작업 인라인 편집

작업 복제

작업 재배열

하위 작업 수정

변경 사항이 프로젝트의 타임라인에 어떻게 영향을 주는지 알 수 있지만 즉시 저장되지는 않습니다. 프로젝트 타임라인을 영구적으로 업데이트하도록 저장하거나 취소할 수 있습니다.

이전에는 간트 차트에서 작업 목록 변경 사항을 미리 볼 수 없었습니다.

간트 차트에서 작업을 편집하는 방법에 대한 자세한 내용은 &quot;작업 목록 간트 차트에서 정보 업데이트&quot;를 참조하십시오.

## 템플릿의 작업 목록 간트 차트 액세스 {#access-the-task-list-gantt-chart-on-templates}

이제 프로젝트 템플릿 내에서 작업 목록 간트 차트에 액세스할 수 있습니다.

이전에는 템플릿 내의 작업 목록에서 간트 차트를 볼 수 없었습니다.

자세한 내용은 &quot;간트 차트 시작&quot;을 참조하십시오.

## 간트 차트 내보내기를 위한 새로운 용지 크기 {#new-paper-sizes-for-gantt-chart-export}

이제 A1 및 A2 용지 크기로 간트 차트를 인쇄할 수 있습니다.

이전에는 Letter, Legal, Ledger, A3(일부 언어에만 사용 가능) 및 A4로만 내보낼 수 있었습니다.

자세한 내용은 &quot;간트 차트를 PDF으로 내보내기&quot;를 참조하십시오.

## 간트 차트에서 프로젝트 보기 이름이 변경됨 {#renamed-the-project-view-on-the-gantt-chart}

간트 차트에서 &quot;프로젝트&quot; 보기 옵션의 이름을 &quot;모두 맞추기&quot;로 변경했습니다. 보기 옵션은 여전히 이전과 동일하게 작동합니다. 새 이름은 옵션을 선택할 때 표시되는 내용에 대해 보다 설명적입니다.

자세한 내용은 &quot;간트 차트에서 정보 보기&quot;를 참조하십시오.

## 편집 모드에서 간트 차트의 대화 상자에 대한 액세스 권한 제거됨 {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

간트 차트가 편집 모드에 있는 동안에는 고급 할당 대화 상자에 더 이상 액세스할 수 없습니다. 작업 목록 간트 차트가 편집 모드에 있는 동안에는 인라인 편집만 수행할 수 있습니다.

이전에는 간트 차트가 편집 모드에 있는 동안 고급 할당 대화 상자에 액세스할 수 있었지만 간트 차트와 닫힌 편집 모드에서 변경 사항을 저장했습니다.

작업 목록 간트 차트 편집에 대한 자세한 내용은 &quot;작업 목록 간트 차트에서 정보 업데이트&quot;를 참조하십시오.

## 감사 로그 내보내기 {#export-audit-logs}

이제 감사 로그 항목을 CSV 파일로 내보낼 수 있습니다. 한 번에 최대 50,000개의 감사 로그 항목을 CSV 파일로 내보낼 수 있습니다.

자세한 내용은 &quot;감사 로그 관리&quot;를 참조하십시오.
