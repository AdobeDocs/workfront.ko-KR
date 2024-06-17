---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 에서 이메일 알림 설정 구성 [!DNL Workfront Proof]
description: Workfront Proof에서 생성된 이메일 알림은 공동 작업자에게 댓글, 답글 또는 의사 결정과 같은 증명에 대한 최근 활동에 대해 알립니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2049'
ht-degree: 0%

---

# 에서 이메일 알림 설정 구성 [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품의 기능에 대해 설명합니다 [!DNL Workfront Proof]. 내부 교정에 대한 정보 [!DNL Adobe Workfront], 참조 [증명](../../../review-and-approve-work/proofing/proofing.md).

이메일 알림은 공동 작업자에게 댓글, 답글 또는 의사 결정과 같은 증명에 대한 최근 활동에 대해 알립니다.

다음 영역의 검토자에 대한 이메일 알림을 설정할 수 있습니다.

새 증명 페이지에서 검토자에 대한 이메일 알림을 설정할 수 있습니다. [!UICONTROL 새 버전] 페이지 및 관리 [!UICONTROL 워크플로] 의 섹션 [!UICONTROL 증명 세부 정보] 페이지를 가리키도록 업데이트하는 중입니다. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* 새 증명 페이지
* 다음 [!UICONTROL 새 버전] 페이지
* 다음 [!UICONTROL 워크플로] 의 섹션 [!UICONTROL 증명 세부 정보] 페이지를 가리키도록 업데이트하는 중입니다.

