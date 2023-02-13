---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 기본 워크플로우를 사용하여 고급 증명 만들기
description: 기본 워크플로우를 사용하면 여러 검토자가 증명을 읽을 수 있지만 단계별로 구성되지 않습니다. 추가한 모든 검토자는 만든 후 즉시 증명에 액세스할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 1%

---

# 기본 워크플로우를 사용하여 고급 증명 만들기

기본 워크플로우를 사용하면 여러 검토자가 증명을 읽을 수 있지만 단계별로 구성되지 않습니다. 추가한 모든 검토자는 만든 후 즉시 증명에 액세스할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: 선택 또는 더 높음</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
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
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 기본 워크플로우를 사용하여 고급 증명 만들기

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 탭.
1. 클릭 **새로 추가** > 증명, 컨텐츠를 업로드한 다음 아래 나열된 섹션을 통해 작동합니다.

   또는

   기존 문서를 마우스로 가리킨 다음 **증명 만들기** > **고급 증명** 및 아래 나열된 섹션을 통해 작업할 수 있습니다.

## 워크플로우 구성 및 검토자 추가

1. 워크플로우 유형 섹션에서 **기본**.
1. 추가할 사용자를 지정한 다음 증명 역할을 선택합니다.

   ![](assets/new-proof---roles-350x213.png)

1. 다음 표에는 각 역할 및 해당 역할과 연관된 권한이 나와 있습니다.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>증명 보기</strong> </p> </th> 
      <th> <p><strong>마크업 추가</strong> </p> </th> 
      <th> <p><strong>댓글 추가</strong> </p> </th> 
      <th> <p><strong>답글이 없는 경우 댓글 편집</strong> </p> </th> 
      <th> <p><strong>결정</strong> </p> </th> 
      <th> <p><strong>다른 사람이 작성한 댓글 삭제</strong> </p> </th> 
      <th>댓글 해결</th> 
      <th>주석에 작업 적용</th> 
      <th> <p><strong>증명 편집</strong> </p> </th> 
      <th>다른 사람과 증명 공유</th> 
      <th>새 버전 만들기</th> 
      <th> <p><strong>홈 영역에서 승인 요청 보기</strong> </p> </th> 
      <th>새 검토자 추가</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>읽기 전용</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>검토자</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>승인자</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>검토자 및 승인자</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>작성자</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>중재자</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. 새 Workfront 계획의 사용자는 시스템의 모든 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다. 레거시 플랜의 사용자는 시스템에서 증명 라이센스를 가진 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다.
1. (선택 사항) 드롭다운 메뉴가 여전히 열려 있는 상태에서 메뉴 하단에 있는 사용 가능한 추가 권한을 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">댓글 해결 및 작업 적용 </td> 
      <td> <p>Workfront 사용자가 다음을 수행할 수 있습니다.</p> 
       <ul> 
        <li>설명이 지정된 후에 설명을 확인합니다. <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">증명 댓글 해결</a>.</li> 
        <li>다음에 설명된 대로 주석에 작업 적용 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">증명 주석에 작업 사용</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">태깅으로 증명 공유</td> 
      <td> <p>검토자가 다음에 설명된 대로 모든 Workfront 사용자를 증표에 추가할 수 있습니다. <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">사용자에게 태그를 지정하여 증명 공유</a>.</p> <p>참고:  <p>이 두 옵션을 사용할 수 없는 경우(흐리게 표시됨) 사용자에게 이미 사용 권한 프로필이 있어 주석을 확인하고, 작업에 주석을 적용하고, 사용자에게 태그를 지정할 수 있습니다. </p> <p>옵션이 표시되지 않으면 추가한 사용자가 Workfront 라이선스 소유자가 아닙니다.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 증명에 추가한 다른 사용자에 대해 1-3단계를 반복합니다.
