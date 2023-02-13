---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 자동 미리 알림 설정
description: 자동 미리 알림 설정
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# 자동 미리 알림 설정

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront 관리자는 모든 작업 또는 문제가 기한, 지연 또는 계획된 완료 날짜 근처에 있을 때 이메일 알림을 트리거하도록 자동 미리 알림을 설정할 수 있습니다. 이러한 설정을 구성하면 자동 미리 알림을 비활성화할 수 없습니다.

지연 알림의 경우 작업이나 문제가 완료될 때까지 매일 밤 이메일이 전송됩니다.

자동 미리 알림은 다음 중 하나 이상에 보낼 수 있습니다.

* 작업 또는 문제에 지정된 사용자
* 사용자의 즉시 관리자
* 바로 아래 관리자의 관리자

>[!NOTE]
>
>자동 미리 알림으로 트리거되는 전자 메일의 콘텐츠 또는 제목 줄은 변경할 수 없습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

## 자동 미리 알림 설정

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **이메일** >**자동 미리 알림**.

1. 에서 **에 늦게 알림 보내기** 영역에서 다음 옵션 중 하나를 선택합니다.

   <table>
    <tr>
        <td>지정된 대상 사용자</td>
        <td>작업 또는 문제에 할당된 사용자가 작업 항목이 늦은 경우 나중에 알림을 받으려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>사용자의 관리자</td>
        <td>사용자 관리자가 직접 보고서의 작업 항목이 늦은 것에 대한 지연 알림을 받도록 하려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>관리자의 관리자</td>
        <td>직접 보고서 사용자 중 한 명이 지각하는 작업 항목에 대한 지연 알림을 즉시 관리자 관리자가 받게 하려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>지정된 대상 사용자</td>
        <td>(에서 <b>미리 알림 보내기</b> 영역.) 사용자에게 할당된 작업 또는 문제에 대해 만기 날짜가 가까워지는 작업 항목에 대한 알림을 받으려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
</table>

1. 작업 항목의 만기 일자 이전 또는 이후의 시간을 선택하여 자동 미리 알림을 보낼 시간을 선택합니다.

   시간은 작업 또는 문제의 계획 완료 날짜로부터 계산됩니다.

   작업 또는 문제의 계획 완료 날짜에 시간을 추가할 분, 시간, 일, 주 또는 개월 수를 지정합니다. 선택 **경과된 시간(분)**, **경과시간**, **경과된 일 수**, 또는 **경과된 주** 일정에 표시된 대로 주말, 휴일 및 비근무 시간을 포함하는 시간을 추가하려면

   예를 들어, 금요일에 작업이 지정되고 기간이 3일 경과된 경우, 작업 완료 날짜는 월요일로 설정됩니다(토요일과 일요일이 주말로 가정). 작업에 3일(경과되지 않음)의 기간이 있는 경우 작업 완료 날짜가 수요일로 설정됩니다.

   ![](assets/time-increments-for-automatic-reminder.png)

1. **저장**&#x200B;을 클릭합니다.

## 자동 미리 알림 받기

자동 미리 알림 알림에서 지정된 엔티티인 경우 지정된 기한이 충족되면 이메일을 받게 됩니다. 지연 알림의 경우 작업이나 문제가 완료될 때까지 매일 밤 이메일이 전송됩니다.

특정 종속성 유형이 있는 작업은 기한이 지났더라도 지정된 시작 날짜 이후에 배달될 수 있습니다. 예를 들어 작업에 Finish-Start(fs) 종속성이 있는 선행 작업이 있는 경우 선행 작업이 완료될 때까지 작업을 시작할 수 없으므로 지정된 시작 날짜가 지났더라도 전자 메일에 포함되지 않습니다.

자동 미리 알림 전자 메일 수신에 대한 자세한 내용은 [자동 미리 알림](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 섹션 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md).

## 자동 미리 알림 보내기

자동 미리 알림은 Workfront 관리자가 선택한 시간이 충족되는 즉시 전송됩니다.

자동 미리 알림 이메일 전송을 수동으로 트리거하려면 진단을 사용하여 그렇게 할 수 있습니다. Workfront에서 진단 액세스 및 사용에 대한 자세한 내용은 [진단 기능을 사용하여 자동화된 프로세스를 트리거합니다](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