자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [에서 증명 세부 정보 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


모든 사용자는 공동 작업자가 자신의 환경 설정을 가지고 있거나 계정 관리자에게 경고 빈도에 대한 권장 사항이 있는 경우 증명을 공유할 때 자동으로 적용되는 자신의 이메일 경고 설정을 지정할 수도 있습니다. 사용자 세부 정보 페이지에서 증명 기본값으로 설정할 수 있습니다.

모든 사용자는 증명을 공유할 때 자동으로 적용되는 자신만의 이메일 경고 설정을 지정할 수도 있습니다. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>이러한 설정은 사용자가 증명을 만들고 이러한 공동 작업자를 추가할 때 제안됩니다. 하지만 이는 제안일 뿐이므로 검토 프로세스 중에 언제든지 조정할 수 있으며 변경 사항은 변경 후에 수행된 모든 활동에 적용됩니다. 증명 기본 설정은 증명 수준의 설정에 의해 재정의됩니다.

을 사용하는 사용자 [!UICONTROL 관리자] 또는 [!UICONTROL 청구 관리자] 프로필은 계정 설정 내에서 계정의 다른 사용자에 대한 증명 기본값을 설정할 수도 있습니다.

프로필에 대한 자세한 내용은 [에서 증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">제품</td> 
   <td>Workfront Proof Standalone</td> 
  </tr> 
</table>

+++

## 개인 설정에서 증명 기본값 구성([!DNL Workfront Proof] 사용자만)

생성한 증명에 대한 증명 설정을 구성할 수 있습니다.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**.

1. 다음을 클릭합니다. **[!UICONTROL 증명 기본값]** 탭.
1. 클릭 **[!UICONTROL 기본 이메일 알림 설정]** 확장하기 위해
1. 다음 두 설정 오른쪽에 있는 드롭다운 목록에서 아래 표에 설명된 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 기본 이메일 경고]**: 나와 공유된 모든 증명에 영향을 줍니다. 증명 수준에서 이 설정을 재정의할 수 있습니다.
   * **[!UICONTROL 새 게스트 검토자에 대한 기본 이메일 경고]**: 이전에 계정에 연락처로 존재하지 않았던 검토자에게 영향을 줍니다.

   >[!NOTE]
   >
   >다음 옵션 중 하나를 선택하지 않으면 [!DNL Workfront Proof] 은(는) 교정본 활동에 대한 일별 요약을 보냅니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront]은(는) 새 댓글, 답글 또는 결정 등 증명에 대한 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>활동을 볼 수 있으므로 증명 프로세스를 관리하는 사용자에게 적합한 옵션입니다. </p><p>사용자는 자신의 활동에 대한 이메일 알림을 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 내 댓글에 답글 작성]</td> 
      <td>누군가 자신의 의견에 명시적으로 답글을 달 경우에만 검토자에게 이메일이 전송됩니다(자신의 의견에 대한 자신의 답글은 제외). 즉, 증명에 있는 사람이 새 댓글을 달면 검토자에게 알림이 전송되지 않습니다.<p>이 설정은 증명의 클라이언트가 증명의 다른 댓글에 대한 알림을 받지 않고 자신의 댓글에 대한 답글에만 알림을 받도록 하는 데 권장됩니다.</p><p>이 이메일 경고 설정을 사용하는 검토자는 다른 새 댓글에 대해 알림을 받지 못하지만 증명 뷰어에서 증명에 대한 모든 댓글을 볼 수 있습니다.</p><p>주석에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] 다른 사용자가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명 진행 상황을 모니터링하고 어떤 사용자가 결정을 내렸는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않으면 자신의 결정에 대한 알림이 전송되지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 최종 결정]</td> 
      <td>[!DNL Workfront] 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 설계자가 사용하는 경우가 많으며, 일반적으로 실제 검토 토론에 참여하지 않아도 됩니다. 최종 결정이 내려지면 디자이너는 알림을 받은 다음 필요한 변경 작업을 수행할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료되어야 알림을 받아야 하는 부서 리더에게도 유용할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시간별 요약]</td> 
      <td>[!DNL Workfront] 은(는) 매 시간마다 해당 시간에 발생한 모든 댓글, 답글 및 의사 결정에 대한 요약이 포함된 전자 메일을 검토자에게 보냅니다.<p>지난 1시간 내에 자신의 활동 이외의 활동이 발생한 경우에만 이메일이 전송됩니다. </p><p>이 경고는 프로젝트의 개요를 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트 개요가 필요하지만 증명에 대한 모든 활동을 즉시 알릴 필요가 없는 선임 검토자입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 일일 요약]</td> 
      <td>[!DNL Workfront] 은(는) 자신의 활동 이외의 활동이 있는 날에만 나열된 모든 댓글, 답글 및 결정을 포함하는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트가 쏟아지지 않고 프로젝트 요약을 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 리더입니다.</p><p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 없음]</td> 
      <td>[!DNL Workfront] 은 이메일 경고를 전송하지 않습니다.<br>이 기능은 참조용으로만 증명에 추가되고 변경 사항에 대한 알림이 필요하지 않은 사용자에게 유용합니다.<p>시스템 기본값은 [!UICONTROL Daily summary]([!UICONTROL Not Set]으로도 표시됨)입니다. 사용자 또는 검토자가 다른 변경 내용을 적용하지 않으면 모든 증명에 이 설정이 적용됩니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">증명이 준비되면 [!UICONTROL 이메일 확인]</td> 
      <td>증명을 만들 때 [!UICONTROL Proof made] 이메일을 수신할지 여부를 지정합니다. 자세한 내용은 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL Proof Made] 이메일</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 나에게 보낸 이메일 형식] </td> 
      <td> <p>HTML 스타일의 이메일과 일반 텍스트 이메일 중에서 선택합니다. </p> <p><b>메모</b></p>
      <p>증명 기본 설정은 증명 수준의 설정에 의해 재정의됩니다. 그러나 [!UICONTROL Account] 설정에서 전체 계정에 대해 증명 이메일 알림이 비활성화되어 있으면 증명에 대해 [!UICONTROL 비활성화된 이메일 알림]을 선택하지 않았더라도 공동 작업자에게 이메일 알림이 전송되지 않습니다.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 아래 **[!UICONTROL 메시지 설정]**, 다음 중 하나를 변경합니다.

   | 증명 템플릿 | 설명 |
   |---|---|
   | **[!UICONTROL 증명 제목 템플릿]** | 새 증명 페이지, 새 버전 페이지, 메시지 페이지 및 알림 페이지에 표시됩니다. 전송되기 전에 편집할 수 있습니다. |
   | **[!UICONTROL 증명 메시지 템플릿]** | 새 증명 페이지, 새 버전 페이지, 메시지 페이지 및 알림 페이지에 표시됩니다. 전송되기 전에 편집할 수 있습니다. |

## 수신자에 대한 이메일 경고 변경

일괄 처리 작업에서 특정 수신자에 대한 이메일 경고를 변경할 수 있습니다.

1. 클릭 **[!UICONTROL 연락처]** 을 클릭합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![](assets/more-button-small.png) 수신자에 대해 를 클릭한 다음 **[!UICONTROL 멤버 세부 정보 보기]** 드롭다운 메뉴에서 을(를) 선택합니다.

1. 를 엽니다. **[!UICONTROL 공유 항목]** 섹션.
1. 이메일 경고를 변경할 각 항목의 왼쪽에 있는 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 자세히]** 공유 항목 목록 위에서 **[!UICONTROL 이메일 경고 변경]** 드롭다운 메뉴에서 을(를) 선택합니다.

1. 이메일 경고를 변경한 다음 를 클릭합니다. **[!UICONTROL 제출]**.

## 사용자에 대한 증명 기본값 구성

다음과 같은 경우 [!DNL Workfront Proof] 관리자, 계정의 사용자에 대한 증명 기본값을 설정할 수 있습니다.

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**.

1. 를 엽니다. **[!UICONTROL 사용자]** 탭.
1. 를 엽니다. **[!UICONTROL 자세히]** 메뉴 ![More_button_small.png](assets/more-button-small.png) 사용자 이름 오른쪽에 있습니다.

