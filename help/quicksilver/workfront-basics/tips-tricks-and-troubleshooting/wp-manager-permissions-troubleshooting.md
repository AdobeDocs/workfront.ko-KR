---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager 권한 문제 해결
description: 다음은 사용 가능한 권한 프로필입니다. [!DNL Adobe] 교정 사용자를 위한 Workfront - 나를 편집합니다.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 증명 관리자] 권한 문제 해결

다음은 사용 가능한 권한 프로필입니다. [!DNL Adobe Workfront] 교정 사용자의 경우:

* [!UICONTROL 관리자]
* [!UICONTROL 감독자]
* [!UICONTROL 관리자]

<!--For detailed information about these options and how to configure them, see .-->

사용자에게 부여할 때 [!UICONTROL 관리자] 사용 권한으로는 다음 문제 해결 정보를 사용할 수 있습니다.

* **문제:** 사용 중인 사용자 [!UICONTROL 관리자] 사용 권한에서는 다른 사용자가 만든 증명을 볼 수 없습니다. 대신, 이 경우 [!UICONTROL 액세스 거부] 화면.

   ![](assets/access-denied-350x161.png)

   **솔루션:** 사용 중인 사용자 [!UICONTROL 관리자] 증명에 권한을 명시적으로 추가해야 합니다. 증명을 항상 을(를) 통해 만들어야 합니다 [!UICONTROL 고급 교정 옵션] 창 및 사용자는 항상 이 옵션을 통해 추가해야 합니다.

* **문제:** 사용 중인 사용자 [!UICONTROL 관리자] 사용 권한은 다른 사용자가 만든 증명에 증명 버전을 추가할 수 없습니다. 다른 사용자가 만든 증명에 증명을 제출할 수 있지만 다른 사용자가 만든 원본 집합에는 버전이 연결되어 있지 않습니다.\
   **솔루션:** 사용 중인 사용자 [!UICONTROL 관리자] 권한이 있는 사용자가 [!UICONTROL 관리자] 권한:

   * 증명에 명시적으로 추가
   * 다음으로 설정 [!UICONTROL 작성자] (증명 역할)

* **문제:** 사용 중인 사용자 [!UICONTROL 관리자] 권한은 다른 사용자가 소유하지 않거나 만들지 않은 증표에 대한 다른 사용자의 주석을 편집할 수 없습니다.\
   **솔루션:** 사용자가 [!UICONTROL 관리자] 권한은 증명을 소유하고 있지 않지만, 주석을 편집하고, 다음과 같이 추가할 수 있어야 합니다. [!UICONTROL 작성자] 또는 [!UICONTROL 중재자]).\
   다음 세 가지 유형의 권한은에서 사용할 수 있습니다 [!DNL Workfront] 대상 [!UICONTROL 계획자], [!UICONTROL 작업자], [!UICONTROL 요청자], [!UICONTROL 검토자] 라이센스 유형. 의 시스템 관리자 또는 사용자 관리자 [!DNL Workfront] 사용자 프로필을 편집하고 조정할 수 있습니다 [!DNL Workfront Proof] 여기에서 사용 권한.
