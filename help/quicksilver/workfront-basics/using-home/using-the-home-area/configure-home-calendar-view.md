---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 홈 캘린더 보기 설정 구성
description: 웹 기반 버전의 Outlook과 통합되도록 홈 캘린더 설정을 구성하고 사용 가능한 작업 시간에 대한 워크로드를 추적하는 데 도움이 될 수 있습니다.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 구성 [!UICONTROL 홈 캘린더] 설정 보기

<!--Audited: 01/2024-->

다음을 구성할 수 있습니다. [!UICONTROL 홈 캘린더] 다음을 수행하는 설정:

* 클라우드 호스팅된 [!DNL Office 365] 또는 [!DNL Outlook Live]에서 웹 기반 버전의 [!DNL Outlook]과 통합합니다. Outlook 일정에서 선택한 모든 이벤트와 연결된 일정을 표시할 수 있습니다. [!UICONTROL 홈 캘린더] Adobe Workfront.
* 에서 사용 가능한 작업 시간에 대한 워크로드를 추적하는 데 도움이 됩니다. [!UICONTROL 할당] 막대.

홈 캘린더에 대한 자세한 내용은 [[!UICONTROL 홈 캘린더] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

이 문서에서는 홈 캘린더 설정을 구성하고 홈 캘린더를 외부 Outlook 캘린더와 통합하는 방법에 대해 설명합니다.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>현재: [!UICONTROL Work] 이상</p> 
   또는
   <p>새로운 기능: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*보유 중인 플랜 또는 라이선스 유형을 확인하려면 다음 연락처로 문의하십시오. [!DNL Workfront] 관리자. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 통합 기본 정보 [!DNL Microsoft Outlook] 캘린더

홈 캘린더 를 구성할 때 다음 사항을 고려하십시오. [!DNL Microsoft Outlook] 캘린더:

* 의 웹 기반 버전만 통합할 수 있습니다. [!DNL Outlook] 클라우드 호스팅 [!DNL Office 365] 또는 [!DNL Outlook Live].

  온프레미스 [!DNL Outlook] 및 [!DNL Outlook] 클라우드 기반 기업에서 [!DNL Exchange] 서버가 지원되지 않습니다.

  조직에서 단일 사인온을 사용하는 경우 다음이 필요합니다. [!DNL Microsoft 365 E3] 또는 [!DNL E5].

* 다음 항목과 연결된 첨부 파일 [!DNL Outlook] 이벤트가 다음에 연결되지 않음 [!DNL Outlook] 홈 캘린더의 이벤트입니다.
* 와 통합 [!DNL Outlook] 각 사용자에 대해 개별적으로 달력을 완료해야 합니다.
* 에 표시되는 이벤트 [!UICONTROL 예정] 표시줄이 다음에 표시되지 않음 [!DNL Microsoft] 캘린더에서 드래그하지 않은 경우 [!UICONTROL 작업 목록] (으)로 [!DNL Adobe Workfront] 달력. 자세한 내용은 [[!UICONTROL 예정] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 및 [의 작업 목록 [!UICONTROL 홈 캘린더]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) 위치: [[!UICONTROL 홈 캘린더] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* 과 통합을 활성화한 경우 [!DNL Outlook], 로 끌어온 작업 항목만 [!UICONTROL 홈 캘린더] 그 시점부터는 앞으로 동기화됩니다. 통합을 활성화하기 전에 홈 캘린더에 있었던 항목은 표시되지 않으며, 항목을 표시하려는 경우 홈 캘린더로 다시 드래그해야 합니다. [!DNL Outlook].
* 을(를) 공유(또는 공유 해제)할 때 [!DNL Outlook] 다른 사람과 함께 있는 캘린더 또는 다른 사람과 공유하는 캘린더에 대한 권한 수준을 변경할 때 이 변경 사항은 약 30분 동안 캘린더에 영향을 주지 않습니다. 자세한 내용은 [!DNL Microsoft Outlook] 설명서를 참조하십시오.\
   따라서 를 통합할 때 [!DNL Workfront] 이 포함된 캘린더 [!DNL Outlook] 다른 사용자와 공유하는 캘린더에는 사용자의 [!DNL Workfront] 약 30분 동안 일정 항목.

>[!NOTE]
>
>다음 [!DNL Outlook] 달력 구성은 [!DNL Outlook] 추가 기능 ([!UICONTROL [!DNL Outlook] 통합] 또는 [!DNL Workfront Outlook]). 캘린더를 구성하는 데 필요한 설치는 없지만 을(를) 위한 설치는 필요합니다. [!DNL Outlook] 추가 기능. 에 대한 자세한 내용은 [!DNL Outlook] 추가 기능 참조 [설정 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## 구성 [!UICONTROL 홈 캘린더] 설정을 보고 Outlook 일정과 통합

1. 다음에서 [!UICONTROL 홈 캘린더] 보기, 클릭 **[!UICONTROL 설정]** 톱니바퀴 아이콘 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) 오른쪽 위 모서리에서 을 엽니다. **[!UICONTROL 캘린더 설정]** 오른쪽 패널

   에 액세스하는 방법에 대한 정보가 필요한 경우 [!UICONTROL 홈 캘린더] 보기, 참조 [보기 [!UICONTROL 홈 캘린더]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (선택 사항) [!DNL Microsoft Outlook] 캘린더, 클릭 **[!UICONTROL 계정 추가]** 의 오른쪽 위 모서리 **[!UICONTROL 캘린더 설정]** 패널. 그런 다음 메시지가 표시되면 [!DNL Microsoft Outlook] 로그인 정보. 이 단계를 반복하여 여러 을 추가할 수 있습니다 [!DNL Outlook] 계정.

   >[!NOTE]
   >
   >다음을 제공해야 합니다. [!DNL Workfront] 액세스 권한 [!DNL Outlook] 달력. 권한 부여를 통해 [!DNL Workfront] 달력 데이터에 대한 액세스를 유지하려면 다음을 읽어 보십시오. [!DNL outlook] 프로필 작성, 읽기 및 업데이트 [!DNL Microsoft] 달력.

1. 브라우저 창을 새로 고쳐 의 정보를 봅니다. [!DNL Outlook] 캘린더의 계정 및 [!UICONTROL 캘린더 설정] 패널.
1. 다음을 클릭합니다. **[!UICONTROL 설정]** 오른쪽 위 모서리에 있는 톱니바퀴 아이콘을 다시 클릭하여 **[!UICONTROL 캘린더 설정]** 패널. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (선택 사항) 각 [!DNL Microsoft] 이전 단계에서 추가한 계정에서 **[!UICONTROL 보기]** 또는 **[!UICONTROL 동기화]**:

   * **[!UICONTROL 보기]**: 표시되는 읽기 전용 옵션입니다 [!DNL Microsoft] 의 캘린더 이벤트 [!UICONTROL 홈 캘린더].
   * **[!UICONTROL 동기화]**: 이 옵션을 사용하면 다음 작업 간에 양방향 동기화가 허용됩니다. [!DNL Microsoft] 및 [!UICONTROL 홈] 달력. 다른 말로 하자면 [!DNL Workfront] [!UICONTROL 홈 캘린더] 다음으로 항목 내보내기 [!DNL Microsoft] 달력 및 [!DNL Microsoft] Workfront으로 일정 항목 가져오기 [!UICONTROL 홈 캘린더] 실시간으로.

     ![](assets/view-sync-checkboxes-qs.png)

1. (선택 사항) [!DNL Workfront] 계정 또는 통합 계정에서 보려는 관련 달력을 선택합니다. [!UICONTROL 홈 캘린더] (PTO, 생일 또는 휴일 달력 등) 그런 다음 브라우저의 [!UICONTROL 새로 고침] 또는 [!UICONTROL 다시 로드] 단추를 클릭하여 변경 사항을 확인합니다.

1. (선택 사항) **[!UICONTROL 일반]** 아래 섹션 **[!UICONTROL 주 시작 요일]**&#x200B;을 클릭하고 홈 캘린더에서 작업 주의 첫 번째 날로 표시할 요일을 선택합니다.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 다음 옵션을 구성합니다.

   * **[!UICONTROL 내 근무일]:** 근무일을 선택합니다.
   * **[!UICONTROL 내 평소 시작 시간]:** 근무일을 시작하는 시간을 선택합니다.
   * **[!UICONTROL 내 평소 종료 시간]:** 근무일을 종료하는 시간을 선택합니다.

   [!DNL Workfront] 이 세 가지 설정을 사용하여 한 주에 작업하는 시간을 계산합니다. 이 숫자는 다음 항목에 영향을 줍니다. [!UICONTROL 할당] 작업 시간 대비 작업 부하를 추적하는 데 도움이 되는 막대 자세한 내용은 [[!UICONTROL 할당] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) 이 문서에서 [[!UICONTROL 홈 캘린더] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. 바깥쪽을 클릭합니다. **[!UICONTROL 캘린더 설정]** 닫을 영역입니다.

   [!DNL Workfront] 변경 사항을 자동으로 저장합니다.

사용에 대한 자세한 내용 [!UICONTROL 캘린더] 작업 할당 및 통합 달력 이벤트를 관리하려면 다음을 참조하십시오. [사용 [!UICONTROL 홈 캘린더] 보기](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
