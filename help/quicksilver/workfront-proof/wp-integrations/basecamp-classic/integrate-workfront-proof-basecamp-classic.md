---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: 통합 [!DNL Workfront Proof] Basecamp Classic 사용
description: 만약 [!DNL Basecamp] 프로젝트 관리를 위해 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 통합 [!DNL Workfront Proof] with [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

만약 [!DNL Basecamp] 프로젝트 관리를 위해 [!DNL Workfront Proof].

## 이해 [!DNL Basecamp] 통합 [!DNL Workfront]

통합 [!DNL Basecamp] 에서는 모든 내에서 증명을 보고 검토하고 승인할 수 있습니다 [!DNL Basecamp]. 사용자는 자신의 [!DNL Workfront Proof] 계정을 사용하여 [!DNL Basecamp] 프로젝트. 검토자가 다음을 수행할 수 있습니다. [교정 뷰어의 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp]: Basecamp 메시지에 포함된 미니 증명 사용.

통합 시 [!DNL Workfront Proof], [!DNL Basecamp] 에서는 사용자가 증명을 사용하여 다음을 수행할 수 있습니다.

* 사용자는 내에서 증명을 검토하고 승인할 수 있습니다 [!DNL Basecamp Classic].
* 사용자는 검토 도구를 쉽게 사용할 수 있습니다.
* 프로젝트 검토 팀에서 메시지를 받습니다 [!DNL Basecamp] 검토와 승인을 위한 작은 증명.
* 사용자는 검토 및 승인을 위해 전체 페이지로 전환할 수 있습니다.
* 사용자는 미니 및 전체 크기 증명 모두에 댓글 및 마크업을 추가할 수 있습니다.

   >[!NOTE]
   >
   >댓글에 답글을 달면 편집하거나 삭제할 수 없습니다.

* 검토자는 다른 검토자가 만든 및 마크업에 응답할 수 있습니다.
* 새로운 버전의 증명을 사용할 수 있으면 사용자에게 경고가 표시됩니다.
* 그렇지 않은 사용자 [!DNL Workfront Proof] 사용자는 [!DNL Basecamp].

통합 [!DNL Workfront Proof] with [!DNL Basecamp] 는 다음 두 가지 수준에서 설정해야 합니다.

* 구성 [!DNL Basecamp] in [계정 설정:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 이렇게 하면 전체 조직에 Basecamp 통합을 사용할 수 있습니다.
* 자세한 내용은 [활성화 [!DNL Basecamp] 통합 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* 구성 [!DNL Basecamp] in [개인 설정](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): 이를 통해 증명 생성자와 소유자가 개인 정보에 연결할 수 있습니다 [!DNL Basecamp] 계정 및 권한 부여 [!DNL Workfront Proof] 액세스 권한. 자세한 내용은 [개인 설정 구성](#configuring-personal-settings).

통합할 수 있습니다 [!DNL Workfront] 다음 중 하나를 사용하여 [!DNL Basecamp] 또는 [!DNL Basecamp Classic]. 각 버전 [!DNL Basecamp] 는 다른 API를 사용하므로 는 다른 구성 프로시저를 필요로 합니다.

구성에 대한 자세한 내용 [!DNL Basecamp Classic]를 참조하십시오. [활성화 [!DNL Basecamp] 통합 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 참조하십시오.

구성에 대한 자세한 내용 [!DNL Basecamp]를 참조하십시오. [통합 [!DNL Workfront Proof] with [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## 활성화 [!DNL Basecamp] 통합 [!DNL Workfront Proof]

로서의 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 또는 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)의 전체 계정에 대해 Basecamp 통합을 설정할 수 있습니다 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. 이동 [계정 설정입니다.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. 를 엽니다. **[!UICONTROL 통합]** 탭 (1)
1. Basecamp 통합을 사용하려면 를 클릭합니다. **[!UICONTROL 활성화]** (2).
1. 확인 [!DNL Basecamp Classic] 는 (3)과 통합하는 버전입니다.
1. (조건부) 없을 경우 [!DNL Basecamp] URL이 표시됩니다(4). **[!UICONTROL 편집]** 및에 대한 URL을 입력합니다. [!DNL Basecamp] 계정(http:// 제외).
1. 클릭 **[!UICONTROL 저장]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (선택 사항) [!DNL Basecamp] 로그인한 후 브라우저의 URL입니다 [!DNL Basecamp Classic] (6)

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   통합하면 [!DNL Workfront Proof] with [!DNL Basecamp]로 설정되면 사용자는 개인 설정을 구성할 수 있습니다. 개인 설정 설정에 대한 자세한 내용은 [개인 설정 구성](#configuring-personal-settings).

   활성화할 수 없는 경우 [!DNL Basecamp] 통합, [!DNL Workfront Proof] 계정 ID는 에서 사용하는 계정 ID와 동일하지 않을 수 있습니다 [!DNL Basecamp].

## 개인 설정 구성

설정 후 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 조직의 경우 증명을 만들거나 제출하는 각 작성자는 자신의 보고서를 설정해야 합니다  [개인 설정.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>이러한 단계를 완료하는 것이 가장 쉽습니다 [!DNL Basecamp] 하나의 브라우저 창에서 세션을 열고 [!DNL Workfront Proof] 세션이 다른 창에서 열립니다.

* [검색 [!DNL Basecamp] API 토큰](#retrieving-your-basecamp-api-token)
* [추가 [!DNL Basecamp] 개인 설정에 대한 API 토큰](#adding-your-basecamp-api-token-to-your-personal-settings)

### 검색 [!DNL Basecamp] API 토큰

의 개별 수준에서 통합을 완료하려면 [!DNL Workfront Proof]를 채울 때는 사용자에게 개별 인증 토큰이 필요합니다 [!DNL Basecamp] API.

를 검색하려면 [!DNL Basecamp] API 토큰:

1. 사용자 [!DNL Basecamp] 계정이 필요합니다.
1. 클릭 **[!UICONTROL 내 정보]** (1) 입력되어 있습니다.\
   다음 [!UICONTROL 내 정보] 페이지가 표시됩니다.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. 에서 [!UICONTROL 인증 토큰] 섹션을 클릭합니다. **[!UICONTROL 토큰 표시]** (2) 개인 인증 토큰을 표시할 수 있습니다.
1. 을(를) 선택합니다 **[!UICONTROL 피드 리더용 토큰]** 또는 **[!UICONTROL Basecamp API]** (3) 그런 다음 토큰을 클립보드에 복사합니다.

1. 붙여넣기 [!DNL Basecamp] 에 API 토큰 추가 [!UICONTROL 피드 리더용 토큰] 또는 [!UICONTROL Basecamp API] 상자.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### 추가 [!DNL Basecamp] 개인 설정에 대한 API 토큰

을(를) 붙여넣으려면 [!DNL Basecamp] 에 API 토큰 추가 [!DNL Workfront Proof] [개인 설정](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. 로 이동합니다. [[!UICONTROL 통합] - 사용자 설정](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) 다음 위치에서 [개인 설정](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   관리자는 먼저 [!DNL Basecamp Classic] 통합을 통해 개인 설정을 사용할 수 있습니다. 통합 설정에 대한 자세한 내용은 [활성화 [!DNL Basecamp] 통합 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 참조하십시오.

1. 에서 [!DNL Basecamp] API 토큰 상자(2)에서 방금 복사한 토큰을 붙여 넣습니다. [!DNL Basecamp] [!UICONTROL 내 정보] 페이지를 필드(3)에 넣습니다.\
   복사 관련 정보 [!DNL Basecamp] API 토큰은 다음을 참조하십시오. [검색 [!DNL Basecamp] API 토큰](#retrieving-your-basecamp-api-token) 참조하십시오.

1. 클릭 **[!UICONTROL 저장]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

사용자 [!DNL Workfront Proof] [개인 설정](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) 이제 와(과) 통합되었습니다. [!DNL Basecamp Classic] 계정이 필요합니다.
