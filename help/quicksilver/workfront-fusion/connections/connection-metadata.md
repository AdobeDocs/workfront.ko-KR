---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Adobe Workfront Fusion의 연결 메타데이터
description: Adobe Workfront Fusion에는 Adobe Workfront 라이센스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Adobe Workfront Fusion의 연결 메타데이터

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion]에는 [!DNL Adobe Workfront] 라이선스 외에 [!DNL Adobe Workfront Fusion] 라이선스가 필요합니다.

모든 연결이 동일한 것은 아닙니다. 연결의 차이점을 이해하는 것은 비즈니스 컨텍스트를 아는 데 매우 중요합니다. Fusion은 메타데이터를 사용하여 연결의 중요한 속성을 식별합니다.

새 연결을 만들 때 연결 메타데이터를 설정할 수 있습니다. 이러한 속성은 연결 설정에 사용된 동일한 대화 상자에 있습니다.

![연결 메타데이터](assets/connection-metadata-setup.png)

Fusion 사용자는 연결 영역에서 연결을 보고 편집할 수 있습니다.

![연결 영역의 연결 메타데이터](assets/connections-area-metadata.png)

## 환경 유형

Fusion 연결은 운영 시스템과 비운영 시스템 모두에서 사용할 수 있습니다. 차이점을 아는 것은 프로덕션 환경을 보호하는 데 매우 중요합니다. 환경 유형은 다른 연결 메타데이터와 마찬가지로 정보 제공 용도로만 사용됩니다. 사용자는 여전히 이 속성을 정확하게 설정할 책임이 있습니다.

## 인증 유형

Fusion 연결은 서비스 계정과 개인 계정 모두에 사용할 수 있습니다. 서비스 계정은 시나리오가 Fusion으로 자동화할 때 인증에 사용됩니다. 개인 계정은 특정 사용자를 기반으로 한 인증입니다. 사용되는 인증 유형은 시나리오의 요구 사항에 따라 다릅니다. 개인 계정은 자동화된 사용자 작업에 사용해야 합니다. 예를 들어 Fusion 시나리오가 특정 사용자에 의한 승인을 자동화하는 경우 인증 유형은 해당 사용자에 대한 것이어야 합니다. 그렇지 않으면 Fusion이 Fusion 역할을 하며 유형은 &quot;서비스 계정&quot;이어야 합니다.

다른 연결 메타데이터와 마찬가지로 유형은 정보 제공 목적으로만 사용됩니다. 사용자는 여전히 이 속성을 수동으로 정확하게 설정할 책임이 있습니다.

인증 유형에 대한 자세한 내용은 Adobe 인증 가이드의 [인증](https://developer.adobe.com/developer-console/docs/guides/authentication/)을 참조하십시오.
