---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: 문서에 대한 요약 개요
description: The Summary allows you to interact with important information directly from the documents list.
author: Courtney
feature: Digital Content and Documents
exl-id: 7a4a4bd3-ad60-4d84-b4b0-332c2a4eb8fb
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 5%

---

# 문서에 대한 요약 개요

<!--Audited: April, 2024-->

You can use the Summary panel to access and update important information directly from the documents list.


+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 문서를 관리하는 모든 Workfront 패키지</p>
<p>Adobe 엔터프라이즈 스토리지를 사용하여 문서를 관리하는 모든 워크플로 패키지</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p> 
   <p>요청 이상</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p>  </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서와 연관된 객체에 대한 액세스 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Summary for documents in the legacy documents experience

조직이 기존 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. 기존 Workfront 스토리지에 대한 자세한 내용은 [기존 Workfront 스토리지와 Adobe 엔터프라이즈 스토리지의 차이점](/help/quicksilver/review-and-approve-work/esm-overview.md)을 참조하십시오.

### Open the Summary view in the legacy documents experience

{{step1-to-documents}}

1. **문서** 페이지에서 목록에서 문서를 선택합니다.

1. 페이지의 오른쪽 상단 모서리에서 **요약 열기** 아이콘 ![요약 열기 아이콘](assets/qs-summary-in-new-toolbar-small.png)을 클릭합니다. **문서 요약** 사이드 패널이 열립니다.

   ![Summary details](assets/document-summary-panel.png)

   After you open the Summary, it will remain open on this page (even if you click on other documents) until you manually close it.


### 세부 사항

Use the Details section to view high-level overview information and interact with custom forms. Click Details at the top of the section to go to the full Document Details page.

* [개요](#overview)
* [사용자 정의 양식](#custom-forms)

#### 개요 {#overview}

개요 섹션을 확장하여 이미지 썸네일을 보거나 다운로드하고, 증명을 열고, 기본 설명을 업데이트하고, 문서를 체크 아웃하는 등의 작업을 수행합니다.

![문서 요약 개요](assets/details-section.png)

#### 사용자 정의 양식 {#custom-forms}

사용자 정의 Forms 섹션을 사용하여 문서와 연결된 모든 사용자 정의 양식을 추가, 편집 또는 볼 수 있습니다. 사용자 정의 양식의 이름을 입력하여 문서에 추가하십시오. 자세한 내용은 [문서에 사용자 정의 양식 추가 또는 편집](../../documents/managing-documents/add-custom-form-documents.md)을 참조하십시오.

![문서 요약에 사용자 정의 양식 추가](assets/custom-forms-section.png)

### 업데이트

업데이트 섹션을 사용하여 문서 또는 증명에서 수행한 업데이트 내용을 볼 수 있습니다. 요약에는 처음 두 개의 주석이 표시됩니다. 업데이트에 대한 자세한 내용은 [증명에 대한 댓글](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md)을 참조하세요.

요약 패널의 ![업데이트 섹션](assets/updates-section.png)

### 승인

승인 섹션을 사용하여 문서 승인을 요청합니다. 승인에 대해 다른 사람에게 알리거나, 승인을 다시 제출하고, 이전 결정을 취소하거나, 승인을 삭제할 수도 있습니다. 문서 승인자는 요약을 사용하여 결정할 수 있습니다.

증명 워크플로에 증명 승인을 추가해야 합니다. 승인에 대한 자세한 내용은

* [작업 승인](../../review-and-approve-work/manage-approvals/approving-work.md)
* [문서 승인 요청](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

![문서 요약 승인](assets/approvals-section.png)

### 버전

버전 섹션을 사용하여 특정 문서에 대해 작성된 버전 수를 볼 수 있습니다. 자세히 아이콘 ![자세히 아이콘](assets/more-icon.png)을 클릭하여 다음을 수행합니다.

* 증명을 엽니다.
* 증명 또는 문서를 다운로드합니다.
* 브라우저에서 지원하는 문서를 미리 봅니다.
* 문서 세부 정보로 이동합니다.
* 증명 또는 문서를 삭제합니다.

![문서 요약 버전](assets/versions-section.png)

## Summary for documents in the new documents experience

조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 엔터프라이즈 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

### 세부 사항

Use the Details section to view high-level overview information and interact with custom forms.

![Document summary details in new documents experience](assets/summary-details.png)

### 승인

Use the Approvals section to create an approval workflow. You can also remind participants about an approval or delete the approval. Document approvers can access the Frame.io viewer or use the Summary to make a decision.

For more information about approvals and Frame.io, see

* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Create a document review or approval request](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

![Document summary approvals in new documents experience](assets/summary-approvals.png)


<!-- resubmit the approval and cancel the previous decision, or delete the approval. Document approvers can use the Summary to make a decision.-->


### 버전

버전 섹션을 사용하여 특정 문서에 대해 작성된 버전 수를 볼 수 있습니다. Click the More icon to do the following:

* Rename a version
* View document details
* Request approval on a specific version
* Frame.io에서 열기
* Download the version
* Share the version
* Delete the version

![Document summary versions in new documents experience](assets/summary-versions.png)

### 기록

Use the History section to view a list of all activities related to the document.

![Document summary history in new documents experience](assets/summary-history.png)