---
title: 2026년 4분기 문서 개선 사항
description: 2026년 4분기 문서 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 5e13c944ac485a6999dd0a788cfbb0f5d5169742
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 0%

---

# 2026년 4분기 문서 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 4분기 릴리스의 문서 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)를 참조하십시오.

<!--

## System Administrators full access to approval templates

>[!NOTE]
>
>Preview: September 4, 2026
>Production fast release: September 4, 2026
>Production for everyone: September 4, 2026
>[!BADGE Off schedule]{type=Neutral}

System Administrators can now view, edit, delete, and bulk-delete every approval template in the account, regardless of who created or shared it. Previously, System Administrators were subject to the same sharing rules as other users, and could only see or manage templates they created or that were shared with them.

For more information, see [Manage approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

-->

## Workfront의 프레임 주석 가시성

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

문서에 대한 승인 워크플로가 만들어지면 사용자는 Frame.io 뷰어에 주석을 달고 댓글을 달 수 있습니다. 이러한 주석은 Workfront 주석 패널에 표시되지 않지만 Frame.io 뷰어에서 볼 수 있습니다.

이제 Workfront의 [주석] 패널에 Frame.io에서 새 주석을 사용할 수 있을 때를 알려주는 메시지가 표시됩니다.

자세한 내용은 [문서에 업데이트 추가](/help/quicksilver/documents/managing-documents/add-update-documents.md)를 참조하십시오.

## 승인 이메일 링크에서 직접 증명 액세스

>[!NOTE]
>
>미리보기: 해당 사항 없음
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

문서에 증명이 첨부되면 이제 승인 이메일의 &quot;검토로 이동&quot; 링크에 증명 뷰어가 직접 열리므로 검토자와 승인자는 즉시 검토를 시작할 수 있습니다. 문서에 증명이 없는 경우 이전과 마찬가지로 링크가 문서의 승인 섹션을 계속 엽니다.

## Adobe 클라우드 스토리지를 사용하여 오브젝트 승인에 팀 추가

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

이제 각 사용자를 개별적으로 추가하는 대신 문서 승인 또는 승인 템플릿에서 Workfront 팀을 승인자 또는 검토자로 추가할 수 있습니다.

* Adobe 클라우드 스토리지의 오브젝트: Workfront은 각 활성 팀 구성원을 개별적으로 추가하므로 승인자 목록은 항상 현재 팀에 있는 사람을 반영합니다.
* 기존 Workfront 저장소를 사용하는 개체: 기본적으로 팀이 단일 참가자로 추가되지만, 이제 각 팀 구성원을 개별 참가자로 추가하도록 선택할 수 있습니다.
* 승인 템플릿에서 Workfront은 팀에 대한 참조를 저장하고 템플릿을 저장할 때가 아니라 문서에 템플릿을 적용할 때 이를 활성 멤버로 확장합니다.

자세한 내용은 다음 문서를 참조하십시오.

* [새 문서 영역에 승인 작업 과정 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [기존 문서 영역에 승인 작업 과정 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [문서에 대한 승인 워크플로 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## 프로젝트 템플릿에서 Frame.io 작업 공간 설정

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

조직에서 Adobe 클라우드 스토리지를 사용하고 Frame.io Enterprise 라이선스가 있는 경우 이제 프로젝트 템플릿의 프로젝트 세부 정보에서 Frame.io 작업 영역을 선택할 수 있습니다. 템플릿에서 만든 프로젝트는 자동으로 템플릿에 설정된 작업공간을 사용하므로 프로젝트를 만들 때 추가 작업 없이 원하는 Frame.io 작업공간으로 프로젝트가 라우팅됩니다.

새 필드에는 프로젝트를 할당할 수 있는 권한이 있는 Frame.io 작업 공간이 나열됩니다. 필드는 언제든지 템플릿에서 편집할 수 있습니다. 변경 사항은 업데이트 후 생성된 프로젝트에만 적용되므로 기존 프로젝트는 원래 작업 영역을 유지합니다.

템플릿에서 프로젝트가 생성되면 해당 Frame.io 작업 영역 필드는 읽기 전용이며 Frame.io의 작업 영역에 연결됩니다.

Frame.io 엔터프라이즈 라이센스가 없는 경우 프로젝트는 Workfront의 기본 작업 영역으로 계속 이동합니다.

자세한 내용은 [프로젝트 템플릿 편집](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) 및 [프로젝트 개요 영역의 정보 관리](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md)를 참조하십시오.

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

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

## 이메일 제목 줄의 사용자 지정 메시지

>[!NOTE]
>
>미리보기: 해당 사항 없음
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

문서 승인에 대해 사용자 정의 메시지를 설정하면 이제 해당 메시지가 승인 요청 이메일의 제목 줄에도 표시되며, 기한을 설정할 때 해당 기한이 표시됩니다. 이렇게 하면 검토자가 이메일을 열지 않고도 받은 편지함에서 직접 관심이 필요한 항목을 확인할 수 있습니다.

자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

## 새 문서 영역에 다시 디자인된 버전 패널

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 새 문서 영역의 버전 패널에 새로운 디자인이 제공됩니다.

* 버전은 Frame.io와의 일관성을 유지하기 위해 V1, V2 등으로 레이블이 지정됩니다.
* 각 버전은 &quot;승인됨&quot; 또는 &quot;철회됨&quot;과 같은 승인 상태를 목록에 바로 표시합니다.
* 이제 패널에 버전 기록만 나열됩니다. 맨 위에는 더 이상 별도의 &quot;최신 파일&quot; 항목이 없습니다.

이전에는 번호가 매겨지지 않고 버전이 타임스탬프로 표시되었습니다.

자세한 내용은 [문서 버전 관리](/help/quicksilver/documents/managing-documents/manage-document-versions.md)를 참조하십시오.

## 새 문서 영역에서 다시 디자인된 승인 패널

>[!NOTE]
>
>미리 보기: 2026년 9월 3일
>프로덕션 빠른 릴리스: 2026년 9월 17일
>모두를 위한 프로덕션: 2026년 10월 15일

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 이제 새 문서 영역의 승인 패널에 버전 간 승인 내역이 표시됩니다.

* 패널에는 현재 버전뿐만 아니라 버전이 하나씩인 모든 버전에 대한 승인 워크플로가 나열됩니다.
* 철회된 워크플로우는 목록에 유지되므로 이전 결정을 검토할 수 있습니다.
* 버전을 확장하여 패널을 종료하지 않고 단계, 승인자 결정, 결정 규칙 및 기한을 확인합니다.

이전에는 승인 패널에만 현재 버전의 워크플로가 표시되었습니다.

자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

## Adobe 클라우드 스토리지 개체의 댓글에 이미지 첨부

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 7월 30일
>모두를 위한 프로덕션: 2026년 7월 30일
>[!BADGE 일정 해제]{type=Neutral}

이제 Adobe 클라우드 스토리지를 통합 검토 및 승인의 일부로 사용하는 조직은 추적 가능한 단일 주석 스레드에서 이미지 파일을 주석에 직접 첨부하여 피드백, 컨텍스트 및 지원 비주얼을 함께 유지할 수 있습니다. 이로써 기존 Workfront 스토리지의 조직만 주석에 이미지를 첨부할 수 있었던 이전 공백이 해결됩니다.

이제 모든 미디어 유형 이미지 형식이 Adobe 클라우드 스토리지 조직에서 지원됩니다. 이전 개체 주석은 .jpg, .gif 및 .png 파일만 계속 지원합니다. 이미지가 아닌 파일은 기존 또는 Adobe 클라우드 스토리지 개체에 대한 주석에서 지원되지 않습니다.

자세한 내용은 [작업 업데이트](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하세요.

## Experience Manager Assets의 자산을 Adobe 클라우드 스토리지와 연결

>[!NOTE]
>
>미리 보기: 2026년 7월 30일
>프로덕션 빠른 릴리스: 2026년 8월 13일
>모두를 위한 프로덕션: 2026년 10월 15일

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Experience Manager Assets의 개별 에셋을 문서를 지원하는 모든 Workfront 개체에 연결할 수 있습니다. 연결된 컨텐츠는 자동으로 동기화 상태를 유지합니다. Experience Manager Assets에서 변경한 사항이 Workfront에 표시되며, Workfront에서 나가지 않고 새 에셋 버전을 가져올 수 있습니다.

연결은 콘텐츠 관리자를 통해 제공되므로 콘텐츠를 선택하는 동안 AI 검색, 스마트 제안, 캠페인 개요 분석 등을 받을 수도 있습니다.

자세한 내용은 [Experience Manager Assets의 콘텐츠를 Adobe 클라우드 저장소와 연결](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md)을 참조하십시오.

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

