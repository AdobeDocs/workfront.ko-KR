---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 홈 달력 보기 설정 구성
description: 웹 기반 버전의 Outlook과 통합되도록 홈 달력 설정을 구성하고 사용 가능한 작업 시간에 따라 작업 로드를 추적하는 데 도움이 됩니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 구성 [!UICONTROL 홈 달력] 설정 보기

을 구성할 수 있습니다 [!UICONTROL 홈 달력] 설정:

* 의 웹 기반 버전과 통합 [!DNL Outlook] 클라우드에서 호스팅 [!DNL Office 365] 또는 [!DNL Outlook Live]. Outlook 일정과 사용자가 선택한 관련 달력(예: 생일 및 휴일 달력)의 모든 이벤트를 [!UICONTROL 홈 달력].
* 작업 로드의 사용 가능한 작업 시간과 비교하여 작업 로드를 추적하는 데 도움이 됩니다. [!UICONTROL 할당] 모음

홈 일정에 대해 자세히 알아보려면 [[!UICONTROL 홈 달력] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

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

보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 통합 정보 [!DNL Microsoft Outlook] 달력

을 사용하여 홈 달력을 구성할 때 다음 사항을 고려하십시오. [!DNL Microsoft Outlook] 달력:

* 웹 기반 버전의 [!DNL Outlook] 클라우드에서 호스팅 [!DNL Office 365] 또는 [!DNL Outlook Live].

   온-프레미스 [!DNL Outlook] 및 [!DNL Outlook] 클라우드 기반 엔터프라이즈 [!DNL Exchange] 서버가 지원되지 않습니다.

   조직에서 단일 사인온을 사용하는 경우 [!DNL Microsoft 365 E3] 또는 [!DNL E5].

* 관련 첨부 파일 [!DNL Outlook] 이벤트는 [!DNL Outlook] 홈 달력의 이벤트.
* 통합 [!DNL Outlook] 달력은 각 사용자에 대해 개별적으로 완료해야 합니다.
* 에 표시되는 이벤트 [!UICONTROL 기한] 표시줄이 [!DNL Microsoft] 달력에서 사용자가 [!UICONTROL 작업 목록] 아래와 같이 [!DNL Adobe Workfront] 달력. 자세한 내용은 [[!UICONTROL 기한] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 및 [의 작업 목록 [!UICONTROL 홈 달력]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL 홈 달력] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* 통합을 활성화할 때 [!DNL Outlook]를 클릭합니다. [!UICONTROL 홈 달력] 이 시점부터 앞으로 동기화됩니다. 통합을 활성화하기 전에 홈 달력에 있던 항목이 표시되지 않으며, 해당 항목을 홈 달력에 다시 표시하려면 해당 항목을 홈 달력으로 다시 드래그해야 합니다 [!DNL Outlook].
* 공유(또는 공유 안 함)할 때 [!DNL Outlook] 다른 사람과 캘린더를 변경하거나 다른 사람과 공유하는 캘린더에 대한 권한 수준을 변경할 때 이 변경 사항이 일정에는 약 30분 동안 영향을 주지 않습니다(자세한 내용은 다음을 참조하십시오) [!DNL Microsoft Outlook] 설명서).\
   따라서, [!DNL Workfront] 캘린더가 포함된 [!DNL Outlook] 다른 사용자와 공유하는 달력은 사용자의 [!DNL Workfront] 30분 정도 일정표.

>[!NOTE]
>
>다음 [!DNL Outlook] 달력 구성은 완전히 별개입니다 [!DNL Outlook] 추가 기능 ([!UICONTROL [!DNL Outlook] 통합] 또는 [!DNL Workfront Outlook]). 일정을 구성하는 데 필요한 설치 작업은 없지만 [!DNL Outlook] 추가 기능. 에 대한 자세한 내용은 [!DNL Outlook] 추가 기능 참조 [설정 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## 구성 [!UICONTROL 홈 달력] 설정 보기

1. 에서 [!UICONTROL 홈 달력] 보기를 클릭하고 **[!UICONTROL 설정]** 톱니바퀴 아이콘 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) 오른쪽 위 모서리에서 **[!UICONTROL 달력 설정]** 창 오른쪽의 패널.

   액세스 방법에 대한 정보가 필요한 경우 [!UICONTROL 홈 달력] 보기, [보기 [!UICONTROL 홈 달력]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (선택 사항) [!DNL Microsoft Outlook] 달력 **[!UICONTROL 계정 추가]** 오른쪽 위 모서리에서 **[!UICONTROL 달력 설정]** 패널. 그런 다음 메시지가 표시되면 을 입력합니다 [!DNL Microsoft Outlook] 로그인 정보. 이 단계를 반복하여 여러 개 추가할 수 있습니다 [!DNL Outlook] 계정.

   >[!NOTE]
   >
   >다음을 수행해야 합니다 [!DNL Workfront] 액세스 권한 [!DNL Outlook] 달력. 권한 부여 허용 [!DNL Workfront] 달력 데이터에 대한 액세스를 유지하려면 [!DNL outlook] 프로필, 읽기 및 업데이트 [!DNL Microsoft] 달력.

1. 브라우저 창을 새로 고쳐 브라우저에서 정보를 확인합니다. [!DNL Outlook] 달력 및 [!UICONTROL 달력 설정] 패널.
1. 을(를) 클릭합니다. **[!UICONTROL 설정]** 오른쪽 위 모서리에서 다시 톱니바퀴 아이콘을 클릭하여 **[!UICONTROL 달력 설정]** 패널. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (선택 사항) 각 [!DNL Microsoft] 이전 단계에서 추가한 계정에서는 **[!UICONTROL 보기]** 또는 **[!UICONTROL 동기화]**:

   * **[!UICONTROL 보기]**: 표시되는 읽기 전용 옵션입니다 [!DNL Microsoft] 달력 이벤트 [!UICONTROL 홈 달력].
   * **[!UICONTROL 동기화]**: 이 옵션을 사용하면 [!DNL Microsoft] 및 [!UICONTROL 홈] 달력. 다시 말하면 [!DNL Workfront] [!UICONTROL 홈 달력] 항목으로 내보내기 [!DNL Microsoft] 달력 및 [!DNL Microsoft] 달력 항목을 Workfront으로 가져오기 [!UICONTROL 홈 달력] 실시간으로

      ![](assets/view-sync-checkboxes-qs.png)

1. (선택 사항) 아래의 [!DNL Workfront] 계정 또는 통합 계정에서 볼 관련 달력을 선택합니다 [!UICONTROL 홈 달력] (예: 유급휴가, 생일 또는 휴일 달력) 브라우저의 [!UICONTROL 새로 고침] 또는 [!UICONTROL 다시 로드] 버튼을 클릭하여 변경 사항을 확인합니다.

1. (선택 사항)에서 **[!UICONTROL 일반]** 섹션 **[!UICONTROL 주 시작 날짜]**&#x200B;을 눌러 홈 달력에서 작업 주의 첫 번째 요일로 표시할 날짜를 선택합니다.

1. 다음 옵션을 구성합니다.

   * **[!UICONTROL 내 근무일 수]:** 작업할 날짜를 선택합니다.
   * **[!UICONTROL 일반적인 시작 시간]:** 근무일을 시작하는 시간을 선택합니다.
   * **[!UICONTROL 일반적인 종료 시간]:** 작업 시간을 선택합니다.

   [!DNL Workfront] 이 세 가지 설정을 사용하여 한 주에 작업하는 시간을 계산합니다. 이 숫자는 [!UICONTROL 할당] 막대 - 사용 가능한 작업 시간에 따라 작업 로드를 추적하는 데 도움이 됩니다. 자세한 내용은 [[!UICONTROL 할당] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) 기사 [[!UICONTROL 홈 달력] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. 를 클릭합니다. **[!UICONTROL 달력 설정]** 해제 영역.

   [!DNL Workfront] 변경 내용을 자동으로 저장합니다.

를 사용하는 방법에 대한 자세한 내용은 [!UICONTROL 달력] 작업 지정 및 통합 달력 이벤트를 관리하려면 다음을 참조하십시오 [를 사용하십시오 [!UICONTROL 홈 달력] 보기](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
