---
title: 미리 알림 설정
description: 미리 알림 설정
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 1%

---

# 미리 알림 설정

미리 알림 은 지정된 기준에 따라 수신자에게 이메일을 보냅니다. 미리 알림 알림에 대한 계획자 액세스 레벨과 관리 액세스 권한이 있는 Adobe Workfront 관리자 또는 사용자는 프로젝트, 작업, 문제, 작업표와 같은 작업 항목에 미리 알림 알림을 수동으로 연관시킬 수 있습니다.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>미리 알림 알림에 대한 관리자 액세스 권한이 있는 계획자 이상</p> <p>계획 사용자 관리 액세스 권한을 제공하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 미리 알림 이메일 사용자 지정

사용자 정의 이메일 제목과 본문이 포함된 사용자 정의 이메일을 사용하여 미리 알림 알림을 사용자 지정할 수 있습니다. 이메일 본문에 사용자 지정 HTML을 포함할 수 있습니다.

또는 미리 알림 알림에 포함된 기본 이메일을 사용할 수 있습니다. 기본 이메일은 미리 알림 이름을 전자 메일 제어로 사용하고 알림을 트리거한 이벤트를 포함하여 전자 메일 본문의 개체 이름을 사용합니다.

미리 알림 이메일을 사용자 지정하려면 이메일 템플릿을 만들어 미리 알림 알림에 첨부해야 합니다.

