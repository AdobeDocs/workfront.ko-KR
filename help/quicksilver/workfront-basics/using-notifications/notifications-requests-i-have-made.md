---
content-type: reference
navigation-topic: notifications
title: '알림: 내가 한 요청'
description: 다음 알림은 Adobe Workfront에서 수행한 요청에 대해 알려줍니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 7%

---

# 알림: 내가 한 요청

다음 알림은에서 수행한 요청에 대해 알려 줍니다. [!DNL Adobe Workfront].

수신하는 알림 구성에 대한 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

참조: [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>내가 한 요청</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 승인 요청이 완료되었습니다.</strong> </p> <p>문서에 대한 승인을 요청한 사용자는 문서 승인 요청이 완료되면 이메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다.<em> &lt;approver name=""&gt; 이(가) &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; 이 문서입니다.</em></p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> 문서 이름<br>승인자 이름 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 기본 담당자인 문제에 대한 문서가 변경되거나 업로드됨</strong> </p> <p>문서를 업로드하거나 변경한 사용자가 기본 연락처가 아닌 경우 문제의 기본 연락처는 문서가 문제에 대해 업로드되거나 변경될 때 이메일 알림을 받습니다.</p> <p>에 설명된 대로 프로젝트가 [!UICONTROL 도움말 요청 큐]로 설정된 경우에만 알림이 전송됩니다. <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL 요청 대기열 만들기]</a>).</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>문서가에 추가됨 &lt;issue name=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다. <em>요청 요약 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 문서가 업로드된 개체 이름<br>상위 개체 이름<br>문서 참조 번호<br>문서를 업로드한 사용자의 이름<br>문서 이름<br>추가된 날짜<br>문서 세부 정보(형식, 크기, 버전 번호)<br>문서 썸네일<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL 다운로드]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*업로드된 총 문서 수<br>*문서 이름<br>*상위 개체 이름<br>*문서를 추가한 사용자의 이름<br>*일별 요약 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 업로드 요청이 이행되었습니다.</strong> </p> <p>문서 업로드 요청이 이행되면 문서 요청자는 이메일 알림을 수신합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문서 요청 위치] &lt;user name=""&gt; 이행됨</em></p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> <p>문서를 업로드한 사용자의 이름<br>문서가 업로드된 개체 이름<br>문서 이름<br><br></p> </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 다른 사람에게 할당한 개인 작업이 완료되었습니다.</strong> </p> <p>임시 작업이 완료되면 다른 사용자에게 임시 작업을 할당한 사용자에게 알림이 전송됩니다. </p> <p>임시 작업에 대한 자세한 내용은 <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">[!UICONTROL Home] 영역에서 작업 항목 만들기</a>.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>작업 완료: &lt;task name=""&gt;</em></p> <p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 작업 이름<br>기본 프로젝트 이름(개인 작업을 받은 사용자의 개인 프로젝트)<br>작업 참조 번호<br>작업 소유자 이름<br>새 작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br><br><br></td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 기본 담당자인 문제가 완료되었습니다.</strong> </p> <p>문제가 완료되면 문제에 대한 기본 담당자가 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제 완료]: &lt;issue name=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청 요약 &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 완료한 사용자의 이름<br>새 상태<br>문제가 완료된 날짜 및 시간<br>이전 문제 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제를 완료한 사용자의 이름<br>*일별 요약 날짜 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트에 문제를 추가합니다.</strong> </p> <p>문제에 대한 기본 담당자는 프로젝트에서 문제를 추가할 때 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제 제출됨]: &lt;issue name=""&gt; 날짜 &lt;project name=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청 요약 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>사용자 이름<br>문제 이름<br>일자 입력됨<br>문제 우선 순위<br>문제 상태<br>할당 대상 이름<br>기본 담당자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문제 수<br>*문제 이름<br>*일별 요약 날짜 </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>요청을 제출합니다(확인).</strong> </p> <p>문제에 대한 기본 담당자는 문제를 제출하면 이메일 알림을 받습니다.</p> <p>알림은 프로젝트 상태가 [!UICONTROL Current]이고 프로젝트가 [!UICONTROL 도움말 요청 큐]로 설정된 경우에만 전송됩니다( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL 요청 대기열 만들기]</a>).</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 요청 제출됨]: &lt;request name=""&gt; 날짜 &lt;project request="" queue="" name=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청 요약 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>프로젝트 이름(요청 대기열 이름)<br>Portfolio 이름<br>문제 참조 번호<br>문제 이름<br>일자 입력됨<br>문제 우선 순위<br>문제 상태<br>할당 대상 이름<br>기본 담당자<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*제출된 총 요청 수<br>*요청 이름<br>*요청 우선 순위<br>*일별 요약 날짜</p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 요청이 마감되었습니다(확인).</strong> </p> <p>요청이 닫히면 문제의 기본 담당자가 이메일 알림을 받습니다.</p> <p>에 설명된 대로 프로젝트 상태가 현재이고 프로젝트가 [!UICONTROL 도움말 요청 큐]로 설정된 경우에만 알림이 전송됩니다 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>).</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 요청이 닫혔습니다]:"&lt;request name=""&gt;"</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청의 [!UICONTROL 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 요청 이름<br>프로젝트 이름<br>요청 참조 번호<br>요청을 닫은 사용자의 이름<br>문제 상태<br>요청이 종료된 날짜 및 시간<br>이전 요청 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*종료된 총 요청 수<br>*요청 이름<br>*요청을 닫은 사용자의 이름<br>*일별 요약 날짜 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 내 요청에 할당되었습니다.</strong> </p> <p>문제에 대한 기본 담당자는 사용자가 문제에 할당되었을 때 기본 담당자와 할당된 사용자가 동일한 사용자가 아닌 경우 이메일 알림을 받습니다.</p> <p>에 설명된 대로 프로젝트 상태가 현재이고 프로젝트가 [!UICONTROL 도움말 요청 큐]로 설정된 경우에만 알림이 전송됩니다 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL 요청 대기열 만들기]</a>).</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL이 요청에 할당되었습니다]: "&lt;request name=""&gt;"</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청의 [!UICONTROL 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>요청 이름<br>요청 유형<br>일자 입력됨<br>문제 우선 순위<br>기본 담당자<br>계획된 완료 일자<br>문제 상태<br><strong>자세한 내용 보기</strong> 단추 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*할당된 총 요청 수<br>*요청 이름<br>*할당 대상 이름<br>*일별 요약 날짜</p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 만든 프로젝트의 상태 변경</strong> </p> <p>프로젝트를 만든 사용자는 프로젝트 상태가 변경되면 이메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 프로젝트 상태 변경]: &lt;project name=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청의 [!UICONTROL 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>상태를 변경한 사용자의 이름<br>새 상태<br>프로젝트 상태가 변경된 날짜 및 시간<br>이전 프로젝트 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 새 상태<br>*프로젝트 상태를 변경한 사용자의 이름<br>*일별 요약 날짜</p> </td> 
   <td> <p><strong>인스턴트</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 요청의 상태 변경</strong> </p> <p>상태를 변경한 사용자가 기본 담당자도 아닌 경우 문제의 기본 담당자는 문제 상태가 변경되면 이메일 알림을 받습니다.</p> <p>에 설명된 대로 프로젝트 상태가 현재이고 프로젝트가 [!UICONTROL 도움말 요청 큐]로 설정된 경우에만 알림이 전송됩니다. <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL 요청 대기열 만들기]</a>).</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;request name=""&gt; 은(는) &lt;new status=""&gt;</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> 요청 요약 &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 요청 이름<br>프로젝트 이름<br>요청 참조 번호<br>요청 상태를 변경한 사용자의 이름<br>새 상태<br>요청 상태가 변경된 날짜 및 시간<br>이전 요청 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*상태가 변경된 총 요청 수<br>*요청 이름<br>*이전 요청 상태<br>*새 요청 상태<br>*상태를 변경한 사용자의 이름<br>*일별 요약 날짜<br></td> 
   <td> <p><strong>일별</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
