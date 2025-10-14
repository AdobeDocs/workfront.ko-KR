---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 샌드박스 테스트 환경 미리 보기- [!DNL Workfront Proof]
description: 미리 보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경이며  [!DNL Workfront Proof]에 의해 매주 주말마다 새로 고쳐집니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 샌드박스 테스트 환경 미리 보기 - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

미리 보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경이며 매주 주말마다 [!DNL Workfront Proof]에 의해 새로 고쳐집니다.

## 미리보기 샌드박스 이해

미리보기 샌드박스는 조직의 사용자가 프로덕션 환경에 영향을 주지 않고 프로덕션 환경의 데이터를 안전하게 테스트하고 작업할 수 있는 환경 역할을 합니다. 교육 세션을 실행하고, 새로운 기능을 테스트하고, 설정 기능을 결정하는 데 이상적입니다.

또한 새 제품 기능은 프로덕션 환경에 제공되기 전에 미리보기 샌드박스 환경에 업로드됩니다. 사용자는 프로덕션 환경에서 일반적인 워크플로우에 영향을 주지 않고 새로운 기능을 사용해 볼 수 있습니다.

미리보기 샌드박스에는 실제 프로덕션 데이터가 포함됩니다. 데이터는 프로덕션에서 미리보기로 이동하며, 역으로는 이동하지 않습니다. 주말마다 새로 고침되므로 데이터가 프로덕션 환경에 비해 최대 1주일 정도 늦어질 수 있습니다. 마지막 새로 고침 시간 이후 생성된 항목은 다음 새로 고침이 수행되기 전까지 미리보기 샌드박스 환경에 있습니다.

## 미리보기 샌드박스 액세스

기본적으로 시스템 관리자는 샌드박스 미리보기 환경에 액세스할 수 있습니다. 이 섹션에 설명된 대로 샌드박스 미리보기 환경에 액세스할 수 없는 경우 [!DNL Workfront] 관리자 또는 지원 팀에 문의하십시오.

* [독립 실행형 샌드박스 미리 보기 액세스 [!DNL Workfront Proof] 고객](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [&#x200B; [!DNL Workfront]+[!DNL Workfront Proof] 고객으로 샌드박스 미리 보기 액세스](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 독립 실행형 [!DNL Workfront Proof] 고객으로 미리 보기 샌드박스에 액세스

1. 다음 URL로 이동: `https://preview.proofhq.com`.
1. 미리보기 자격 증명을 사용하여 로그인합니다.\
   미리보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 로그인은 매주 주말에 새로 고침이 발생할 때만 동기화됩니다. 자동으로 동기화되지 않습니다.

### [!DNL Workfront+Workfront] 증명 고객으로 샌드박스 미리 보기 액세스

시스템 관리자는 [!DNL Workfront] 인터페이스를 통해 [!DNL Workfront Proof] 미리 보기 샌드박스에 액세스할 수 있습니다.

[!DNL Workfront Proof] 미리 보기 샌드박스에 액세스하려면:

1. [!DNL Workfront] 환경에 로그인합니다.
1. 전역 탐색 모음에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 시스템]** >**[!UICONTROL 환경 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 테스트 환경]** 섹션에서 **[!UICONTROL 샌드박스 미리 보기]**&#x200B;를 클릭합니다.

1. 미리보기 자격 증명으로 로그인합니다.\
   미리보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.
1. 전역 탐색 모음에서 [!DNL Workfront Proof] 아이콘을 클릭합니다.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   [!DNL Workfront Proof] 미리 보기 환경이 표시됩니다.

## 미리보기 샌드박스에서 이메일 수신

전자 메일 알림은 [!DNL Workfront Proof] 미리 보기 환경에서 트리거되지 않습니다.
