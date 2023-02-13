---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 사용자에게 태그를 지정하여 증명 공유
description: 언어 교정 뷰어의 증명에 주석을 달 때 다른 사용자에게 태그를 지정하여 전자 메일을 통해 주석에 주의를 기울이고 증명 워크플로우에 추가할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 사용자에게 태그를 지정하여 증명 공유

언어 교정 뷰어의 증명에 주석을 달 때 다른 사용자에게 태그를 지정하여 전자 메일을 통해 주석에 주의를 기울이고 증명 워크플로우에 추가할 수 있습니다.

증명에 대한 댓글에 있는 사용자에게 태그를 지정할 때 태깅할 수 있는 사용자는 개별 사용자 권한 및 조직의 멤버십과 같은 다양한 요소에 따라 다를 수 있습니다.

* 증명 생성자, 소유자 또는 특정 사용 권한이 활성화되어 있는 경우 증명 워크플로우 외부의 사용자에게 태그를 지정하고 증명을 사용자와 공유할 수 있습니다.
* 증명에 외부 사용자로 추가되고 다른 증명 계정을 사용하는 다른 환경의 구성원인 경우 원래 환경에서 해당 사용자만 태깅할 수 있습니다. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 액세스 요구 사항 {#access-requirements}

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">증명 역할</td> 
   <td>작성자, 중재자</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>감독자 또는 관리자</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 사용자에게 태그를 지정하여 증명 공유

에 요약된 증명 권한 프로필 또는 증명 역할을 가진 사용자 [액세스 요구 사항](#access-requirements) 위의 섹션에서는 기본적으로 사용자에게 증명을 공유하도록 태그를 지정할 수 있습니다. 증명 소유자 또는 작성자인 경우 증명 권한 프로필 또는 증명 역할과 관계없이 사용자에게 증명을 공유하도록 태그를 지정할 수도 있습니다. 증명 권한 프로필 또는 증명 역할이 낮은 사용자가 증명을 만들 때 사용자에게 태그를 지정하면 증명을 공유할 수 있습니다. 자세한 내용은 [워크플로우 구성 및 검토자 추가](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) 의 섹션 [기본 워크플로우를 사용하여 고급 증명 만들기](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 문서.

>[!NOTE]
>
>다음 중 하나가 true인 경우에만 이메일 주소를 사용하여 외부 협력자에 태그를 지정할 수 있습니다.>
>* 조직의 Workfront 계정에 있는 사용자가 이전에 증표에 공동 작업자의 이메일 주소를 추가했습니다.
>* 공동 작업자는 이메일 주소를 사용하여 이전에 조직의 Workfront 계정에 있는 증명을 구독했습니다.
>


다른 사람에게 태그를 지정하고 댓글에 증명을 공유하려면 다음을 수행하십시오.

1. 증명에 댓글을 달려면 at 기호(@)와 사람 이름 또는 이메일 주소를 차례로 입력합니다. 입력을 시작하면 사용 가능한 이름이 드롭다운 목록에 나타납니다.
1. 드롭다운 목록에 있는 사람 이름을 선택합니다.

   >[!TIP]
   >
   >다른 사람을 선택하지 않고 드롭다운 목록을 닫으려면 를 누를 수 있습니다 **Esc** 키를 클릭하거나 목록 바깥쪽을 클릭합니다.

1. 주석에서 태깅하려는 다른 사용자에 대해 1-2단계를 반복합니다.
1. 설명을 완료한 다음 을 클릭합니다 **Post**.
1. (조건부) 증명에 아직 추가되지 않은 사람에 태그를 지정한 경우 **증명 역할** 및 **이메일 경고** 표시되는 상자에 나열된 각 사용자에 대해 설정한 다음 **사용자 추가 및 댓글 게시**.

   ![](assets/add-people-to-proof-350x220.png)

   증명 역할에 대한 자세한 내용은 을 참조하십시오. 증명 이메일 경고에 대한 자세한 내용은 문서의 섹션을 참조하십시오 [Workfront 증명의 이메일 알림 설정 구성](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   증명에 자동화된 워크플로우가 있는 경우 태그하는 사용자가 현재 단계에 추가됩니다. 자세한 내용은 [자동화된 워크플로우 개요](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   태그 사용자가 사용 중인 증명 이메일 경고 설정과 관계없이, 증명 댓글에 대한 알림 이메일을 수신하게 됩니다.

   * 사용자가 일별 요약 또는 시간별 요약 이메일을 수신하면 Workfront에서 알림을 별도로 전송하고 증명 댓글에 대한 정보를 요약 이메일에 포함합니다.
   * 사용자가 모든 활동에 대한 경고를 받거나 해당 댓글에 대한 응답을 받으면 해당 알림이 이러한 댓글 및 답글에 대한 알림을 대체합니다.

증명에 사용자를 추가하는 다른 방법에 대한 자세한 내용은 [Adobe Workfront에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
