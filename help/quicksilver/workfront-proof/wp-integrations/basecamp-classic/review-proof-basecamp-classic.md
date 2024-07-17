---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Basecamp Classic에서 증명 검토
description: 베이스캠프는 37시그널이 개발한 온라인 프로젝트 관리 도구다. 프로젝트 관리에 Basecamp를 사용하는 경우  [!DNL Workfront Proof]을(를) 사용하여 프로젝트 팀에 보다 풍부한 검토 및 승인 도구를 제공할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b14f33dc-e059-4ee2-a429-9f1852a2b9bb
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# [!DNL Basecamp] Classic에서 증명 검토

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Basecamp]은(는) [!DNL 37signals]이(가) 개발한 온라인 프로젝트 관리 도구입니다. 프로젝트 관리에 [!DNL Basecamp]을(를) 사용하는 경우 [!DNL Workfront Proof]을(를) 사용하여 프로젝트 팀에 더 풍부한 검토 및 승인 도구를 제공할 수 있습니다.

## [!DNL Basecamp Classic]의 증명 검토 이해

[!DNL Workfront Proof]과(와) 통합되면 [!DNL Basecamp]에서 사용자는 증명을 사용하여 다음을 수행할 수 있습니다.

* 사용자는 [!DNL Basecamp Classic] 내에서 증명을 검토하고 승인할 수 있습니다.
* 사용자는 검토 도구를 즉시 사용할 수 있습니다.
* 프로젝트 검토 팀이 [!DNL Basecamp]에서 검토 및 승인을 위한 미니 증명과 함께 메시지를 받습니다.
* 사용자는 검토 및 승인을 위해 전체 페이지 증명으로 전환할 수 있습니다.
* 사용자는 미니 및 전체 크기의 증명 모두에 주석과 마크업을 추가할 수 있습니다.
* 댓글에 회신하면 해당 댓글을 편집/삭제할 수 없습니다. 댓글에 대한 자세한 내용은 [증명에 대한 댓글](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md)을 참조하세요.
* 검토자는 다른 검토자가 만든 및 마크업에 응답할 수 있습니다. 댓글에 대한 자세한 내용은 [증명에 대한 댓글](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md)을 참조하세요.
* 새 증명 버전을 사용할 수 있게 되면 사용자에게 경고가 표시됩니다.
* [!DNL Workfront Proof]명의 사용자가 아닌 사용자는 [!DNL Basecamp]에서 증명 작업을 수행할 수 있습니다.

## 알림 이메일을 통해 증명 보기

[!DNL Basecamp]에 증명을 연결하면 [!DNL Workfront Proof]에서 모든 검토자에게 다음 정보가 포함된 증명 알림 이메일(1)을 보냅니다.

* **증명 세부 정보** (2): 증명에 대한 정보를 표시합니다. 표시되는 정보는 Workfront 관리자가 Basecamp를 구성한 방법에 따라 다릅니다.
* **[!UICONTROL 증명으로 이동] 링크** (3): Workfront에서 증명을 엽니다.
* **[!DNL Basecamp]URL** (4): 기본 캠프에서 증명을 엽니다. Basecamp가 아닌 검토자가 증명에 추가되면 이메일 알림에 Basecamp 링크가 포함되지 않습니다.
* **[!UICONTROL 증명 진행 상황]** (5): 승인 단계를 나열하고 증명 진행 상황 표시기를 표시합니다.
* **[!UICONTROL 단계]** (6): 검토자와 개별 진행 상황을 나열합니다.

![Basecamp_ProofHQ_email_notification1__1_.png](assets/basecamp-proofhq-email-notification1--1--350x202.png)

이메일 알림에서 증명을 열려면 다음을 수행하십시오.

