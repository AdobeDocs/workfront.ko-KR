---
content-type: reference
navigation-topic: notifications
title: '알림: 승인 정보'
description: 다음 알림은 관련된 작업 항목에서 발생하는 승인 활동에 대해 경고합니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 알림: 승인 정보

다음 알림은 관련된 작업 항목에서 발생하는 승인 활동에 대해 경고합니다. 받는 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

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
   <td> <p><strong>위임된 문제 승인 요청이 완료되었습니다</strong> </p> <p>다른 사용자에게 위임한 문제 승인이 해당 사용자에 의해 승인 또는 거부되었습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제 승인/거부 [이(가) 귀하를 대신하여] &lt;사용자 이름&gt;</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Approval Information] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>귀하를 대신하여 문제를 승인/거부한 사용자 이름<br>승인 결정<br>문제 상태<br>승인을 요청한 사용자 이름<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*총 위임된 문제 승인 수<br>*문제 이름<br>*승인자 이름<br>*일별 다이제스트 날짜<br><br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 프로젝트 승인 요청이 완료되었습니다</strong> </p> <p>다른 사용자에게 위임한 프로젝트 승인이 해당 사용자에 의해 승인 또는 거부되었습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Project Approval/ Rejection Made Your 대신하여 수행한] &lt;User Name&gt;</em></p> <p><em>일별 요약 알림의 제목은 다음과 같습니다. [!UICONTROL Digest of Approval Information] &lt;일별 요약 날짜&gt;</em> </p> </td> 
   <td> 프로젝트 이름<br>[!UICONTROL Portfolio 이름]<br>[!UICONTROL 프로젝트 참조 번호]<br>귀하를 대신하여 프로젝트를 승인/거부한 사용자의 이름<br>[!UICONTROL 승인 결정]<br>[!UICONTROL 프로젝트 상태]<br>승인을 요청한 사용자의 이름<br><strong>[!UICONTROL 자세히 보기]</strong> 단추<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*승인자 이름<br>[!UICONTROL *일별 다이제스트 날짜]<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 작업 승인 요청이 완료되었습니다</strong> </p> <p>다른 사용자에게 위임한 작업 승인이 해당 사용자에 의해 승인 또는 거부되었습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Task Approval/ Rejection Made Your 대신하여] &lt;User Name&gt;</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Approval Information] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>대신 작업을 승인/거부한 사용자의 이름<br>승인 결정<br>작업 상태<br>승인을 요청한 사용자의 이름<br><strong>자세한 내용 보기</strong> 단추<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*위임된 작업 승인의 총 수<br>*작업 이름<br>*승인자 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 승인 요청이 취소되었습니다</strong> </p> <p>문서 승인 요청이 취소되면 문서의 문서 승인자가 이메일 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;사용자 이름&gt; [!UICONTROL이 문서 승인 요청을 취소했습니다.]</em></p> <p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 승인 요청을 취소한 사용자의 이름<br>[!UICONTROL 문서 이름] </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 승인자로 위임되었습니다</strong> </p> <p>누군가가 나에게 승인을 위임한 경우 이메일 알림을 받게 됩니다. </p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Delegated] &lt;Object Type&gt; [!UICONTROL Approval - Please Review] &lt;Object Name&gt;</em></p> <p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> <p>[!UICONTROL 개체 이름]<br>[!UICONTROL 상위 개체 이름]<br>[!UICONTROL 개체 참조 번호]<br>승인을 위해 개체를 제출한 사용자의 이름<br>개체를 승인하는 사용자를 대신하여 사용자의 이름<br>개체 상태<br>승인이 요청된 날짜와 시간<br>개체 우선 순위<br>승인 단계 이름<br>[!UICONTROL 계획된 완료 날짜] 개체의 <br><strong>[!UICONTROL 승인 결정]</strong> 단추</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 승인되었습니다</strong> </p> <p>타임시트가 승인되면 이메일 알림을 받게 됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 타임시트 승인됨]: &lt;타임시트 시작 날짜&gt; - &lt;타임시트 종료 날짜&gt;</em>입니다.</p> <p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 타임시트를 승인한 사용자의 이름<br>타임시트가 승인된 날짜와 시간<br>타임시트의 상태([!UICONTROL 승인됨])<br>타임시트의 시작 날짜와 종료 날짜<br>타임시트에 기록된 총 시간<br>타임시트에 기록된 초과 작업 시간 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
 </tbody> 
</table>
