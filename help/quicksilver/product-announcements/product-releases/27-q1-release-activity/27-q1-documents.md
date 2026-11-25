---
title: 2027년 1분기 문서 개선 사항
description: 2027년 1분기 문서 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 86dd87865046a4f2dc75e13feb370e338bbf4c92
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%
---

# 2027년 1분기 문서 개선 사항

이 페이지에서는 미리보기 환경에 대한 2027년 1분기 릴리스의 문서 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2027년 1분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2027년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-release-overview.md)를 참조하십시오.

## Adobe Cloud Drive v1.2.0의 새로운 기능

>[!NOTE]
>
>미리 보기: 2026년 11월 25일
>프로덕션 빠른 릴리스: 2026년 11월 25일
>모두를 위한 프로덕션: 2026년 11월 25일
>[!BADGE 동시 릴리스]{type=Neutral}
>[!BADGE 워크플로우 Ultimate]{type=Informative}

Adobe Cloud Drive v1.2.0에는 파일을 업로드하고, 동기화를 관리하고, 클라우드 콘텐츠로 작업하는 새로운 방법이 도입되었습니다.

* **클라우드에 업로드(직접 업로드):** Finder 또는 파일 탐색기에서 파일을 마우스 오른쪽 단추로 클릭하여 Adobe 클라우드 저장소의 프로젝트에 직접 업로드합니다. 먼저 Adobe Cloud Drive 폴더로 복사하지 마십시오. 동기화 활동의 직접 업로드 섹션에서 진행 상황을 모니터링합니다.
* **동기화 일시 중지 및 다시 시작:** 느린 연결 또는 유료 연결에서 Adobe 클라우드 드라이브를 일시 중지한 다음 준비가 되면 다시 시작합니다.
* **버전 기록:** 저장된 클라우드 버전의 파일을 검색하고, 버전 이름 및 설명을 편집하고, 이전 버전으로 되돌립니다.
* **로컬 저장소 관리:** 로컬 디스크 사용을 모니터링하고, 저장소 제한을 설정하고, 이 장치에서 Always로 표시된 파일을 봅니다.
* **동기화 활동:** 최근 업로드, 다운로드 및 변경 내용을 검토하고 동기화할 수 없는 항목을 식별합니다.
* **Workfront에서 열기:** Finder, 파일 탐색기 또는 동기화 활동에서 직접 항목의 Workfront 위치를 엽니다.

자세한 내용은 [Adobe 클라우드 드라이브 사용](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md) 및 [Adobe 클라우드 드라이브 문제 해결](/help/quicksilver/documents/adobe-cloud-drive/troubleshoot-adobe-cloud-drive.md)을 참조하십시오.

<!--

## Delegate unified document approvals

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now delegate your unified document approvals to another user, who can approve, reject, or mark reviews complete on your behalf during the delegation period. Delegated decisions show both names in the approval workflow, so it's clear who made each decision.

Legacy document and proof approvals remain unsupported.

For more information, see [Delegate approval request](/help/quicksilver/review-and-approve-work/manage-approvals/delegate-approval-requests.md).

-->

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: November 5, 2026
>Production fast release: December 17, 2026
>Production for everyone: January 21, 2027

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

<!--

## Turn the Approved with changes decision on or off

>[!NOTE]
>
>Preview: November 5, 2026
>Production fast release: December 17, 2026
>Production for everyone: January 21, 2027

If your organization uses Adobe cloud storage, System Administrators can now turn the "Approved with changes" decision on or off for document approvals. When it's on, reviewers see three decisions (Approved, Approved with changes, and Needs Work) in both the Workfront approval interface and the Frame.io viewer. When it's off, reviewers see only Approved and Needs Work.

The setting lives on the Approval Settings page in Setup, and a live preview on that page shows exactly which decisions reviewers currently see.

For more information, see [Configure the Approved with changes decision](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/configure-approved-with-changes.md).

-->

## 통합 검토 및 승인 이메일 알림 구성


>[!NOTE]
>
>미리 보기: 2026년 11월 5일
>프로덕션 빠른 릴리스: 2026년 11월 12일
>모두를 위한 프로덕션: 2027년 1월 21일

이제 통합 검토 및 승인 이메일 알림을 구성할 수 있습니다. Workfront은 항상 이러한 이메일을 전송했지만 지금까지 구성할 수 없었습니다. 이제 통합 승인으로 그룹화되고 기본적으로 활성 상태인 알림이 18개 있습니다. Workfront 관리자는 설정 내의 모든 사용자에 대해 이러한 기능을 활성화하거나 비활성화할 수 있으며, 사용자는 프로필에서 이러한 기능을 관리할 수 있습니다.

이 업데이트의 일부로, 이러한 알림의 이메일 제목 줄이 약간 변경되었습니다. 제목 줄은 이제 &quot;{Document}에 승인이 필요합니다.&quot;와 같은 결과를 가져옵니다. 승인의 전체 결과에 대한 알림은 &quot;최종 결정&quot;으로 시작하므로 개별 승인자의 결정과 구별할 수 있습니다.

자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.
