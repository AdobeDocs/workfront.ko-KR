---
content-type: reference
navigation-topic: notifications
title: '알림: 나에게 할당된 작업 정보'
description: 다음 알림은 사용자에게 할당된 작업 항목에서 발생하는 활동에 대해 알려줍니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 1%

---

# 알림: 나에게 할당된 작업 정보

다음 알림은 사용자에게 할당된 작업 항목에서 발생하는 활동에 대해 알려줍니다.

받는 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

[이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md)도 참조하세요.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th> <p>포함된 필드 </p> <p> *일별 다이제스트 필드만</p> </th> 
   <th>기본 상태</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>내 팀에 할당된 작업의 전임 작업이 완료되었습니다</strong> </p> <p>할당된 팀은 작업 중 하나의 전임 작업이 완료되면 이메일 알림을 받습니다. </p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>완료: &lt;작업 이름&gt;</em>입니다.</p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>전임 작업 이름<br>전임 작업 프로젝트<br>전임 작업 참조 번호<br>전임 작업을 완료한 사용자의 이름<br>전임 작업의 상태<br>전임 작업이 완료된 날짜 및 시간<br>전임 작업의 이전 상태<br><strong>자세한 정보 보기</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 전임 작업의 총 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜 </p> </td> 
   <td><strong>일별</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>내 작업 중 하나의 전임 작업이 완료되었습니다.</strong> </p> <p>작업 할당자는 작업 중 하나의 전임 작업이 완료되면 이메일 알림을 받습니다. </p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]입니다. &lt;작업 이름&gt;</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>전임 작업 이름<br>전임 작업 프로젝트<br>전임 작업 참조 번호<br>전임 작업을 완료한 사용자의 이름<br>전임 작업의 상태<br>전임 작업이 완료된 날짜 및 시간<br>전임 작업의 이전 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 전임 작업의 총 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜 </p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>내가 완료한 작업이 승인 또는 거부되었습니다.</strong> </p> <p>작업이 승인 또는 거부되면 작업 할당자는 이메일 알림을 받습니다.</p> <p>알림은 프로젝트 상태가 현재인 경우에만 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]: &lt;프로젝트 이름&gt;</em>의 &lt;작업 이름&gt;입니다.</p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>승인을 승인한 사용자 이름<br>새 작업 상태<br>작업을 승인하거나 거부한 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*작업을 승인하거나 거부한 총 작업 수<br>*작업 이름<br>*작업을 승인하거나 거부한 사용자 이름<br>*승인 결정([!UICONTROL 승인]/[!UICONTROL 거부]<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>나에게 할당된 작업이 완료되었습니다</strong> </p> <p>작업이 완료되면 작업 할당자는 전자 메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]: &lt;프로젝트 이름&gt;</em>의 &lt;작업 이름&gt;입니다.</p> <p> <p>참고: 작업이 [!UICONTROL Complete]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "Complete"가 표시됩니다.</p> </p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>작업을 완료한 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>내 팀에 할당된 작업의 모든 전임 작업이 완료되었습니다</strong> </p> <p>할당된 팀은 작업 중 하나의 전임 작업이 완료된 것으로 표시되면 이메일 알림을 받습니다.</p> <p>검토 또는 요청자 라이선스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>작업 완료: &lt;이름&gt;</em>입니다.</p> <p> 일별 요약 알림의 제목은 <em> 사용자에게 할당된 작업 요약입니다. &lt;일별 요약 날짜&gt; </em></p> </td> 
   <td> 작업 이름<br>작업 프로젝트<br>작업 참조 번호<br>전임 작업을 완료한 사용자의 이름<br>전임 작업의 상태<br>전임 작업이 완료된 날짜 및 시간<br>전임 작업의 이전 상태<br><strong>자세한 정보 보기</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜 </td>
   <td><strong>즉시</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>내 작업의 전임 작업이 모두 완료되었습니다</strong> </p> <p>작업 할당자는 완료된 각 전임 작업에 대한 이메일 알림을 받습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]입니다. &lt;작업 이름&gt;</em><br></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 작업 이름<br>작업 프로젝트<br>작업 참조 번호<br>전임 작업을 완료한 사용자의 이름<br>전임 작업의 상태<br>전임 작업이 완료된 날짜 및 시간<br>전임 작업의 이전 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜 </td> 
   <td><strong>즉시</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>내가 해결한 문제가 승인 또는 거부됨</strong> </p> <p>문제의 할당자는 승인 결정(승인 또는 거부)이 내려지면 이메일 알림을 받습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>승인 보류 중인 문제: &lt;계획된 시작 일자&gt; &lt;문제 참조 번호&gt; - &lt;프로젝트 이름&gt;</em>의 &lt;문제 이름&gt;입니다.</p> <p> 일별 요약 알림의 제목은 <em> 사용자에게 할당된 작업 요약입니다. &lt;일별 요약 날짜&gt; </em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 승인하거나 거부한 사용자 이름<br>승인 결정(승인됨 또는 거부됨)<br>문제 상태<br>승인을 요청한 사용자 이름<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*문제 승인 또는 거부된 총 수<br>*문제 이름<br>*문제를 승인하거나 거부한 사용자 이름<br>*승인 결정(승인됨 또는 거부됨)<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>내게 할당된 문제가 완료되었습니다</strong> </p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>완료: &lt;프로젝트 이름&gt;</em>의 &lt;문제 이름&gt;입니다.</p> <p><em> 일별 요약 알림의 제목은 &lt;일별 요약 일자&gt; </em>입니다. </p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 완료한 사용자의 이름<br>새 문제 상태<br>문제가 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제를 완료한 사용자의 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서를 업로드하거나 내가 할당된 요청에 따라 변경합니다</strong> </p> <p>문제 피할당자는 추가한 문제에 대한 문서가 업로드되거나 문서 세부 정보가 변경되면 이메일 알림을 받습니다.</p> <p>문제를 트리거한 사용자가 문제 피할당자인 경우 이메일 알림이 전송되지 않습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 프로젝트가 도움말 요청 큐(<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a>에 설명된 대로)로 설정된 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>문서가 &lt;요청 이름&gt;</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>요청 이름<br>프로젝트 이름(요청 큐 이름)<br>문서 참조 번호 <br>문서를 업로드한 사용자의 이름<br>문서 이름 <br>날짜에 추가됨<br>문서 세부 정보(형식, 크기, 버전 번호)<br>문서 축소판<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL 다운로드]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*업로드되거나 변경된 총 문서 수<br>*문서 이름<br>*개체 이름<br>*문서를 업로드한 사용자의 이름<br>*일별 다이제스트</p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>나에게 할당된 작업의 기한 변경</strong> </p> <p>계획된 완료 일자를 변경한 사용자가 작업 할당자도 아닌 경우 작업 할당자는 작업의 [!UICONTROL 계획된 완료 일자]가 변경될 때 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Planning] 이외의 다른 상태인 경우에만 알림이 전송됩니다.</p> <p>개인 작업과 관련하여 알림이 전송되지 않습니다.</p> <p> 검토 또는 요청자 라이선스가 있는 사용자가 알림을 받지 않습니다. </p> <p> 인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 기한이 변경되었습니다.]</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>새 기한([!UICONTROL 계획된 완료 일자])<br>기한이 변경된 날짜와 시간<br>기한이 변경된 사용자 이름<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*기한이 변경된 총 작업 수<br>*작업 이름<br>*새 계획된 완료 일자<br>*기한이 변경된 사용자 이름<br>*일일 다이제스트 날짜 </td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 할당된 문제의 기한이 변경되었습니다.</strong> </p> <p>[!UICONTROL 계획된 완료 일자]를 변경한 사용자가 피할당자가 아닌 경우 문제 피할당자는 [!UICONTROL 계획된 완료 일자]가 변경될 때 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Planning] 이외의 다른 상태인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 기한이 변경되었습니다]</em></p> <p> </p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>새 기한([!UICONTROL 계획된 완료 일자])<br>기한이 변경된 날짜와 시간<br>기한이 변경된 사용자 이름<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*기한이 변경된 총 문제 수<br>*문제 이름<br>*새 [!UICONTROL 계획된 완료 일자]<br>*기한이 변경된 사용자 이름<br>*일별 다이제스트 날짜<br></p> </td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>내가 할당된 작업의 상태 변경</strong> <p>작업 할당자는 상태를 변경한 사용자가 할당자도 아닌 경우 작업 상태가 변경되면 이메일 알림을 받습니다.</p> <p>참고: 이 알림은 작업 상태가 완료로 변경될 때 전송되지 않습니다. 완료된 작업에는 별도의 알림이 사용됩니다. <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">내가 할당된 작업이 완료되었습니다</a>, 위의 내용을 참조하십시오.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;작업 이름&gt; 보낸 사람 &lt;프로젝트 이름&gt;: &lt;새 상태&gt;</em></p> <p> </p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>상태를 변경한 사용자 이름<br>새 상태<br>상태가 변경된 날짜 및 시간<br>미리 보기 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*상태가 변경된 총 작업 수<br>*작업 이름<br>*이전 작업 상태<br>*새 작업 상태<br>*상태를 변경한 사용자 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 작업 항목 중 하나의 상태 변경</strong> </p> <p>직접 상태를 변경하지 않는 한, 할당된 문제에 대한 상태가 변경되면 이메일 알림을 받습니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;문제 이름&gt; 보낸 사람: &lt;프로젝트 이름&gt; &lt;새 상태&gt;</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Work Assigned or You] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>상태를 변경한 사용자 이름<br>새 상태<br>이전 문제 상태<br><strong>자세한 정보</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*상태가 변경된 총 문제 수<br>*작업 이름<br>*이전 문제 상태<br>*새 문제 상태<br>*상태를 변경한 사용자 이름<br>*일별 다이제스트 날짜<br> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
 </tbody> 
</table>
