---
content-type: reference
navigation-topic: notifications
title: '알림: 기타 정보'
description: 다음 알림은 후원 중인 프로젝트에서 발생하는 활동에 대해 경고합니다.
author: Courtney
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# 알림: 기타 정보

다음 알림은 후원 중인 프로젝트에서 발생하는 활동에 대해 경고합니다.

받는 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

[이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md)도 참조하세요.

>[!NOTE]
>
>일별 알림을 활성화하거나 비활성화할 수 없으며 이 범주의 이벤트에 대한 일별 요약 이메일을 받지 않습니다. [!UICONTROL 기타] 범주에 대해 개별 인스턴트 알림을 활성화하거나 비활성화할 수 있습니다.

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
   <td> <p><strong>메시지를 [!UICONTROL 알림 센터]로 보냅니다.</strong> </p> <p>[!UICONTROL Announcement Center]에 새 메시지가 전송되면 이메일 알림을 받게 됩니다. </p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL [!DNL Adobe Workfront] Announcement]입니다. &lt;Announcement 제목&gt;</em></p> </td> 
   <td> 공지 제목<br>공지에 포함된 메시지 텍스트<br>첨부 문서<br>공지를 보낸 사용자 이름<br>공지를 보낸 날짜 및 시간 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작업 할당 변경이 내 직원 중 한 명에게 영향을 미칩니다</strong> </p> <p>관리자로 지정된 사용자의 부하 직원 중 하나가 새 작업에 할당되면 관리자는 할당에 대한 이메일을 수신합니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 작업 리소스 할당]입니다. &lt;작업 이름&gt;</em></p> </td> 
   <td>프로젝트 이름<br>작업 이름<br>작업을 만든 날짜와 시간<br>작업을 만든 사용자의 이름<br>할당 이름<br>기한(계획된 완료 날짜)<br>작업 상태<br></td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 업로드 요청을 받은 후 요청이 취소되었습니다</strong> </p> <p>문서 요청이 취소되면 문서 요청자는 이메일 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>&lt;요청을 취소한 사용자 이름&gt;입니다. </em></p> <p>이메일 알림의 본문에는 다음 텍스트가 포함되어 있습니다.</p> <p><em>[!UICONTROL Hi] &lt;사용자 이름&gt;, <br><br>&lt;요청을 취소한 사용자의 이름&gt;[!UICONTROL에는 이전에 받은 요청과 관련하여 더 이상 업로드가 필요하지 않습니다. 귀하에게 알려드리고자 합니다.]</em> </p> </td> 
   <td>요청을 취소한 사용자의 이름<br>원본 문서 업로드 요청의 텍스트<br>원본 문서 요청의 "[!UICONTROL CANCELLED]" 배너<br>원본 문서 요청의 날짜 및 시간<br></td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>주의가 필요한 오류가 발견되었습니다</strong> </p> <p>이메일을 통해 댓글에 답글을 다는 사용자는 답글이 게재되지 않을 때 이메일 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Failed on] &lt;subject of original message&gt;</em></p> <p>전자 메일을 사용하여 댓글에 회신하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">전자 메일 알림에 회신</a>을 참조하십시오.</p> </td>
   <td> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문제 할당 변경이 내 직원 중 한 명에게 영향을 미칩니다</strong> </p> <p>문제에 할당된 사용자의 관리자는 해당 사용자가 문제에서 제거되거나 문제에 할당되면 이메일 알림을 수신합니다. </p> <p>프로젝트 상태가 현재 또는 계획인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>문제 할당: &lt;문제 이름&gt;</em>입니다.</p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>할당한 사용자 이름<br>문제 유형<br>문제에 할당된 사용자 이름<br>문제 날짜 입력<br>문제 우선 순위<br>기본 담당자<br>문제 [!UICONTROL 계획된 완료 날짜]<br>문제 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 직원 중 한 명이 프로젝트에 추가됨</strong> </p> <p>관리자는 사용자 중 한 명이 프로젝트에 추가되면 이메일 알림을 받습니다. 이 알림은 프로젝트의 상태에 관계없이 전송됩니다. </p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다.</p> <p>이메일 제목은 <em>프로젝트 할당: &lt;사용자 이름&gt;[&lt;프로젝트 GUID&gt;_ &lt;사용자 GUID&gt;]</em>입니다.</p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트에 사용자를 추가한 사용자의 이름<br>프로젝트에 추가된 사용자의 이름<br>프로젝트 [!UICONTROL 계획된 시작 일자]<br>프로젝트 [!UICONTROL 계획된 완료 일자]<br>프로젝트 완료율<br>프로젝트에 있는 다른 사용자의 이름<br>프로젝트 상태<br>프로젝트 소유자<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br><br><br></p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 포트폴리오 또는 프로그램에 누군가가 프로젝트를 추가합니다</strong> </p> <p>새 프로젝트가 포트폴리오 또는 프로그램에 추가되면 포트폴리오 및/또는 프로그램 소유자는 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 프로젝트가 &lt;Portfolio 이름&gt;[프로젝트 GUID]</em></p> </td> 
   <td> Portfolio 이름<br>프로젝트 참조 번호<br>포트폴리오/프로그램에 프로젝트를 추가한 사용자의 이름<br><br></td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>다른 사용자가 나와 개체를 공유합니다</strong> </p> <p>누군가 나를 오브젝트에 대한 [!UICONTROL 공유] 권한 목록에 추가하면 이메일 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 액세스 권한 부여됨]: &lt;개체 이름&gt;</em>입니다.</p> <p>프로젝트가 [!UICONTROL 현재] 상태인 경우에만 알림이 전송됩니다.</p> </td> 
   <td> 개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>개체에 대한 원래 액세스<br>개체에 새 액세스 권한이 부여됨<br>액세스 권한이 부여된 날짜 및 시간 <br>액세스 권한을 부여한 사용자의 이름 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>다른 사용자가 내 팀과 개체를 공유합니다</strong> </p> <p>누군가 오브젝트에 대한 공유 권한 목록에 내 팀을 추가하면 이메일 알림을 받게 됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 액세스 권한 부여됨]: &lt;개체 이름&gt; [액세스 규칙 GUID]</em>입니다.</p> </td> 
   <td> 개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>이전 액세스<br>새 액세스<br>액세스 권한이 부여된 날짜 및 시간<br>팀 이름<br>액세스 권한을 부여한 사용자의 이름 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 구독 중인 작업, 문제 또는 프로젝트에 업데이트가 이루어짐</strong> </p> <p>누군가가 내가 구독 중인 항목에 댓글을 다는 경우 이메일 알림을 받습니다.</p> <p>구독 전자 메일의 제목: <em>[!UICONTROL 구독하는 &lt;개체 유형&gt;이(가) 업데이트되었습니다. &lt;개체 이름&gt;</em></p> </td> 
   <td> 개체 이름<br> 개체 참조 번호<br> 구독한 항목에 댓글을 단 사용자의 이름<br> 날짜 댓글이 작성됨<br> 댓글이 구독한 항목에 추가됨  </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
 </tbody> 
</table>
