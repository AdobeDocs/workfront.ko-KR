---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft] 팀에서  [!DNL Adobe Workfront] 작업 만들기'
description: 팀 소유자가 귀하의 팀에 대해 Adobe을 설치 및 구성 [!DNL Workfront] 했으며 귀하가 Microsoft Teams에서 Workfront에 로그인한 경우 Microsoft TeamsMicrosoft Teams 에서  [!DNL Workfront] 개인 작업을 만들 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# [!DNL Microsoft Teams]에서 [!DNL Adobe Workfront]개 작업 만들기

<!--

>[!NOTE]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr>
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 전제 조건

다음 조건이 충족되는 경우 [!DNL Microsoft Teams]의 [!DNL Adobe Workfront]에서 개인 작업을 만들 수 있습니다.

* 팀 소유자가 귀하의 팀에 대해 [!DNL Workfront for Microsoft Teams]을(를) 설치하고 구성했습니다.
* [!DNL Microsoft Teams]에서 [!DNL Workfront]에 로그인했습니다.

>[!NOTE]
>
>[!DNL Microsoft Teams]은(는) 더 이상 [!DNL Internet Explorer]을(를) 지원하지 않습니다. [!DNL Adobe Workfront for Microsoft Teams] 통합을 사용하려면 [!DNL Internet Explorer] 이외의 웹 브라우저를 사용해야 합니다.

[!DNL Workfront for Microsoft Teams]을(를) 설치하고 [!DNL Microsoft Teams]에서 [!UICONTROL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

## [!DNL Microsoft Teams]에서 개인 작업 만들기

1. [!DNL Microsoft Teams]에서 [!DNL Workfront]에 로그인합니다.

   [!DNL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

1. **[!UICONTROL 새 작업]** 카드를 열려면:

   * [!DNL Workfront] 봇 채팅 채널에 있는 경우 [!UICONTROL 대화] 필드에 **[!UICONTROL 새 작업]**&#x200B;을 입력하여 새 작업을 만드십시오.
   * [!DNL Workfront] 보트 채팅 채널 이외의 채팅 채널에 있는 경우:

      * [!UICONTROL 대화] 필드에 **[!DNL @workfront]**&#x200B;을(를) 입력한 다음 원하는 [!DNL Workfront] 봇 채널을 선택하십시오.
      * [!UICONTROL 대화] 필드에 **[!UICONTROL 새 작업]**&#x200B;을(를) 계속 입력하여 새 작업을 만듭니다.

        [!UICONTROL 새 작업] 카드가 [!DNL Workfront] 봇 채널에 표시됩니다.

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. [!UICONTROL Workfront] 봇 채널에서 [!UICONTROL 새 작업] 카드에 다음 정보를 지정합니다.

   * **[!UICONTROL 작업 제목]** 필드에 작업 이름이 있습니다.
   * **[!UICONTROL 작업 설명을 쓰기]** 필드에 작업 설명이 있습니다.
   * **[!UICONTROL 기한]** 필드에서 작업을 완료해야 하는 날짜입니다.

1. **[!UICONTROL 저장].** 클릭

   새 개인 작업이 [!DNL Workfront]에 만들어졌습니다. [!UICONTROL 참조 번호]이(가) 할당되어 [!UICONTROL 새 작업] 카드에 표시됩니다.

   참조 번호에 대한 자세한 내용은 [개체 이해 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 문서에서 [[!UICONTROL 개체의 참조 번호]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) 섹션을 참조하십시오.

1. (선택 사항) 작업 정보를 추가로 편집하려면 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. (선택 사항) [!DNL Workfront]의 새 탭에서 작업을 열고 추가로 작업을 편집하거나, 프로젝트로 이동하거나, 다른 사람에게 할당하려면 [!DNL Workfront]]**의**[!UICONTROL &#x200B;보기를 클릭합니다.
