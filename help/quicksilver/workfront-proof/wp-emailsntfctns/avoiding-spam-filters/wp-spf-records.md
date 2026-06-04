---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof 레코드
description: 'Workfront Proof은 notification@proofing.yourdomain.com 과 같은 Workfront Proof 이메일 주소에서 검토자에게 이메일 알림을 보냅니다. 받는 사람의 메일 서버가 모든 Workfront Proof 이메일 알림을 신뢰하도록 하려면  [!DNL Workfront Proof] 계정에 연결된 사용자 지정 도메인에 대해  [!DNL Sender Policy] 프레임워크(SPF) 레코드를 설정해야 합니다(예: proofing.yourdomain.com).'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 0%

---

# Workfront Proof 레코드

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront Proof]이(가) notification@proofing.yourdomain.com과 같은 [!DNL Workfront Proof] 전자 메일 주소에서 검토자에게 전자 메일 알림을 보냅니다. 받는 사람의 메일 서버에서 [!DNL Workfront Proof] 전자 메일 알림을 모두 신뢰하도록 하려면 [!DNL Workfront Proof] 계정에 연결된 사용자 지정 도메인에 대해 [!UICONTROL SPF(보낸 사람 정책 프레임워크]) 레코드를 설정해야 합니다(예: **proofing.yourdomain.com**).

SPF 레코드를 설정하려면 주 도메인에 사용되는 SPF 레코드를 포함해야 합니다.

1. 다음 값으로 도메인의 **[!UICONTROL DNS TXT]** 항목을 추가하십시오.

   `v=spf1 a:mx.proofhq.com -all`

   전자 메일 관리자 또는 IT 담당자가 이 설정을 지원할 수 있습니다.

   >[!TIP]
   >
   >[[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx)에서 사용 가능한 도구를 사용하여 [!DNL Workfront]개의 SPF 레코드를 검토할 수 있습니다.
