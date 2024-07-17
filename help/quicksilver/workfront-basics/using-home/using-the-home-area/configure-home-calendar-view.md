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

# [!UICONTROL 홈 일정] 보기 설정 구성

<!--Audited: 01/2024-->

다음을 수행하도록 [!UICONTROL 홈 캘린더] 설정을 구성할 수 있습니다.

* 클라우드 호스팅된 [!DNL Office 365] 또는 [!DNL Outlook Live]에서 웹 기반 버전의 [!DNL Outlook]과 통합합니다. Adobe Workfront의 [!UICONTROL 홈 일정]에서 선택한 Outlook 일정과 연결된 모든 일정을 표시할 수 있습니다.
* [!UICONTROL 할당] 막대에서 사용 가능한 작업 시간에 대한 작업량을 추적하는 데 도움이 됩니다.

홈 캘린더에 대한 자세한 내용은 [[!UICONTROL 홈 캘린더] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)를 참조하세요.

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

*보유 중인 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Microsoft Outlook] 캘린더 통합 기본 정보

[!DNL Microsoft Outlook] 캘린더로 홈 캘린더를 구성할 때 다음 사항을 고려하십시오.

* 클라우드 호스팅 [!DNL Office 365] 또는 [!DNL Outlook Live]에서는 [!DNL Outlook]의 웹 기반 버전만 통합할 수 있습니다.

  클라우드 기반 엔터프라이즈 [!DNL Exchange] 서버의 온-프레미스 [!DNL Outlook] 및 [!DNL Outlook]은(는) 지원되지 않습니다.

  조직에서 SSO(Single Sign-On)를 사용하는 경우 [!DNL Microsoft 365 E3] 또는 [!DNL E5]이(가) 필요합니다.

