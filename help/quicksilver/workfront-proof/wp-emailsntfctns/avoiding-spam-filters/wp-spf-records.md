---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront 증명 SPF 레코드
description: 'Workfront 증명 은 notification@proofing.yourdomain.com과 같은 Workfront 증명 이메일 주소에서 검토자에게 이메일 알림을 보냅니다. 수신자의 메일 서버가 모든 Workfront 증명 이메일 알림을 신뢰하는지 확인하려면 [!DNL Sender Policy] 에 연결된 사용자 지정된 도메인에 대한 SPF(Framework) 레코드 [!DNL Workfront Proof] account(예: proofing.yourdomain.com)'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Workfront 증명 SPF 레코드

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] 검토자로부터 전자 메일 알림을 보냅니다. [!DNL Workfront Proof] notification@proofing.yourdomain.com과 같은 이메일 주소입니다. 받는 사람의 메일 서버가 모두 신뢰할 수 있도록 하기 위해 [!DNL Workfront Proof] 이메일 알림, 설정 [!UICONTROL 보낸 사람 정책 프레임워크] (SPF) 레코드에 연결된 사용자 지정된 도메인에 대한 레코드 [!DNL Workfront Proof] 계정(예: **proofing.yourdomain.com**).

SPF 레코드를 설정하려면 주 도메인에 사용되는 SPF 레코드를 포함해야 합니다.

1. 추가 **[!UICONTROL DNS TXT]** 다음 값이 있는 도메인의 항목:

   `v=spf1 a:mx.proofhq.com -all`

   이메일 관리자 또는 IT 담당자가 이를 설정하는 데 도움을 줄 수 있습니다.

   >[!TIP]
   >
   >에서 무료 도구를 사용할 수 있습니다. [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) 검토하려면 [!DNL Workfront] SPF 레코드.
