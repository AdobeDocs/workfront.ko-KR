---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 지연 증명 이메일
description: 증명이 마감일에 근접하거나 마감일에 도달하면 지연 증명 이메일이 수신자에게 전송됩니다. 이러한 유형의 이메일은 증명 수준에서 비활성화할 수 없지만 계정 및 사용자 개인 설정 수준에서 구성할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 지연 증명] 전자 메일

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

증명이 마감일에 근접하거나 마감일에 도달하면 [!UICONTROL 지연 증명] 전자 메일이 수신자에게 전송됩니다. 이러한 유형의 이메일은 증명 수준에서 비활성화할 수 없지만 계정 및 사용자 개인 설정 수준에서 구성할 수 있습니다.

* 증명이 마감일에 도달하고 모든 검토 또는 결정이 수행되지 않은 경우 [!UICONTROL 지연 증명] 이메일이 검토자에게 자동으로 전송됩니다.

  이러한 이메일은 기본적으로 활성화되어 있으며 전체 계정에 대해 조정할 수 없지만 사용자가 증명 기본값에서 비활성화할 수 있습니다.

* 인증이 마감일에 가까워지면 위험 상태의 이메일이 검토자에게 전송됩니다. 기본적으로 비활성화되어 있으며 [!UICONTROL 계정 설정]에서 활성화할 수 있습니다. 사용하도록 설정하면 [!UICONTROL 증명 기본값]에서도 조정할 수 있습니다.

이러한 알림은 사용자 지정할 수 없습니다.

알림을 받을 사람은 다음과 같습니다.

* 증명이 늦을 때 [!UICONTROL 전자 메일] 경고가 활성화된 경우에만 소유자가 [!UICONTROL 소유자의 증명 기본값]에서 확인됩니다.
* 증명에 대해 아직 결정을 내리지 않은 승인자 결정에 대한 자세한 내용은 [증명 뷰어에서 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)을 참조하십시오.

>[!NOTE]
>
>[!UICONTROL 계정 설정]에서 이메일 알림을 기본값으로 사용하지 않도록 설정한 경우 검토자와 승인자가 아직 의견 및 결정을 제출하지 않았더라도 [!UICONTROL 지연 증명] 이메일이 전송되지 않습니다. 증명 기본값에서 [!UICONTROL 지연 증명] 이메일을 비활성화할 수도 있습니다.

증명 알림에 대해 다음 사항을 고려하십시오.

* [!DNL Workfront] 관리자 또는 [!DNL Workfront Proof] 관리자는 [사이트 브랜딩 [!DNL Workfront Proof] 에 설명된 대로 전자 메일 알림에 조직의 로고를 포함할 수 있습니다.](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)
* 동일한 검토자와 여러 증명을 공유해야 하지만 해당 검토자가 여러 이메일을 받지 않도록 하려는 경우 해당 증명을 동시에 업로드할 수 있습니다. 모든 검토자는 모든 증명이 자세히 설명되어 있으며 각 증명에 대한 개인 URL이 포함된 하나의 이메일을 받게 됩니다.

  >[!NOTE]
  >
  >증명 작성자는 생성된 각 증명에 대해 별도의 [!UICONTROL 증명 작성] 이메일을 받습니다. 자세한 내용은 [증명 [!UICONTROL 확인] 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)을 참조하세요.

* 사용자 또는 검토자가 예상 전자 메일 알림을 받지 못한 경우 [스팸 필터를 사용하지 않도록 전자 메일 구성 [!DNL Workfront Proof] 을 참조하세요](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
