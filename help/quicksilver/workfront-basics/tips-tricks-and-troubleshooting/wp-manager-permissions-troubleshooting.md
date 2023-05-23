---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager 권한 문제 해결
description: 사용 가능한 권한 프로필 [!DNL Adobe] 증명 사용자를 위한 Workfront은 관리자, 감독자 및 관리자입니다.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 증명 관리자] 권한 문제 해결

다음은에서 사용할 수 있는 권한 프로필입니다. [!DNL Adobe Workfront] 증명 사용자의 경우:

* [!UICONTROL 관리자]
* [!UICONTROL 감독자]
* [!UICONTROL 관리자]

<!--For detailed information about these options and how to configure them, see .-->

사용자에게 권한을 부여할 때 [!UICONTROL 관리자] 사용 권한, 다음 문제 해결 정보를 사용할 수 있습니다.

* **문제:** 을 사용하는 사용자 [!UICONTROL 관리자] 다른 사용자가 만든 증명은 권한으로 볼 수 없습니다. 대신, [!UICONTROL 액세스 거부됨] 화면.

   ![](assets/access-denied-350x161.png)

   **해결 방법:** 을 사용하는 사용자 [!UICONTROL 관리자] 증명에 권한을 명시적으로 추가해야 합니다. 증명은 항상 [!UICONTROL 고급 증명 옵션] 창 및 사용자는 항상 이 옵션을 통해 추가해야 합니다.

* **문제:** 을 사용하는 사용자 [!UICONTROL 관리자] 다른 사용자가 만든 증명에 증명 버전을 추가할 수 없습니다. 문서 집합에 증명을 제출할 수 있지만 다른 사용자가 만든 원본 집합에는 버전이 연결되지 않습니다.\
   **해결 방법:** 을 사용하는 사용자 [!UICONTROL 관리자] 사용 권한은 다음 사용자가 보유한 경우에만 다른 사용자의 증명에 버전을 제출할 수 있습니다. [!UICONTROL 관리자] 다음 두 가지 경우의 권한:

   * 증명에 명시적으로 추가됨
   * 다음으로 설정 [!UICONTROL 작성자] (증명 역할) 증명

* **문제:** 을 사용하는 사용자 [!UICONTROL 관리자] 권한이 없거나 작성하지 않은 증명에 대한 다른 사용자의 주석을 편집할 수 없습니다.\
   **해결 방법:** 다음과 같은 경우 [!UICONTROL 관리자] 권한은 증명을 소유하지 않지만 주석을 편집하고 추가할 수 있어야 합니다. [!UICONTROL 작성자] (또는 [!UICONTROL 중재자]).\
   다음 세 가지 유형의 권한은에서 사용할 수 있습니다 [!DNL Workfront] 대상 [!UICONTROL 플래너], [!UICONTROL 작업자], [!UICONTROL 요청자], [!UICONTROL 검토자] 라이센스를 입력합니다. 의 시스템 관리자 또는 사용자 관리자 [!DNL Workfront] 사용자의 프로필을 편집하고 조정할 수 있음 [!DNL Workfront Proof] 권한 부여
