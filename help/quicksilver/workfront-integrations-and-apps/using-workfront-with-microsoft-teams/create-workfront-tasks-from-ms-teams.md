---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Adobe Workfront] 팀에서  [!DNL Microsoft] 작업 만들기'
description: 팀 소유자가 귀하의 팀에 대해 Adobe을 설치 및 구성 [!DNL Workfront] 했으며 귀하가 Microsoft Teams에서 Workfront에 로그인한 경우 Microsoft TeamsMicrosoft Teams 에서  [!DNL Workfront] 개인 작업을 만들 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# [!DNL Adobe Workfront]에서 [!DNL Microsoft Teams]개 작업 만들기

>[!IMPORTANT]
>
>[Microsoft이 새 팀 클라이언트로 전환](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)됨에 따라 클래식 팀 클라이언트는 2025년 7월 1일 이후에 더 이상 사용할 수 없습니다. Workfront과 같은 Microsoft Teams 및 통합 앱을 계속 사용하려면 이 날짜 이전에 고객이 New Teams 클라이언트로 전환해야 합니다.
>
>이제 업데이트된 Workfront 통합을 사용할 수 있으며 새 팀 경험과 완전히 호환됩니다. 대부분의 경우 사용자가 전환되면 Workfront이 자동으로 표시됩니다. 그렇지 않은 경우 Microsoft Teams App Store에서 수동으로 통합을 설치할 수 있습니다. 새 Teams 클라이언트에서 Workfront 통합을 설치하거나 확인하려면 [Microsoft Teams용 설치 [!DNL Adobe Workfront] 를 참조하십시오](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).



## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
   <p>작업 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

다음 조건이 충족되는 경우 [!DNL Adobe Workfront]의 [!DNL Microsoft Teams]에서 개인 작업을 만들 수 있습니다.

* 팀 소유자가 귀하의 팀에 대해 [!DNL Workfront for Microsoft Teams]을(를) 설치하고 구성했습니다.
* [!DNL Workfront]에서 [!DNL Microsoft Teams]에 로그인했습니다.

>[!NOTE]
>
>[!DNL Microsoft Teams]은(는) 더 이상 [!DNL Internet Explorer]을(를) 지원하지 않습니다. [!DNL Adobe Workfront for Microsoft Teams] 통합을 사용하려면 [!DNL Internet Explorer] 이외의 웹 브라우저를 사용해야 합니다.

[!DNL Workfront for Microsoft Teams]을(를) 설치하고 [!UICONTROL 에서 &#x200B;]Workfront[!DNL Microsoft Teams]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

## [!DNL Microsoft Teams]에서 개인 작업 만들기

1. [!DNL Workfront]에서 [!DNL Microsoft Teams]에 로그인합니다.

   [!DNL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

1. **[!UICONTROL 새 작업]** 카드를 열려면:

   * [!DNL Workfront] 봇 채팅 채널에 있는 경우 **[!UICONTROL 대화]** 필드에 [!UICONTROL 새 작업]을 입력하여 새 작업을 만드십시오.
   * [!DNL Workfront] 보트 채팅 채널 이외의 채팅 채널에 있는 경우:

      * **[!DNL @workfront]**&#x200B;대화[!UICONTROL &#x200B; 필드에 &#x200B;]을(를) 입력한 다음 원하는 [!DNL Workfront] 봇 채널을 선택하십시오.
      * **[!UICONTROL 대화]** 필드에 [!UICONTROL 새 작업]을(를) 계속 입력하여 새 작업을 만듭니다.

        [!UICONTROL 새 작업] 카드가 [!DNL Workfront] 봇 채널에 표시됩니다.

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. [!UICONTROL Workfront] 봇 채널에서 [!UICONTROL 새 작업] 카드에 다음 정보를 지정합니다.

   * **[!UICONTROL 작업 제목]** 필드에 작업 이름이 있습니다.
   * **[!UICONTROL 작업 설명을 쓰기]** 필드에 작업 설명이 있습니다.
   * **[!UICONTROL 기한]** 필드에서 작업을 완료해야 하는 날짜입니다.

1. **[!UICONTROL 저장].** 클릭

   새 개인 작업이 [!DNL Workfront]에 만들어졌습니다. [!UICONTROL 참조 번호]이(가) 할당되어 [!UICONTROL 새 작업] 카드에 표시됩니다.

   참조 번호에 대한 자세한 내용은 [[!UICONTROL 개체 이해] 문서에서 &#x200B;](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)개체의 참조 번호[&#x200B; [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 섹션을 참조하십시오.

1. (선택 사항) 작업 정보를 추가로 편집하려면 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. (선택 사항) **[!UICONTROL 의 새 탭에서 작업을 열고 추가로 작업을 편집하거나, 프로젝트로 이동하거나, 다른 사람에게 할당하려면[!DNL Workfront]]**&#x200B;의 [!DNL Workfront]보기를 클릭합니다.
