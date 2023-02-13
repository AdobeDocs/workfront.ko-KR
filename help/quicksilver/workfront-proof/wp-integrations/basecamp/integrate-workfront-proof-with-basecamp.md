---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 통합 [!DNL Workfront Proof] with [!DNL Basecamp]
description: 만약 [!DNL Basecamp] 프로젝트 관리를 위해 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# 통합 [!DNL Workfront Proof] with [!DNL Basecamp]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

만약 [!DNL Basecamp] 프로젝트 관리를 위해 [!DNL Workfront Proof].

## 이해 [!DNL Basecamp] 통합 [!DNL Workfront]

통합 [!DNL Basecamp] 에서는 모든 내에서 증명을 보고 검토하고 승인할 수 있습니다 [!DNL Basecamp]. 사용자는 자신의 [!DNL Workfront Proof] 계정을 사용하여 [!DNL Basecamp] 프로젝트. 검토자는 를 통해 의견을 작성하고 결정할 수 있습니다 [!DNL Basecamp]: Basecamp 메시지에 포함된 미니 증명 사용.

통합 시 [!DNL Workfront Proof], [!DNL Basecamp] 에는 다음 교정 기능이 있습니다.

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

* 구성 [!DNL Basecamp] in [계정 설정:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 이렇게 하면 전체 조직에 Basecamp 통합을 사용할 수 있습니다. 자세한 내용은 [Basecamp 통합 활성화 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* 구성 [!DNL Basecamp] in [개인 설정](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): 이를 통해 증명 생성자와 소유자가 개인 기본 맵 계정에 연결하고 권한을 부여할 수 있습니다 [!DNL Workfront Proof] 액세스 권한. 자세한 내용은 [개인 설정 구성](#configuring-personal-settings).

통합할 수 있습니다 [!DNL Workfront] 다음 중 하나를 사용하여 [!DNL Basecamp] 또는 [!DNL Basecamp Classic]. 각 버전 [!DNL Basecamp] 는 다른 API를 사용하므로 는 다른 구성 프로시저를 필요로 합니다.

구성에 대한 자세한 내용 [!DNL Basecamp Classic]를 참조하십시오. [통합 [!DNL Workfront Proof] with [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## 활성화 [!DNL Basecamp] 통합 [!DNL Workfront Proof]

로서의 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 또는 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)를 설정하는 경우 [!DNL Basecamp] 통합 을 통해 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. in [!UICONTROL 베이스캠프]를 입력하여 다음 정보를 수집합니다.

   * 사용자의 URL입니다 [!DNL Basecamp] account
   * URL은 &quot;[!UICONTROL 내 정보]&quot; 섹션

1. 로그아웃됨 [!DNL Basecamp].
1. 클릭 **[!UICONTROL 계정 설정]** 오른쪽 상단 근처에 있습니다.
1. 을(를) 클릭합니다. **[!UICONTROL 통합]** 탭.
1. 에서 **[!UICONTROL [!DNL Basecamp]]** 섹션, 오른쪽 **[!UICONTROL [!DNL Basecamp]통합]**&#x200B;를 클릭합니다. **[!UICONTROL 활성화]**.

1. 다음 **[!UICONTROL [!DNL Basecamp]버전]**&#x200B;를 확인하여 **[!UICONTROL 클래식 버전]** 는 통합하려는 버전입니다.

1. (조건부) 없을 경우 [!DNL Basecamp] URL이 표시되면 **[!UICONTROL 편집]**&#x200B;에 사용할 URL을 입력합니다 [!DNL Basecamp] http://을 포함하지 않고 계정을 클릭한 다음 **[!UICONTROL 저장]**.

1. 창의 오른쪽 위 모서리에서 을(를) 클릭합니다. **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**.

1. 을(를) 클릭합니다. **[!UICONTROL 통합]** 탭.
1. 아래 **[!DNL Basecamp]**, 오른쪽에 **[!UICONTROL 기본 맵 통합]**&#x200B;를 클릭합니다. **[!UICONTROL 활성화]**.

1. 옵션이 나타납니다. **[!UICONTROL [!DNL Basecamp]API 토큰]**&#x200B;를 클릭합니다. **[!UICONTROL 편집]**.

1. 표시되는 상자에서 &quot;[!UICONTROL 내 정보]&quot; 섹션 [!DNL Basecamp]를 클릭한 다음 **[!UICONTROL 저장]**.\
   통합하면 [!DNL Workfront Proof] with [!DNL Basecamp]로 설정되면 사용자는 개인 설정을 구성할 수 있습니다. 개인 설정 설정에 대한 자세한 내용은 [개인 설정 구성](#configuring-personal-settings)

1. 활성화할 수 없는 경우 [!DNL Basecamp] 통합, [!DNL Workfront Proof] 계정 ID는 에서 사용하는 계정 ID와 동일하지 않을 수 있습니다 [!DNL Basecamp].
1. 통합하면 [!DNL Workfront Proof] with [!DNL Basecamp]로 설정되면 사용자는 개인 설정을 구성할 수 있습니다. 개인 설정 설정에 대한 자세한 내용은 [개인 설정 구성](#configuring-personal-settings).

## 개인 설정 구성

설정 후 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 조직의 경우 증명을 만들거나 제출하는 작성자가 각각  [개인 설정.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. 이동 **[!UICONTROL 개인** &#x200B; ** 설정]**.

1. 를 엽니다. **[!UICONTROL 통합]** 탭 (1)
1. 를 사용하려면 [!DNL Basecamp] 통합, 클릭 **[!UICONTROL 활성화]** (2).
1. 클릭 **[!UICONTROL 에 연결 [!DNL Basecamp] account]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. 에 로그인합니다. [!DNL Basecamp] (1)\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. 클릭 **[!UICONTROL 네, 접근 권한을 허용하겠습니다]** 권한 부여 [!DNL Workfront Proof] 계정(2)에 액세스합니다.\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (선택 사항) 개인 통합이 활성 (3)일 때 [!DNL Basecamp] 계정.

   1. 클릭 **[!UICONTROL 스위치 [!DNL Basecamp] account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      다음 [!UICONTROL Switch Basecamp 계정] 이동 [!UICONTROL 개인 설정] 페이지, 여기에서 [!DNL Basecamp] 와 통합할 계정 [!DNL Workfront Proof] 계정이 필요합니다.

   1. 클릭 **[!UICONTROL 와 다시 통합[!DNL Basecamp]]** (5) [!DNL Basecamp] account\

      이 경우 [!UICONTROL 개인 설정] 페이지에 최신 목록을 표시하고 [!DNL Basecamp] 계정.

   1. 클릭 **[!UICONTROL 이 계정과 통합]** 연결 [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      이제 다음에 증명을 추가할 수 있습니다. [!DNL Basecamp] 프로젝트를 참조하십시오.