1. 클릭 **[!UICONTROL 사용자 세부 정보 보기]** 드롭다운 메뉴에서 을(를) 선택합니다.
1. 아래 **[!UICONTROL 설정]**, 클릭 **[!UICONTROL 기본 이메일 경고 설정]** 확장하기 위해

1. 다음 두 가지 설정의 오른쪽에 있는 드롭다운 목록에서 아래 표에 설명된 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 기본 이메일 경고]**: 나와 공유된 모든 증명에 영향을 줍니다. 증명 수준에서 이 설정을 재정의할 수 있습니다.
   * **[!UICONTROL 새 게스트 검토자에 대한 기본 이메일 경고]**: 이전에 계정에 연락처로 존재하지 않았던 검토자에게 영향을 줍니다.

   >[!NOTE]
   >
   >사용자에 대해 다음 옵션 중 하나를 선택하지 않으면 [!DNL Workfront Proof] 은 사용자에게 증명에 대한 활동에 대한 일별 요약을 보냅니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] 새 댓글, 회신 또는 결정 등 증명에 대한 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>활동을 볼 수 있으므로 증명 프로세스를 관리하는 사용자에게 적합한 옵션입니다. </p><p>사용자는 자신의 활동에 대한 이메일 알림을 받지 않습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 내 댓글에 답글 작성]</td>
      <td>누군가 자신의 의견에 명시적으로 답글을 달 경우에만 검토자에게 이메일이 전송됩니다(자신의 의견에 대한 자신의 답글은 제외). 즉, 증명에 있는 사람이 새 댓글을 달면 검토자에게 알림이 전송되지 않습니다.<p>이 설정은 증명의 클라이언트가 증명의 다른 댓글에 대한 알림을 받지 않고 자신의 댓글에 대한 답글에만 알림을 받도록 하는 데 권장됩니다.</p><p>이 이메일 경고 설정을 사용하는 검토자는 다른 새 댓글에 대해 알림을 받지 못하지만 증명 뷰어에서 증명에 대한 모든 댓글을 볼 수 있습니다.</p><p>주석에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] 다른 사용자가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명 진행 상황을 모니터링하고 어떤 사용자가 결정을 내렸는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않으면 자신의 결정에 대한 알림이 전송되지 않습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 최종 결정]</td>
      <td>[!DNL Workfront] 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 설계자가 사용하는 경우가 많으며, 일반적으로 실제 검토 토론에 참여하지 않아도 됩니다. 최종 결정이 내려지면 디자이너는 알림을 받은 다음 필요한 변경 작업을 수행할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료되어야 알림을 받아야 하는 부서 리더에게도 유용할 수 있습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 시간별 요약]</td>
      <td>[!DNL Workfront] 은(는) 매 시간마다 해당 시간에 발생한 모든 댓글, 답글 및 의사 결정에 대한 요약이 포함된 전자 메일을 검토자에게 보냅니다.<p>지난 1시간 내에 자신의 활동 이외의 활동이 발생한 경우에만 이메일이 전송됩니다. </p><p>이 경고는 프로젝트의 개요를 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트 개요가 필요하지만 증명에 대한 모든 활동을 즉시 알릴 필요가 없는 선임 검토자입니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 일일 요약]</td>
      <td>[!DNL Workfront] 은(는) 자신의 활동 이외의 활동이 있는 날에만 나열된 모든 댓글, 답글 및 결정을 포함하는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트가 쏟아지지 않고 프로젝트 요약을 볼 수 있는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 리더입니다.</p><p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL 이메일 없음]</td>
      <td>[!DNL Workfront] 은 이메일 경고를 전송하지 않습니다.<br>이 기능은 참조용으로만 증명에 추가되고 변경 사항에 대한 알림이 필요하지 않은 사용자에게 유용합니다.<p>시스템 기본값은 [!UICONTROL Daily summary]([!UICONTROL Not Set]으로도 표시됨)입니다. 사용자 또는 검토자가 다른 변경 내용을 적용하지 않으면 모든 증명에 이 설정이 적용됩니다.</p></td>
     </tr>
    </tbody>
   </table>

1. 남은 시간 **[!UICONTROL 기본 이메일 경고 설정]**, 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">증명이 준비되면 [!UICONTROL 이메일 확인]</td> 
      <td>증명을 만들 때 [!UICONTROL Proof made] 이메일을 수신할지 여부를 지정합니다. 자세한 내용은 <a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL Proof Made] 이메일.</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 나에게 보낸 이메일 형식] </td> 
      <td> <p>HTML 스타일의 이메일과 일반 텍스트 이메일 중에서 선택합니다. </p> <p><b>메모</b></p> <p>증명 기본 설정은 증명 수준의 설정에 의해 재정의됩니다. 그러나 [!UICONTROL Account] 설정에서 전체 계정에 대해 증명 이메일 알림이 비활성화되어 있으면 증명에 대해 [!UICONTROL 비활성화된 이메일 알림]을 선택하지 않았더라도 공동 작업자에게 이메일 알림이 전송되지 않습니다.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
