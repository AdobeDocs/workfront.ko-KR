---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 지연 증명 이메일
description: 증명이 마감일 또는 최종 기한에 도달하면 수신자에게 지연 증명 이메일이 전송됩니다. 이러한 유형의 이메일은 증명 수준에서 비활성화할 수 없지만 계정 및 사용자 개인 설정 수준에서 구성할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 지연 증명] 이메일

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

다음 [!UICONTROL 지연 증명] 증명이 마감일 또는 최종 기한에 도달하면 수신자에게 이메일이 전송됩니다. 이러한 유형의 이메일은 증명 수준에서 비활성화할 수 없지만 계정 및 사용자 개인 설정 수준에서 구성할 수 있습니다.

* [!UICONTROL 지연 증명] 증명이 마감일에 도달하고 모든 검토 또는 결정을 내리지 않은 경우 이메일은 자동으로 검토자에게 전송됩니다.

   이러한 이메일은 기본적으로 활성화되어 있으므로 전체 계정에 대해 조정할 수 없지만 사용자가 교정을 기본값으로 비활성화할 수 있습니다.

* 증명이 마감에 가까워지면 위험 시 이메일이 검토자에게 전송됩니다. 기본적으로 비활성화되어 있으며, [!UICONTROL 계정 설정]. 활성화한 후에는 [!UICONTROL 교정 기본값].

이러한 알림은 사용자 지정할 수 없습니다.

알림을 받을 사람은 다음과 같습니다.

* 소유자, [!UICONTROL 이메일] 증명을 최신으로 설정할 때 경고 [!UICONTROL 소유자의 제품 교정 기본값].
* 증명서에 대한 결정을 아직 내리지 않은 모든 승인자 결정에 대한 자세한 내용은 [교정 뷰어의 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>이메일 알림이 [!UICONTROL 계정 설정], 아니요 [!UICONTROL 지연 증명] 검토자와 승인자가 의견과 결정을 아직 제출하지 않은 경우에도 이메일이 전송됩니다. 비활성화하거나 [!UICONTROL 지연 증명] 전자 메일이 Proofing 기본값으로 설정됩니다.

증명 알림에 대해서는 다음 사항을 고려하십시오.

* 사용자 [!DNL Workfront] 관리자 또는 [!DNL Workfront Proof] 관리자는 에 설명된 대로 이메일 알림에 조직의 로고를 포함할 수 있습니다. [브랜드 [!DNL Workfront Proof] 사이트](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* 동일한 검토자와 여러 증명을 공유해야 하고 여러 개의 이메일을 받지 못하게 하려면 동시에 업로드할 수 있습니다. 모든 검토자는 모든 증명을 설명하는 하나의 이메일을 받고 각 증명에 대한 개인 URL을 포함합니다.

   >[!NOTE]
   >
   >증명 작성자는 별도로 수신합니다 [!UICONTROL 증명] 만든 각 증명에 대해 이메일을 보냅니다. 자세한 내용은 [다음 [!UICONTROL 증명] 이메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* 사용자나 검토자가 예상 전자 메일 알림을 받지 못하는 경우 다음을 참조하십시오.  [구성 [!DNL Workfront Proof] 스팸 필터를 피하기 위한 이메일](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
