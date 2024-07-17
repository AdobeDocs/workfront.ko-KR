---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: ' [!DNL Workfront Proof]에서 드롭 영역 구성'
description: ' [!DNL Workfront Proof] 관리자는 사용자의 Dropzone 설정을 설정하고 보고 편집할 수 있습니다. Dropzone에 대한 자세한 내용은 Dropzone 을 참조하십시오.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# [!DNL Workfront Proof]에서 드롭 영역 구성

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront Proof] 관리자는 사용자의 Dropzone 설정을 설정하고 보고 편집할 수 있습니다. 드롭 영역에 대한 자세한 내용은 [드롭 영역](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)을 참조하세요.

1. **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**&#x200B;을 클릭한 다음 **[!UICONTROL 드롭 영역]** 탭을 엽니다.

1. **[!UICONTROL 드롭 영역 세부 정보]** 섹션에서 다음 중 하나를 변경합니다.

   * **[!UICONTROL 웹 드롭 영역]**: 드롭 영역을 활성화하거나 비활성화합니다.
   * **[!UICONTROL 웹 드롭 영역 URL]**: 드롭 영역을 통해 증명을 제출하려면 브라우저에 입력해야 하는 URL입니다.
   * **[!UICONTROL 전자 메일 드롭 영역]**: 전자 메일 드롭 영역을 활성화하거나 비활성화합니다.

     >[!NOTE]
     >
     >드롭 영역으로 전자 메일을 보내는 것은 더 이상 지원되지 않습니다.

   * **[!UICONTROL 드롭 영역 소유자]**: 드롭 영역 소유자를 설정하거나 편집합니다. 드롭 영역에 대한 새로운 제출 알림을 받을 사람입니다. Dropzone 소유자로 설정하려면 사용자가 감독자, 관리자, 청구 관리자 또는 계정 생성자여야 합니다. 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)을 참조하세요.

   * **[!UICONTROL 작성자의 기본 역할]**: 모든 제출자가 이 역할을 기본값으로 사용하여 증명에 추가됩니다.
   * **[!UICONTROL 모든 작성자에 대한 전자 메일 알림]**: 여기에서 증명 작성자(제출자)에 대한 전자 메일 경고 기본 설정을 지정하십시오. 사용 가능한 여러 경고 설정에 대한 자세한 내용은 [다음 위치에서 전자 메일 알림 설정 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)을 참조하십시오.

   * **[!UICONTROL 새 버전 함수]**: Dropzone에서 새 버전 함수를 사용하도록 설정하고 사용하지 않도록 설정합니다. 이를 통해 직원들이 Dropzone을 통해 새 버전의 증명을 제출할 수 있는 기능을 제공하거나 제거할 수 있습니다.
   * **[!UICONTROL 다음 기간 후 초안 증명 삭제(일)]**: 초안 증명이 삭제되는 기간(일)을 지정합니다. 파일을 드롭 영역에 업로드한 후 드롭 영역 제출이 완료되지 않은 경우 증명이 초안 상태로 유지됩니다.
   * **[!UICONTROL 검토자 역할 숨기기]**: Dropzone에 사용자를 추가할 때 검토자 역할 필드를 숨깁니다.
   * **[!UICONTROL 활성화 시 증명 메시지 보내기]**: 증명이 활성화될 때 자동으로 검토자에게 증명 알림 이메일을 보내도록 [!DNL Workfront Proof]을(를) 구성합니다.
   * **[!UICONTROL 제출 시 증명 활성화]**: 제출 시 증명을 자동으로 활성화하도록 [!DNL Workfront Proof]을(를) 구성합니다(수동으로 활성화해야 함).

   * 증명을 드롭 영역(예: 계정의 다른 폴더)에서 이동하면 드롭 영역 설정이 증명에 더 이상 적용되지 않습니다. 이는 이메일 경고 설정과 관련하여 특히 중요합니다.

1. **[!UICONTROL 드롭 영역 필드]** 섹션을 변경하여 드롭 영역을 통해 증명을 제출할 때 드롭 영역 제출 페이지의 [!UICONTROL 증명 세부 정보] 섹션에 표시되는 필드를 지정합니다.
1. **[!UICONTROL 허용된 도메인]** 섹션에서 드롭 영역 사용을 허용할 도메인을 지정합니다.

   * **[!UICONTROL 도메인 추가]**&#x200B;를 클릭하여 도메인을 추가할 수 있습니다. 도메인 세부 정보를 모두 추가했으면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   * 이전에 추가한 기존 도메인을 **[!UICONTROL 편집]** 및 **[!UICONTROL 삭제]**&#x200B;할 수 있습니다.

1. **[!UICONTROL 알릴 사람]**&#x200B;에서 새 증명이 Dropzone [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)에 제출될 때 Dropzone 소유자와 함께 알림을 받을 사람을 지정합니다

   * **[!UICONTROL 직원 추가]**&#x200B;를 클릭하고 받는 사람의 세부 정보를 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   * 이전에 추가한 사람을 **[!UICONTROL 삭제]**&#x200B;합니다.
