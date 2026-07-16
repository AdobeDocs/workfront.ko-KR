---
product-area: documents
navigation-topic: approvals
title: 새 문서 버전 업로드 및 승인 요청
description: 새 문서 버전을 업로드하고 Adobe Workfront의 다른 사용자에게 승인을 요청할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 2%

---

# 새 문서 버전 업로드 및 승인 요청

이전 검토에서 문서가 &quot;작업 필요&quot;로 표시되어 있는 경우, 원본 문서에 새 버전을 업로드하고 다른 버전의 승인을 시작할 수 있습니다. 새 버전의 문서를 업로드하면 이전 버전이 잠깁니다.

새 버전의 파일 이름이 이전 버전의 파일 이름과 다른 경우 Workfront에 새 파일 이름으로 문서가 표시됩니다.

미결 승인이 있는 문서에 새 버전을 추가하면 이전 버전의 승인이 &quot;철회됨&quot;으로 표시됩니다. 일부 참가자가 아직 결정을 내리지 않았더라도 기존 승인 절차는 종료된다.

최신 문서 버전을 삭제하면 이전 버전이 잠긴 상태로 유지됩니다. 이전 버전을 편집해야 하는 경우 수동으로 잠금을 해제해야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 승인을 관리하는 모든 Workfront 패키지</p>
<p>Adobe 클라우드 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>요청 이상</p>
   <p>기여자 이상</p>
   <p>Frame.io 통합을 사용하는 경우 승인 워크플로를 만들려면 표준 라이선스가 있어야 합니다.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서와 연관된 객체에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## 드래그 앤 드롭을 사용하여 이전 문서 영역에 새 버전을 추가합니다.

조직이 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. Workfront 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소와 레거시 Workfront 저장소 간의 차이점](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)을 참조하십시오.

>[!NOTE]
>
>드래그 앤 드롭은 Internet Explorer에서 작동하지 않습니다.

문서에 대한 또 다른 검토 및 승인이 필요한 경우 Workfront에서 새 문서 버전을 만들 수 있습니다. 이전 참여자, 새 참여자 또는 두 가지 모두를 혼합하여 추가할 수 있습니다. 문서 세부 정보 페이지에서 이전 버전 및 참여자에 대한 정보를 볼 수 있습니다.

단일 단계 승인의 경우 기본적으로 요청 승인 대화 상자가 기본 모드로 열립니다. 고급 모드로 전환하여 다단계 승인 또는 병렬 경로를 구성합니다.

새 버전을 추가하고 승인을 요청하려면:

1. Workfront의 문서로 이동합니다.

1. 이전 문서 위에 새 파일을 끌어다 놓습니다. Workfront은 자동으로 새 버전을 만듭니다.

1. 문서 업로드가 완료되면 문서를 선택하여 문서 요약 패널을 엽니다. 버전 번호가 패널 맨 위에 나타납니다.

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 만들기**&#x200B;를 클릭합니다. **승인 요청** 대화 상자가 기본 모드에서 열립니다.

1. 승인 워크플로를 구성합니다. 필드 설명, 고급 모드 전환 및 병렬 경로 흐름은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

1. 이전 문서 버전에서 동일한 검토자와 승인자를 복사하려면 **복사**&#x200B;를 클릭합니다.
1. **승인 요청**&#x200B;을 클릭합니다.

   승인 워크플로가 시작되고 승인자는 새 문서 버전에 대한 승인이 필요하다는 알림을 받습니다. 이전 문서 버전이 잠기고 이전 버전에서 미결 승인이 철회됩니다.

## 드래그 앤 드롭을 사용하여 새 문서 영역에 새 버전을 추가합니다.

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

>[!NOTE]
>
>드래그 앤 드롭은 Internet Explorer에서 작동하지 않습니다.

문서에 대한 또 다른 검토 및 승인이 필요한 경우 Workfront에서 새 문서 버전을 만들 수 있습니다. 문서의 새 버전에 승인 워크플로를 추가할 수 있습니다.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

단일 단계 승인의 경우 기본적으로 요청 승인 대화 상자가 기본 모드로 열립니다. 고급 모드로 전환하여 다단계 승인 또는 병렬 경로를 구성합니다.

새 버전을 추가하고 승인을 요청하려면:

1. Workfront의 문서로 이동합니다.

1. 이전 문서 위에 새 파일을 끌어다 놓습니다. Workfront은 자동으로 새 버전을 만듭니다.

1. 문서 업로드가 완료되면 문서를 선택하여 요약 패널을 엽니다. 기본적으로 최신 버전의 문서가 선택되어 있습니다.

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 만들기**&#x200B;를 클릭합니다. **승인 요청** 대화 상자가 기본 모드에서 열립니다.

1. 승인 워크플로를 구성합니다. 필드 설명, 고급 모드 전환 및 병렬 경로 흐름은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

1. 이전 문서 버전에서 동일한 검토자와 승인자를 복사하려면 **복사**&#x200B;를 클릭합니다.
1. **승인 요청**&#x200B;을 클릭합니다.

   승인 워크플로가 시작되고 승인자는 새 문서 버전에 대한 승인이 필요하다는 알림을 받습니다. 이전 문서 버전이 잠기고 이전 버전에서 미결 승인이 철회됩니다.
