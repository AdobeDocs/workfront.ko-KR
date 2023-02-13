---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 에서 전자 메일 알림 설정 구성 [!DNL Workfront Proof]
description: 이메일 알림은 공동 작업자에게 설명, 회신, 의사 결정 등 증명에 대한 최근 활동에 대해 알려줍니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# 에서 전자 메일 알림 설정 구성 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

이메일 알림은 공동 작업자에게 설명, 회신, 의사 결정 등 증명에 대한 최근 활동에 대해 알려줍니다.

검토자를 위한 이메일 알림은 새 증명 페이지에서 설정할 수 있습니다. [!UICONTROL 새 버전] 페이지에서 관리 [!UICONTROL 워크플로우] 섹션 [!UICONTROL 증명 세부 사항] 페이지. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [의 증명 세부 정보 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

또한 모든 사용자는 증명을 공유할 때 자동으로 적용되는 고유한 이메일 경고 설정을 설정할 수도 있습니다. 공동 작업자가 기본 설정을 가지고 있거나 계정 관리자가 경고 빈도에 대한 권장 사항을 가지고 있는 경우. 사용자 세부 사항 페이지에서 기본값이라는 증명을 설정할 수 있습니다.

>[!NOTE]
>
>이러한 설정은 사용자가 증명을 만들고 이러한 공동 작업자를 추가할 때 권장됩니다. 하지만 이러한 제안은 제안만 하므로 검토 프로세스 중에 언제든지 조정할 수 있으며, 변경 사항은 변경 후 수행된 모든 활동에 적용됩니다. 증명 기본 설정은 증명 수준의 설정에 의해 재정의됩니다.

사용 중인 사용자 [!UICONTROL 관리자] 또는 [!UICONTROL 청구 관리자] 또한 프로필 은 계정 설정 내에서 계정에 있는 다른 사용자의 증명 기본값을 설정할 수도 있습니다.

프로필에 대한 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [개인 설정에서 증명 기본값 구성([!DNL Workfront Proof] 사용자만 해당)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [수신자에 대한 이메일 경고 변경](#change-email-alerts-for-a-recipient)
* [사용자에 대한 증명 기본값 구성](#configure-proof-defaults-for-a-user)

## 개인 설정에서 증명 기본값 구성([!DNL Workfront Proof] 사용자만 해당)

증명을 만들 때 증명 설정을 구성할 수 있습니다.

증명 설정에 대한 자세한 내용은 [!DNL Workfront] 관리자 또는 [!DNL Workfront Proof] 관리자가 구성할 수 있습니다. 자세한 내용은

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**.

1. 을(를) 클릭합니다. **[!UICONTROL 교정 기본값]** 탭.
1. 클릭 **[!UICONTROL 기본 전자 메일 알림 설정]** 를 확장하려면 다음을 수행하십시오.
1. 다음 두 설정 오른쪽에 있는 드롭다운 목록에서 아래 표에 설명된 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 기본 이메일 경고]**: 은 사용자와 공유되는 모든 증표에 영향을 줍니다. 이 설정은 증명 수준에서 대체할 수 있습니다.
   * **[!UICONTROL 새 게스트 검토자에 대한 기본 전자 메일 경고]**: 이전에 계정에 연락처로 존재하지 않았던 검토자에게 영향을 줍니다.

   >[!NOTE]
   >
   >다음 옵션 중 하나를 선택하지 않으면 [!DNL Workfront Proof] 증명에서 활동에 대한 일별 요약을 보냅니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront]은 증명에 새 주석, 회신, 의사 결정 등 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>이것은 언어 교정 프로세스를 관리하는 사람에게 매우 좋은 옵션입니다. 언어 교정 프로세스를 관리하는 사람은 진행 중인 활동을 볼 수 있기 때문입니다. </p><p>사용자는 자신의 활동에 대한 이메일 경고를 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 내 댓글에 회신]</td> 
      <td>누군가 자신의 댓글에 명시적으로 답장하는 경우에만 검토자에게 이메일이 전송됩니다(자체 댓글에 대해서는 자신의 답글이 제외됨). 즉, 증명의 누군가가 새 주석을 작성하면 검토자가 알림을 받지 않습니다.<p>이 설정은 증거에 대한 다른 댓글에 대한 알림을 받지 않고, 자신의 댓글에 대한 응답만 받도록 클라이언트가 증명에 대해 권장됩니다.</p><p>이 전자 메일 경고 설정을 사용하는 검토자는 다른 새 주석에 대한 알림을 받지 않지만 언어 교정 뷰어에서 증명에 대한 모든 주석을 볼 수 있습니다.</p><p>주석에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 결정]</td> 
      <td>[!DNL Workfront] 누군가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하고 있는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명의 진행 상황을 모니터링하여 어떤 사용자가 결정을 했는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않은 경우, 사용자의 결정에 대한 알림을 받지 않습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 최종 결정]</td> 
      <td>[!DNL Workfront] 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 종종 디자이너가 사용하는데, 일반적으로 실제 검토 토론에 참여할 필요가 없습니다. 최종 결정을 내리면 디자이너에게 알림이 전송되고 필요한 변경 사항에 대해 조치를 취할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료된 경우에만 알림을 받아야 하는 부서 리더에게 유용할 수도 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시간별 요약]</td> 
      <td>[!DNL Workfront] 매시간 검토자에게 해당 시간에 발생한 모든 댓글, 회신 및 의사 결정에 대한 요약으로 이메일을 보냅니다.<p>이메일 은 사용자 이외의 활동이 지난 시간 내에 발생하는 경우에만 전송됩니다. </p><p>이 경고는 프로젝트 개요를 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례 예제는 프로젝트 개요가 필요하지만 증명의 모든 활동에 대해 즉시 알림을 받을 필요가 없는 선임 검토자입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] 사용자 이외의 활동이 있는 경우에만 나열된 모든 댓글, 회신 및 의사 결정이 있는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트로 압도되지 않고 프로젝트 요약을 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 책임자입니다.</p><p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 이메일 없음]</td> 
      <td>[!DNL Workfront] 은 이메일 경고를 전송하지 않습니다.<br>이 기능은 참조 목적으로만 증명에 추가되고 변경 사항에 대한 알림을 받을 필요가 없는 사용자에게 유용합니다.<p>시스템 기본값은 [!UICONTROL 일별 요약]([!UICONTROL Not Set]으로 표시됨)입니다. 사용자 또는 검토자가 다른 변경 작업을 수행하지 않는 경우 모든 증명에 이 설정이 있습니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 증명 준비 시 이메일 확인]</td> 
      <td>증명을 만들 때 [!UICONTROL 증명] 이메일을 수신할지 여부를 지정합니다. 자세한 내용은 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL Proof Made] 전자 메일</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 나에게 보낸 전자 메일의 형식]</strong> </td> 
      <td> <p>HTML 스타일이 지정된 이메일과 일반 텍스트 이메일 중에서 선택합니다. </p> <p>참고:  교정 기본 설정은 증명 수준의 설정에 의해 재정의됩니다. 그러나 [!UICONTROL 계정] 설정에서 전체 계정에 대해 증명 이메일 알림이 비활성화된 경우 증명에서 [!UICONTROL 비활성화된 이메일 경고]를 선택하지 않더라도 공동 작업자에게 이메일 경고가 전송되지 않습니다.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 아래 **[!UICONTROL 메시지 설정]**, 다음 중 하나를 변경합니다.

   | **[!UICONTROL 증명 제목 템플릿]** | 새 증명 페이지, 새 버전 페이지, 메시지 페이지 및 알림 페이지에 표시됩니다. 전송되기 전에 편집할 수 있습니다. |
   |---|---|
   | **[!UICONTROL 증명 메시지 템플릿]** | 새 증명 페이지, 새 버전 페이지, 메시지 페이지 및 알림 페이지에 표시됩니다. 전송되기 전에 편집할 수 있습니다. |

   {style=&quot;table-layout:auto&quot;}

