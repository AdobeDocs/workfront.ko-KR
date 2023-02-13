---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Workfront 증명의 증명 상태 이해
description: in [!DNL Workfront Proof], 증명은 다른 상태에 있습니다. 이러한 상태는 댓글 또는 의사 결정 등 증명에서 수행할 수 있는 작업을 결정합니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Workfront 증명의 증명 상태 이해

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

in [!DNL Workfront Proof], 증명은 다른 상태에 있습니다. 이러한 상태는 댓글 또는 의사 결정 등 증명에서 수행할 수 있는 작업을 결정합니다.

## 증명 상태 이해

네 가지 상태는 다음과 같습니다.

* [활성](#active)
* [잠김](#locked)
* [초안(Dropzone만)](#draft-dropzone-only)
* [제출됨(Dropzone만)](#submitted-dropzone-only)

### 활성 {#active}

에 업로드되는 증명 [!DNL Workfront Proof] 새 증명 페이지를 통해 또는 Dropzone이 처리된 후 활성 상태로 나타납니다. 증명의 활성 사용자는 증명의 검토, 주석 작성 및 결정 작업을 수행할 수 있습니다.

>[!NOTE]
>
>제출 시 증명 활성화 옵션이 활성화된 경우에만 Dropzone을 통해 업로드되는 증명을 활성 상태로 표시됩니다. 이 옵션이 활성화되지 않으면 증명을 수동으로 활성화해야 합니다.

Dropzone 설정에 대한 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### 잠김 {#locked}

검토를 마치면 증명을 잠글 수 있습니다. 증명을 잠그면 더 이상 증표에 대한 의견이나 결정을 내릴 수 없지만, 증명을 열 수 있습니다.

증명에 대한 편집 권한이 있는 모든 사용자는 이를 잠금 해제할 수 있습니다.

권한에 대한 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>증명이 잠겨 있으면 더 이상 전자 메일 알림이 전송되지 않습니다. 예를 들어, 증명을 마감일 전에 잠근 경우, 마감일이 되면 알림 이메일이 전송되지 않습니다.

### 초안(Dropzone만) {#draft-dropzone-only}

Dropzone을 통해 증명을 제출하면 관리자가 이를 활성화하기 전에 초안 상태로 전환됩니다. 초안 영역에 있으면 증표에 대해 작업을 수행할 수 없습니다.

### 제출됨(Dropzone만) {#submitted-dropzone-only}

관리자가 초안을 활성화하면 증명이 드롭존에 제출됨으로 표시됩니다. 제출되면 증명에 대한 조치를 취할 수 있습니다.

## 증명 상태 보기 및 변경

모든 활성 또는 잠긴 증명 표시와 같이 특정 상태의 모든 증명 목록을 보는 방법에 대한 자세한 내용은 [의 보기 페이지에서 항목 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 기사 [의 보기 페이지에서 항목 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 액세스 권한 [!DNL Workfront Proof] 대시보드.

   자세한 내용은 [액세스 [!DNL Workfront Proof] Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. 설정 **[!UICONTROL 대시보드]**&#x200B;를 클릭하고 **[!UICONTROL 확장]** 보거나 변경할 증명 옆에 있는 화살표

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   다음 **[!UICONTROL 워크플로우 프로세스]** 섹션이 나타납니다.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 보기 **[!UICONTROL 주/도]** 에서 **[!UICONTROL 워크플로우 프로세스]**.

1. (선택 사항) 상태를 변경하려면 현재 위로 마우스를 가져갑니다 **[!UICONTROL 주/도]** 드롭다운 메뉴를 클릭한 다음 새 상태를 선택합니다.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
