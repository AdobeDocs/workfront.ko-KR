---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 증명 댓글 및 결정에 대한 알림 관리
description: Adobe Workfront 사용자이든 외부 협력자이든 증명을 사용하여 작업하는 경우 증명의 주석 및 결정에 대해 받을 이메일 알림을 지정할 수 있습니다. 자세한 내용은 알림 에서 증명 설명 및 결정 개요를 참조하십시오.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# 증명 댓글 및 결정에 대한 알림 관리

Adobe Workfront 사용자이든 외부 협력자이든 증명을 사용하여 작업하는 경우 증명의 주석 및 결정에 대해 받을 이메일 알림을 지정할 수 있습니다. 자세한 내용은 [증명 주석 및 의사 결정에 대한 알림 개요](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>이러한 알림은 검토자 간 증명 흐름에 대해 받을 수 있는 이메일 경고와 다릅니다. 또한 Workfront에서 구성할 수 있는 이메일 경고 설정과는 다릅니다. 

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Select 또는 Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 증명 댓글 및 결정에 대한 알림 관리

1. 수신할 알림을 구성할 증명을 엽니다.
1. 왼쪽 도구 모음이 표시되지 않으면 **메뉴** Web Proofing Viewer의 왼쪽 위 모서리에 있는 아이콘

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 왼쪽 도구 모음에서 **설정** 아이콘. ![Settings_icon.png](assets/settings-icon.png)

1. 아래 **다음에 대한 이메일 알림 보내기**&#x200B;를 클릭하여 증명에 사용할 설정을 클릭합니다.

   선택한 설정은 열려 있는 증명에만 적용됩니다.

   시스템 기본값은 입니다. **일별 요약**. 사용자 또는 검토자가 다른 변경 작업을 수행하지 않는 경우 모든 증명에 이 설정이 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모든 활동</td> 
      <td>증명에 새 댓글, 회신, 의사 결정 등 활동이 있을 때마다 이메일이 검토자에게 전송됩니다.<br><p>이것은 언어 교정 프로세스를 관리하는 사람에게 매우 좋은 옵션입니다. 언어 교정 프로세스를 관리하는 사람은 진행 중인 활동을 볼 수 있기 때문입니다. 사용자는 자신의 활동에 대한 이메일 경고(예: 댓글, 회신 및 의사 결정)를 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 댓글에 답글</td> 
      <td>누군가 자신의 댓글에 명시적으로 답장하는 경우에만 검토자에게 이메일이 전송됩니다(자체 댓글에 대해서는 자신의 답글이 제외됨). 즉, 증명의 누군가가 새 주석을 작성하면 검토자가 알림을 받지 않습니다.<p>이 설정은 증거에 대한 다른 댓글에 대한 알림을 받지 않고, 자신의 댓글에 대한 응답만 받도록 클라이언트가 증명에 대해 권장됩니다.</p><p>이 전자 메일 경고 설정을 사용하는 검토자는 다른 새 주석에 대한 알림을 받지 않지만 언어 교정 뷰어에서 증명에 대한 모든 주석을 볼 수 있습니다.<br></p><p>자세한 내용은 다음을 참조하십시오. <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정</td> 
      <td>누군가 결정을 내릴 때만 이메일이 검토자에게 전송됩니다.<br><p>이 전자 메일 경고는 승인 프로세스를 관리하는 사람(예: 프로젝트 관리자)에게 유용할 수 있습니다. 승인 프로세스를 관리하는 사람이 증명의 진행 상황을 모니터링하고 사용자가 결정을 내리는지 확인할 수 있기 때문입니다.<br></p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않은 경우, 사용자의 결정에 대한 알림을 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">최종 결정</td> 
      <td>증명에 대한 최종 결정이 있을 때(증명의 마지막 승인자가 결정을 했을 때) 이메일이 전송됩니다.<br><p>이 경고는 디자이너가 실제 검토 토론에 참여할 필요가 없기 때문에 디자이너에서 종종 사용됩니다. 최종 결정을 내리면 디자이너에게 알림이 전송되고 필요한 변경 사항에 대해 조치를 취할 수 있습니다.<br></p><p>이 경고는 검토 프로세스가 완료된 경우에만 알림을 받아야 하는 부서 리더에게 유용할 수도 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간별 요약</td> 
      <td>지난 시간에 발생한 모든 댓글, 회신 및 의사 결정에 대한 요약으로 매시간마다 검토자에게 이메일이 전송됩니다.<br><p>이메일 은 사용자 이외의 활동이 지난 시간 내에 발생하는 경우에만 전송됩니다. 다른 사용자의 활동이 없으면 이메일이 전송되지 않습니다.<br></p><p>이 경고는 프로젝트 개요를 보는 좋은 방법입니다.<br></p><p>이 요약의 사용 사례 예제는 프로젝트 개요가 필요하지만 증명의 모든 활동에 대해 즉시 알림을 받을 필요가 없는 선임 검토자입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">일별 요약</td> 
      <td>(기본 설정): 모든 댓글, 회신 및 의사 결정이 나열된 전자 메일이 매일 전송됩니다. 사용자 이외의 활동이 있는 경우에만 이메일이 전송됩니다.<br><p>이 경고는 하루 종일 여러 업데이트로 압도되지 않고 프로젝트 요약을 보는 좋은 방법입니다.<br></p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 책임자입니다.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">이메일 없음</td> 
      <td>이메일 경고가 전송되지 않습니다.<br><p>이 설정은 참조용으로만 증명에 추가되고 변경 사항에 대한 알림을 받을 필요가 없는 사용자에게 유용합니다.</p><p>참고: <p>이 옵션은 증명 설명 및 결정에 대해 받을 수 있는 이메일 경고만 끕니다. 새 증명 또는 지연 증명 이메일과 같이 증명 플로우에 대해 수신할 수 있는 이메일 경고는 끄지 않습니다. 증명 흐름에 대한 이메일 경고에 대한 자세한 내용은 다음 문서를 참조하십시오. </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">새로운 증명 이메일</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">새 버전 이메일</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">지연 증명 이메일</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">증명의 이메일</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