이메일 템플릿을 만드는 방법에 대한 자세한 내용은 [이메일 템플릿 구성](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## 미리 알림 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **이메일** > **알림 을 참조하십시오**.

1. 을(를) 클릭합니다. **미리 알림 알림** 탭을 클릭한 다음 **새 미리 알림 알림**.

1. 드롭다운 목록에서 미리 알림 알림과 연결할 객체 유형을 클릭합니다.

   예를 들어 작업표에 미리 알림 알림을 첨부하려면 **작업표**.

1. 에서 **새 미리 알림 알림** 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">미리 알림 이름</td> 
      <td>미리 알림 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">적합한 기간</td> 
      <td> <p>시간, 작업 일, 일(달력 일), 주 또는 월의 날짜 이전 또는 이후의 월을 지정합니다. <strong>타이밍</strong> 필드.</p> <p><b>메모</b>:  
        <ul> 
         <li> <p>미리 알림 은 지정된 날짜 이후 24시간 후에 시작되고 모든 기준이 충족되면 시작됩니다.</p> </li> 
         <li> <p>프로젝트, 작업 및 문제에 대한 미리 알림 알림은 매일 밤 자정, 미국 산지 타임에 트리거됩니다. 해당 날짜부터 미리 알림 알림을 받을 수 있는 모든 개체는 해당 시간 직후 지정된 사용자에게 알림을 트리거합니다.</p> </li> 
         <li> <p>작업표에 대한 미리 알림 알림은 표준 시간대와 작업표의 종료 날짜, 시작 날짜 또는 마지막 업데이트 날짜에 따라 지정된 시간에 전송됩니다.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간</td> 
      <td> <p>미리 알림 알림을 트리거하여 예약할 이벤트를 선택합니다.</p> <p>미리 알림 알림이 프로젝트, 작업 또는 문제에 대한 경우 사용 가능한 옵션은 완료 날짜 또는 시작 날짜와 관련되어 있습니다. 미리 알림 알림은 프로젝트, 작업 및 문제의 완료 및 시작 날짜에 대한 타임스탬프를 고려합니다.</p> <p>미리 알림 메시지가 작업표에 적용되는 경우 사용 가능한 옵션은 종료 날짜, 시작 날짜 또는 마지막 업데이트 날짜와 관련되어 있습니다. 작업표의 미리 알림 알림은 작업표 종료, 시작 및 마지막 업데이트 날짜의 타임스탬프를 고려합니다. 작업표는 시작 날짜의 자정(오전 12:00)에 시작하여 종료 날짜(오후 11:59)의 자정 직전에 종료됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기준</td> 
      <td> <p>미리 알림 일정을 잡을 기준을 선택합니다. 기준 선택이 충족되지 않으면 미리 알림 알림이 예약되지 않습니다.</p> <p>4단계에서 선택한 객체 유형에 따라 다음 기준 옵션을 사용할 수 있습니다.</p> 
       <ul> 
        <li><strong>현재 프로젝트의 불완전함:</strong> (작업 및 문제 미리 알림에 사용 가능) 미리 알림 알림이 연결된 객체 상태가 완전하지 않고 프로젝트 상태가 현재인 경우에만 미리 알림 메시지가 전송되도록 예약됩니다.</li> 
        <li><strong>현재 프로젝트의 모든 항목:</strong>(작업 및 문제 미리 알림에 사용 가능) 미리 알림 알림은 객체 상태와 관계없이, 미리 알림 알림과 연관된 프로젝트 상태가 [현재]인 경우에만 전송되도록 예약됩니다.</li> 
        <li><strong>불완전한 프로젝트:</strong> (프로젝트 미리 알림에 사용 가능) 프로젝트 상태가 완료가 아닌 경우 미리 알림 알림이 전송되도록 예약됩니다.</li> 
        <li><strong>전체 프로젝트:</strong> (프로젝트 미리 알림에 사용 가능) 프로젝트 상태가 완료됨일 때 미리 알림 알림이 전송되도록 예약됩니다.</li> 
        <li><strong>작업표 열기:</strong> (작업표 미리 알림에 사용 가능) 작업표 상태가 [열림]일 때 미리 알림 메시지를 보내도록 예약합니다.</li> 
        <li><strong>제출된 작업표:</strong> (작업표 미리 알림에 사용 가능) 작업표 상태가 제출되면 미리 알림 알림을 전송하도록 예약되어 있습니다.</li> 
        <li><strong>작업표 열기 또는 주당 40시간 미만:</strong> (작업표 미리 알림에 사용 가능) 작업표 상태가 [열림]이거나 작업표에 기록되는 시간이 40시간 미만인 경우 미리 알림 알림을 보내도록 예약합니다.</li> 
        <li><strong>이메일 템플릿:</strong> 드롭다운에서 미리 알림에 첨부할 이메일 템플릿을 선택합니다.<br>이메일 템플릿을 작성하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">이메일 템플릿 구성</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수신자</td> 
      <td>알림을 받을 사용자 유형을 선택합니다. 소유자, 승인자 또는 할당자와 같은 다양한 객체 이해 관계자에서 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
1. 에 설명된 대로 작업 항목에 미리 알림 첨부 [개체에 미리 알림 첨부](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## 미리 알림 받기

미리 알림 알림이 첨부된 항목에 조건이 충족되면 미리 알림 알림에 정의된 사용자에게 전자 메일 알림이 트리거됩니다.

미리 알림 수신에 대한 자세한 내용은 [미리 알림 알림](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) 섹션 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md).

## 미리 알림 게재 테스트

미리 알림 기능은 매일 밤 자정, 산지 타임에 트리거됩니다. 미리 알림 알림을 받을 수 있는 모든 개체는 해당 직후 지정된 사용자에게 알림을 트리거합니다.

미리 알림 알림을 수동으로 트리거하려면 미리 알림에 대한 조건을 먼저 충족해야 합니다.\
예를 들어, 리마인더를 프로젝트에 대한 계획 완료 날짜 이후 1시간 동안 트리거하도록 설정하면 리마인더를 설정할 때부터 지금 사이에 경과해야 합니다. 미리 알림을 활성화하기 전에 전달된 계획된 완료 날짜가 있는 모든 프로젝트는 알림을 트리거하지 않습니다.

미리 알림 알림을 수동으로 트리거하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **진단** Workfront의 왼쪽 아래 모서리에 있습니다.

1. 클릭 **미리 알림 보내기** 그리고 화면 상단에서 메시지가 전송되었다는 확인을 기다립니다.

   미리 알림 알림에 지정된 사용자는 이메일을 받습니다.
