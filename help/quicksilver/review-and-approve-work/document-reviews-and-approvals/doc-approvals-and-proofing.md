---
product-area: documents
navigation-topic: approvals
title: 통합 승인 및 증명 함께 사용
description: 증명이 포함된 통합 승인을 사용할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 0%

---

# 통합 승인 및 증명 함께 사용

Workfront의 통합 승인에는 문서를 검토하고 승인하는 데 도움이 되는 새로운 기능 세트가 도입되었습니다. 기존 증명 뷰어와 함께 통합 승인 워크플로를 사용하여 검토 중인 문서에 주석 및 마크업을 추가할 수 있습니다.

통합 승인과 증명을 함께 사용할 때 워크플로에는 다음과 같은 몇 가지 주요 차이점이 있습니다.

* 참가자는 증명 워크플로가 아니라 문서 요약에 표시됩니다.

* 문서 목록의 전송됨, 열림, 주석, 결정(SOCD) 세부 사항은 증명 관련이며 문서의 결정 상태를 반영하지 않습니다.

## 문서 업로드 및 증명 만들기

1. 새 문서를 추가할 프로젝트, 작업 또는 문제로 이동합니다.
1. **문서** 탭을 클릭한 다음 **새로 추가** 드롭다운 메뉴를 클릭합니다.
또는
문서를 문서 목록으로 드래그 앤 드롭합니다.

   >[!NOTE]
   >
   >사용자 프로필에 **문서를 업로드할 때 자동으로 증명 생성**&#x200B;이 활성화되어 있으면 간단한 증명이 자동으로 만들어집니다.

1. 문서 위로 마우스를 가져간 다음 문서 이름 아래에 나타나는 **증명 만들기** 링크를 클릭하고 **단순 증명**&#x200B;을 선택합니다. 승인에 증명 워크플로를 사용하지 않으므로 간단한 증명을 만들어야 합니다.

참여자로 할당된 사용자는 증명 뷰어를 사용하여 문서에 주석 및 마크업을 추가할 수 있습니다. 다음 섹션으로 이동하여 검토 참여자를 추가하는 방법을 알아보십시오.

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 요약 문서를 열고 참여자 할당

단일 단계 승인의 경우 기본적으로 요청 승인 대화 상자가 기본 모드로 열립니다. 고급 모드로 전환하여 다단계 승인 또는 병렬 경로를 구성합니다.

참여자를 지정하려면

1. 업로드한 문서를 선택하고 문서 요약을 엽니다.

   ![문서 요약 열기](assets/open-doc-summary.png)

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 만들기**&#x200B;를 클릭합니다. **승인 요청** 대화 상자가 기본 모드에서 열립니다.

1. 승인 워크플로를 구성합니다. 필드 설명, 고급 모드 전환 및 병렬 경로 흐름은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

1. **승인 요청**&#x200B;을 클릭합니다. 참가자에게는 이메일을 통해 알림이 전송됩니다.

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 필요에 따라 새 버전 만들기

한 차례의 검토 및 승인이 필요한 경우 새 증명 버전을 만들고 이전 참여자, 새 참여자 또는 두 참여자의 조합을 추가할 수 있습니다. 요약 문서에서 이전 버전 및 참여자에 대한 정보를 볼 수 있습니다.

단일 단계 승인의 경우 기본적으로 요청 승인 대화 상자가 기본 모드로 열립니다. 고급 모드로 전환하여 다단계 승인 또는 병렬 경로를 구성합니다.

새 버전을 추가하려면 다음을 수행하십시오.

1. Workfront의 이전 문서 위에 새 파일을 끌어다 놓습니다. Workfront은 자동으로 새 버전을 만듭니다.

1. 문서 업로드가 완료되면 문서를 선택한 다음 **증명 만들기** > **단순 증명**&#x200B;을 클릭합니다.

1. 문서를 다시 선택하고 문서 요약을 엽니다.

   ![문서 요약 열기](assets/open-doc-summary.png)

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 만들기**&#x200B;를 클릭합니다. **승인 요청** 대화 상자가 기본 모드에서 열립니다.

1. 승인 워크플로를 구성합니다. 필드 설명, 고급 모드 전환 및 병렬 경로 흐름은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

1. **승인 요청**&#x200B;을 클릭합니다. 참가자에게는 이메일을 통해 알림이 전송됩니다.

## 증명 검토 및 결정

지정된 모든 승인자가 &quot;승인됨&quot;을 선택할 때까지 문서가 승인됨 상태로 이동하지 않습니다.

문서를 검토하고 승인하려면 다음과 같이 하십시오.

1. 리뷰 전자 메일 알림으로 이동한 다음 **리뷰로 이동**&#x200B;을 클릭합니다.

1. Workfront에 있으면 **증명으로 이동**&#x200B;을 클릭하세요.

1. 콘텐츠를 검토하고 주석 또는 마크업을 추가합니다. 증명 뷰어를 사용하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 증명 검토: 문서 인덱스](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.

1. 다음 결정 중 하나를 선택합니다.

   * **승인**: 문서를 변경할 필요가 없으며 사용할 준비가 되었습니다.
   * **변경 사항과 함께 승인**: 문서를 변경해야 하며, 문서를 사용할 준비가 되었습니다. 추가 승인이 필요하지 않습니다.
   * **작업 필요**: 문서를 변경해야 하며 사용할 준비가 되지 않았습니다. 지정된 변경 사항이 적용되면 문서를 새 버전으로 업로드하고 다른 승인을 거쳐야 합니다. 새 버전을 업로드하는 방법에 대한 자세한 내용은 이 문서에서 [필요에 따라 새 버전 만들기](#create-a-new-version-as-needed)를 참조하십시오.

결정을 내리면 문서 소유자에게 이메일을 통해 알림이 전송됩니다.