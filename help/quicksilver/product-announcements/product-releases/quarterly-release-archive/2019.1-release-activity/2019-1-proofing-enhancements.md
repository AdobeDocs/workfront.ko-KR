---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 증명 개선 사항
description: 이 페이지에서는 2019.1 릴리스에 포함된 모든 증명 개선 사항에 대해 설명합니다. 이제 프로덕션 환경에서 기능을 사용할 수 있습니다.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1 증명 개선 사항

이 페이지에서는 2019.1 릴리스에 포함된 모든 증명 개선 사항에 대해 설명합니다. 이제 프로덕션 환경에서 기능을 사용할 수 있습니다.

2019.1의 모든 변경 사항 목록은 을 참조하십시오. [2019.1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## 관리자용

* [증명을 여는 수신자가 아닌 사용자를 위한 기본 증명 역할 구성](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## 모든 사용자의 경우

* [웹 증명 뷰어의 증명 대화형 콘텐츠](#proof-interactive-content-in-the-web-proofing-viewer)
* [증명 뷰어의 주석에 대한 기본 정렬 순서는 이제 가장 오래된 항목에서 가장 늦은 항목입니다.](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [비디오 범위에 연결된 증명 뷰어의 댓글에 대한 검토 개선](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [증명 알림 또는 증명 뷰어에서 문서 세부 정보에 연결](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [증명 뷰어에서 이메일 알림 변경](#change-your-email-notifications-in-the-proofing-viewer)
* [Desktop Proofing Viewer에서 배경색 변경](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Desktop Proofing Viewer의 증명에서 캐시된 브라우저 데이터 지우기](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## 증명을 여는 수신자가 아닌 사용자를 위한 기본 증명 역할 구성 {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

이제 Workfront 관리자는 증명 워크플로의 지정 수신자가 아니지만 해당 Workfront 개체(예: 프로젝트, 작업 또는 문제)를 통해 증명에 액세스할 수 있는 사용자에 대해 기본 증명 역할을 구성할 수 있습니다.

이전에는 워크플로에 추가되지 않고 증명에 액세스할 수 있었던 사용자와 게스트의 기본 증명 역할이 검토자였습니다.

이 기능은 Workfront Proof가 아닌 Workfront에서 생성된 증명에만 적용됩니다.

## 웹 증명 뷰어의 증명 대화형 콘텐츠 {#proof-interactive-content-in-the-web-proofing-viewer}

조직의 보안 정책에서 독립형 Desktop Proofing Viewer 앱 사용을 허용하지 않는 경우 Workfront 관리자는 이제 웹 증명 뷰어에서 대화형 콘텐츠를 활성화할 수 있습니다. 증명을 만들기 전에 콘텐츠가 ZIP 파일에 번들로 제공되어야 합니다.

자세한 내용은 이 문서에서 를 참조하십시오.

비디오

## 증명 뷰어의 주석에 대한 기본 정렬 순서는 이제 가장 오래된 항목에서 가장 늦은 항목입니다.  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

언어 대화에서와 같이, 증명 뷰어에서 증명에 대한 댓글의 기본 정렬 순서는 이제 가장 오래된 항목부터 가장 늦은 항목까지 입니다.

이전에는 기본 정렬 순서가 가장 최근에서 가장 오래된 순으로 정렬되었습니다.

다른 정렬 옵션을 선택할 수 있으며, 이 옵션은 사용자가 연 다른 모든 증명에 대해 기억됩니다.

자세한 내용은 이 문서의 섹션을 참조하십시오.

## 비디오 범위에 연결된 증명 뷰어의 댓글에 대한 검토 개선 {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

이제 교정 뷰어에서 비디오 푸티지 범위와 관련된 주석을 검토할 때 재생 을 클릭하여 푸티지의 전체 범위를 볼 수 있습니다. 범위의 끝에 도달하면 재생이 일시 중지됩니다. 댓글은 열려 있으므로 현재 위치를 추적하지 못할 수 있습니다.

이전에는 비디오 푸티지 범위에 대한 주석을 열 때 [재생]을 클릭하기 전에 주석에 표시된 프레임 번호를 확인하여 수동으로 범위의 시작 부분을 찾아야 했습니다. 그렇지 않은 경우, 증명 뷰어는 비디오 타임라인에서 마지막으로 클릭한 곳마다 재생을 시작했으며 범위 끝에서 일시 중지되지 않았습니다. 또한 [재생]을 클릭하면 주석이 축소되므로 더 이상 어떤 주석을 검토하는지 명확하지 않습니다.

비디오 증명 검토에 대한 자세한 내용은 을 참조하십시오.

비디오

## 증명 알림 또는 증명 뷰어에서 문서 세부 정보에 연결 {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

이제 증명을 검토하도록 초대하는 이메일을 받거나 증명 뷰어에서 증명을 검토하고 있을 때 증명에 대한 문서 세부 정보 페이지에 빠르게 액세스할 수 있습니다. 이 페이지에서 증명과 연결된 Workfront 개체(예: 작업, 프로젝트 또는 문제)를 볼 수 있습니다. 이를 통해 증명에서 수행해야 하는 작업을 이해하는 데 도움이 되는 컨텍스트를 제공합니다.

이 기능은 시스템에 추가하는 신규 사용자에 대해서만 작동할 수 있습니다. 이 문제는 일시적입니다.

자세한 내용은 문서 를 참조하십시오.

비디오

## 증명 뷰어에서 이메일 알림 변경 {#change-your-email-notifications-in-the-proofing-viewer}

이제 모든 증명 검토자가 증명에 대해 수신할 증명 알림을 지정할 수 있습니다. 이는 외부 이해 관계자와 협업할 때 특히 중요하다.

이전에는 증명 소유자 또는 트래픽 관리자만 증명에 추가한 검토자에 대해 증명 이메일 경고를 구성할 수 있었습니다. 외부 공동 작업자는 Workfront에 대한 필수 액세스 권한과 적절한 권한 수준이 없기 때문에 증명에 대해 받은 이메일 경고를 제어할 수 없습니다.

이러한 설정은 Workfront에서 구성할 수 있는 이메일 경고 설정과 별개입니다.

자세한 내용은 [증명 댓글 및 결정에 대한 알림 관리](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

비디오

## Desktop Proofing Viewer에서 배경색 변경 {#change-the-background-color-in-the-desktop-proofing-viewer}

이제 Desktop Proofing Viewer의 배경색을 기본색에 가까운 검정색에서 흰색으로 변경할 수 있습니다. 이렇게 하면 배경이 투명한 증명 콘텐츠를 더 쉽게 볼 수 있습니다.

자세한 내용은 [증명 뷰어 설정 구성](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

비디오

## Desktop Proofing Viewer의 증명에서 캐시된 브라우저 데이터 지우기 {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

브라우저의 쿠키 및 캐시 설정이 팝업과 같은 콘텐츠를 차단하도록 설정된 경우 Desktop Proofing Viewer에서도 이러한 차단 동작이 발생할 수 있으므로 검토자가 증명에서 팝업 콘텐츠를 보고 댓글을 달 수 없습니다.

이제 모든 콘텐츠가 Desktop Proofing Viewer에 나타나고 검토자가 이를 보고 댓글을 달 수 있도록 증명과 함께 저장할 수 있는 브라우저 캐시 데이터를 지울 수 있습니다.

자세한 내용은 [증명 뷰어 설정 구성](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

비디오
