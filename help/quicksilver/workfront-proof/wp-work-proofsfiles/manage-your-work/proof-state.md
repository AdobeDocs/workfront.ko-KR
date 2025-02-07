---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Workfront Proof의 증명 상태 이해
description: ' [!DNL Workfront Proof]에서 증명이 다른 상태에 있습니다. 이 상태는 댓글이나 의사 결정 등 증명에 대해 취할 수 있는 조치를 결정합니다.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Workfront Proof의 증명 상태 이해

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront Proof]에서 증명이 다른 상태에 있습니다. 이 상태는 댓글이나 의사 결정 등 증명에 대해 취할 수 있는 조치를 결정합니다.

## 증명 상태 이해

네 가지 상태는 다음과 같습니다.

* [활성](#active)
* [잠김](#locked)
* [초안(드롭 영역만)](#draft-dropzone-only)
* [제출됨(드롭 영역만)](#submitted-dropzone-only)

### 활성 {#active}

새 증명 페이지나 드롭 영역을 통해 [!DNL Workfront Proof]에 업로드된 증명은 처리된 후 활성으로 표시됩니다. 증명이 활성 상태일 때 사용자는 증명을 검토하고, 댓글을 달고, 증명에 대한 결정을 내릴 수 있습니다.

>[!NOTE]
>
>드롭 영역을 통해 업로드된 증명은 제출 시 증명 활성화 옵션이 활성화된 경우에만 활성으로 표시됩니다. 옵션이 활성화되지 않은 경우 증명을 수동으로 활성화해야 합니다.

드롭 영역 설정에 대한 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

### 잠김 {#locked}

검토를 마치면 증명을 잠글 수 있습니다. 증명을 잠그면 증명에 더 이상 댓글이나 결정을 내릴 수 없지만 증명을 계속 열 수 있습니다.

증명에 대한 편집 권한이 있는 모든 사용자가 잠금을 해제할 수 있습니다.

권한에 대한 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)을 참조하세요.

>[!NOTE]
>
>증명이 잠겨 있을 때 이메일 알림이 더 이상 전송되지 않습니다. 예를 들어, 기한 전에 증명이 잠긴 경우 기한에 도달해도 알림 이메일이 전송되지 않습니다.

### 초안(드롭 영역만) {#draft-dropzone-only}

드롭존을 통해 증명을 제출하면 관리자가 활성화하기 전에 초안 상태로 전환됩니다. 초안 영역에 있는 경우 증명에 대해 어떤 작업도 수행할 수 없습니다.

### 제출됨(드롭 영역만) {#submitted-dropzone-only}

관리자가 초안을 활성화하면 증명이 드롭존에 제출됨으로 표시됩니다. 제출 후 증명에 대한 조치를 취할 수 있습니다.

## 증명 상태 보기 및 변경

모든 활성 증명 또는 잠긴 증명 보기와 같이 특정 상태의 모든 증명 목록을 보는 방법에 대한 자세한 내용은 [보기 페이지의 항목 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 문서의 [보기 페이지의 항목 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)를 참조하십시오.

1. [!DNL Workfront Proof] 대시보드에 액세스합니다.

   자세한 내용은 [Adobe Workfront에서  [!DNL Workfront Proof] 액세스](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)를 참조하십시오.

1. **[!UICONTROL 대시보드]**&#x200B;에서 보려는 증명 옆의 **[!UICONTROL 확장]** 화살표를 클릭하거나 상태를 변경합니다.

   ![확장](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   **[!UICONTROL 워크플로 프로세스]** 섹션이 나타납니다.

   ![워크플로 프로세스](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. **[!UICONTROL 워크플로 프로세스]**&#x200B;에서 **[!UICONTROL 상태]**&#x200B;를 봅니다.

1. (선택 사항) 상태를 변경하려면 현재 **[!UICONTROL 상태]** 위로 마우스를 가져간 후 드롭다운 메뉴를 클릭한 다음 새 상태를 선택합니다.

   ![새 상태](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
