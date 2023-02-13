---
content-type: reference
navigation-topic: notifications
title: '알림: 승인 정보'
description: 다음 알림은 관련된 작업 항목에서 발생하는 승인 활동에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 고유한 이벤트 알림 활성화 또는 비활성화를 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# 알림: 승인 정보

다음 알림은 관련된 작업 항목에서 발생하는 승인 활동에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

참조 - [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>위임된 문제 승인 요청이 완료되었습니다.</strong> </p> <p>다른 사용자에게 위임한 문제 승인이 해당 사용자에 의해 승인되거나 거부되었습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL이 사용자를 대신하여 승인/거부를 수행] &lt;user name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>귀하를 대신하여 문제를 승인/거부한 사용자의 이름입니다<br>승인 결정<br>문제 상태<br>승인을 요청한 사용자의 이름<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*총 위임된 문제 승인 수<br>*문제 이름<br>*승인자 이름<br>*일별 다이제스트 날짜<br><br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 프로젝트 승인 요청이 완료되었습니다.</strong> </p> <p>다른 사용자에게 위임한 프로젝트 승인이 해당 사용자에 의해 승인되거나 거부되었습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 프로젝트 승인/거부가 사용자를 대신하여 수행] &lt;user name=""&gt;</em></p> <p><em>일별 다이제스트 알림의 주제는 다음과 같습니다. [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 프로젝트 이름<br>[!UICONTROL Portfolio 이름]<br>[!UICONTROL 프로젝트 참조 번호]<br>귀하를 대신하여 프로젝트를 승인/거부한 사용자의 이름입니다<br>[!UICONTROL 승인 결정]<br>[!UICONTROL 프로젝트 상태]<br>승인을 요청한 사용자의 이름<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*승인자 이름<br>[!UICONTROL *일별 다이제스트 날짜]<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 작업 승인 요청이 완료되었습니다.</strong> </p> <p>다른 사용자에게 위임한 작업 승인이 해당 사용자에 의해 승인되거나 거부되었습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Task Approval/ Received On Your Behalted By] &lt;user name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>귀하를 대신하여 작업을 승인/거부한 사용자의 이름입니다.<br>승인 결정<br>작업 상태<br>승인을 요청한 사용자의 이름<br><strong>자세한 내용은</strong> 버튼<br>*프로젝트 참조 번호<br>*프로젝트 이름<br>*총 위임된 작업 승인 수<br>*작업 이름<br>*승인자 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 승인 요청이 취소되었습니다.</strong> </p> <p>문서의 문서 승인자는 문서 승인 요청이 취소되면 전자 메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;user name=""&gt; [!UICONTROL에서 문서 승인 요청을 취소했습니다.]</em></p> <p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 승인 요청을 취소한 사용자의 이름<br>[!UICONTROL 문서 이름] </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>나는 승인자로 위임되었습니다.</strong> </p> <p>사용자에게 승인을 위임한 사람이 있으면 이메일 알림을 받게 됩니다. </p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Delegated] &lt;object type=""&gt; [!UICONTROL Approval - Please Review] &lt;object name=""&gt;</em></p> <p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> <p>[!UICONTROL 개체 이름]<br>[!UICONTROL 부모 개체 이름]<br>[!UICONTROL 개체 참조 번호]<br>승인을 위해 개체를 제출한 사용자의 이름입니다<br>객체를 승인하는 사용자를 대신하여 사용자의 이름입니다<br>개체 상태<br>승인을 요청한 날짜 및 시간<br>개체 우선 순위<br>승인 단계 이름<br>개체의 [!UICONTROL 계획된 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 버튼</p> </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 승인되었습니다.</strong> </p> <p>작업표가 승인되면 전자 메일 알림을 받게 됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 작업표 승인됨]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 작업표를 승인한 사용자의 이름입니다<br>작업표가 승인된 날짜 및 시간<br>작업표 상태([!UICONTROL 승인됨])<br>작업표 시작 날짜 및 종료 날짜<br>작업표에 기록된 총 시간<br>작업표에 기록된 초과 시간 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
 </tbody> 
</table>
