---
product-area: setup
navigation-topic: notifications
title: 고유한 이벤트 알림 활성화 또는 비활성화
description: Adobe Workfront 관리자는 Workfront에서 이벤트가 발생할 때 사용자가 받는 이벤트 알림을 구성합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# 고유한 이벤트 알림 활성화 또는 비활성화

Adobe [!DNL Workfront] 관리자는 Workfront에서 이벤트가 발생할 때 사용자가 받는 이벤트 알림을 구성합니다(에 설명된 대로) [[!UICONTROL 이벤트 구성] 시스템의 모든 사용자에 대한 알림](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

그룹 관리자는 사용자와 홈 그룹의 사용자를 위해 활성화되는 이벤트 알림을 구성할 수도 있습니다. 만약 [!UICONTROL 홈 그룹] 는 하위 그룹이므로 그룹 위의 최상위 그룹에 대해 활성화된 이벤트 알림을 받게 됩니다.

수신한 알림을 구성하여 이를 추가로 사용자 지정할 수 있습니다. 이벤트가 발생하면 알림을 수신할지 또는 일별 다이제스트 이메일에서 수신할지를 선택할 수도 있습니다.

이메일 알림에 대한 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* 알림 유형을 활성화한 다음 해당 유형의 알림을 받지 않는 경우 해당 유형이 역할에 적용되지 않기 때문일 수 있습니다.
>* 다음 [!DNL Workfront] 관리자 또는 그룹 관리자가 알림을 구성할 수 없습니다 [!DNL Workfront Goals]. 다음 알림에 대한 자세한 정보 [!DNL Workfront] 관리자가 구성할 수 있습니다. 자세한 내용은 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 에 대한 개별 알림 구성에 대한 자세한 내용은 [!DNL Workfront Goals] 이 문서를 계속 읽으십시오.
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 전자 메일 알림 설정을 보고 수정합니다

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]을 클릭한 다음 프로필 사진 옆에 있는 사용자 이름을 클릭합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png) 를 클릭한 다음 **[!UICONTROL 편집]**.

1. 에서 **[!UICONTROL 개인 편집]** 표시되는 상자에서 로 이동합니다. **[!UICONTROL 알림 을 참조하십시오]** 섹션을 참조하십시오.

1. 해당 카테고리와 관련된 알림 설정을 보려면 카테고리를 클릭합니다.

   ![](assets/my-profile-notifications.png)

1. 오른쪽 확인란을 선택하거나 선택 취소하여 매일 또는 즉시 알림을 수신할지 여부를 지정합니다.

   카테고리에 대한 확인란을 사용하여 해당 카테고리의 모든 알림을 활성화하거나 비활성화할 수도 있습니다.

   >[!NOTE]
   >
   >프로젝트의 팀 멤버인 경우 더 이상 프로젝트에 액세스할 수 없는 경우에도 팀에서 제거될 때까지 전자 메일 알림을 계속 받게 됩니다. 팀에서 사용자 제거에 대한 지침은 [프로젝트에서 사용자 제거](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   대상 **[!UICONTROL 통신]** 카테고리에서는 인스턴트 게재에만 사용할 개별 알림을 선택할 수 있습니다. 일별 다이제스트에 알림을 전달하려면 모두 선택해야 합니다.

   지정된 카테고리에 대한 모든 이메일 알림이 활성화되면 카테고리 제목의 상자가 선택된 것으로 나타납니다. 지정된 카테고리의 모든 이메일 알림이 비활성화되면 상자를 선택하지 않습니다. 일부 알림이 활성화되고 다른 알림이 비활성화되면 카테고리 확인란이 직선(직선)으로 표시됩니다.\
   알림 설정을 수정할 때 레이블은 **[!UICONTROL 편집됨]** 알림 설정이 수정되었음을 알리는 해당 알림 설정에 대해 나타납니다.

1. 일별 다이제스트로 전송할 알림을 선택한 경우, 맨 위에서 받을 시간을 선택합니다 **[!UICONTROL 알림 을 참조하십시오]** 의 섹션 **[!UICONTROL Email Daily Digest after]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   일별 다이제스트는 선택한 시간 24시간 전에 알림의 기준을 충족하는 이벤트를 포함합니다. 각 알림 유형에 대해 일별 다이제스트 이메일 하나를 받게 됩니다.\
   일별 다이제스트는 시스템에서 전달을 위해 대기하는 이메일 수에 따라 사용자가 선택하는 시간 이후에 도착할 수 있습니다. 나열된 시간은 브라우저 설정에 지정된 현지 시간입니다.

1. (조건부 및 선택 사항) 미리 보기 환경에서 전자 메일 알림 설정을 수정할 때 **[!UICONTROL 이 테스트 환경에서 전자 메일 받기]** 이메일 수신을 설정하는 중입니다. 이메일은 미리 보기 환경에서 자동으로 생성되지 않습니다.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. 클릭 **[!UICONTROL 변경 내용 저장]**.
