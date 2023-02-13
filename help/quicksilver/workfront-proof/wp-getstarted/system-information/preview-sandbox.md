---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 샌드박스 테스트 환경 미리 보기 - [!DNL Workfront Proof]
description: 미리 보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경으로, 주말마다 새로 고침됩니다 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 샌드박스 테스트 환경 미리 보기 - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

미리 보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경으로, 주말마다 새로 고침됩니다 [!DNL Workfront Proof].

## 미리 보기 샌드박스 이해

미리 보기 샌드박스는 프로덕션 환경에 영향을 주지 않고 조직의 사용자가 프로덕션 환경에서 데이터를 안전하게 테스트하고 사용할 수 있는 환경 역할을 합니다. 교육 세션을 실행하고, 새로운 기능을 테스트하고, 설정 기능을 결정하는 데 이상적입니다.

또한 새 제품 기능은 프로덕션 환경에 전달되기 전에 미리 보기 샌드박스 환경에 업로드됩니다. 사용자는 프로덕션 환경에서 일반적인 워크플로우에 영향을 주지 않고 새로운 기능을 사용해 볼 수 있습니다.

미리 보기 샌드박스에는 실제 프로덕션 데이터가 포함되어 있습니다. 데이터는 프로덕션에서 미리 보기로 전송되며 거꾸로 전송되지 않습니다. 매주 새로 고쳐지므로 프로덕션 환경보다 최대 1주일 정도 뒤처질 수 있습니다. 마지막 새로 고침 시간 이후에 생성된 항목은 다음 새로 고칠 때까지 미리 보기 샌드박스 환경에 있습니다.

## 미리 보기 샌드박스 액세스

기본적으로 시스템 관리자는 미리 보기 샌드박스 환경에 액세스할 수 있습니다. 이 섹션에 설명된 대로 샌드박스 환경 미리 보기에 액세스할 수 없는 경우 [!DNL Workfront] 관리자 또는 지원 팀

* [독립형 미리 보기 샌드박스 액세스 [!DNL Workfront Proof] 고객](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [로 미리 보기 샌드박스 액세스 [!DNL Workfront]+[!DNL Workfront Proof] 고객](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 독립형 미리 보기 샌드박스 액세스 [!DNL Workfront Proof] 고객

1. 다음 URL로 이동합니다.  `https://preview.proofhq.com`.
1. 미리 보기 자격 증명을 사용하여 로그인합니다.\
   미리 보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리 보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 로그인은 새로 고침이 발생하는 경우에만 동기화되며, 이러한 로그인은 주말마다 발생합니다. 자동으로 동기화되지 않습니다.

### 로 미리 보기 샌드박스 액세스 [!DNL Workfront+Workfront] 증명 고객

시스템 관리자는 [!DNL Workfront Proof] 를 통해 샌드박스 미리 보기 [!DNL Workfront] 인터페이스.

에 액세스하려면 [!DNL Workfront Proof] 샌드박스 미리 보기:

1. 에 로그인합니다. [!DNL Workfront] 환경.
1. 클릭 **[!UICONTROL 설정]** 를 클릭합니다.
1. 클릭 **[!UICONTROL 시스템]** >**[!UICONTROL 기본 설정]**.

1. 에서 **[!UICONTROL 테스트 환경]** 섹션을 클릭합니다. **[!UICONTROL 샌드박스 미리 보기]**.

1. 미리 보기 자격 증명으로 로그인합니다.\
   미리 보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리 보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 로그인은 새로 고침이 발생하는 경우에만 동기화됩니다. 자동으로 동기화되지 않습니다.
1. 을(를) 클릭합니다. [!DNL Workfront Proof] 아이콘을 클릭합니다.\
   ![prop_access_profhq.png](assets/proof-access-proofhq-350x39.png)\
   다음 [!DNL Workfront Proof] 미리 보기 환경이 표시됩니다.

## 미리 보기 샌드박스에서 이메일 수신

이메일 알림은 앱에서 트리거되지 않습니다 [!DNL Workfront Proof] 미리 보기 환경.
