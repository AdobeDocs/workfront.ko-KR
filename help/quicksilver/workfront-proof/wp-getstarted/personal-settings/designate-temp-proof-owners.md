---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: personal-settings
title: ' [!DNL Workfront Proof]에서 임시 증명 소유자 지정'
description: 장기간 부재 중인 경우 계정의 다른 사용자에게 증명 소유권을 위임할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d00636d7-1eb1-4aac-9663-6335e7675836
source-git-commit: bf6c6c497d98d91ca78f892606a52f82ee4b5666
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# [!DNL Workfront Proof]에서 임시 증명 소유자 지정

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

장기간 부재 중인 경우 계정의 다른 사용자에게 증명 소유권을 위임할 수 있습니다.

>[!NOTE]
>
>이 함수는 [!DNL Workfront Proof]에서만 사용할 수 있습니다.

증명의 임시 소유권을 지정하려면 다음을 수행합니다.

1. [!DNL Workfront Proof] 내에서 **[!UICONTROL 개인 설정]**(으)로 이동합니다.\
   ![personal-settings.png](assets/personal-settings-350x83.png)

1. **[!UICONTROL 부재 중]** 탭을 클릭합니다. 다음 설정을 사용할 수 있습니다.

   * **[!UICONTROL 증명을 계정의 다른 사용자에게 위임]**&#x200B;합니다.
   * 확인란을 선택하거나 선택 취소하여 **[!UICONTROL 부재 중]** 기능을 사용하도록 설정하고 사용하지 않도록 설정합니다.
   * **[!UICONTROL 시작 날짜]**&#x200B;를 선택하십시오.

     **[!UICONTROL 즉시 시작]** 옵션을 선택하면 기능을 활성화한 후 바로 선택한 사용자에게 증명 소유권이 위임됩니다.

     특정 시작 날짜 및 시간이 설정되면 기능은 선택한 날짜 및 선택한 시간에 활성화됩니다.

   * **[!UICONTROL 종료 날짜]**&#x200B;를 선택하십시오.

     종료 날짜를 선택하지 않으면 기능을 수동으로 비활성화할 때까지 증명 소유권이 위임됩니다.

     특정 종료 날짜 및 시간이 설정되면 기능은 선택한 날짜 및 선택한 시간에 비활성화됩니다.

     ![out-of-office-options.png](assets/out-of-office-options-350x234.png)

1. 증명을 위임하면 위임된 소유자가 증명 세부 정보 페이지의 **[!UICONTROL 세부 정보]** 섹션에 표시됩니다. 증명 세부 정보 페이지의 **[!UICONTROL 활동]** 섹션에 소유권 위임 노트가 표시됩니다.

   ![activity-section-delegated.png](assets/activity-section-delegated-350x318.png)

   기능이 활성화된 동안 [!UICONTROL 부재 중] 알림이 원본 증명 소유자의 계정에도 표시됩니다. 이는 원래 소유자에게 알림 메시지를 보내는 역할을 하며, 이 소유자는 위임을 즉시 종료하거나 [!UICONTROL 개인 설정]으로 이동하여 이를 조정할 수 있습니다.

   ![notification-on-account.png](assets/notification-on-account-350x15.png)

   증명에 대한 소유권을 원래 소유자가 다시 가져오면 위임된 소유자는 증명 세부 정보 페이지의 [!UICONTROL 세부 정보] 섹션에서 사라지고 [!UICONTROL 부재 중] 알림은 더 이상 원래 증명 소유자의 계정에 표시되지 않습니다. 증명 소유권이 되돌려졌음을 보여 주는 메모가 증명 세부 정보 페이지의 [!UICONTROL 활동] 섹션에 표시됩니다.

   >[!NOTE]
   >
   >위임된 소유자는 수동으로 제거하지 않는 한 증명 워크플로에 남아 있습니다.

   ![[!UICONTROL activity-section-taken-back].png](assets/activity-section-taken-back-350x99.png)
