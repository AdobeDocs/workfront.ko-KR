---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 사용자를 태그로 지정하여 증명 공유
description: 증명 뷰어에서 증명에 댓글을 달 때 다른 사용자를 태그로 지정하여 이메일을 통해 댓글에 주의를 집중시키고 증명의 워크플로에 추가할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: fe269b088c82e7045ffbb5155d54432e0b413cbe
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 사용자를 태그로 지정하여 증명 공유

증명 뷰어에서 증명에 댓글을 달 때 다른 사용자를 태그로 지정하여 이메일을 통해 댓글에 주의를 집중시키고 증명의 워크플로에 추가할 수 있습니다.

증명에 대한 댓글에서 사용자를 태그 지정할 때 태그 지정할 수 있는 사용자는 개별 사용자 권한 및 조직의 멤버십과 같은 다양한 요소에 따라 다를 수 있습니다.

* 증명 작성자, 소유자 또는 특정 권한이 활성화된 경우 증명 워크플로 외부의 사용자에 태그를 지정하고 해당 사용자와 증명을 공유할 수 있습니다.
* 증명에 외부 사용자로 추가되었으며 다른 증명 계정을 가진 다른 환경의 멤버인 경우 원래 환경의 해당 사용자만 태그를 지정할 수 있습니다. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 액세스 요구 사항 {#access-requirements}

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>임의</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">증명 역할</td> 
   <td>작성자, 중재자</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">교정쇄 권한 프로필</td> 
   <td>감독자 또는 관리자</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자를 태그로 지정하여 증명 공유

위의 [액세스 요구 사항](#access-requirements) 섹션에 설명된 증명 권한 프로필 또는 증명 역할을 가진 사용자는 기본적으로 증명을 공유하도록 사용자를 태그 지정할 수 있습니다. 증명 소유자 또는 작성자인 경우 증명 권한 프로필 또는 증명 역할에 관계없이 증명 공유를 위해 사용자에 태그를 지정할 수도 있습니다. 낮은 증명 권한 프로필 또는 증명 역할을 가진 사용자가 증명을 만들 때 증명에 태그를 지정하여 공유할 수 있도록 설정할 수 있습니다. 자세한 내용은 [기본 워크플로를 사용하여 고급 증명 만들기](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) 문서의 [워크플로 구성 및 검토자 추가](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 섹션을 참조하십시오.

>[!NOTE]
>
>다음 중 하나가 참인 경우에만 이메일 주소를 사용하여 외부 공동 작업자에 태그를 지정할 수 있습니다.>
>* 조직의 Workfront 계정의 사용자가 이전에 증명에 공동 작업자의 이메일 주소를 추가했습니다.
>* 공동 작업자는 이전에 이메일 주소를 사용하여 조직의 Workfront 계정에서 증명을 구독했습니다.
>

다른 사람에게 태그를 지정하고 댓글에서 증명을 공유하려면 다음을 수행하십시오.

1. 증명에 댓글을 달 때 @ 기호를 입력한 다음 사용자 이름 또는 이메일 주소를 입력합니다. 입력을 시작하면 사용 가능한 이름이 드롭다운 목록에 나타납니다.
1. 드롭다운 목록에 표시되는 개인의 이름을 선택합니다.

   >[!TIP]
   >
   >아무도 선택하지 않고 드롭다운 목록을 닫으려면 **Esc** 키를 누르거나 목록 바깥쪽을 클릭하면 됩니다.

1. 댓글에 태깅할 다른 모든 사용자에 대해 1~2단계를 반복합니다.
1. 댓글을 작성한 후 **게시물**&#x200B;을 클릭하세요.
1. (조건부) 증명에 아직 추가되지 않은 사용자를 태그 지정한 경우 표시되는 상자에 나열된 각 사용자에 대해 **증명 역할** 및 **알림 메일** 설정을 지정한 다음 **사람 추가 및 댓글 게시**&#x200B;를 클릭합니다.

   ![증명에 사람 추가](assets/add-people-to-proof-350x220.png)

   증명 역할에 대한 자세한 내용은 을 참조하십시오. 증명 전자 메일 경고에 대한 자세한 내용은 문서 [Workfront Proof에서 전자 메일 알림 설정 구성](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)의 섹션을 참조하십시오.

   증명에 자동화된 워크플로가 있는 경우 태그한 사용자가 진행 중인 단계에 추가됩니다. 자세한 내용은 [자동화된 워크플로 개요](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)를 참조하십시오.

   태그하면 사용 중인 증명 이메일 경고 설정에 관계없이 누구나 증명 댓글에 대한 알림 이메일을 받게 됩니다.

   * 사용자가 일일 요약 또는 시간별 요약 이메일을 수신하면 Workfront은 알림을 별도로 보내고 요약 이메일에 증명 댓글에 대한 정보를 포함합니다.
   * 사용자가 모든 활동에 대한 알림 또는 댓글에 대한 답글에 대한 알림을 받으면 이러한 댓글 및 답글에 대한 알림이 알림으로 바뀝니다.

증명에 사용자를 추가하는 다른 방법에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)를 참조하십시오.
