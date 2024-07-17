---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 증명된 이메일
description: 증명 생성 이메일은 증명을 만든 경우에만 증명 생성자에게 전송됩니다. 어떤 사람이 증명을 만들고 다른 사람을 소유자로 만든 경우 새 소유자만 증명 전자 메일도 받습니다. 작성자 및/또는 소유자는 증명을 받을 수 없으며, 증명 확인 이메일만 받습니다. 새 증명 이메일에 대한 자세한 내용은 새 증명 이메일 을 참조하십시오.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# [!UICONTROL 증명 작성] 전자 메일

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

증명을 만든 경우에만 [!UICONTROL 증명 작성] 이메일이 증명 작성자에게 전송됩니다. 사용자가 증명을 만들고 다른 사용자를 소유자로 지정한 경우 새 소유자만 [!UICONTROL 증명 완료] 전자 메일도 받습니다. 작성자 및/또는 소유자는 증명을 받지 못합니다. [!UICONTROL 증명 완료] 이메일만 받습니다. [!UICONTROL 새 증명] 전자 메일에 대한 자세한 내용은 [[!UICONTROL 새 증명] 전자 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)을 참조하세요.

사용자는 아래에 설명된 대로 프로필 설정에서 [!UICONTROL 증명] 이메일을 비활성화할 수 있습니다.

>[!NOTE]
>
> 증명의 작성자 또는 소유자가 [!UICONTROL 새 증명] 페이지에서 [!UICONTROL 이메일로 사람들에게 알림] 상자를 선택하더라도 기본적으로 개인 설정에서 [!UICONTROL 증명 작성]된 이메일이 비활성화되어 있으면 [!UICONTROL 증명 작성] 또는 [!UICONTROL 새 증명]된 이메일을 받지 못합니다.

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

[!UICONTROL 증명된] 이메일에는 귀하의 개인 메시지(포함된 경우)와 다음 증명 세부 정보가 포함되어 있습니다.

* 교정쇄 이름
* 증명에 대한 개인 링크
* 버전 번호
* 증명의 썸네일
* 교정 진행 상황
* 다른 사람과 증명 공유를 위한 링크
* 이를 통해 원본 파일에 대한 증명 URL 및/또는 다운로드 링크를 공유할 수 있습니다.

>[!NOTE]
>
> 증명 링크를 공유하면 증명에 검토자를 명시적으로 추가할 수 없으며 공개 증명 URL만 공유하게 되고 수신자는 증명에 대한 읽기 전용 액세스 권한을 받게 됩니다.

자세한 내용은 [증명 공유 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)를 참조하십시오.

이 링크가 받는 사람의 전자 메일에 표시되지 않도록 하려면 증명에서 [!UICONTROL 공개 공유] 설정을 사용하지 않도록 설정해야 합니다([!UICONTROL 원본 파일 다운로드] 및 [!UICONTROL 공개 URL]).

## [!UICONTROL 증명 작성] 전자 메일 비활성화

1. **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**&#x200B;을 클릭하고 **[!UICONTROL 증명 기본값]** 탭을 연 다음 **[!UICONTROL 증명이 준비되면 전자 메일 확인]** 옆에 있는 **[!UICONTROL 비활성화]**&#x200B;를 클릭합니다.

1. ![Proof_Made_-_proof_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. 자세한 지침은 [Workfront Proof에서 전자 메일 알림 설정 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)을 참조하세요.
1. [!UICONTROL 계정 설정]에서 전자 메일 알림을 기본값으로 사용하지 않도록 설정한 경우, 개인 설정에서 [!UICONTROL 증명 작성] 또는 [!UICONTROL 새 증명] 전자 메일을 받지 못합니다. [!UICONTROL 새 증명] 페이지에서 [!UICONTROL 전자 메일로 사람들에게 알림] 상자를 선택하더라도 증명의 작성자 또는 소유자는 해당 전자 메일을 받지 못합니다.
