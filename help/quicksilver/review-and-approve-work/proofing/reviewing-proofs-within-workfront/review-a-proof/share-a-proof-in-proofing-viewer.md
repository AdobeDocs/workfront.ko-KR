---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 증명 뷰어에서 증명 공유
description: 증명 소유자 또는 작성자가 공유를 활성화한 경우 증명 뷰어에서 증명을 공유할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 증명 뷰어에서 증명 공유

증명 소유자 또는 작성자가 공유를 활성화한 경우 증명 뷰어에서 증명을 공유할 수 있습니다.

>[!IMPORTANT]
>
>공개 URL 또는 포함 코드를 통한 증명 공유 허용 설정을 활성화해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## URL 공유

소유자가 공유를 위해 증명을 구성한 경우 URL을 통해 증명을 공유할 수 있습니다. 증명 소유자는 언제든지 공유 설정을 업데이트할 수 있습니다. 자세한 내용은 [증명 설정 편집](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)을 참조하세요.

1. 왼쪽 아이콘 메뉴가 표시되지 않으면 증명 뷰어의 왼쪽 위 모서리에 있는 **메뉴** 아이콘을 클릭합니다.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. 증명 뷰어의 왼쪽 아이콘 메뉴에서 **공유** 아이콘을 클릭합니다.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. 표시되는 **증명 공유** 옵션에서 **공유 가능한 링크 가져오기**&#x200B;가 선택되어 있는지 확인하십시오.

1.  다음 중 하나를 수행합니다.

   * 클립보드에 링크를 복사하려면 **링크 복사**&#x200B;를 클릭하세요.

     이제 채팅 또는 이메일 애플리케이션과 같은 서드파티 도구를 통해 링크를 배포할 수 있습니다.

   * Adobe Workfront에서 직접 링크를 이메일로 보내려면 다음을 수행합니다.

      1. **또는**(으)로 연결된 전자 메일 링크에서 입력을 시작하고 받는 사람의 이름을 선택합니다. 또는 공유할 외부 사용자의 이메일 주소를 지정합니다.

         >[!NOTE]
         >
         >증명을 공유할 때 별칭 이메일이 표시되는 경우, 해당 별칭 이메일이 있는 경우 원본 이메일을 입력하여 새 게스트 사용자를 만들지 마십시오.

      1. 다음 옵션 중에서 선택합니다.

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">공개 링크 보내기</td>
            <td><p>이메일 알림에 사용자가 사용 중인 증명 뷰어 내의 증명으로 사용자를 안내하고 보기 액세스 권한을 부여하는 버튼을 포함합니다.</p><p>증명에 대해 <strong>공개 URL 또는 포함 코드를 통해 증명 구독</strong>이 꺼져 있으면 사용자가 Workfront 로그인 자격 증명으로 로그인하여 증명에 주석을 추가할 수 있습니다. 이 기능이 켜지면 이메일 주소와 이름을 제공하는 모든 사람(암호 필요 없음)이 서명하고 증명에 주석을 추가할 수 있습니다.</p></td>
           </tr>
           <tr>
            <td role="rowheader">다운로드 링크 보내기</td>
            <td>사용자에게 파일 세부 사항, 파일 이름 및 파일 크기를 제공하고 파일이 인라인으로 표시되는 다운로드 페이지로 안내하는 이메일 알림의 버튼을 포함합니다. 사용자는 다운로드 페이지에서 다운로드 링크를 클릭하여 파일을 다운로드할 수 있습니다.</td>
           </tr>
           <tr>
            <td role="rowheader">사용자 정의 메시지 추가</td>
            <td>이메일 알림에 대한 사용자 정의 제목과 본문을 지정할 수 있습니다.</td>
           </tr>
          </tbody>
         </table>

      1. **보내기**&#x200B;를 클릭합니다.

         수신자는 증명 및 포함하기로 선택한 버튼에 대한 정보가 포함된 이메일 알림을 받게 됩니다.

         ![](assets/proof-share-email-350x87.png)

## 포함 코드 공유

증명 소유자가 이에 대해 구성한 경우 포함 코드를 통해 증명을 공유할 수 있습니다.

포함 코드를 통해 증명을 공유하려면 다음을 수행하십시오.

1. 증명 뷰어 왼쪽의 도구 모음에서 **공유** 아이콘을 클릭합니다.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. 표시되는 **증명 공유** 옵션에서 **포함 코드 가져오기**&#x200B;를 클릭한 다음 **복사**&#x200B;를 클릭합니다.

## 사용자를 추가하여 증명 공유

다음 권한 중 하나가 있는 경우 증명을 검토하는 동안 증명에 사용자를 추가할 수 있습니다.

* 감독자 또는 관리자 권한
* 관리자 권한이며 증명 작성자 또는 소유자입니다.
* 작성자 또는 중재자 증명 역할이 있는 관리자 권한

증명에 자동화된 워크플로가 있는 경우 사용자를 개별 단계에 추가할 수 있습니다. 자세한 내용은 [자동화된 워크플로 개요](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)를 참조하십시오.

기본적으로 증명에 추가하는 사용자는 다음과 같습니다.

