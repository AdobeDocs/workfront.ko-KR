---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 스팸 필터를 사용하지 않도록  [!DNL Workfront Proof] 이메일 구성
description: "이메일 클라이언트의 스팸 필터는 성가시고 악의적인 스팸 이메일로부터 사용자를 보호하는 중요한 역할을 합니다. 그러나 스팸 필터에 올바른 설정이 없으면 다음의 중요한 [!DNL Workfront Proof] 이메일을 볼 수 없게 됩니다. 증명 이메일 알림, 뉴스레터 및 특수 통신."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 스팸 필터를 사용하지 않도록 [!DNL Workfront Proof]개 이메일 구성

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

이메일 클라이언트의 스팸 필터는 성가시고 악의적일 수 있는 스팸 이메일을 보호하는 중요한 역할을 합니다. 그러나 스팸 필터에 올바른 설정이 없으면 증명 이메일 알림, 뉴스레터 및 특수 통신과 같은 중요한 [!DNL Workfront Proof]개의 이메일을 볼 수 없습니다.

[!DNL Workfront Proof] 이메일이 스팸 폴더 대신 받은 편지함으로 항상 라우팅되도록 하려면 다음 내용을 허용 목록에 추가하다에 추가해야 합니다.

* [!DNL Workfront Proof] 메일 서버: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 전자 메일 주소(예: notification@proofhq.com)

허용 목록에 추가하다 허용 목록에 추가하다 허용 목록에 추가하다에 추가할 URL에 대한 자세한 내용은 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 기사의 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

## [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 전자 메일 주소

전자 메일 클라이언트 유형에 따라 스팸 필터가 나중에 전자 메일을 스팸 폴더로 라우팅하지 못하도록 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 전자 메일 주소를 다음 중 하나에 추가해야 할 수 있습니다.

* 내 연락처 목록
* [!UICONTROL 수신 허용 - 보낸 사람] 목록
* 해당 주소에서 받은 편지함으로 이메일을 보내기 위해 만드는 필터

스팸 폴더에서 기존 [!DNL Workfront Proof]개의 전자 메일을 제거하고 차단된 주소 목록에 &quot;[!UICONTROL 보낸 사람]&quot; 주소가 있는지 확인해야 할 수도 있습니다. 이 도움말 페이지에서는 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 나열하고 다음 전자 메일 클라이언트의 스팸 필터에 추가하는 방법을 보여 줍니다.

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>여기에 설명된 절차에 대한 질문이 있는 경우 이메일 클라이언트의 도움말을 참조하십시오.

자세한 내용은 [일반 전자 메일 클라이언트에 대한 스팸 설정 구성](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md)을 참조하십시오.

## 복사할 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 전자 메일 주소

[!DNL Workfront Proof] 전자 메일이 받은 편지함에 도달하는지 확인하려면 전자 메일 클라이언트의 스팸 필터에 별도로 두 개의 [!DNL Workfront Proof] 전자 메일 주소를 추가해야 합니다.

* [!DNL Workfront Proof]에서 많은 전자 메일 통신을 보내는 일반 지원 주소 [!DNL support@proofhq.com]
* [!DNL Workfront Proof]이(가) 증명 생성자 및 검토자에게 증명 링크가 있는 증명 알림 이메일을 보내는 알림 주소입니다. 일반 주소, notification@support.proofhq.com 또는 사용자 지정된 하위 도메인이나 화이트 레이블 도메인이 있는 경우 특정 주소일 수 있습니다.

[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 전자 메일 클라이언트의 필터에 추가하려면:

1. 일반 [!DNL Workfront Proof] 지원 &quot;[!UICONTROL from]&quot; 전자 메일 주소(support@proofhq.com)를 복사하여 전자 메일 클라이언트에 지정된 필드에 붙여넣습니다.
1. 다음 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 전자 메일 주소 중 적절한 주소를 복사하여 전자 메일 클라이언트에 대해 지정된 필드에 별도로 붙여넣습니다.

   * 사용자 지정된 하위 도메인 또는 흰색 레이블 도메인이 없는 경우 notification@support.proofhq.com
   * notification@yoursubdomain.proofhq.com 사용자 지정된 하위 도메인이 있는 경우 이 주소에서 하위 도메인 이름으로 바꿉니다.
   * notification@yoursubdomain.yourdomain.com (흰색 레이블 도메인이 있는 경우) 이 주소에서 하위 도메인 이름과 도메인 이름을 바꾸십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