## 수신자에 대한 이메일 경고 변경

배치 작업에서 특정 수신자에 대한 이메일 경고를 변경할 수 있습니다.

1. 클릭 **[!UICONTROL 연락처]** 왼쪽 탐색 패널
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 받는 사람에 대한 (세 점) 메뉴를 클릭한 다음 **[!UICONTROL 멤버 세부 정보 보기]** 드롭다운 메뉴에서 을 클릭합니다.

1. 를 엽니다. **[!UICONTROL 공유 항목]** 섹션을 참조하십시오.
1. 전자 메일 경고를 변경할 각 항목 왼쪽에 있는 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 자세히]** 공유 항목 목록 위에 있는 **[!UICONTROL 전자 메일 경고 변경]** 드롭다운 메뉴에서 을 클릭합니다.

1. 전자 메일 경고를 변경한 다음 **[!UICONTROL 제출]**.

## 사용자에 대한 증명 기본값 구성

만약 [!DNL Workfront Proof] 관리자는 계정의 사용자에 대한 증명 기본값을 설정할 수 있습니다.

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**.

1. 를 엽니다. **[!UICONTROL 사용자]** 탭.
1. 를 엽니다. **[!UICONTROL 자세히]** 메뉴 아래의 제품에서 사용할 수 있습니다. ![More_button_small.png](assets/more-button-small.png)

1. 클릭 **[!UICONTROL 사용자 세부 사항 보기]** 드롭다운 메뉴에서 을 클릭합니다.
1. 아래 **[!UICONTROL 설정]**&#x200B;를 클릭합니다. **[!UICONTROL 기본 전자 메일 경고 설정]** 를 확장하려면 다음을 수행하십시오.

