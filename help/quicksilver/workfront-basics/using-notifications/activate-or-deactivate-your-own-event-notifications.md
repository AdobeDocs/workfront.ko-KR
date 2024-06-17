---
product-area: setup
navigation-topic: notifications
keywords: 수정,이메일,알림,설정
title: 이메일 알림 수정
description: 이 문서에서는 사용자 프로필에서 이메일 알림을 관리하는 방법을 설명합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: f9afe7c8f04777dd547ea1e202e7844bdfd3518e
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 이메일 알림 수정

<!-- Audited: 1/2024 -->

내 Adobe [!DNL Workfront] 관리자는에서 설명한 대로 Workfront에서 이벤트가 발생할 때 사용자가 수신하는 이메일 알림을 구성합니다. [[!UICONTROL 이벤트 구성] 시스템의 모든 사용자를 위한 알림](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

그룹 관리자는 사용자와 사용자의 알림을 구성할 수도 있습니다. [!UICONTROL 홈 그룹]. 다음의 경우 [!UICONTROL 홈 그룹] 는 하위 그룹이며, 그룹 위의 최상위 그룹에 대해 활성화된 알림을 받습니다.

수신할 알림을 구성하여 이를 추가로 사용자 정의할 수 있습니다. 이벤트 발생 시 알림을 수신할지 또는 일일 요약 이메일 1개로 알림을 수신할지 선택할 수도 있습니다.

이메일 알림에 대한 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* 알림 유형을 활성화한 다음 해당 유형의 알림을 받지 않는 경우, 해당 유형이 역할에 적용되지 않기 때문일 수 있습니다.
>* 다음 [!DNL Workfront] 관리자 또는 그룹 관리자가 다음에 대한 알림을 구성할 수 없음: [!DNL Workfront Goals]. 알림에 대한 자세한 내용은 [!DNL Workfront] 관리자가 구성할 수 있습니다. 다음을 참조하십시오. [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 의 개별 알림 구성에 대한 자세한 내용 [!DNL Workfront Goals] 이 문서를 계속 읽으십시오.
>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td>  <p>신규:</p> 
   <ul><li>기여자 이상</li></ul>
   <p>현재:</p>
   <ul><li>요청 이상</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 이메일 알림 설정 보기 및 수정

{{step1-click-profile-pic}}

1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png) 이름 옆에 있는 을(를) 클릭한 다음 을(를) 클릭합니다 **[!UICONTROL 편집]**.

1. 다음에서 **[!UICONTROL 사용자 편집]** 표시되는 상자에서 **[!UICONTROL 알림]** 섹션.

1. 범주를 클릭하여 해당 범주와 관련된 알림 설정을 봅니다.

   ![](assets/my-profile-notifications.png)

1. 오른쪽에 있는 확인란을 선택하거나 선택 해제하여 알림을 매일 수신할지, 즉시 수신할지 또는 둘 다 수신할지 여부를 지정합니다.

   범주의 확인란을 사용하여 해당 범주의 모든 알림을 활성화하거나 비활성화할 수도 있습니다.

   >[!NOTE]
   >
   >프로젝트의 팀원인 경우 더 이상 프로젝트에 액세스할 수 없는 경우에도 팀에서 제거될 때까지 프로젝트에 대한 이메일 알림을 계속 수신하게 됩니다. 팀에서 사용자를 제거하는 방법에 대한 지침은 [프로젝트에서 사용자 제거](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   의 경우 **[!UICONTROL 커뮤니케이션]** 범주, 인스턴트 게재에 대해서만 개별 알림을 선택할 수 있습니다. 일별 요약으로 알림을 전달하려면 알림을 모두 선택해야 합니다.

   지정된 카테고리에 대한 모든 이메일 알림이 활성화되면 카테고리 제목의 상자가 선택된 상태로 표시됩니다. 지정된 범주의 모든 이메일 알림이 비활성화되면 상자를 선택 취소합니다. 일부 알림이 활성화되고 다른 알림이 비활성화되면 카테고리 확인란이 직선으로 표시됩니다.\
   알림 설정을 수정할 때 레이블은 **[!UICONTROL 편집됨]** 은 해당 알림 설정에 대해 표시되어 해당 알림 설정이 수정되었음을 알려줍니다.

1. 일별 요약으로 보낼 알림을 선택한 경우, 맨 위에서 알림을 받을 시간을 선택합니다. **[!UICONTROL 알림]** 의 섹션 **[!UICONTROL 다음 이후 이메일 일일 요약:]** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   일별 요약에는 선택한 시간보다 24시간 전에 알림 기준을 충족하는 이벤트가 포함됩니다. 각 알림 유형에 대해 일별 요약 이메일 1개를 받습니다.\
   시스템에서 게재를 위해 큐에 올라가 있는 이메일 수에 따라, 선택한 시간 후에 일별 요약이 도착할 수 있습니다. 나열된 시간은 브라우저 설정에 지정된 현지 시간입니다.

1. (조건부 및 선택 사항) 미리 보기 환경에서 이메일 알림 설정을 수정할 때 **[!UICONTROL 이 테스트 환경에서 이메일 수신]** 이메일을 수신하도록 설정합니다. 이메일은 미리보기 환경에서 자동으로 생성되지 않습니다.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.
