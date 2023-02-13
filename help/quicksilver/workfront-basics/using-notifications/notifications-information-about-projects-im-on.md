---
content-type: reference
navigation-topic: notifications
title: "알림: 내 프로젝트 정보"
description: 다음 알림은 작업 중인 프로젝트에서 발생하는 활동에 대해 알려줍니다.
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 6%

---

# 알림: 현재 진행 중인 프로젝트 정보

다음 알림은 작업 중인 프로젝트에서 발생하는 활동에 대해 알려줍니다.

수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>내가 진행 중인 프로젝트에 문서가 추가되었습니다.</strong> </p> <p>문서를 추가한 사용자를 제외하고 프로젝트 팀 구성원은 프로젝트에 문서가 추가되면 전자 메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 문서가 Private가 아닌 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL Document가에 추가됨] &lt;project name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다 <em>[!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문서 참조 번호<br>문서를 추가한 사용자의 이름입니다<br>문서 이름<br>날짜에 추가됨<br>문서 세부 정보(형식, 크기, 버전 번호)<br>문서 축소판<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL Download]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문서 수<br>*문서 이름<br>*문서를 업로드한 사용자의 이름입니다<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트에서 마일스톤 작업이 완료되었습니다.</strong> </p> <p>프로젝트에 대한 이정표 작업이 완료되면 프로젝트 팀 구성원이 알림을 받습니다. 개인 작업이 완료되면 알림이 전송되지 않습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>제목란 <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트가 활성화됩니다.</strong> </p> <p>프로젝트 상태가 [!UICONTROL Current]로 설정되어 있으면 프로젝트 팀 구성원이 전자 메일 알림을 받습니다.</p> <p>참고: 프로젝트 상태가 [!UICONTROL Current]로 설정된 경우 알림을 받으려면 프로젝트의 스태핑 탭에 사용자가 나열되어야 합니다. 프로젝트 팀에 사용자 추가에 대한 자세한 내용은 <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">프로젝트 팀 관리</a>.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>&lt;project name=""&gt; [!UICONTROL이 최신 상태입니다. - 프로젝트로 이동하여 작업을 확인하십시오!]</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 상태<br>프로젝트 [!UICONTROL 계획된 완료 날짜]<br>프로젝트 소유자<br>사용자, 작업 역할 중 하나 또는 팀 중 하나에 할당된 작업 목록<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 상태<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>내 팀이 진행 중인 프로젝트가 활성화됩니다.</strong> <p>프로젝트가 활성화되면 팀 구성원이 전자 메일 알림을 받습니다. 알림을 받으려면 팀을 하나 이상의 작업에 할당해야 합니다.</p><p>개별 사용자와 팀이 모두 프로젝트의 작업에 할당되는 경우 팀이 알림을 받지 않습니다.</p><p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <i>&lt;project name=""&gt; [!UICONTROL이 활성 상태입니다. - 프로젝트로 이동하여 작업을 확인하십시오!]</i></p><p>일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 상태<br>프로젝트 [!UICONTROL 계획된 완료 날짜]<br>프로젝트 소유자<br>팀에 할당된 작업 목록<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 상태<br>*일별 다이제스트 날짜</td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트가 완료됨</strong> </p> <p>프로젝트 상태가 [!UICONTROL 완료]이면 프로젝트 팀 구성원이 전자 메일 알림을 받습니다.</p> <p>팁: 프로젝트가 정기적으로 완료되는 경우, 이 옵션을 활성화하면 많은 프로젝트에서 제한된 작업 수가 있는 사용자를 위해 많은 이메일을 만들 수 있습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL 프로젝트 상태 변경]: &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트를 완료한 사용자의 이름입니다<br>프로젝트 상태<br>프로젝트가 완료된 날짜 및 시간<br>이전 프로젝트 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 상태<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트에서 작업이 완료되었습니다.</strong> </p> <p>프로젝트에서 작업이 완료되면 프로젝트 팀 구성원이 전자 메일 알림을 받습니다. <br>프로젝트 팀에 대한 자세한 내용은 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>참고: 작업이 [!UICONTROL 완료]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL 완료]"가 표시됩니다.</p> </p> <p><em> 일별 다이제스트 알림의 주제는 다음과 같습니다. [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>작업 상태<br>작업 상태가 변경된 날짜 및 시간<br>이전 작업 상태<br><strong>자세한 내용은</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트에 문제가 추가됨</strong> </p> <p>프로젝트에 문제가 추가되면 프로젝트 팀 구성원이 전자 메일 알림을 받게 됩니다.</p> <p>프로젝트 상태가 현재인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL 문제 추가됨] &lt;project name=""&gt;</em></p> <p> </p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름입니다<br>문제 유형<br>문제 이름<br>입력한 날짜<br>문제 우선순위<br>지정 대상 이름 <br>문제 상태<br>기본 연락처<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트에 추가된 총 문제 수<br>*문제 이름<br>*문제에 지정된 사용자의 이름<br>*일별 다이제스트 날짜 </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트에서 문제가 완료됨</strong> </p> <p>프로젝트 팀 구성원은 프로젝트에서 문제가 완료되면 이메일 알림을 받습니다.<br>프로젝트 팀에 대한 자세한 내용은 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL Complete]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제를 완료한 사용자의 이름입니다<br>문제 상태<br>문제가 완료된 날짜 및 시간<br>이전 문제 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제에 지정된 사용자의 이름<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트에 할당 해제된 문제가 추가됨</strong> </p> <p>프로젝트에 할당되지 않은 문제가 추가되면 프로젝트 팀 구성원이 전자 메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL 다음에서 이 새 문제에 할당해야 하는 사람] &lt;project name=""&gt;?</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름입니다<br>문제 이름<br>문제 유형<br>입력한 날짜<br>문제 우선순위<br>지정 대상 이름(비어 있음) <br>문제 상태<br>기본 연락처<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름입니다<br>*일별 다이제스트 날짜<br></td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트를 추가했습니다.</strong> </p> <p>프로젝트에 추가된 사용자는 사용자가 프로젝트에 자신을 추가하지 않는 한 추가될 때 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL 프로젝트에 추가되었습니다.] &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트에 사용자를 추가한 사용자의 이름입니다<br>프로젝트 [!UICONTROL 계획된 시작 날짜]<br>프로젝트 [!UICONTROL 계획된 완료 날짜]<br>프로젝트 완료율<br>프로젝트에 있는 다른 사용자의 이름 <br>프로젝트 소유자<br><strong>자세한 내용은</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 진행 중인 프로젝트의 상태 변경</strong> </p> <p>프로젝트 팀 구성원은 프로젝트 상태가 변경되면 전자 메일 알림을 받습니다. <br>프로젝트 팀에 대한 자세한 내용은 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다 <em>[!UICONTROL 프로젝트 상태 변경]: &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다 <em> [!UICONTROL Digest of Projects You Are On] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 상태를 변경한 사용자의 이름입니다<br>새 프로젝트 상태<br>프로젝트 상태가 변경된 날짜 및 시간<br>이전 프로젝트 상태<br><strong>[!UICONTROL 자세한 내용 보기]</strong> 버튼<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 상태<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
 </tbody> 
</table>
