---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 프로젝트 개선 사항
description: 이 페이지에서는 2020.1 릴리스의 프로젝트에 대한 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 현재 미리보기 환경에서 사용할 수 있으며 2020년 3월 말 또는 4월 초에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 2020.1 프로젝트 개선 사항

이 페이지에서는 2020.1 릴리스의 프로젝트에 대한 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 현재 미리보기 환경에서 사용할 수 있으며 2020년 3월 말 또는 4월 초에 프로덕션 환경에서 사용할 수 있습니다.

2020.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 [2020.1 릴리스 개요](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)를 참조하십시오.

## 업데이트에서 태그가 지정된 사용자를 보다 쉽게 확인

이제 업데이트에서 태그가 지정된 사용자를 더 쉽게 볼 수 있습니다. 태그 지정된 사용자 이름은 파란색으로 표시되고 사용자 프로필에 연결됩니다.

태그 지정된 사용자는 주석 상자 아래에도 나열됩니다.

이 개선 전에는 이전에 태그 지정한 사용자가 알림 상자에 표시되지 않았습니다.

자세한 내용은 [업데이트에 다른 사용자 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

## 업데이트 댓글 또는 회신에 인용된 텍스트 포함 및 식별

주석을 입력할 때 주석의 일부를 인용된 텍스트로 표시하여 자신의 주석과 구분할 수 있습니다. HTML 편집기에서 견적 차단 버튼을 사용합니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.


## 업데이트 댓글 또는 회신에서 이전 댓글 인용

업데이트 스레드에서 댓글을 달면 스레드에 이전 댓글의 텍스트를 빠르게 포함할 수 있습니다. 견적을 작성할 설명 옆에 있는 기타 메뉴에서 견적 회신 옵션을 찾습니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## 추가 위험 정보

프로젝트의 위험을 더 잘 이해할 수 있도록 이제 위험이 입력된 사용자와 사용자, 그리고 프로젝트에서 위험이 업데이트된 시기를 확인할 수 있습니다. 위험 보기에서 공개 Workfront API를 통해 이 정보에 액세스할 수 있습니다. 이러한 필드는 2020.1 프로덕션과 함께 릴리스되는 API 버전 11에서 사용할 수 있습니다.

Workfront의 위험에 대한 자세한 내용은 [프로젝트에 대한 위험 만들기 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)을 참조하세요.

## 기준선 및 기준선 작업에 추가된 추가 필드

프로젝트의 재무 진행 상황을 더 잘 이해할 수 있도록 이제 기준선 작업 보고서나 기준선 작업 보고서에 추가 비용 및 수익 정보를 포함할 수 있습니다. 추가 재무 정보는 현재 저장한 베이스라인에 추가되지 않지만 새 베이스라인에 추가됩니다.

기준선 및 기준선 작업 개체에서 액세스할 수 있는 프로젝트 및 작업 재무 필드에 대한 자세한 내용은 [프로젝트 기준선에 포함된 프로젝트 재무](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md)을 참조하십시오.

## &quot;승인 보류 중 마감&quot; 상태의 문제는 불완전한 것으로 간주됩니다.

Workfront이 &quot;승인 보류 중&quot; 상태에서 문제를 처리하는 방법이 변경되었습니다. 이제 이러한 문제는 열림으로 인식되며 승인이 해결될 때까지 프로젝트를 완료로 표시할 수 없습니다.

이 변경 전에는 &quot;승인 보류 중 마감&quot; 상태의 문제가 마감으로 간주되었습니다.

이 변경 전에 마감됨 - 승인 보류 중 상태에 배치된 모든 문제는 이전에 수행한 것과 동일한 방식으로 작동하며, 완료된 것으로 간주되고 프로젝트도 완료할 수 있습니다. 이 변경 후에 이 상태에 배치되는 모든 문제는 불완전한 것으로 간주됩니다.

프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 목록에 액세스](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)를 참조하십시오.