1. 공유하는 각 사용자의 경우 **이메일 경고** 드롭다운 목록에서 사람들이 증명에 대한 댓글 및 결정을 할 때 이 사용자가 받는 이메일 경고 유형을 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모든 활동</td> 
      <td>Workfront은 증명에 새 댓글, 회신, 의사 결정 등 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>이것은 언어 교정 프로세스를 관리하는 사람에게 매우 좋은 옵션입니다. 언어 교정 프로세스를 관리하는 사람은 진행 중인 활동을 볼 수 있기 때문입니다. </p><p>사용자는 자신의 활동에 대한 이메일 경고를 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 댓글에 답글</td> 
      <td>누군가 자신의 댓글에 명시적으로 답장하는 경우에만 검토자에게 이메일이 전송됩니다(자체 댓글에 대해서는 자신의 답글이 제외됨). 즉, 증명의 누군가가 새 주석을 작성하면 검토자가 알림을 받지 않습니다.<p>이 설정은 증거에 대한 다른 댓글에 대한 알림을 받지 않고, 자신의 댓글에 대한 응답만 받도록 클라이언트가 증명에 대해 권장됩니다.</p><p>이 전자 메일 경고 설정을 사용하는 검토자는 다른 새 주석에 대한 알림을 받지 않지만 언어 교정 뷰어에서 증명에 대한 모든 주석을 볼 수 있습니다.</p><p>주석에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정</td> 
      <td>Workfront은 누군가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하고 있는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명의 진행 상황을 모니터링하여 어떤 사용자가 결정을 했는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않은 경우, 사용자의 결정에 대한 알림을 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">최종 결정</td> 
      <td>Workfront은 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 종종 디자이너가 사용하는데, 일반적으로 실제 검토 토론에 참여할 필요가 없습니다. 최종 결정을 내리면 디자이너에게 알림이 전송되고 필요한 변경 사항에 대해 조치를 취할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료된 경우에만 알림을 받아야 하는 부서 리더에게 유용할 수도 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간별 요약</td> 
      <td>Workfront에서는 매시간마다 발생한 모든 댓글, 회신, 의사 결정에 대한 요약으로 이메일을 검토자에게 보냅니다.<p>이메일 은 사용자 이외의 활동이 지난 시간 내에 발생하는 경우에만 전송됩니다. </p><p>이 경고는 프로젝트 개요를 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례 예제는 프로젝트 개요가 필요하지만 증명의 모든 활동에 대해 즉시 알림을 받을 필요가 없는 선임 검토자입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">일별 요약</td> 
      <td>Workfront은 사용자 이외의 활동이 있는 경우에만 나열된 모든 댓글, 회신 및 의사 결정이 있는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트로 압도되지 않고 프로젝트 요약을 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 책임자입니다.</p><p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이메일 없음</td> 
      <td>Workfront은 이메일 경고를 전송하지 않습니다.<br>이 기능은 참조 목적으로만 증명에 추가되고 변경 사항에 대한 알림을 받을 필요가 없는 사용자에게 유용합니다.<p>시스템 기본값은 일별 요약 (설정이 안 됨으로 표시됨)입니다. 사용자 또는 검토자가 다른 변경 작업을 수행하지 않는 경우 모든 증명에 이 설정이 있습니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 계속 [증명에 대한 이메일 설정 구성](#configure-email-settings-for-the-proof) 아래의 제품에서 사용할 수 있습니다.

## 증명에 대한 이메일 설정 구성 {#configure-email-settings-for-the-proof}

1. 에서 **이메일 알림** 섹션에서 선택한 사용자에게 이메일 알림 및 사용자 지정 메시지를 전송할지 여부를 선택합니다 [기본 워크플로우를 사용하여 고급 증명 만들기](#workflow) 이 문서의 앞 부분:

   <table>
   <tbody>
   <tr>
   <td>이 증명에 대해 수신자에게 알림</td>
   <td>사용자에게 이메일 알림을 전송하려면 이 옵션을 선택합니다. When <strong>기본 공유</strong> 에서 선택됨 <strong>워크플로우</strong> 섹션을 통해 증명을 만들 때 이메일 알림이 전송됩니다. When <strong>자동화된 워크플로우</strong> 에서 선택됨 <strong>워크플로우</strong> 섹션에 있는 경우, 증명으로 인해 사용자가 연결된 자동화된 워크플로우의 단계가 되면 이메일 알림이 전송됩니다.</td>
   </tr>
   <tr>
   <td>사용자 지정 메시지 추가</td>
   <td>알림에 사용자 지정 메시지를 포함하려면 이 옵션을 선택합니다. 제목과 메시지 본문을 지정할 수 있습니다. 메시지 본문에 굵게, 글머리 기호 및 하이퍼링크와 같은 서식 있는 텍스트 서식이 포함될 수 있습니다.</td>
   </tr>
   </tbody>
   </table>


1. 계속 [증명 설정 구성](#configure-proof-settings) 아래의 제품에서 사용할 수 있습니다.

## 증명 설정 구성 {#configure-proof-settings}

1. 에서 **증명 설정** 섹션에서 다음 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">로그인 필요 - 증명은 다른 사용자만 공유할 수 있습니다</td> 
      <td>이 옵션이 비활성화되어 있으면(기본값) URL을 가진 모든 사용자가 증명을 볼 수 있습니다. <br>이 옵션을 선택한 경우:
       <ul>
        <li>Workfront 증명 사용자만 증명을 볼 수 있습니다.</li>
        <li>증명에 추가되지 않으면 사용자가 증명에 로그인할 수 없습니다.</li>
        <li>구독을 사용하도록 설정할 수 없습니다.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">이 증명에 필요한 결정은 하나만</td> 
      <td>이 옵션을 선택하면 결정권자 중 한 명이 결정을 하면 리뷰가 완료됩니다.<br>이 옵션은 기본적으로 비활성화됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요</td> 
      <td>사용자는 증명을 결정할 때 사용자 이름과 암호를 지정해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 모든 결정을 내릴 때 증명 잠금</td> 
      <td>이 설정을 사용하면 모든 결정을 수행한 후 증명 상태가 잠깁니다. 최종 승인자가 결정을 내릴 때 상태가 자동으로 잠금 해제에서 잠금으로 변경됩니다.<br>이 옵션은 기본적으로 비활성화됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">원본 파일 다운로드</td> 
      <td>이 옵션을 선택하면 검토자가 증명을 만든 원본 파일을 다운로드할 수 있습니다.<br>이 옵션을 선택 취소하면 더 이상 다운로드 아이콘이 표시되지 않습니다.<br>이 옵션은 기본적으로 활성화되어 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 공유</td> 
      <td>이 옵션을 선택하면 공개 URL 또는 포함 코드를 통해 증명을 공유할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 구독</td> 
      <td>이 옵션을 선택하면 증명에 명시적으로 추가되지 않은 사람이 증명에 가입할 수 있습니다. 증명을 구독하는 사람에게 다음 설정에서 정의하는 역할 및 전자 메일이 부여됩니다.
       <ul>
        <li><strong>가입자 역할:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 증명 역할입니다. </li>
        <li><strong>구독자에 대한 전자 메일 경고 설정:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 전자 메일 경고입니다.</li>
       </ul><p>
        <ul>
         <li><strong>다음에 필요한 이메일 링크를 통한 증명 액세스:</strong> 구독자가 증명 링크가 포함된 이메일을 수신하는지 여부를 구성합니다. 선택할 수 있습니다 <strong>이메일 없음</strong> (증명 액세스에 이메일 링크가 필요하지 않음), <strong>증명 알림 이메일만</strong> (구독자는 확인 없이 이메일을 통해 증명의 링크를 수신함) 또는 <strong>유효성 검사 및 증명 알림 이메일</strong> (구독자는 이메일을 통해 증명의 링크를 받고 링크를 클릭하여 증표에 액세스해야 하며, 이 옵션의 목적은 사용자가 액세스할 수 있는 올바른 이메일 주소를 입력했는지 확인하는 것입니다.)</li>
        </ul><p>참고:  증명에 자동화된 워크플로우가 첨부된 경우 모든 구독이 증명 소유자에 대한 확인 이메일을 생성하므로 사용자가 추가되어야 하는 단계를 결정할 수 있습니다.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **증명 만들기**.

   Workfront에서 선택한 문서 또는 웹 사이트의 증명을 생성하기 시작합니다. 파일 크기와 유형에 따라 문서 업로드의 지연 시간이 다를 수 있습니다. 더 큰 파일이 생성되려면 시간이 더 오래 걸리므로 기다려 주십시오. 페이지에서 멀리 이동할 수 있으며 Workfront에서 계속해서 파일을 생성합니다. 최대 파일 업로드 크기는 4GB입니다.

1. 증명을 생성한 후 **공개 증명** 교정 뷰어를 실행하려면

   ![](assets/open-proof-350x132.png)

   계정에 언어 교정이 설정되어 있지 않은 사용자는 여전히 문서를 보고 증표에 주석을 달 수 있습니다.