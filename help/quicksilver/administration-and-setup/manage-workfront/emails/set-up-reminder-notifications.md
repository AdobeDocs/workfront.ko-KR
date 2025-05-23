---
title: 미리 알림 설정
description: 미리 알림 은 지정된 기준에 따라 사용자에게 전송되는 이메일을 생성합니다. 미리 알림 은 사용자에게 작업, 문제, 프로젝트 또는 타임시트에 대해 수행해야 하는 작업을 알려줍니다.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 2%

---

# 미리 알림 설정

<!-- Audited: 1/2024 -->

Workfront 관리자는 사용자를 위한 미리 알림을 만들고 사용자가 특별히 주의를 기울여야 하는 오브젝트와 연결할 수 있습니다.

미리 알림 은 지정된 기준에 따라 사용자에게 전송되는 이메일을 생성합니다. 미리 알림 은 사용자에게 작업, 문제, 프로젝트 또는 타임시트에 대해 수행해야 하는 작업을 알려줍니다.

미리 알림을 만든 후 사용자는 이를 프로젝트, 작업, 문제 및 타임시트와 같은 작업 항목에 수동으로 연결할 수 있습니다. 자세한 내용은 [미리 알림을 개체에 첨부](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md)를 참조하십시오.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준 </p>
 <p>또는</p> 
<p>현재: 플랜</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>미리 알림에 대한 관리 액세스 권한이 있는 플래너 이상</p></td> 
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 미리 알림 이메일 사용자 지정

미리 알림 이메일에서 제목, 본문 및 HTML을 사용자 지정할 수 있습니다.

또는 미리 알림에 포함된 기본 이메일을 사용할 수 있습니다. 기본 이메일은 알림을 트리거한 이벤트를 포함하여 미리 알림 이름을 이메일 제목과 이메일 본문의 개체 이름으로 사용합니다.

미리 알림 이메일을 사용자 지정하려면 이메일 템플릿을 만들고 미리 알림 첨부해야 합니다.

전자 메일 서식 파일을 만드는 방법에 대한 자세한 내용은 [전자 메일 서식 파일 구성](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md)을 참조하십시오.

## 미리 알림 만들기

{{step-1-to-setup}}

