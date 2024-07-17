---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3 릴리스 활동
description: 이 페이지에서는 2017.2 Beta 2 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 24일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 말에서 8월 초에 제공될 예정입니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# 2017.2 Beta 3 릴리스 활동

이 페이지에서는 2017.2 Beta 2 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 5월 24일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 7월 말에서 8월 초에 제공될 예정입니다.

>[!IMPORTANT]
>
>이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.2의 모든 변경 사항 목록은 [2017.2 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)를 참조하십시오.

2017.2 Beta 2 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

**관리자용:**

* [휴지통에서 항목을 대량으로 복원](#restoring-items-in-bulk-from-the-recycle-bin)
* [사용자 정보가 Workfront에서 ProofHQ(ProofHQ 및 Workfront)로 동기화됨](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**모든 사용자의 경우:** 

* [구독한 사용자 보기](#view-subscribed-users)
* [간트 차트에 마일스톤을 표시하는 방법 구성](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [PDF으로 내보낼 때 간트 차트 범례 포함](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [내 작업 영역(Workfront)에서 증명 승인 보기](#view-proof-approvals-in-the-my-work-area-workfront)
* [내 작업 영역(Workfront)에서 증명 승인 요청의 주소를 지정할 때 사용자 이름 보기](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [비디오 증명에 대한 증명 뷰어 개선(ProofHQ 및 Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [대체 해상도로 리치 미디어 증명 보기(ProofHQ 및 Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [문서 버전 보고서(Workfront)의 새 &#39;증명 작성자&#39; 개체](#new-proof-creator-object-in-document-version-report-workfront)
* [새 리소스 풀 기능이 미리 보기에서 일시적으로 제거됨](#new-resource-pool-functionality-temporarily-removed-from-preview)

## 휴지통에서 항목을 대량으로 복원 {#restoring-items-in-bulk-from-the-recycle-bin}

이제 삭제된 프로젝트, 작업, 문제 또는 문서를 한 번에 최대 10개까지 복원할 수 있습니다.

이 변경 이전에는 한 번에 하나의 삭제된 항목만 복원할 수 있었습니다.

항목 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)을 참조하세요.

## 구독한 사용자 보기 {#view-subscribed-users}

이제 구독 링크 옆에 표시되는 구독자의 수를 확장하여 항목에 구독하는 사용자를 확인할 수 있습니다.

이 개선 이전에는 항목을 구독하는 사용자를 볼 수 없었습니다.

항목 구독에 대한 자세한 내용은 [Adobe Workfront에서 항목 구독](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)을 참조하세요. 

## 간트 차트에 마일스톤을 표시하는 방법 구성 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

이제 간트 차트에서 마일스톤 정보를 볼 수 있는 두 가지 옵션이 있습니다. 다음 이정표 표시기 중 하나 또는 둘 다를 구성할 수 있습니다.

* 마일스톤 다이아몬드(아이콘)

  이 아이콘은 마일스톤과 연결된 작업 후에 간트 차트에 표시됩니다.

* 마일스톤 라인

  간트 차트의 모든 작업에 걸쳐 마일스톤과 연결된 작업 뒤에 선이 표시됩니다.

이 변경 이전에는 간트 차트에 &quot;마일스톤&quot;이라는 마일스톤을 표시할 수 있는 옵션이 하나만 있었습니다. 이 옵션을 사용하면 마일스톤 다이아몬드 아이콘과 마일스톤 라인이 모두 활성화됩니다. 이러한 지표는 분리할 수 없습니다.

간트 차트에 정보가 표시되는 방식을 구성하는 방법에 대한 자세한 내용은 [간트 차트에 정보가 표시되는 방식 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)을 참조하십시오.

## PDF으로 내보낼 때 간트 차트 범례 포함 {#include-the-gantt-chart-legend-when-exporting-to-pdf}

이제 간트 차트를 PDF으로 내보낼 때 차트 자체와 함께 차트의 범례도 내보내시겠습니까? 범례에 포함된 항목은 UI의 간트 차트에 표시되도록 활성화한 옵션입니다. 이러한 옵션은 프로젝트의 작업에 있는 경우 범례에 포함됩니다. 예를 들어 간트 차트에서 이정표를 표시하도록 활성화하면 범례에도 이정표가 표시되지만 이정표와 연관된 작업이 하나 이상 있는 경우에만 표시됩니다.

이 변경 이전에는 내보낸 PDF에서 범례를 제외할 수 없었고, 범례에는 간트의 사용 여부와 관계없이 가능한 모든 옵션과 마커가 포함되어 있었습니다.

간트 차트 내보내기에 대한 자세한 내용은 [PDF으로 간트 차트 내보내기](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)를 참조하십시오.

## 사용자 정보가 Workfront에서 ProofHQ(ProofHQ 및 Workfront)로 동기화됨 {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

이제 사용자 정보(이름 및 이메일)는 Workfront에서 사용자가 생성되거나 업데이트될 때 Workfront에서 ProofHQ로 동기화됩니다. 

Workfront에서 ProofHQ로의 사용자 동기화에 대한 자세한 내용은 을 참조하십시오.

## 문서 버전 보고서의 새 &#39;증명 작성자&#39; 개체(Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

이제 문서 버전 보고서를 만들 때 새 증명 작성자 개체가 있습니다. 이 개체를 사용하면 증명을 만든 사용자에 대한 정보를 보고할 수 있습니다. 

문서 버전 보고서의 새 증명 작성자 개체에는 다른 유형의 개체 보고서에서 기존 사용자 개체에서 사용할 수 있는 모든 필드가 포함되어 있습니다.

>[!NOTE]
>
> 이 정보는 이 기능이 각 미리보기 또는 프로덕션 환경에 처음 도입된 시점부터 보고서에서만 사용할 수 있습니다. 이 기능이 도입되기 전의 요청자 오브젝트와 관련된 보고서에 있는 정보는 사용할 수 없습니다.

[사용자 지정 보고서 만들기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)에 설명된 대로 문서 버전 보고서를 만들 때 증명 작성자 개체에 액세스합니다.

문서 버전 개체 보고서에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)의 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 섹션을 참조하십시오.

## 내 작업 영역에서 증명 승인 보기(Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

승인을 위해 제출한 모든 증명 승인이 이제 내 작업 영역의 **승인을 위해 제출한 작업** 탭에 표시됩니다.

이 변경 이전에는 **승인을 위해 제출한 작업** 탭에 증명 승인이 포함되지 않았습니다.

증명 승인은 다음 기준을 충족해야 표시됩니다.

* 승인은 현재 승인 보류 중입니다.
* 승인 프로세스는 허가된 Workfront 사용자인 사용자에게 할당됩니다(허가된 Workfront 사용자가 아닌 사용자에게 할당된 승인 프로세스는 표시되지 않음)
* 이 기능이 릴리스된 후 승인 프로세스가 시작되었습니다(이 기능이 릴리스되기 전에 조정된 승인 프로세스는 표시되지 않음).

자세한 내용은 [승인 보기](../../../../review-and-approve-work/manage-approvals/view-approvals.md)에서 [승인 보기](../../../../review-and-approve-work/manage-approvals/view-approvals.md)를 참조하십시오.

## 내 작업 영역(Workfront)에서 증명 승인 요청의 주소를 지정할 때 사용자 이름 보기 {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

이제 내 작업 영역에서 증명 승인을 승인할 때 승인을 요청한 사용자의 이름이 표시됩니다.

자세한 내용은 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md)에서 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md)을 참조하세요. 

## 비디오 증명에 대한 증명 뷰어 개선(ProofHQ 및 Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Workfront 및 ProofHQ의 증명 뷰어가 새로운 모양과 느낌, 향상된 성능을 위한 HTML5 아키텍처, 새로운 기능 지원을 통해 업데이트되고 있습니다.

새 증명 뷰어에는 다음과 같은 개선 사항이 포함되어 있습니다.

* 프레임별 교정
* 비디오 버퍼링
* 주석 목록의 검색 기능
* 주석에 설정된 모든 작업은 주석 목록의 각 주석에 표시됩니다
* 전체 화면 모드
* 더 빠른 콘텐츠 또는 더 느린 콘텐츠 검토
* 댓글 및 답글 추가 시 맞춤법 검사기

### 미리보기

새 증명 뷰어는 다음 미리보기 환경에서 테스트할 수 있습니다.

* ProofHQ 미리보기 환경

  ProofHQ 미리 보기 환경에 대한 자세한 내용은 [미리 보기 샌드박스 테스트 환경- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)을 참조하십시오.

* Workfront 미리보기 환경(계정이 교정을 통해 활성화된 경우)

  Workfront 미리보기 환경에 대한 자세한 내용은  [Adobe Workfront 미리 보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

이 릴리스에서는 새 증명 뷰어가 비디오 증명만 지원합니다. 즉, 모든 비디오 증명은 새 증명 뷰어를 활용하는 반면, 모든 정적 및 리치 미디어 증명은 기존 증명 뷰어를 계속 활용합니다.

### 프로덕션

17.2 릴리스로 프로덕션 환경에 릴리스된 경우 관리자는 새 증명 뷰어 또는 이전 증명 뷰어가 조직의 사용자에게 적합한지 여부를 선택할 수 있습니다. 기본적으로 기존 증명 뷰어가 사용됩니다.

새 비디오 증명 뷰어를 사용하는 방법에 대한 자세한 내용은  

## 대체 해상도로 리치 미디어 증명 보기(ProofHQ 및 Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

이제 사용자 지정 해상도를 지정하거나 이미지를 원하는 해상도로 드래그하여 리치 미디어 증명의 해상도를 조정할 수 있습니다.

이 변경 이전에는 콘텐츠를 검토하고 있던 화면 또는 장치에 고유한 해상도만 사용하여 증명을 검토할 수 있었습니다.

비교 모드를 사용하여 다양한 증명 해상도를 비교할 수 있습니다.

자세한 내용은 [데스크톱 증명 뷰어에서 증명 열기](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md)를 참조하십시오. 

## 새 리소스 풀 기능이 미리 보기에서 일시적으로 제거됨 {#new-resource-pool-functionality-temporarily-removed-from-preview}

개발 문제로 인해 새 리소스 계획 탭을 제거하고 레거시 리소스 계획 탭의 이름을 &quot;리소스 계획&quot;이라는 원래 이름으로 다시 바꾸기로 결정했습니다.

이 변경 사항으로 새 리소스 풀 기능도 제거되었습니다. 리소스 계획의 새 탭과 리소스 풀의 기능이 2017년 6월 말에 샌드박스 미리보기 환경으로 돌아갑니다.
