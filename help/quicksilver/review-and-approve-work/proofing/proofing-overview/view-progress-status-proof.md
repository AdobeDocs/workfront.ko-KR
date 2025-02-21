---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명 진행 상황 및 상태 개요
description: 검토 프로세스를 통해 증명이 진행되는 방식에 대한 정보를 확인하고 문서 영역에서 증명 결정 상태에 대한 전반적인 요약을 볼 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# 증명 진행 상황 및 상태 개요

검토 프로세스를 통해 증명이 진행되는 방식에 대한 정보를 확인하고 문서 영역에서 증명 결정 상태에 대한 전반적인 요약을 볼 수 있습니다.

## 증명 진행 개요

증명 진행률은 수신자에게 증명을 보낸 시점부터 증명에 대한 결정을 내릴 때까지 증명에 대한 작업이 완료됨을 나타냅니다. 진행률 아이콘 S, O, C 및 D가 증명 이름 옆에 나타나고 증명 진행률에 대한 정보를 제공합니다.

![기존 진행률을 편집하는 사용자](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>진행 아이콘</strong> </p> </td> 
   <td> <p><strong>설명</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>전송됨</strong> </p> </td> 
   <td> <p>지정된 수신자에게 증명이 전송되었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>열림</strong> </p> </td> 
   <td> <p>할당된 모든 수신자가 증명 또는 증명 세부 정보 페이지를 엽니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>댓글 작성</strong> </p> </td> 
   <td> <p>할당된 모든 수신자가 증명에 대해 하나 이상의 댓글을 남깁니다.</p> <p>증명에 할당된 검토자가 없으면 <strong>C</strong> 아이콘이 진행률 표시줄에 나타나지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>결정</strong> </p> </td> 
   <td> <p>모든 할당된 승인자는 증명에 대해 결정을 내리고, 증명 작성자가 하나의 결정만 필요하다고 지정하지 않는 한 모든 할당된 승인자는 증명에 대해 결정을 내립니다.</p> <p>증명에 대해 지정된 승인자(결정자)가 없는 경우 <strong>D</strong> 아이콘이 진행률 표시줄에 표시되지 않습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

진행률 아이콘은 다음 색상으로 표시되어 증명의 진행률에 대한 특정 정보를 나타낼 수 있습니다.

* **녹색**: 완료되었습니다.
* **흰색**: 완료되지 않았습니다.
* **주황**: 완료되지 않았으며 기한은 24시간 이내입니다.
* **빨강**: 완료되지 않았고 기한을 넘겼습니다.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## 증명 상태 개요

증명 상태는 증명에 필요한 결정의 상태를 표시합니다. 증명의 상태는 &quot;최악의 경우&quot; 참가자에 의해 결정됩니다. 예를 들어 증명에 대한 세 가지 결정이 있다고 가정해 보겠습니다. 두 개의 상태는 **수락됨**&#x200B;이고 한 개의 상태는 **거부됨**&#x200B;입니다. **Rejected**&#x200B;의 &quot;최악의 경우&quot; 결정은 다른 결정 및 증명의 전체 상태를 **Rejected**&#x200B;로 표시합니다. 

![기존 진행률 증명 편집](assets/proof-edit-existing-progress-350x62.png)

표준 상태 옵션은 다음과 같습니다.

* 보류 중
* 승인됨
* 변경 사항과 함께 승인됨
* 변경 필요
* 관련 없음

사용자 지정 결정이 계정에 구성된 경우 상태 옵션이 사용자 지정 결정 설정을 반영합니다.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
