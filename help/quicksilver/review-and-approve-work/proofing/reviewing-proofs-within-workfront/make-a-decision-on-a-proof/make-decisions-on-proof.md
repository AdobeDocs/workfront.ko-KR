---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 증명 뷰어에서 증명 결정
description: 증명 뷰어에서 직접 증명에 대한 결정을 내릴 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# 증명 뷰어에서 증명 결정

증명 뷰어에서 직접 증명에 대한 결정을 내릴 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Select 또는 Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 역할</td> 
   <td>승인자, 검토자 및 승인자, 작성자, 중재자</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

## 증명 뷰어에서 증명 결정

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 증명을 찾은 다음 **증명 열기**&#x200B;를 클릭합니다.

1. 증명 뷰어의 위쪽 가운데에서 **결정**&#x200B;을 클릭합니다.

1. 표시되는 **증명 결정** 상자에서 다음 결정 중 하나를 클릭합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인됨</td> 
      <td>증명이 자동화된 워크플로의 다음 단계로 이동할 준비가 되었습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">변경 사항과 함께 승인됨</td> 
      <td>증명에는 몇 가지 변경이 필요하지만 자동 워크플로우의 다음 단계로 이동하기 전에 개정을 볼 필요는 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">변경 필요</td> 
      <td>증명을 변경하려면 수정해야 하며, 자동 워크플로우의 다음 단계로 이동하기 전에 다른 수정 버전을 확인해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">관련 없음</td> 
      <td>증명은 귀하와 관련이 없으며 귀하는 결정을 내릴 필요가 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 결정</td> 
      <td> <p>선택 및 프리미엄 계획에서 Workfront 관리자 또는 Workfront Proof 관리자는 의사 결정의 이름을 바꾸고, 순서를 변경하고, 숨길 수 있습니다. 자세한 내용은 <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Workfront Proof에서 승인 결정 옵션 구성</a>을 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) Adobe Workfront 관리자 또는 Workfront Proof 관리자가 이유 섹션을 추가한 경우 결정에 적용할 수 있는 이유를 선택합니다. 관리자가 의사 결정 이유를 구성하는 방법에 대한 자세한 내용은  [Workfront Proof에서 승인 결정 옵션을 구성합니다](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. (선택 사항) **확인 메일 보내기**&#x200B;를 선택하여 확인 메일을 받습니다.
1. **결정**&#x200B;을 클릭합니다.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
