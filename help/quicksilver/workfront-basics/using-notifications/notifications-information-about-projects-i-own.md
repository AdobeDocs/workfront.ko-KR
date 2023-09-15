---
content-type: reference
navigation-topic: notifications
title: '알림: 내가 소유한 프로젝트에 대한 정보'
description: 다음 알림은 사용자가 소유한 프로젝트에서 발생하는 활동에 대해 경고합니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 6%

---

# 알림: 내가 소유한 프로젝트에 대한 정보

다음 알림은 사용자가 소유한 프로젝트에서 발생하는 활동에 대해 경고합니다. 수신하는 알림 구성에 대한 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

참조: [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>내가 소유한 프로젝트에 문서가 추가됨</strong> </p> <p>문서를 추가한 사용자가 프로젝트 소유자도 아닌 경우 프로젝트 소유자는 문서가 프로젝트에 추가될 때 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 문서가 비공개인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문서가]에 추가됨 &lt;project name=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>문서를 추가한 사용자의 이름<br>문서 이름<br>추가된 날짜<br>문서 세부 정보(형식, 크기, 버전 번호)<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL 다운로드]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문서 수<br>*문서 이름<br>*문서를 추가한 사용자의 이름<br>*일별 요약 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 마일스톤 작업이 완료되었습니다.</strong> </p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 완료]: &lt;task name=""&gt; 날짜 &lt;project name=""&gt;</em></p> <p>참고: 작업이 [!UICONTROL Complete]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL Complete]"가 표시됩니다.</p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>새 작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 요약 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트가 늦어지고 있습니다.</strong> </p> <p>프로젝트가 지연되면 프로젝트 소유자에게 이메일 알림이 전송됩니다. 진행 상태가 "[!UICONTROL At Risk]", "[!UICONTROL Behind]" 또는 "[!UICONTROL Late]일 때 프로젝트가 예약보다 늦습니다."</p> <p>가장 좋은 방법은 이 알림을 활성 상태로 유지하는 것입니다. </p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 프로젝트 진행 상황 변경]: &lt;project name=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 진행 상태<br>프로젝트 [!UICONTROL 계획된 시작 일자]<br>프로젝트 [!UICONTROL 계획된 완료 일자]<br>프로젝트 [!UICONTROL 예상 시작 일자]<br>프로젝트 [!UICONTROL 예상 완료 일자]<br>프로젝트 완료율<br>프로젝트 상태<br>프로젝트 소유자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 진행 상태<br>*일별 요약 날짜<br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에 문제가 추가됨</strong> </p> <p>문제가 프로젝트에 추가되면 프로젝트 소유자에게 이메일 알림이 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제 추가됨] &lt;project name=""&gt;</em></p> <p> </p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자 이름<br>문제 이름<br>문제 유형<br>일자 입력됨<br>문제 우선 순위<br>할당 대상 이름 <br>문제 상태<br>기본 담당자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트에 추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름<br>*일별 요약 날짜</p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 작업이 완료되었습니다.</strong> </p> <p>프로젝트에서 작업이 완료되면 프로젝트 소유자에게 알림이 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 완료]: &lt;task name=""&gt; 날짜 &lt;project name=""&gt;</em></p> <p> <p>참고: 작업이 [!UICONTROL Complete]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL Complete]"가 표시됩니다.</p> </p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름 <br>작업 상태<br>작업 완료 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수 <br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 요약 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트의 작업이 지연되고 있습니다.</strong> </p> <p>프로젝트의 작업이 지연되면 프로젝트 소유자에게 이메일 알림이 전송됩니다. 진행 상태가 "[!UICONTROL At Risk]" 또는 "[!UICONTROL Behind]" 또는 "[!UICONTROL Late]"일 때 작업이 지연되고 있습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 작업 진행 상황 변경]: &lt;task name=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>새 작업 진행 상태<br>작업 [!UICONTROL 계획된 시작 일자]<br>작업 [!UICONTROL 계획된 완료 일자]<br>작업 [!UICONTROL 예상 시작 일자]<br>작업 [!UICONTROL 예상 완료 일자]<br>작업 완료율<br>작업 상태<br>할당 대상 이름<br>이름으로 입력됨<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*지연되는 총 작업 수<br>*작업 이름<br>*할당 대상 이름<br>*일별 요약 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 소유한 프로젝트에서 문제가 완료됨</strong> </p> <p>프로젝트 소유자는 프로젝트에서 문제가 완료되면 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다. </p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 완료]: &lt;issue name=""&gt; 날짜 &lt;project name=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 완료한 사용자의 이름<br>문제 상태<br>문제가 완료된 날짜 및 시간<br>이전 문제 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제에 할당된 사용자의 이름<br>*일별 요약 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>미할당 문제를 내가 소유한 프로젝트에 추가합니다.</strong> </p> <p>미할당 문제가 프로젝트에 추가되면 프로젝트 소유자에게 이메일 알림이 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 다음에 대한 새로운 문제에 누구에게 할당되어야 합니까?] &lt;project name=""&gt;?</em></p> <p> </p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 다이제스트 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자 이름<br>문제 이름<br>문제 유형<br>일자 입력됨<br>문제 우선 순위<br>할당 대상 이름(비어 있음)<br>문제 상태<br>기본 담당자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름<br>*일별 요약 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 새 프로젝트의 소유자로 설정되었습니다.</strong> </p> <p>사용자가 프로젝트 소유자로 할당되면 해당 사용자는 이메일 알림을 받습니다.</p> <p>프로젝트 소유자가 할당한 사용자와 동일한 경우 이메일 알림이 전송되지 않습니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다.</p> <p>할당된 항목이 있으므로 이 항목을 켜십시오. </p> <p> 할당, 공유, 액세스 권한 부여</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 이제 의 프로젝트 소유자입니다.] &lt;project name=""&gt;</em></p> <p>이메일 알림의 본문에는 다음 텍스트가 포함되어 있습니다.<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL 이(가) 나를 의 소유자로 만들었습니다.] &lt;project name=""&gt;. [!UICONTROL 프로젝트 소유자는 프로젝트 활동에 대한 추가 이메일 알림을 받거나, 프로젝트 시간을 승인해야 하거나, 프로젝트와 관련된 작업 승인에 참여할 수 있습니다. 다 네 거야.]</em> </p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 완료 일자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*일별 요약 날짜</p> </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 프로젝트 중 하나의 작업에 대한 커밋 일자 변경</strong> </p> <p>커밋 일자를 변경한 사용자가 프로젝트 소유자도 아닌 경우 프로젝트 소유자는 프로젝트의 작업에 대한 커밋 일자가 변경될 때 이메일 알림을 수신합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 커밋 일자] &lt;task name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 다이제스트 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>커밋 일자를 변경한 사용자의 이름<br>새 커밋 일자<br>작업 [!UICONTROL 계획된 완료 일자]<br>프로젝트 타임라인이 이 변경의 영향을 받는 방법에 대한 정보<br>할당 대상 이름<br>이름으로 입력됨<br>프로젝트 소유자<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*커밋 일자가 변경된 총 작업 수<br>*작업 이름<br>*일별 요약 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 프로젝트 중 하나의 문제에 대한 커밋 일자 변경</strong> </p> <p>커밋 일자를 변경하는 사용자가 프로젝트 소유자와 동일한 사용자가 아닌 경우 프로젝트 소유자는 프로젝트에서 문제에 대한 커밋 일자가 변경될 때 이메일 알림을 수신합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 커밋 일자] &lt;issue name=""&gt; [!UICONTROL is now] &lt;new commit="" date=""&gt;</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다. <em> 소유한 프로젝트의 [!UICONTROL 다이제스트] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>커밋 일자를 변경한 사용자의 이름<br>새 커밋 일자<br>문제 계획된 완료 일자<br>할당 대상 이름<br>이름으로 입력됨<br>프로젝트 소유자<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*커밋 일자가 변경된 총 문제 수<br>*문제 이름<br>*일별 요약 날짜<br></p> </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
