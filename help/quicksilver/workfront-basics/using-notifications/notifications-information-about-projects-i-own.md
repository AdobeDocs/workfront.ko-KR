---
content-type: reference
navigation-topic: notifications
title: '알림: 내 소유 프로젝트 정보'
description: 다음 알림은 사용자가 소유한 프로젝트에서 발생하는 활동에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 고유한 이벤트 알림 활성화 또는 비활성화를 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# 알림: 소유한 프로젝트 정보

다음 알림은 사용자가 소유한 프로젝트에서 발생하는 활동에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>내가 소유한 프로젝트에 문서가 추가됨</strong> </p> <p>문서를 추가한 사용자가 프로젝트 소유자이기도 하지 않는 한 프로젝트 소유자는 프로젝트에 문서가 추가되면 전자 메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 문서가 Private가 아닌 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Document가에 추가됨] &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>문서를 추가한 사용자의 이름입니다<br>문서 이름<br>날짜에 추가됨<br>문서 세부 정보(형식, 크기, 버전 번호)<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL Download]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문서 수<br>*문서 이름<br>*문서를 추가한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 마일스톤 작업이 완료되었습니다.</strong> </p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>참고: 작업이 [!UICONTROL 완료]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL 완료]"가 표시됩니다.</p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>새 작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름입니다<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트가 늦어지고 있습니다.</strong> </p> <p>프로젝트가 예정보다 늦어지면 프로젝트 소유자는 이메일 알림을 받습니다. 진행 상태가 "[!UICONTROL At Risk]," "[!UICONTROL Behind]" 또는 "[!UICONTROL Late]"일 때 프로젝트가 지연됩니다.</p> <p>가장 좋은 방법은 이 알림을 활성 상태로 유지하는 것입니다. </p> <p>[!UICONTROL Review] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 프로젝트 진행률 변경]: &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 진행 상태<br>프로젝트 [!UICONTROL 계획된 시작 날짜]<br>프로젝트 [!UICONTROL 계획된 완료 날짜]<br>프로젝트 [!UICONTROL 예상 시작 날짜]<br>프로젝트 [!UICONTROL 예상 완료 날짜]<br>프로젝트 완료율<br>프로젝트 상태<br>프로젝트 소유자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 진행 상태<br>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에 문제가 추가됨</strong> </p> <p>프로젝트에 문제가 추가되면 프로젝트 소유자는 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제 추가됨] &lt;project name=""&gt;</em></p> <p> </p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름입니다<br>문제 이름<br>문제 유형<br>입력한 날짜<br>문제 우선순위<br>지정 대상 이름 <br>문제 상태<br>기본 연락처<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트에 추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름입니다<br>*일별 다이제스트 날짜</p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 작업이 완료되었습니다.</strong> </p> <p>프로젝트 소유자는 프로젝트에 대한 작업이 완료되면 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>참고: 작업이 [!UICONTROL 완료]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL 완료]"가 표시됩니다.</p> </p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름 <br>작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수 <br>*작업 이름<br>*작업을 완료한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트의 작업이 지연되고 있습니다.</strong> </p> <p>프로젝트 소유자는 프로젝트에 대한 작업이 일정에 따라 지연되면 이메일 알림을 받습니다. 진행 상태가 "[!UICONTROL At Risk]" 또는 "[!UICONTROL Behind]" 또는 "[!UICONTROL Late]"일 때 작업이 지연됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 작업 진행 변경]: &lt;task name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>새 작업 진행 상태<br>작업 [!UICONTROL 계획된 시작 날짜]<br>작업 [!UICONTROL 계획된 완료 날짜]<br>작업 [!UICONTROL 예상 시작 날짜]<br>작업 [!UICONTROL 예상 완료 날짜]<br>작업 완료율<br>작업 상태<br>지정 대상 이름<br>입력한 이름<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*예정보다 늦어진 총 작업 수<br>*작업 이름<br>*지정 대상 이름<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 문제가 완료됨</strong> </p> <p>프로젝트 소유자는 해당 프로젝트에서 문제가 완료되면 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자가 알림을 받지 않습니다. </p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Complete]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 완료한 사용자의 이름입니다<br>문제 상태<br>문제가 완료된 날짜 및 시간<br>이전 문제 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제에 지정된 사용자의 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>미할당 문제를 내가 소유한 프로젝트에 추가합니다.</strong> </p> <p>프로젝트에 미지정 문제가 추가되면 프로젝트 소유자가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 다음에서 이 새 문제에 할당해야 하는 사람] &lt;project name=""&gt;?</em></p> <p> </p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트 다이제스트 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름입니다<br>문제 이름<br>문제 유형<br>입력한 날짜<br>문제 우선순위<br>지정 대상 이름(비어 있음)<br>문제 상태<br>기본 연락처<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>나는 새 프로젝트의 소유자로 설정되었습니다.</strong> </p> <p>사용자가 프로젝트 소유자로 지정되면 해당 사용자는 이메일 알림을 받게 됩니다.</p> <p>프로젝트 소유자가 할당을 수행한 동일한 사용자라면 이메일 알림이 전송되지 않습니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>그들이 어떤 것에 할당되어 있기 때문에 이것을 켜세요. </p> <p> 할당, 공유, 액세스 권한 얻기</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 이제 프로젝트의 소유자입니다.] &lt;project name=""&gt;</em></p> <p>전자 메일 알림 본문에 다음 텍스트가 포함되어 있습니다.<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL을 통해 사용자가 &lt;project name=""&gt;. [!UICONTROL 프로젝트 소유자는 프로젝트 활동에 대한 추가 이메일 알림을 받거나, 프로젝트 시간을 승인하거나, 프로젝트와 관련된 작업을 승인하는 작업에 참여할 수 있습니다. 모두 당신 것입니다.]</em> </p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 완료 날짜<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 프로젝트 중 하나의 작업에 대한 커밋 일자 변경</strong> </p> <p>커밋 날짜를 변경한 사용자가 프로젝트 소유자이기도 하지 않는 한 프로젝트 소유자는 프로젝트의 작업에 대한 커밋 날짜가 변경될 때 전자 메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 커밋 날짜] &lt;task name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트 다이제스트 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>커밋 날짜를 변경한 사용자의 이름<br>새 커밋 날짜<br>작업 [!UICONTROL 계획된 완료 날짜]<br>프로젝트 타임라인이 이 변경의 영향을 받는 방식에 대한 정보입니다<br>지정 대상 이름<br>입력한 이름<br>프로젝트 소유자<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*커밋 날짜가 변경된 총 작업 수<br>*작업 이름<br>*일별 다이제스트 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 프로젝트 중 하나의 문제에 대한 커밋 일자 변경</strong> </p> <p>커밋 날짜를 변경하는 사용자가 프로젝트 소유자와 동일한 사용자의 경우 외에는 프로젝트 소유자가 프로젝트 문제에 대한 커밋 날짜가 변경될 때 이메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 커밋 날짜] &lt;issue name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL Digest] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>커밋 날짜를 변경한 사용자의 이름<br>새 커밋 날짜<br>출고 계획 완료 일자<br>지정 대상 이름<br>입력한 이름<br>프로젝트 소유자<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*커밋 날짜가 변경된 총 문제 수<br>*문제 이름<br>*일별 다이제스트 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