* [!DNL Outlook] 이벤트와 연결된 첨부 파일이 홈 캘린더의 [!DNL Outlook] 이벤트에 첨부되지 않았습니다.
* [!DNL Outlook] 일정과의 통합은 각 사용자에 대해 개별적으로 완료해야 합니다.
* [!UICONTROL 기한] 표시줄에 표시되는 이벤트는 [!UICONTROL 작업 목록]에서 [!DNL Adobe Workfront] 일정으로 드래그하지 않으면 [!DNL Microsoft] 일정에 표시되지 않습니다. 자세한 내용은 [[!UICONTROL 홈 일정] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)의 [!UICONTROL 홈 일정]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view)에서 [[!UICONTROL 기한] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 및 [작업 목록을 참조하십시오.

* [!DNL Outlook]과(와) 통합을 사용하도록 설정하면 해당 시점부터 [!UICONTROL 홈 일정](으)로 드래그된 작업 항목만 동기화됩니다. 통합을 활성화하기 전에 홈 캘린더에 있었던 항목은 표시되지 않습니다. [!DNL Outlook]에 표시하려면 항목을 홈 캘린더로 다시 끌어와야 합니다.
* [!DNL Outlook] 캘린더를 다른 사람과 공유(또는 공유 해제)하거나 다른 사람과 공유하는 캘린더의 사용 권한 수준을 변경할 때 이 변경 사항은 약 30분 동안 캘린더에 영향을 주지 않습니다. 자세한 내용은 [!DNL Microsoft Outlook] 설명서를 참조하십시오.\
   따라서 [!DNL Workfront] 일정을 다른 사용자와 공유하는 [!DNL Outlook] 일정과 통합하면 해당 사용자는 약 30분 동안 [!DNL Workfront] 일정 항목을 볼 수 없습니다.

>[!NOTE]
>
>[!DNL Outlook] 일정 구성은 [!DNL Outlook] 추가 기능([!UICONTROL [!DNL Outlook] 통합] 또는 [!DNL Workfront Outlook])과 완전히 별개입니다. 일정을 구성하는 데 필요한 설치가 없지만 [!DNL Outlook] 추가 기능에는 설치가 필요합니다. [!DNL Outlook] 추가 기능에 대한 자세한 내용은 [설정 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)을 참조하세요.

## [!UICONTROL 홈 일정] 보기 설정을 구성하고 Outlook 일정과 통합

1. [!UICONTROL 홈 캘린더] 보기에서 오른쪽 상단의 **[!UICONTROL 설정]** 톱니바퀴 아이콘 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)을(를) 클릭하여 오른쪽의 **[!UICONTROL 캘린더 설정]** 패널을 엽니다.

   [!UICONTROL 홈 일정] 보기에 액세스하는 방법에 대한 정보가 필요한 경우 [[!UICONTROL 홈 일정 보기]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)를 참조하세요.

1. (선택 사항) [!DNL Microsoft Outlook] 일정을 통합하려면 **[!UICONTROL 일정 설정]** 패널의 오른쪽 상단 모서리에서 **[!UICONTROL 계정 추가]**&#x200B;를 클릭합니다. 그런 다음 로그인하라는 메시지가 표시되면 [!DNL Microsoft Outlook] 로그인 정보를 입력하십시오. 이 단계를 반복하여 [!DNL Outlook] 계정을 여러 개 추가할 수 있습니다.

   >[!NOTE]
   >
   >[!DNL Outlook] 일정에 액세스하려면 [!DNL Workfront] 권한을 부여해야 합니다. 권한을 부여하면 [!DNL Workfront]이(가) 일정 데이터에 대한 액세스를 유지하고 [!DNL outlook] 프로필을 읽으며 [!DNL Microsoft] 일정을 읽고 업데이트할 수 있습니다.

1. 브라우저 창을 새로 고쳐 캘린더와 [!UICONTROL 캘린더 설정] 패널에서 [!DNL Outlook] 계정의 정보를 볼 수 있습니다.
1. 오른쪽 상단의 **[!UICONTROL 설정]** 톱니바퀴 아이콘을 다시 클릭하여 **[!UICONTROL 달력 설정]** 패널을 엽니다. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (선택 사항) 이전 단계에서 추가한 각 [!DNL Microsoft] 계정에서 **[!UICONTROL 보기]** 또는 **[!UICONTROL 동기화]**&#x200B;를 선택합니다.

   * **[!UICONTROL 보기]**: [!UICONTROL 홈 일정]에 [!DNL Microsoft] 일정 이벤트를 표시하는 읽기 전용 옵션입니다.
   * **[!UICONTROL 동기화]**: 이 옵션을 사용하면 [!DNL Microsoft]과(와) [!UICONTROL 홈] 캘린더 간에 양방향 동기화가 가능합니다. 즉, [!DNL Workfront] [!UICONTROL 홈 캘린더] 항목을 [!DNL Microsoft] 캘린더로 내보내고 [!DNL Microsoft] 캘린더 항목을 실시간으로 Workfront [!UICONTROL 홈 캘린더](으)로 가져옵니다.

     ![](assets/view-sync-checkboxes-qs.png)

1. (선택 사항) [!DNL Workfront] 계정 또는 통합 계정에서 [!UICONTROL 홈 캘린더]에 표시할 관련 캘린더(예: 유급휴가, 생일 또는 휴일 캘린더)를 선택한 다음 브라우저의 [!UICONTROL 새로 고침] 또는 [!UICONTROL 다시 로드] 단추를 클릭하여 변경 사항을 확인합니다.

1. (선택 사항) **[!UICONTROL 주 시작 일자]** 아래의 **[!UICONTROL 일반]** 섹션에서 홈 캘린더에 표시할 첫 번째 요일로 선택합니다.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 다음 옵션을 구성합니다.

   * **[!UICONTROL 내 근무일]:** 근무일을 선택합니다.
   * **[!UICONTROL 내 평소 시작 시간]:** 업무일 시작 시간을 선택합니다.
   * **[!UICONTROL 내 일반 종료 시간]:** 근무일을 종료하는 시간을 선택합니다.

   [!DNL Workfront]은(는) 이 세 가지 설정을 사용하여 한 주의 작업 시간을 계산합니다. 이 숫자는 [!UICONTROL 할당] 막대에 영향을 미치므로 사용 가능한 작업 시간에 대한 작업 부하를 추적하는 데 도움이 됩니다. 자세한 내용은 문서 [[!UICONTROL 홈 일정] 보기](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)에서 [[!UICONTROL 할당] 막대](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time)를 참조하십시오.

1. **[!UICONTROL 달력 설정]** 영역 바깥쪽을 클릭하여 닫습니다.

   [!DNL Workfront]이(가) 변경 내용을 자동으로 저장합니다.

[!UICONTROL 일정] 보기를 사용하여 작업 할당 및 통합 일정 이벤트를 관리하는 방법에 대한 자세한 내용은 [[!UICONTROL 홈 일정 사용] 보기](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md)를 참조하십시오.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
