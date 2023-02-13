---
title: 21.3 프로젝트 개선 사항
description: 21.3 프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 프로젝트 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.3 릴리스로 수행된 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 7월 21일이 있는 프로덕션 환경에서 사용할 수 있었습니다.

21.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.3 릴리스 개요](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## 그룹과 템플릿 연결

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

프로젝트 생성 프로세스를 간소화할 수 있도록, 그리고 프로젝트 템플릿을 소유하는 그룹을 보다 쉽게 식별하고 보고할 수 있도록 돕기 위해 프로젝트 템플릿에 그룹을 할당하는 기능을 추가했습니다.

프로젝트 템플릿에 그룹을 지정하면 템플릿에서 만든 모든 프로젝트가 자동으로 템플릿 그룹과 연결됩니다. 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

또한 템플리트와 그룹과 연관된 경우 템플리트 및 템플리트 태스크에 그룹 승인 프로세스를 첨부할 수 있습니다. 자세한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 세부 사항 섹션에서 필드를 더 쉽게 편집할 수 있습니다

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

다음 개선 사항을 통해 객체의 세부 정보 섹션에서 정보를 보다 쉽게 편집할 수 있습니다.

* 마우스로 필드 주위에 있는 회색 윤곽선은 편집할 수 있음을 나타냅니다.
* 필드를 한 번 클릭하여 편집할 수 있습니다.

이러한 개선 사항 전에 어떤 필드를 편집할 수 있었는지 필드를 편집하려면 두 번 클릭해야 했는지 알 수 없습니다.

## 핸드오프 날짜를 계산할 때 프로젝트 간 선행 작업을 고려하십시오

Adobe Workfront이 작업의 핸드오프 날짜를 계산하는 방식이 새롭게 향상되면서 이제 프로젝트 간 종속성이 고려됩니다.

이전에는 동일한 프로젝트의 작업 선행 작업만 기준으로 핸드오프 날짜가 계산되었습니다.

이제, 프로젝트 간 전임자가 있는 작업에 대해 항상 정확한 핸드오프 날짜가 되도록 하려면 후속 작업 프로젝트의 타임라인을 다시 계산해야 합니다. 타임라인을 다시 계산한 후 작업의 전달 날짜는 작업의 프로젝트 간 종속성을 고려하여 계산됩니다.

핸드오프 날짜에 대한 자세한 내용은 [작업 핸드오프 날짜 개요](../../../manage-work/tasks/task-information/handoff-task-date.md).

## 스크럼 보드에서 기존 스토리 및 문제 추가

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 스크럼 보드에서 직접 기존 스토리나 문제를 추가할 수 있습니다. 따라서 백로그 페이지로 이동할 필요 없이 현재 반복에 기존 스토리를 더 쉽게 추가할 수 있습니다.

자세한 내용은 [스크럼 보드에서 이야기와 문제 추가](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Screm 보드에서 새 스토리 및 문제 추가

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 Screm 보드에서 직접 새로운 스토리나 문제를 만들 수 있습니다. 이렇게 하면 현재 반복에 새 스토리를 쉽게 추가할 수 있습니다.

자세한 내용은 [스크럼 보드에서 이야기와 문제 추가](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 간판 보드에서 스토리 또는 문제 삭제

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 스토리 또는 발행 카드에서 자세히 아이콘을 클릭하고 삭제를 선택하여 간판 보드에서 스토리를 삭제하거나 직접 발행할 수 있습니다. 스토리나 문제를 삭제하면 30일 동안 휴지통으로 이동되며 시스템 관리자만 복구할 수 있습니다.

자세한 내용은 [간판 보드에서 스토리 또는 문제 삭제](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## 애자일 카드 헤더 및 스토리 보드 업데이트

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 간판 및 스크럼 보드에서 다음과 같은 개선 사항을 사용할 수 있습니다.

* 스토리 카드와 보드 열은 너비가 고정되어 있으므로 브라우저 창 크기를 조정해도 카드 크기가 변경되지 않습니다.
* 스토리 열의 이름이 상위 스토리로 변경되었습니다.
* 각 카드에는 상위 스토리, 하위 작업(상위 스토리와 연관된), 스토리(상위 스토리와 연결되지 않은) 또는 문제로 식별하기 위한 레이블이 맨 위에 있습니다.
* 배경 음영은 열을 시각적으로 나눕니다.

자세한 내용은 [반복 개요](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## 프로젝트, 작업 및 문제 환경 설정 그룹화

앞서 설명했듯이 프로젝트, 작업 및 문제 환경 설정에 대한 그룹 수준 사용자 지정을 2021년 6월 24일까지 단계별로 배포했습니다. 이제 롤아웃이 완료되었으며 모든 고객이 프로덕션 환경에서 사용할 수 있습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 외부 사용자가 문서를 승인할 수 있도록 허용

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 외부 이메일 주소를 사용하여 새로운 Workfront 환경의 문서에 승인자를 할당할 수 있습니다.

이전에는 Workfront Classic에서 이메일 주소로만 외부 사용자를 추가할 수 있었습니다.

자세한 내용은 [문서 승인 요청](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 포트폴리오 또는 프로그램의 세부 정보 섹션에서 정보를 내보냅니다.

>[!NOTE]
>
>이 기능은 2021년 5월 20일 미리 보기 환경에 릴리스되었습니다. 프로덕션 환경은 2021년 6월 3일에 릴리스됩니다.

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 포트폴리오 및 프로그램의 세부 정보 섹션에서 .pdf 파일 정보로 내보낼 수 있습니다. 이 개선 사항 전에 프로젝트, 작업 및 문제에서만 세부 사항 섹션의 정보를 내보낼 수 있습니다.

개체에서 사용자 지정 양식 내보내기에 대한 내용은 [사용자 지정 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 객체 헤더에 계획된 완료 날짜 타임스탬프가 추가되었습니다.

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

액세스 편의성 및 정확성을 높이기 위해 프로젝트, 작업 또는 문제 헤더의 계획 완료 날짜에 타임스탬프를 선택하는 옵션을 추가했습니다.

이 개선 사항 전에 개체의 계획 완료 날짜를 업데이트하면 Workfront에서 자정을 기본 시간으로 선택했습니다. 이제 시간 및 완료 날짜를 사용자 지정할 수 있습니다.

새 Workfront 환경의 개체 헤더에 대한 자세한 내용은 [새 개체 머리글](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## 사용자 지정 양식을 편집하지 않고 개체에 추가합니다

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

다른 사용자가 채우거나 나중에 작성할 사용자 지정 양식을 개체에 더 쉽게 추가할 수 있도록 했습니다. 양식을 추가할 때 양식이 더 이상 자동으로 편집 모드로 전환되지 않습니다. 빈 양식을 개체에 저장하면 됩니다.

이전에는 사용자 지정 양식을 개체에 추가할 때 페이지가 편집 모드로 전환되어 양식에 있는 필수 필드를 모두 완료해야 객체에 저장할 수 있었습니다. 양식을 다른 사용자가 채우도록 했거나 양식에 필수 필드를 어떻게 입력해야 하는지 아직 모를 때 이러한 번거로움이 수정되었습니다.

개체에 사용자 지정 양식 추가에 대한 자세한 내용은 [개체에 사용자 지정 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

