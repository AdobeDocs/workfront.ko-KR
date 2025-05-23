---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 자동 알림 설정
description: 모든 작업 또는 문제가 기한, 지연 또는 계획된 완료 일자에 근접한 경우 이메일 알림을 트리거하는 자동 미리 알림을 설정할 수 있습니다.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 3%

---

# 자동 알림 설정

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront 관리자는 모든 작업 또는 문제가 기한이 지났거나, 기한이 늦었거나, 계획된 완료 일자 근처에 있을 때 이메일 알림을 트리거하기 위한 자동 미리 알림을 설정할 수 있습니다. 이러한 설정을 구성한 후에는 사용자가 자동 미리 알림을 비활성화할 수 없습니다.

지연 알림의 경우 작업 또는 문제가 완료될 때까지 이메일이 매일 밤 전송됩니다.

자동 미리 알림은 다음 중 하나 이상의 사용자에게 보낼 수 있습니다.

* 작업 또는 문제에 할당된 사용자
* 사용자의 직속 관리자
* 직속 관리자의 관리자

>[!NOTE]
>
>자동 미리 알림에 의해 트리거된 이메일의 내용 또는 제목란은 변경할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
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

+++

## 자동 알림 설정

{{step-1-to-setup}}

1. **전자 메일** > **자동 미리 알림**&#x200B;을 클릭합니다.

1. **지연 알림 보내기** 영역에서 다음 옵션 중 하나를 선택하십시오.

   <table>
    <tr>
        <td>"할당 대상" 사용자</td>
        <td>작업 또는 문제에 할당된 사용자가 작업 항목에 대한 지연 알림을 받도록 하려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>사용자의 관리자</td>
        <td>사용자의 관리자가 부하직원의 작업 항목이 지연되는 것에 대해 지연 통지를 받도록 하려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>관리자의 관리자</td>
        <td>직속 관리자의 관리자가 직접 보고서의 사용자 중 한 명의 작업 항목에 대한 지연 알림을 받으려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
    <tr>
        <td>"할당 대상" 사용자</td>
        <td>(<b>기한 알림 보내기</b> 영역에서) 작업 또는 문제에 할당된 사용자가 기한이 임박한 작업 항목에 대한 알림을 받으려면 이 옵션을 선택합니다.</td>
        <td></td>
    </tr>
   </table>

1. 작업 항목의 기한 이전 또는 이후의 시간을 선택하여 자동 미리 알림을 보낼 시간을 선택합니다.

   시간은 작업 또는 문제의 계획된 완료 일자부터 계산됩니다.

   작업 또는 문제의 계획된 완료 일자에 시간을 추가하려면 분, 시간, 일, 주 또는 개월 수를 지정합니다. **경과 시간**, **경과 시간**, **경과 일수** 또는 **경과 주**&#x200B;를 선택하여 일정에 지정된 주말, 휴일 및 휴무 시간을 포함하는 시간을 추가합니다.

   예를 들어 작업이 금요일에 할당되고 기간이 3일인 경우, 작업 완료 날짜가 월요일로 설정됩니다(토요일과 일요일이 주말이라고 가정). 작업의 기간이 3일(경과되지 않음)인 경우 작업 완료 날짜가 수요일로 설정됩니다.

   ![시간 증가](assets/time-increments-for-automatic-reminder.png)

1. **저장**&#x200B;을 클릭합니다.

## 자동 미리 알림 수신

자동 미리 알림 의 지정된 엔티티인 경우 지정된 기한이 충족되면 이메일을 받게 됩니다. 지연 알림의 경우 작업 또는 문제가 완료될 때까지 이메일이 매일 밤 전송됩니다.

기한이 지났더라도 특정 종속성 유형이 있는 작업은 지정된 시작 날짜 이후에 게재될 수 있습니다. 예를 들어 작업에 fs(완료-시작) 종속성이 있는 전임 작업이 있는 경우 전임 작업이 완료될 때까지 작업을 시작할 수 없으므로 지정된 시작 날짜가 지나도 작업이 이메일에 포함되지 않습니다.

자동 미리 알림 전자 메일 수신에 대한 자세한 내용은 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md)의 [자동 미리 알림](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 섹션을 참조하십시오.

## 자동 미리 알림 보내기

Workfront 관리자가 선택한 시간이 충족되는 즉시 자동 미리 알림이 전송됩니다.

자동 미리 알림 이메일 전송을 수동으로 트리거하려면 진단을 사용하여 트리거할 수 있습니다. Workfront의 진단에 액세스하고 사용하는 방법에 대한 자세한 내용은 [진단을 사용하여 자동화된 프로세스를 트리거합니다](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)를 참조하십시오.
