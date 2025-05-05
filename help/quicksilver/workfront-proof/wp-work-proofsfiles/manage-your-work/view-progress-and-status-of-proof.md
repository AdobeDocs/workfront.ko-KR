---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: ' [!DNL Workfront Proof]에서 증명 진행 상황 및 상태 보기'
description: 증명 진행률은 검토자에게 증명을 보낸 시점부터 검토자가 증명에 대한 결정을 내릴 때까지 증명에 대한 작업이 완료됨을 나타냅니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# [!DNL Workfront Proof]에서 증명 진행 상황 및 상태 보기

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

## 증명 진행 상황 이해

증명 진행률은 검토자에게 증명을 보낸 시점부터 검토자가 증명에 대한 결정을 내릴 때까지 증명에 대한 작업이 완료됨을 나타냅니다.

* [진행률 아이콘](#progress-icons)
* [증명 진행률 수준](#levels-of-proof-progress)

### 진행률 아이콘 {#progress-icons}

진행률 아이콘 S, O, C, D가 진행률 표시줄에 표시되어 증명 진행률을 나타냅니다.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

증명에 대한 다음 정보를 나타냅니다.

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
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>전송됨</strong>. 증명이 검토자에게 전송되었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>열림</strong>. 검토자가 증명 세부 정보 페이지를 열거나 증명 뷰어에서 증명 자체를 열었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>댓글</strong>. 검토자(댓글을 달 수 있는 사용자)가 증명에 댓글을 달았습니다.</p> <p>증명에 대한 검토자가 지정되지 않은 경우 이 아이콘이 표시되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>결정</strong>. 그 증명에 대해 평자가 결정을 내렸다.</p> <p>증명에 대해 지정된 승인자(의사 결정자)가 없는 경우 이 아이콘이 표시되지 않습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

이러한 아이콘은 다음 색상으로 표시되어 증명 진행률에 대한 특정 정보를 나타낼 수 있습니다.

* **녹색**. 완료.
* **흰색**. 완료되지 않았습니다.
* **주황색**. 완료되지 않았고 마감이 24시간 이내입니다.
* **빨강**. 완료되지 않았고 마감이 지났습니다.

### 증명 진행률 수준 {#levels-of-proof-progress}

Workfront Proof은 진행률 아이콘을 사용하여 다음 각 수준에서 증명의 진행률을 추적합니다.

* 각 검토자의 경우 증명에 대한 해당 검토자의 활동을 기반으로 합니다.
* 각 단계별로, 증명 과정에서 가장 뒤처진 단계의 심사자를 기준으로 한다. 자세한 내용은 [자동화된 워크플로 단계 개요](../../../review-and-approve-work/proofing/proofing-overview/stages.md)를 참조하십시오.
* 증명은 증명 과정에서 가장 뒤처지는 단계(검토자 그룹)의 진행률을 기준으로 한다.

[!DNL Workfront Proof]이(가) 가장 뒤쳐진 검토자 또는 단계를 사용하여 진행 상황을 결정하는 방법의 예를 들어 증명에 대한 세 명의 검토자가 결정을 내려야 한다고 가정해 봅시다. 두 사람이 결정을 내렸지만 세 번째는 결정을 내리지 못한 경우, 우수 결정으로 인해 증명에 대한 진행률 표시줄에 D가 녹색으로 표시되지 않습니다.

증명에서 [!UICONTROL 기본 결정자] 설정을 선택하고 기본 결정자가 결정을 제출하면 다른 결정이 필요하지 않으므로 증명 진행률 표시줄의 D가 모든 검토자에게 녹색으로 바뀝니다.

마찬가지로 증명에서 [!UICONTROL 한 개의 의사 결정만 필요] 설정을 선택하고 검토자가 의사 결정을 제출하면 다른 의사 결정이 필요하지 않으므로 증명 진행률 표시줄의 D가 모든 검토자에게 녹색으로 바뀝니다.

## 증명 상태 이해

증명 상태는 증명에 필요한 결정의 상태를 표시합니다.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
표준 상태 옵션은 다음과 같습니다.

* 보류 중
* 승인됨
* 변경 사항과 함께 승인됨
* 변경 필요
* 관련 없음

사용자 지정 결정이 계정에 구성된 경우 상태 옵션이 사용자 지정 결정 설정을 반영합니다.

증명의 상태는 &quot;최악의 경우&quot; 참가자에 의해 결정됩니다. 예를 들어 증명에 대한 세 가지 결정이 있다고 가정해 보겠습니다. 두 개의 상태는 **수락됨**&#x200B;이고 한 개의 상태는 **거부됨**&#x200B;입니다. 거부됨의 &quot;최악의 경우&quot; 결정은 다른 결정과 전체 증명 상태를 **거부됨**&#x200B;으로 표시합니다.

## 진행 상황 및 상태 보기 {#viewing-progress-and-status}

각 단계에서 증명, 단계 및 검토자의 진행 상황과 상태를 볼 수 있습니다.

* [증명 요약](#proof-summary)
* [스테이지 작업 메뉴](#stage-actions-menu)
* [증명에 대한 편집 권한이 있는 경우 [!UICONTROL 요약] 섹션에서 검토자 작업 메뉴에도 액세스할 수 있습니다. 자세한 내용은 Workfront Proof의 증명 권한 프로필 및 Workfront Proof의 증명 역할 관리 를 참조하십시오. [!UICONTROL 검토자 작업] 메뉴(1)는 검토자의 세부 사항을 마우스로 가리키면 나타나며 다음을 수행할 수 있습니다.](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [증명 작업 메뉴](#proof-actions-menu)

### 증명 요약 {#proof-summary}

폴더의 각 증명에는 증명의 세부 사항을 빠르게 보고 편집할 수 있는 확장 가능한 요약이 있습니다.

요약을 확장하거나 축소하려면 다음을 수행합니다.

1. 대시보드 또는 목록 보기에서 증명 왼쪽의 화살표를 클릭합니다.

![Summary_expandable.png](assets/summary-expandable-350x68.png)

요약에는 다음이 포함됩니다.

* 워크플로우 (2)
* 버전 (3)
* 폴더 (4)
* 주(5)\
   ![summary_2.png](assets/summary-2-350x160.png)

요약에서는 다음 증명 세부 정보를 보고 편집할 수 있습니다.

* 증명 진행률 (1)
* 각 단계 진행 (2)
* 단계 (3)에 대해 설정된 기한
* 검토자 세부 정보:

   * 각 검토자가 작성한 댓글 및 답글 수(4)
   * 각 검토자의 진행률(5)
   * 결정(결정에 전자 서명이 포함된 경우 결정 옆에 이를 나타내는 아이콘이 표시됩니다.) (6)
   * 증명에서 역할(7)
   * 이메일 경고 설정(8)

>[!NOTE]
>
>증명 세부 정보를 편집할 수 있는 권한은 증명에 대한 권한에 따라 다릅니다([증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 참조).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### [!UICONTROL 단계 작업] 메뉴  {#stage-actions-menu}

워크플로우의 모든 단계에는 별도의 메뉴가 있으므로 해당 단계의 검토자와 관련된 대량 작업을 수행할 수 있습니다.

[!UICONTROL 단계 작업] 메뉴는 단계 섹션(1)을 마우스로 가리키면 다음과 같은 작업을 수행할 수 있도록 표시됩니다.

* [!UICONTROL 모두 메시지] (2)
* [!UICONTROL 공유] (3)
* [!UICONTROL 단계 삭제] (4)

>[!NOTE]
>
>이러한 옵션의 사용 가능 여부는 증명에 대한 권한에 따라 다릅니다([증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 참조).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

증명에 대한 편집 권한이 있는 경우 요약 섹션에서 검토자 작업 메뉴에 액세스할 수도 있습니다. 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오. 검토자 작업 메뉴(1)는 검토자의 세부 사항을 마우스로 가리키면 나타나며 다음을 수행할 수 있습니다.

* 검토자에게 메시지 보내기(2)
* 검토자 세부 정보 편집(3) - 해당 검토자에 대한 표시 이름, 증명 역할 및 이메일 경고를 편집할 수 있습니다.
* 증명 소유자로 설정 (4)
* 그들을 주요 의사 결정자로 지정 (5)
* 증명에서 제거 (6)

>[!NOTE]
>
>이러한 옵션의 가시성은 증명에 대한 권한에 따라 다릅니다([증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 참조).

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### 증명 작업 메뉴 {#proof-actions-menu}

각 증명에는 아래 작업을 수행할 수 있는 메뉴(1)도 있습니다.

* 증명 세부 정보 페이지(2)에 액세스할 수 있습니다.
* 다른 사용자와 증명 공유 (3)
* 검토자에게 메시지 보내기(4)
* 증명의 새 버전 만들기(5)
* 증명 복사 (6)
* 원본 파일 다운로드 (7)
* 증명 링크 공유(8)
* 댓글 인쇄(9)
* 증명의 Excel 요약 요청(10)
* 증명 잠금(11)
* 증명 삭제(12)

![Proof_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>이러한 옵션의 사용 가능 여부는 증명에 대한 권한에 따라 다릅니다([증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 참조).

[!DNL Workfront] 내의 증명 진행 상황 및 상태를 보는 방법에 대한 자세한 내용은 [진행 상황 및 상태 보기](#viewing-progress-and-status)를 참조하십시오.

Desktop Proofing Viewer에서 진행 상황과 상태를 보는 방법에 대한 자세한 내용은 [증명 뷰어에서 워크플로 검토](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md)를 참조하십시오.