1. 다음 두 설정 오른쪽에 있는 드롭다운 목록에서 아래 표에 설명된 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 기본 이메일 경고]**: 은 사용자와 공유되는 모든 증표에 영향을 줍니다. 이 설정은 증명 수준에서 대체할 수 있습니다.
   * **[!UICONTROL 새 게스트 검토자에 대한 기본 전자 메일 경고]**: 이전에 계정에 연락처로 존재하지 않았던 검토자에게 영향을 줍니다.

   >[!NOTE]
   >
   >사용자에 대해 다음 옵션 중 하나를 선택하지 않으면, [!DNL Workfront Proof] 사용자에게 증명 상의 활동에 대한 일별 요약을 보냅니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] 증명에 새 댓글, 회신, 의사 결정 등 활동이 있을 때마다 검토자에게 이메일을 보냅니다. <p>이것은 언어 교정 프로세스를 관리하는 사람에게 매우 좋은 옵션입니다. 언어 교정 프로세스를 관리하는 사람은 진행 중인 활동을 볼 수 있기 때문입니다. </p><p>사용자는 자신의 활동에 대한 이메일 경고를 받지 않습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 내 댓글에 회신]</td>
      <td>누군가 자신의 댓글에 명시적으로 답장하는 경우에만 검토자에게 이메일이 전송됩니다(자체 댓글에 대해서는 자신의 답글이 제외됨). 즉, 증명의 누군가가 새 주석을 작성하면 검토자가 알림을 받지 않습니다.<p>이 설정은 증거에 대한 다른 댓글에 대한 알림을 받지 않고, 자신의 댓글에 대한 응답만 받도록 클라이언트가 증명에 대해 권장됩니다.</p><p>이 전자 메일 경고 설정을 사용하는 검토자는 다른 새 주석에 대한 알림을 받지 않지만 언어 교정 뷰어에서 증명에 대한 모든 주석을 볼 수 있습니다.</p><p>주석에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">증명 댓글 보기 및 회신</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 결정]</td>
      <td>[!DNL Workfront] 누군가 결정을 내릴 때만 검토자에게 이메일을 보냅니다.<p>이 기능은 승인 프로세스를 관리하고 있는 사람(예: 프로젝트 관리자)에게 유용할 수 있으며, 증명의 진행 상황을 모니터링하여 어떤 사용자가 결정을 했는지 확인해야 합니다.</p><p>결정을 제출할 때 이메일 확인 옵션을 선택하지 않은 경우, 사용자의 결정에 대한 알림을 받지 않습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 최종 결정]</td>
      <td>[!DNL Workfront] 증명의 마지막 승인자가 결정을 내리면 이메일을 보냅니다.<p>이 경고는 종종 디자이너가 사용하는데, 일반적으로 실제 검토 토론에 참여할 필요가 없습니다. 최종 결정을 내리면 디자이너에게 알림이 전송되고 필요한 변경 사항에 대해 조치를 취할 수 있습니다.</p><p>이 경고는 검토 프로세스가 완료된 경우에만 알림을 받아야 하는 부서 리더에게 유용할 수도 있습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 시간별 요약]</td>
      <td>[!DNL Workfront] 매시간 검토자에게 해당 시간에 발생한 모든 댓글, 회신 및 의사 결정에 대한 요약으로 이메일을 보냅니다.<p>이메일 은 사용자 이외의 활동이 지난 시간 내에 발생하는 경우에만 전송됩니다. </p><p>이 경고는 프로젝트 개요를 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례 예제는 프로젝트 개요가 필요하지만 증명의 모든 활동에 대해 즉시 알림을 받을 필요가 없는 선임 검토자입니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] 사용자 이외의 활동이 있는 경우에만 나열된 모든 댓글, 회신 및 의사 결정이 있는 하나의 이메일을 보냅니다.<p>이 경고는 하루 종일 여러 업데이트로 압도되지 않고 프로젝트 요약을 보는 좋은 방법입니다.</p><p>이 요약의 사용 사례는 프로젝트의 전체 진행 상황을 모니터링하려는 부서 책임자입니다.</p><p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">증명 댓글 및 결정에 대한 알림 관리</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL 이메일 없음]</td>
      <td>[!DNL Workfront] 은 이메일 경고를 전송하지 않습니다.<br>이 기능은 참조 목적으로만 증명에 추가되고 변경 사항에 대한 알림을 받을 필요가 없는 사용자에게 유용합니다.<p>시스템 기본값은 [!UICONTROL 일별 요약]([!UICONTROL Not Set]으로 표시됨)입니다. 사용자 또는 검토자가 다른 변경 작업을 수행하지 않는 경우 모든 증명에 이 설정이 있습니다.</p></td>
     </tr>
    </tbody>
   </table>

1. 나머지 **[!UICONTROL 기본 전자 메일 경고 설정]**, 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 증명 준비 시 이메일 확인]</td> 
      <td>증명을 만들 때 [!UICONTROL 증명] 이메일을 수신할지 여부를 지정합니다. 자세한 내용은 <a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL 증명] 이메일이 작성되었습니다.</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 나에게 보낸 전자 메일의 형식]</strong> </td> 
      <td> <p>HTML 스타일이 지정된 이메일과 일반 텍스트 이메일 중에서 선택합니다. </p> <p>참고:  교정 기본 설정은 증명 수준의 설정에 의해 재정의됩니다. 그러나 [!UICONTROL 계정] 설정에서 전체 계정에 대해 증명 이메일 알림이 비활성화된 경우 증명에서 [!UICONTROL 비활성화된 이메일 경고]를 선택하지 않더라도 공동 작업자에게 이메일 경고가 전송되지 않습니다.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
