---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 구성 [!DNL Workfront Proof] 스팸 필터를 피하기 위한 이메일
description: "이메일 클라이언트의 스팸 필터는 다음과 같은 중요한 목적을 제공합니다. 스팸 이메일에 대해 번거롭고 악의적인 메시지를 사용하지 않도록 보호합니다. 그러나 스팸 필터에 올바른 설정이 없다면 다음과 같은 중요한 내용이 표시되지 않을 수 있습니다 [!DNL Workfront Proof] 이메일: 증명 이메일 알림, 뉴스레터 및 특별 커뮤니케이션."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 구성 [!DNL Workfront Proof] 스팸 필터를 피하기 위한 이메일

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

이메일 클라이언트의 스팸 필터는 다음과 같은 중요한 목적을 제공합니다. 스팸 이메일에 대해 번거롭고 악의적인 메시지를 사용하지 않도록 보호합니다. 그러나 스팸 필터에 올바른 설정이 없다면 다음과 같은 중요한 내용이 표시되지 않을 수 있습니다 [!DNL Workfront Proof] 이메일: 증명 이메일 알림, 뉴스레터 및 특수 커뮤니케이션.

그리고 [!DNL Workfront Proof] 이메일은 항상 스팸 폴더 대신 받은 편지함으로 라우팅되므로 다음 내용을 페이지에 추가해야 허용 목록에 추가하다 합니다.

* [!DNL Workfront Proof] 메일 서버: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 이메일 주소(예: notification@proofhq.com)

에 추가할 URL에 대한 자세한 내용허용 목록에 추가하다는 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 기사 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 이메일 주소 &quot;

이메일 클라이언트 유형에 따라 다음을 추가해야 할 수 있습니다 [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 스팸 필터가 나중에 스팸 폴더로 이메일을 라우팅하지 못하도록 하기 위해 다음 중 하나에 이메일 주소를 지정합니다.

* 연락처 목록
* 사용자 [!UICONTROL 수신 허용 - 보낸 사람] list
* 해당 주소에서 받은 편지함으로 이메일을 배달하기 위해 만드는 필터입니다

기존 항목을 제거해야 할 수도 있습니다 [!DNL Workfront Proof] 스팸 폴더에서 이메일을 보내고 &quot;[!UICONTROL 변환 전:]&quot;주소는 차단된 주소 목록에 있습니다. 이 도움말 페이지에는 [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 주소 및 는 다음 이메일 클라이언트의 스팸 필터에 추가하는 방법을 보여줍니다.

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>여기에 설명된 절차에 대해 질문이 있는 경우 이메일 클라이언트의 도움말을 확인하십시오.

자세한 내용은 [일반 이메일 클라이언트에 대한 스팸 설정 구성](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## 다음 [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 복사할 이메일 주소

그리고 [!DNL Workfront Proof] 이메일이 받은 편지함에 도달하려면 두 개의 받은 편지함을 추가해야 합니다 [!DNL Workfront Proof] 이메일 주소는 이메일 클라이언트의 스팸 필터에 별도로 저장됩니다.

* 일반 지원 주소 [!DNL support@proofhq.com]: [!DNL Workfront Proof] 많은 이메일 통신을 보냅니다.
* 보낸 알림 주소 [!DNL Workfront Proof] 증명 작성자 및 검토자에게 증명 알림 이메일을 보내고, 증명 링크와 함께 알림 이메일을 보냅니다. 사용자 지정된 하위 도메인 또는 화이트 레이블 도메인이 있는 경우 일반 주소 notification@support.proofhq.com 또는 특정 주소일 수 있습니다.

추가하려면 [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]이메일 클라이언트의 필터에 주소를 지정하는 경우:

1. 일반 복사 [!DNL Workfront Proof] 지원 &quot;[!UICONTROL 변환 전:]&quot; 이메일 주소(support@proofhq.com)을 복사하여 이메일 클라이언트에 표시된 필드에 붙여넣습니다.
1. 다음 중 적절한 하나를 복사합니다 [!DNL Workfront Proof] &quot;[!UICONTROL 변환 전:]&quot; 이메일 주소를 전자 메일 클라이언트에 지정된 필드에 별도로 붙여 넣습니다.

   * 사용자 지정된 하위 도메인 또는 화이트 레이블 도메인이 없는 경우 notification@support.proofhq.com
   * 사용자 지정된 하위 도메인이 있는 경우 notification@yoursubdomain.proofhq.com 이 주소에서 하위 도메인 이름을 대체합니다
   * notification@yoursubdomain.yourdomain.com 에는 흰색 레이블 도메인이 있는 경우 이 주소에서 하위 도메인 이름 및 도메인 이름 대체

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