1. **전자 메일** > **알림** > **미리 알림**&#x200B;을 클릭합니다.

   ![미리 알림 탭](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. **새 미리 알림**&#x200B;을 클릭합니다.

1. 드롭다운 목록에서 미리 알림과 연결할 객체 유형을 클릭합니다.

   예를 들어 미리 알림을 타임시트에 첨부하려면 **타임시트**&#x200B;를 클릭하세요.

1. 표시되는 **새 미리 알림** 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">미리 알림 이름</td> 
      <td>미리 알림의 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">대상 기간</td> 
      <td> <p><strong>시간</strong> 필드에 날짜 전후의 시간, 근무일, 일(달력 일), 주 또는 개월 수를 지정합니다.</p> <p><b>참고</b>:  
        <ul> 
         <li> <p>미리 알림은 지정된 날짜 및 모든 기준이 충족되면 24시간 후에 시작됩니다.</p> </li> 
         <li> <p>프로젝트, 작업 및 문제에 대한 미리 알림은 매일 밤 자정(미국 산지 표준시)에 트리거됩니다. 해당 날짜부터 미리 알림을 받을 자격이 있는 모든 오브젝트는 해당 시간 직후 지정된 사용자에게 알림을 트리거합니다.</p> </li> 
         <li> <p>타임시트에 대한 미리 알림은 시간대 및 타임시트의 종료 날짜, 시작 날짜 또는 마지막 업데이트 날짜를 기준으로 지정된 시간에 전송됩니다.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">타이밍</td> 
      <td> <p>미리 알림을 예약하도록 트리거하는 이벤트를 선택합니다.</p> <p>미리 알림이 프로젝트, 작업 또는 문제를 위한 경우 사용 가능한 옵션은 완료 일자 또는 시작 일자와 관련이 있습니다. 미리 알림은 프로젝트, 작업 및 문제의 완료 및 시작 날짜에 대한 타임스탬프를 고려합니다.</p>

   <p>미리 알림이 타임시트를 대상으로 하는 경우 사용 가능한 옵션은 종료 날짜, 시작 날짜 또는 마지막 업데이트 날짜와 관련이 있습니다. 타임시트에 대한 미리 알림은 타임시트 종료, 시작 및 마지막 업데이트 날짜의 타임스탬프를 고려합니다. 타임시트는 시작 날짜의 자정(오전 12:00)에 시작되고 종료 날짜의 자정 직전(오후 11:59)에 종료됩니다.</p>

   <p><b>메모</b></p>
      <p>타임시트 미리 알림은 24시간마다 한 번만 배포됩니다.</p> <p>24시간 내에 여러 미리 알림을 설정하면 Workfront에서는 해당 알림에 포함된 모든 미리 알림과 함께 하나의 알림 이메일을 보냅니다.</p>
      <p>예를 들어 기한이 되기 10시간 전, 2시간 전, 1시간 전을 트리거하도록 세 개의 미리 알림을 구성하는 경우, 세 개의 미리 알림이 같은 날 동안 발생할 경우 모두 동일한 알림에 결합됩니다.</p> <p>그러나 미리 알림을 기한 이전 26시간 동안 설정하고 다른 알림을 기한 이전 1시간 동안 설정하면 사용자는 두 개의 개별 알림을 받게 됩니다. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기준</td> 
      <td> <p>미리 알림을 예약하려면 조건을 선택하십시오. 기준 선택을 충족하지 않으면 미리 알림이 예약되지 않습니다.</p> <p>4단계에서 선택한 객체 유형에 따라 다음 기준 옵션을 사용할 수 있습니다.</p> 
       <ul> 
        <li><strong>현재 프로젝트에서 미완료:</strong> <i>(작업 및 문제 미리 알림에 사용 가능)</i> 미리 알림과 연결된 개체 상태가 [완료]가 아니고 프로젝트 상태가 [현재]인 경우에만 미리 알림을 보내도록 예약되어 있습니다.</li> 
        <li><strong>현재 프로젝트의 모든 항목:</strong> <i>(작업 및 문제 미리 알림에 사용 가능)</i> 미리 알림이 개체 상태에 관계없이 전송되도록 예약되었으며 미리 알림과 연결된 프로젝트 상태가 현재인 경우에만 미리 알림이 전송됩니다.</li> 
        <li><strong>미완료 프로젝트:</strong> <i>(프로젝트 미리 알림에 사용 가능)</i> 프로젝트 상태가 완료가 아닌 경우 미리 알림이 전송되도록 예약되었습니다.</li> 
        <li><strong>모든 프로젝트:</strong> <i>(프로젝트 미리 알림에 사용 가능)</i> 미리 알림이 프로젝트 상태에 관계없이 전송되도록 예약되었습니다.</li> 
        <li><strong>타임시트 열기:</strong> <i>(타임시트 미리 알림에 사용 가능)</i> 타임시트 상태가 [열림]일 때 미리 알림을 보내도록 예약되어 있습니다.</li> 
        <li><strong>제출된 타임시트:</strong> <i>(타임시트 미리 알림에 사용 가능)</i> 타임시트 상태가 제출되면 미리 알림이 전송되도록 예약되었습니다.</li> 
        <li><strong>타임시트 열기 또는 주당 40시간 미만:</strong> <i>(타임시트 미리 알림에 사용 가능)</i> 타임시트 상태가 [열림]이거나 타임시트에 기록된 시간이 40시간 미만인 경우 미리 알림이 전송되도록 예약되어 있습니다.</li> 
        <li><strong>전자 메일 서식 파일:</strong> 드롭다운에서 미리 알림에 첨부할 전자 메일 서식 파일을 선택합니다.<br>전자 메일 서식 파일을 만드는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">전자 메일 서식 파일 구성</a>을 참조하세요.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수신자</td> 
      <td><p>미리 알림이 사용되는 객체에 따라 알림을 받을 다음 사용자 유형 중에서 선택합니다.</p>
      <ul>
      <li>할당 대상</li>
      <li>작성자</li>
      <li>프로젝트 팀(프로젝트 팀의 모든 사용자가 미리 알림을 받음)</li>
      <li>종속 작업 할당자(종속 작업에 할당된 사용자가 미리 알림을 받음)</li>
      <li>프로젝트 소유자</li>
      <li>할당 대상(작업 또는 문제에 할당된 사용자가 미리 알림을 받음)</li>
      <li>타임시트 소유자</li>
      <li>타임시트 승인자</li>
      <li>타임시트 소유자의 관리자</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
1. [개체에 미리 알림 첨부](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md)에 설명된 대로 작업 항목에 미리 알림을 첨부합니다.

## 미리 알림 수신

미리 알림이 첨부된 항목에 조건이 충족되면 미리 알림에 정의된 사용자에게 이메일 알림이 트리거됩니다.

미리 알림 수신에 대한 자세한 내용은 [Adobe Workfront 알림](../../../workfront-basics/using-notifications/wf-notifications.md)의 [미리 알림](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) 섹션을 참조하십시오.

## 미리 알림 게재 테스트

미리 알림은 매일 밤 자정(산지 표준시)에 트리거됩니다. 미리 알림을 받을 자격이 있는 모든 오브젝트는 그 직후 지정된 사용자에게 알림을 트리거합니다.

미리 알림이 수동으로 트리거되도록 하려면 미리 알림에 대한 조건이 먼저 충족되어야 합니다.\
예를 들어 미리 알림이 프로젝트의 계획된 완료 일자 1시간 후에 트리거되도록 설정된 경우 미리 알림이 설정된 시간과 지금 사이에 해당 시간이 경과해야 합니다. 미리 알림이 활성화되기 전에 계획된 완료 일자가 경과한 프로젝트는 알림을 트리거하지 않습니다.

미리 알림이 수동으로 트리거되도록 하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. Workfront 왼쪽 하단의 **시스템** > **진단**&#x200B;을 클릭합니다.

1. **미리 알림 보내기**&#x200B;를 클릭하고 화면 상단에서 알림이 전송될 때까지 기다립니다.

   미리 알림에 지정된 사용자가 이메일을 받습니다.

![미리 알림 테스트](assets/reminder-test.png)