1. [!DNL Workfront Proof]에서 증명을 열려면 **[!UICONTROL 증명으로 이동]**&#x200B;을 클릭하세요.\
   또는\
   [!DNL Basecamp]에서 증명을 열려면 **[!UICONTROL [!DNL Basecamp]URL]** 필드에 나열된 URL을 클릭합니다.\
   [!DNL Basecamp Classic]에서 증명 검토에 대한 자세한 내용은 이 문서에서 [증명 검토 [!DNL Basecamp]](#reviewing-a-proof-in-basecamp)를 참조하십시오.

## [!DNL Basecamp Classic] 메시지를 통해 증명 보기

[!DNL Basecamp Classic] 메시지에서 증명에 액세스할 수 있습니다.

1. [!DNL Basecamp]에서 프로젝트 페이지(1)로 이동합니다.\
   ![Basecamp_Classic_messages_1.png](assets/basecamp-classic-messages-1-350x120.png)

1. 열려는 증명에 대한 메시지를 클릭합니다. (2)\
   증명에 대한 메시지가 열리고 작은 증명이 표시됩니다. 증명의 이름이 메시지 창(3) 맨 위에 표시됩니다.\
   [!DNL Basecamp Classic] 또는 [!DNL Workfront Proof]에서 썸네일 증명을 볼 수 있습니다.\
   ![Basecamp_Classic_messages_2.png](assets/basecamp-classic-messages-2-350x501.png)

1. [!DNL Workfront proof]에서 전체 화면 모드로 증명을 보려면 증명(4) 위에 나열된 URL을 클릭합니다.
1. (조건부) 브라우저 창 중 하나에서 [!DNL Workfront Proof] 계정에 로그인하지 않은 경우 로그인하여 증명을 검토하십시오.

   1. 증명 위에 있는 **[!UICONTROL 로그인]**(5)을 클릭합니다.
   1. 이메일 주소(6)를 입력합니다.\

      증명에 추가되었을 때 사용한 것과 동일한 이메일 주소를 사용해야 합니다.
   1. **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
   1. [!DNL Workfront Proof] 암호를 입력하십시오(7).\

      또는\
      [!DNL Workfront Proof] 계정이 없는 경우 표시할 공개 이름을 입력하십시오.\
      &quot;[!UICONTROL 내 정보 저장]&quot;을(를) 선택할 수 있으므로 세부 정보를 한 번만 입력하면 됩니다.

1. 증명을 검토하려면 [다음 위치에서 증명 검토 [!DNL Basecamp]](#reviewing-a-proof-in-basecamp)를 계속하십시오.

>[!NOTE]
>
> 메시지 페이지의 미니 증명 아래에 표시된 주석 상자는 메시지 자체에만 적용됩니다. 검토 의견을 제출하려면 미니 증명 상단에 있는 의견 아이콘 버튼을 사용하거나 전체 페이지 증명 상단에 있는 더 큰 [!UICONTROL 의견] 버튼을 사용해야 합니다. 자세한 내용은 [증명 검토 [!DNL Basecamp]](#reviewing-a-proof-in-basecamp)를 참조하십시오.

## [!DNL Basecamp]에서 증명 검토

[!DNL Basecamp]의 미니 증명은 추가하고 증명에 대한 [증명 뷰어에서 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)을 내리는 데 필요한 도구를 제공합니다. 프로젝트에 할당된 모든 사용자는 마크업과 댓글을 볼 수 있으며 실시간으로 자신의 댓글로 응답할 수 있습니다.

증명을 열면 증명이 [!UICONTROL proof] 창(1)에 표시되고 증명 이름과 버전 번호가 왼쪽 상단(2)에 표시됩니다.

![Basecamp_Classic_miniproof.png](assets/basecamp-classic-miniproof-350x350.png)

증명을 검토하려면:

1. 댓글을 추가하려면 증명 상단에 있는 [!UICONTROL 댓글](3)을 클릭하고 댓글을 입력하세요.\
   댓글과 [증명 뷰어에서 증명에 대한 결정을 내립니다](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)(예: [!DNL Workfront Proof] 내의 증명 검토).[!DNL Basecamp]

1. 결정을 추가하려면 증명 상단에 있는 결정 (3)을 클릭하고 승인 결정을 선택합니다.\
   증명 결정에 대한 자세한 내용은 [증명 뷰어에서 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof)을 참조하십시오.

증명 창의 다른 기능은 다음과 같습니다.

* **[!UICONTROL 작업 메뉴]** (4): 증명에 대한 설정을 선택할 수 있습니다.
* **[!UICONTROL 전체 화면 단추]** (5): 전체 화면과 미니 증명 간을 전환할 수 있습니다.
* **[!UICONTROL 사이드바]** (6): 증명 보기를 확장하거나 축소할 수 있습니다.
* **[!UICONTROL 사용자 이름]** (7): Workfront에 로그인한 경우 사용자 이름을 표시합니다.
* **[!UICONTROL 확대/축소 도구]** (8): 증명의 영역을 확대할 수 있습니다.
* **[!UICONTROL 페이지 탐색 도구]** (9): 증명 내의 다른 페이지로 스크롤할 수 있습니다.

<!--For more information on reviewing proofs, see [Legacy proofing viewer Overview](../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/legacy-proofing-viewer.md).-->
