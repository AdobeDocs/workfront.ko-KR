---
title: 21.3 프로젝트 개선 사항
description: 21.3 프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 프로젝트 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.3 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 7월 21일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

21.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [21.3 릴리스 개요](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md)를 참조하십시오.

## 그룹과 템플릿 연결

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

프로젝트 생성 프로세스를 간소화할 수 있고 프로젝트 템플릿을 소유한 그룹을 보다 쉽게 식별하고 보고할 수 있도록 프로젝트 템플릿에 그룹을 할당하는 기능을 추가했습니다.

프로젝트 템플릿에 그룹을 할당하면 템플릿에서 만든 모든 프로젝트가 템플릿의 그룹에 자동으로 연결됩니다. 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하세요.

또한 템플릿이 그룹과 연결되어 있는 경우 그룹 승인 프로세스를 템플릿과 해당 템플릿 작업에 첨부할 수 있습니다. 자세한 내용은 [새 승인 프로세스 또는 기존 승인 프로세스와 작업 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 세부 정보 섹션의 필드를 보다 쉽게 편집할 수 있습니다.

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

다음과 같은 개선 사항을 통해 객체의 세부 정보 섹션에서 정보를 보다 쉽게 편집할 수 있습니다.

* 마우스를 필드 위로 가져가면 필드 주위에 회색 윤곽선이 표시되어 편집할 수 있음을 나타냅니다.
* 필드를 한 번 클릭하여 편집할 수 있습니다.

이 개선 사항 이전에는 편집할 수 있는 필드가 명확하지 않았으며 필드를 편집하려면 더블 클릭해야 했습니다.

## 전달 날짜를 계산할 때 프로젝트 간 전임 작업 고려

Adobe Workfront이 작업에 대한 전달 날짜를 계산하는 방식을 새롭게 개선하면 프로젝트 간 종속성이 고려됩니다.

이전에는 동일한 프로젝트의 작업에 대한 선행 작업만 기준으로 전달 날짜가 계산되었습니다.

이제 프로젝트 간 전임 작업이 있는 작업에 대해 정확한 전달 날짜를 항상 확보하려면 후속 작업의 프로젝트 타임라인을 다시 계산해야 합니다. 타임라인을 다시 계산한 후 작업의 전달 날짜는 작업의 프로젝트 간 종속성을 고려하여 계산됩니다.

전달 날짜에 대한 자세한 내용은 [작업 전달 날짜 개요](../../../manage-work/tasks/task-information/handoff-task-date.md)를 참조하십시오.

## 스크럼 보드에서 기존 스토리 및 문제 추가

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 스크럼 보드에서 직접 기존 스토리 또는 문제를 추가할 수 있습니다. 이렇게 하면 백로그 페이지로 이동할 필요 없이 기존 스토리를 현재 반복에 더 쉽게 추가할 수 있습니다.

자세한 내용은 [스크럼 보드에서 스토리 및 문제 추가](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)를 참조하십시오.

## 스크럼 보드에서 새 스토리 및 문제 추가

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 스크럼 보드에서 직접 새 스토리 또는 문제를 만들 수 있습니다. 이렇게 하면 현재 반복에 새 스토리를 더 쉽게 추가할 수 있습니다.

자세한 내용은 [스크럼 보드에서 스토리 및 문제 추가](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)를 참조하십시오.

## 칸반 보드에서 스토리 또는 문제 삭제

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 스토리 또는 문제 카드에서 자세히 아이콘을 클릭하고 삭제를 선택하여 Kanban 보드에서 직접 스토리 또는 문제를 삭제할 수 있습니다. 스토리나 문제를 삭제하면 30일 동안 휴지통으로 이동되며 시스템 관리자만 복구할 수 있습니다.

자세한 내용은 [Kanban 보드에서 스토리 또는 문제 삭제](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)를 참조하십시오.

## 애자일 카드 헤더 및 스토리 보드 업데이트

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 Kanban 및 Scrum 보드에서 다음과 같은 개선 사항을 사용할 수 있습니다.

* 스토리 카드와 보드 열에는 고정된 너비가 있으므로 브라우저 창 크기를 조정할 경우 카드 크기가 변경되지 않습니다.
* [스토리] 열의 이름이 [상위 스토리]로 변경되었습니다.
* 각 카드에는 상위 스토리, 하위 작업(상위 스토리와 연계됨), 스토리(상위 스토리와 연계되지 않음) 또는 문제로 식별할 수 있는 레이블이 맨 위에 있습니다.
* 배경 음영은 열을 시각적으로 구분합니다.

자세한 내용은 [반복 개요](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md)를 참조하십시오.

## 그룹 프로젝트, 작업 및 문제 환경 설정

앞에서 설명한 대로 2021년 6월 24일까지 단계적으로 프로젝트, 작업 및 문제 환경 설정에 대한 그룹 수준 사용자 지정을 롤아웃했습니다. 이제 롤아웃이 완료되었으며 모든 고객을 위한 프로덕션에서 사용할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 외부 사용자가 문서를 승인하도록 허용

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 외부 이메일 주소를 사용하여 새 Workfront 환경의 문서에 승인자를 할당할 수 있습니다.

이전에는 Workfront Classic에서만 이메일 주소로 외부 사용자를 추가할 수 있었습니다.

자세한 내용은 [문서 승인 요청](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)을 참조하세요.

## 포트폴리오 또는 프로그램의 세부 정보 섹션에서 정보 내보내기

>[!NOTE]
>
>이 기능은 2021년 5월 20일에 미리보기 환경에 릴리스되었습니다. 프로덕션 환경에 2021년 6월 3일에 릴리스됩니다.

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

이제 포트폴리오 및 프로그램의 세부 정보 섹션에서 .pdf 파일 정보를 내보낼 수 있습니다. 이 개선 이전에는 프로젝트, 작업 및 문제에서만 세부 정보 섹션의 정보를 내보낼 수 있었습니다.

개체에서 사용자 정의 양식을 내보내는 방법에 대한 자세한 내용은 [사용자 정의 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)를 참조하십시오.

## 개체 헤더에 계획된 완료 일자 타임스탬프가 추가되었습니다.

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

간편한 액세스와 편리성 및 정확성을 위해 프로젝트, 작업 또는 문제 헤더의 계획된 완료 일자에서 타임스탬프를 선택하는 옵션을 추가했습니다.

이 개선 이전에는 개체의 계획된 완료 일자 를 업데이트할 때 Workfront에서 자정을 기본 시간으로 선택했습니다. 이제 완료 날짜와 시간을 사용자 지정할 수 있습니다.

새 Workfront 경험의 개체 헤더에 대한 자세한 내용은 [새 개체 헤더](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)를 참조하십시오.

## 사용자 정의 양식을 편집하지 않고 오브젝트에 추가

>[!NOTE]
>
>이 기능은 새로운 Adobe Workfront 환경에서만 사용할 수 있습니다.

다른 사용자가 작성하거나 나중에 작성하게 될 사용자 정의 양식을 오브젝트에 더 쉽게 추가할 수 있도록 했습니다. 양식을 추가할 때 양식이 더 이상 자동으로 편집 모드로 전환되지 않습니다. 빈 양식을 오브젝트에 저장할 수 있습니다.

이전에는, 사용자 정의 양식을 오브젝트에 추가할 때 페이지가 편집 모드로 전환되어 해당 오브젝트에 저장하기 전에 양식의 필수 필드를 작성해야 했습니다. 이는 다른 사용자가 양식을 작성해야 할 때 또는 양식의 필수 필드에 무엇을 입력해야 하는지 아직 알 수 없는 경우 불편했습니다.

개체에 사용자 정의 양식을 추가하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