* 증명에 대한 링크가 포함된 이메일 알림을 받습니다.
* [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md)에 설명된 대로 홈 영역에서 증명에 대한 승인 결정을 내릴 수 있습니다.
* 증명을 검토하기 위해 증명을 활성화하지 않아도 됩니다.

자동화된 워크플로가 활성화되고 Workfront에서 증명이 활성화되지 않은 사용자를 증명에 추가하면 자동화된 워크플로 내에 새 단계가 생성됩니다. 추가하려는 사용자가 증명을 처음 볼 때 이 새 단계에 자동으로 추가됩니다. 자세한 내용은 [자동화된 워크플로 개요](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)를 참조하십시오.

개별 사용자와 증명을 공유하려면 다음을 수행하십시오.

1. 증명 뷰어 왼쪽의 도구 모음에서 **공유** 아이콘을 클릭합니다.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. 왼쪽 목록에서 **수신자 추가**&#x200B;를 클릭합니다.
1. **새 증명 수신자**&#x200B;에서 증명을 공유할 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.
1. (선택 사항) 검토자 옵션을 개인 이름 오른쪽에 있는 것으로 변경합니다.

   * **증명 역할**: 자세한 내용은 [Workfront Proof에서 증명 역할 관리](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

   * **단계**: (증명에 자동화된 워크플로가 있는 경우에만 사용 가능). 자세한 내용은  [자동화된 워크플로 단계 개요](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **전자 메일 경고**: 다음 옵션 중 하나를 선택하여 증명에 대한 활동에 대한 알림을 받는 방법을 지정합니다.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">모든 활동</td> 
        <td>Workfront은 새 댓글, 회신 또는 결정과 같은 증명에 대한 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>활동을 볼 수 있으므로 증명 프로세스를 관리하는 사용자에게 적합한 옵션입니다. </p><p>사용자는 자신의 활동에 대한 이메일 알림을 받지 않습니다.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">내 댓글에 대한 답글</td> 
        <td>누군가 자신의 의견에 명시적으로 답글을 달 경우에만 검토자에게 이메일이 전송됩니다(자신의 의견에 대한 자신의 답글은 제외). 즉, 증명에 있는 사람이 새 댓글을 달면 검토자에게 알림이 전송되지 않습니다.<p>이 설정은 증명의 클라이언트가 증명의 다른 댓글에 대한 알림을 받지 않고 자신의 댓글에 대한 답글에만 알림을 받도록 하는 데 권장됩니다.</p><p>이 이메일 경고 설정을 사용하는 검토자는 다른 새 댓글에 대해 알림을 받지 못하지만 증명 뷰어에서 증명에 대한 모든 댓글을 볼 수 있습니다.</p><p>댓글에 대한 자세한 내용은 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>을 참조하세요.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">결정</td> 
        <td>Workfront은 누군가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명 진행 상황을 모니터링하고 어떤 사용자가 결정을 내렸는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않으면 자신의 결정에 대한 알림이 전송되지 않습니다.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">최종 결정</td> 
        <td>Workfront은 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 설계자가 사용하는 경우가 많으며, 일반적으로 실제 검토 토론에 참여하지 않아도 됩니다. 최종 결정이 내려지면 디자이너는 알림을 받은 다음 필요한 변경 작업을 수행할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료되어야 알림을 받아야 하는 부서 리더에게도 유용할 수 있습니다.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">시간별 요약</td> 
        <td>Workfront은 매 시간마다 해당 시간에 발생한 모든 댓글, 답글 및 의사 결정에 대한 요약이 포함된 이메일을 검토자에게 보냅니다.<p>지난 1시간 내에 자신의 활동 이외의 활동이 발생한 경우에만 이메일이 전송됩니다. </p><p>이 경고는 프로젝트의 개요를 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트 개요가 필요하지만 증명에 대한 모든 활동을 즉시 알릴 필요가 없는 선임 검토자입니다.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">일일 요약</td> 
        <td>Workfront은 자신 이외의 활동이 있는 날에만 나열된 모든 댓글, 답글 및 결정을 포함하는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트가 쏟아지지 않고 프로젝트 요약을 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 리더입니다.</p><p>자세한 내용은 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>를 참조하십시오.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">이메일 없음</td> 
        <td>Workfront은 이메일 경고를 전송하지 않습니다.<br>참조용으로만 증명에 추가되고 변경 내용에 대한 알림을 받을 필요가 없는 사용자에게 유용합니다.<p>시스템 기본값은 일별 요약(설정되지 않은 것으로도 표시됨)입니다. 사용자 또는 검토자가 다른 변경 내용을 적용하지 않으면 모든 증명에 이 설정이 적용됩니다.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (선택 사항) 앞의 두 단계를 반복하여 증명에 여러 사용자를 추가합니다. 
1. (선택 사항) 검토자에 대해 **기한**&#x200B;을 설정합니다(증명에 자동화된 워크플로가 없는 경우에만 사용 가능).
1. (선택 사항) **새 받는 사람에게 전자 메일 알림 보내기**&#x200B;를 선택하여 증명에 추가했음을 알려 줍니다.
1. 증명에 사용자를 추가했으면 **완료를 클릭합니다.**
