---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager 권한 문제 해결
description: 증명 사용자를 위해  [!DNL Adobe] Workfront에서 사용할 수 있는 권한 프로필은 관리자, 감독자 및 관리자입니다.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] 증명 관리자] 권한 문제 해결

증명 사용자를 위해 [!DNL Adobe Workfront]에서 사용할 수 있는 권한 프로필은 다음과 같습니다.

* [!UICONTROL 관리자]
* [!UICONTROL 감독자]
* [!UICONTROL 관리자]

<!--For detailed information about these options and how to configure them, see .-->

사용자 [!UICONTROL 관리자]에게 권한을 부여할 때 다음 문제 해결 정보를 사용할 수 있습니다.

* **문제:** [!UICONTROL 관리자] 권한이 있는 사용자는 다른 사용자가 만든 증명을 볼 수 없습니다. 대신 [!UICONTROL 액세스 거부됨] 화면이 표시됩니다.

  ![](assets/access-denied-350x161.png)

  **관리자** 권한이 있는 [!UICONTROL 솔루션:] 사용자를 증명에 명시적으로 추가해야 합니다. 항상 [!UICONTROL 고급 증명 옵션] 창을 통해 증명을 만들어야 하며 항상 이 옵션을 통해 사용자를 추가해야 합니다.

* **문제:** [!UICONTROL 관리자] 권한이 있는 사용자가 다른 사용자가 만든 증명에 증명 버전을 추가할 수 없습니다. 다른 사용자가 만든 원본 집합에는 해당 사용자가 증명을 제출할 수 있지만 해당 버전이 연결되지 않습니다.\
   **해결 방법:** [!UICONTROL 관리자] 권한이 있는 사용자는 다음 두 가지 경우에 [!UICONTROL 관리자] 권한이 있는 사용자가 다른 사용자의 증명에 버전을 제출할 수 있습니다.

   * 증명에 명시적으로 추가됨
   * 증명에서 [!UICONTROL 작성자]&#x200B;(증명 역할)로 설정

* **문제:** [!UICONTROL 관리자] 권한이 있는 사용자가 소유하지 않았거나 만들지 않은 증명에서 다른 사용자의 의견을 편집할 수 없습니다.\
   **해결 방법:** [!UICONTROL 관리자] 권한이 있는 사용자가 증명을 소유하고 있지 않지만 댓글을 편집할 수 있는 경우 [!UICONTROL 작성자]&#x200B;(또는 [!UICONTROL 중재자])로 추가하세요.\
   이 세 가지 유형의 권한은 [!DNL Workfront]에서 [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer] 유형 라이선스에 대해 사용할 수 있습니다. [!DNL Workfront]의 시스템 관리자 또는 사용자 관리자는 사용자의 프로필을 편집하고 [!DNL Workfront Proof] 권한을 조정할 수 있습니다.
