---
content-type: reference
navigation-topic: notifications
title: '알림: 조치 필요'
description: 다음 알림은 작업 항목에 대해 작업을 수행해야 하는지 여부를 알려줍니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# 알림: [!UICONTROL 작업 필요]

다음 알림은 작업 항목에 대해 작업을 수행해야 하는지 여부를 알려줍니다. 받는 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

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
   <td> <p><strong>새 작업 요청을 받습니다</strong> </p> <p>요청을 하는 사용자가 할당자도 아닌 경우 작업 항목의 할당자는 이메일 알림을 받습니다. </p> <p>작업 상태가 [!UICONTROL Complete]이거나 문제 상태가 [!UICONTROL Closed]인 경우 알림이 전송되지 않습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 새 작업 요청]: &lt;요청 이름&gt;</em>입니다.</p> <p>일별 요약 알림의 제목은 <em>[!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>작업 이름</p> <p>[!UICONTROL 계획된 완료 일자]</p> <p>상위</p> <p>할당자</p> <p>할당 대상:</p> <p>[!UICONTROL 상태]</p> <p>[!UICONTROL 설명]</p> <p>[!UICONTROL 보기] 단추<br>일별 다이제스트에 추가하는 옵션</p> <br> </td> 
   <td><strong>즉시 및</strong> <strong>매일</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서를 승인해야 합니다</strong> </p> <p>문서의 승인자가 승인자로 나열되면 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;승인을 제출한 사용자 이름&gt; [!UICONTROL이(가) [!DNL Adobe Workfront]에서 문서를 승인하도록 요청했습니다.]</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>승인을 제출한 사용자의 이름<br>문서 이름<br>문서 참조 번호<br>승인 요청한 날짜 및 시간<br>문서 세부 정보(형식, 크기, 버전 번호)<br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*보류 중인 문서 승인의 총 수<br>*<strong>[!UICONTROL 문서 승인 참조</strong>*<strong>모든 승인 참조]</strong> 단추<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트를 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀에 있지 않아도 됩니다(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되었는지 여부에 따라 달라집니다(<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>에 설명된 대로). </p> <p><strong>이 옵션을 사용하도록 설정하면</strong> 승인과 관련된 작업 역할이 있는 시스템의 모든 사용자에게 전자 메일 알림이 전송됩니다. </p> <p><strong>이 옵션이 비활성화되어 있으면</strong> 승인 프로세스와 연결된 작업 역할이 있는 프로젝트 팀원만 전자 메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자가 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 프로젝트 승인 보류 중]: &lt;프로젝트 이름&gt;</em>입니다.</p> <p> 일별 요약 알림의 제목은 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>승인을 제출한 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>프로젝트 우선 순위<br>승인 단계 승인 보류 중<br>승인 대기 중인 결정 수<br>승인자 이름(사용자만 해당)<br>[!UICONTROL 프로젝트 계획 완료 날짜] <br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*보류 중인 총 프로젝트 승인 수 <br>*<strong>[!UICONTROL 프로젝트 승인]</strong><br>*<strong>[!UICONTROL 참조 모든 승인]</strong> 단추<br>*일별 요약 날짜</p> </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작업을 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀에 있지 않아도 됩니다(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되었는지 여부에 따라 달라집니다(<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>에 설명된 대로). </p> <p><strong>이 옵션을 사용하도록 설정하면</strong> 승인과 관련된 작업 역할이 있는 시스템의 모든 사용자에게 전자 메일 알림이 전송됩니다. </p> <p><strong>이 옵션이 비활성화되어 있으면</strong> 승인 프로세스와 연결된 작업 역할이 있는 프로젝트 팀원만 전자 메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자가 알림을 받습니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 작업 승인 보류 중]: &lt;작업 이름&gt;</em>입니다.</p> <p> 일별 요약 알림의 제목은 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>승인을 제출한 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>작업 우선 순위<br>승인 단계 이름<br>승인자 이름<br>[!UICONTROL 작업 계획 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*보류 중인 총 작업 승인 수<br>*링크 대상<strong>[!UICONTROL 작업 승인 *모든 승인 보기]</strong> 단추<strong></strong>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>타임시트를 승인해야 합니다</strong> </p> <p>타임시트를 제출한 사용자가 타임시트 승인자도 아닌 경우 승인해야 하는 타임시트가 제출되면 타임시트 승인자가 이메일 알림을 받습니다.</p> <p>타임시트의 상태가 [!UICONTROL Submitted]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 타임시트 제출됨]: &lt;타임시트 소유자&gt;, &lt;타임시트 시작 날짜&gt; - &lt;타임시트 종료 날짜&gt;</em>입니다.</p> <p> 일별 요약 알림의 제목은 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 승인을 위해 타임시트를 제출한 사용자의 이름<br>타임시트가 제출된 날짜와 시간<br>타임시트의 상태<br>타임시트에 기록된 시작 날짜와 종료 날짜<br>타임시트에 기록된 시간<br>타임시트에 기록된 초과 시간 수<br><strong>[!UICONTROL 검토]</strong> 및 <strong>[!UICONTROL 승인]</strong> 단추<br>*보류 중인 총 타임시트 승인 수<br>*<strong>[!UICONTROL 타임시트 승인]</strong><br><strong>[!UICONTROL *모든 승인 보기]</strong> 단추<br>*일별 다이제스트 날짜 </td> 
   <td><strong>즉시 및</strong> <strong>매일</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>문제를 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀에 있지 않아도 됩니다(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되었는지 여부(<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL 전역 승인 구성] 설정</a>에 설명된 대로)에 따라 달라집니다. </p> <p><strong>이 옵션을 사용하도록 설정하면</strong> 승인과 관련된 작업 역할이 있는 시스템의 모든 사용자에게 전자 메일 알림이 전송됩니다. </p> <p><strong>이 옵션이 비활성화되어 있으면</strong> 승인 프로세스와 연결된 작업 역할이 있는 프로젝트 팀원만 전자 메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자가 알림을 받습니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 문제 승인 보류 중]: &lt;문제 이름&gt;</em>입니다.</p> <p> 일별 요약 알림의 제목은 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt; </em>입니다.</p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>승인을 위해 문제를 제출한 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>문제 우선 순위<br>승인 단계<br>승인자의 이름<br>[!UICONTROL 문제 계획된 완료 날짜]<br>[!UICONTROL 기본 담당자]<br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*보류 중인 총 문제 승인 수<br>*<strong>[!UICONTROL 문제 승인]</strong><br><strong>[ UICONTROL *모든 승인 보기]</strong> 단추<br>*일별 요약 날짜 </td> 
   <td><strong>즉시 및</strong> <strong>매일</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 프로젝트 승인을 검토해야 합니다</strong> </p> <p>프로젝트 승인이 귀하에게 위임되었으며 이를 검토해야 합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 위임된 프로젝트 승인 - 검토해 주십시오.] &lt;프로젝트 이름&gt;</em></p> <p><em>일별 요약 알림의 제목은 [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다. </p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>승인을 요청한 사용자의 이름<br>프로젝트를 승인하고 있는 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>프로젝트 우선 순위<br>승인 단계<br>승인자의 이름<br>[!UICONTROL 프로젝트 계획 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*총 보류 중인 프로젝트 승인 수<br>*링크 대상 <strong>[!UICONTROL 프로젝트 승인 *모든 승인 보기]</strong> 단추 <br>*날짜 일별 요약 </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 작업 승인을 검토해야 합니다</strong> </p> <p>작업 승인이 귀하에게 위임되었으며 이를 검토해야 합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 위임된 작업 승인 - ]&lt;작업 이름&gt;</em>입니다.</p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>승인을 요청한 사용자의 이름<br>작업을 대신 승인하는 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>작업 우선 순위<br>승인 단계<br>승인자의 이름<br>[!UICONTROL 작업 계획 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 단추 <br>*총 보류 중인 작업 승인 수<br>*연결 대상 <strong>[!UICONTROL 작업 승인 *모든 승인 보기]</strong> 단추<br> 일별 요약 날짜 </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>위임된 문제 승인을 검토해야 합니다</strong> </p> <p>문제 승인이 귀하에게 위임되었으며 이를 검토해야 합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 위임된 문제 승인 - [문제 이름]&lt;1}</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>승인을 요청한 사용자의 이름<br>문제를 승인하고 있는 사용자의 이름<br>승인 보류 중 상태<br>승인 요청한 날짜 및 시간<br>문제 우선 순위<br>승인 단계<br>승인자의 이름<br>문제 계획 완료 날짜<br>기본 담당자<br><strong>[!UICONTROL 승인 결정]</strong> 단추<br>*보류 중인 총 문제 승인 수<br>*<strong>[!UICONTROL 문제 승인]</strong><br><strong>[!UICONTROL 모든 승인 보기]</strong> 단추<br>*일별 요약 날짜<br></td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>문제에 할당됨</strong> </p> <p>문제 피할당자는 이메일 알림을 받습니다. 문제 상태가 [!UICONTROL Closed]이거나 그와 동등한 경우 문제 피할당자가 이메일을 받지 않습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 새 작업 요청]입니다. &lt;문제 이름&gt;</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>[!UICONTROL 문제 참조 번호]<br>사용자 이름<br>문제 기한([!UICONTROL 계획된 완료 일자])<br>사용자에게 문제를 할당한 사용자 이름<br><strong>[!UICONTROL 작업 완료]</strong> 단추<br>*총 할당 수<br>*사용자에게 할당된 총 작업 및 문제 수<br>*<strong>[!UICONTROL 작업 요청]</strong><br>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작업의 기본 피할당자로 설정되었습니다.</strong> </p> <p>할당자가 할당을 수행한 사용자가 아닌 경우 작업 할당자는 자신이 작업의 기본 할당자로 설정된 경우 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 작업이 [!UICONTROL Complete]로 표시되지 않은 경우 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 새 작업 요청]: &lt;작업 이름&gt;</em>입니다.</p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>사용자 이름<br>작업 기한([!UICONTROL 계획된 완료 날짜])<br>사용자에게 작업을 할당한 사용자 이름<br><strong>[!UICONTROL 처리 중]</strong> 단추<br>*사용자에게 할당된 총 작업 및 문제 수<br>*<strong>[!UICONTROL 작업 요청]</strong>*일별 다이제스트 날짜 </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 팀이 새 작업 요청을 받습니다</strong> </p> <p>팀원이 새 작업 요청을 받으면 이메일 알림을 받습니다. (요청을 제출한 사용자가 팀의 멤버인 경우 알림을 받지 않습니다.)</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 작업 요청 상태가 [!UICONTROL New]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 새 작업 요청]: &lt;요청 이름&gt;</em>입니다.</p> <p>일별 요약 알림의 제목은 <em>[!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p> 문제 이름<br>프로젝트 이름(요청 큐 이름)<br>문제 참조 번호<br>팀 이름<br>문제 기한(계획된 완료 날짜)<br>요청을 제출한 사용자의 이름<br><strong>[!UICONTROL 작업]</strong> 단추<br>*팀에 할당된 총 요청 수</p> <p>*작업 요청 이름</p> <p>[!UICONTROL *계획된 완료 일자]</p> <p>*요청을 제출한 사용자의 이름<br>*<strong>[!UICONTROL 팀 요청]</strong><br>*일별 다이제스트 날짜 </p> <p><span class="preview">*팀 할당</span> </p> </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 다시 열렸습니다</strong> </p> <p>타임시트를 다시 연 사용자가 타임시트의 소유자도 아닌 경우 타임시트가 다시 열릴 때 타임시트 소유자에게 전자 메일 알림을 보냅니다.</p> <p>타임시트 상태가 [!UICONTROL Open]인 경우에만 이메일 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 타임시트 다시 열림]: &lt;타임시트 시작 날짜&gt; - &lt;타임시트 종료 날짜&gt;</em>입니다.</p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> 타임시트를 다시 연 사용자의 이름<br>타임시트가 다시 열린 날짜와 시간<br>타임시트의 상태([!UICONTROL 다시 열림])<br>타임시트에 기록된 총 시간 수<br>타임시트에 기록된 초과 작업 시간 수<br><strong>[!UICONTROL 검토]</strong> 단추 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 거부되었습니다</strong> </p> <p>타임시트를 거부한 사용자가 소유자도 아닌 경우 타임시트가 거부되면 타임시트 소유자에게 이메일 알림이 전송됩니다.</p> <p>타임시트 상태가 [!UICONTROL Rejected]인 경우에만 이메일 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 타임시트 거부됨]:&lt;타임시트 시작 날짜&gt; - &lt;타임시트 종료 날짜&gt;</em>입니다.</p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> 타임시트를 거부한 사용자의 이름<br>타임시트의 상태([!UICONTROL 거부됨])<br>타임시트가 거부된 날짜 및 시간<br><strong>[!UICONTROL 검토]</strong> 단추 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 액세스 권한을 요청했습니다</strong> </p> <p>나한테 뭘 좀 해달라고 하니까, 켜봐.</p> <p>프로젝트를 만드는 사람이 해당 프로젝트에 액세스할 수 있습니다.</p> <p>누군가가 액세스를 요청할 때 사용자가 알림을 받게 되는 이유입니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;액세스 권한을 요청한 사용자 이름&gt; [!UICONTROL은(는) &lt;개체 이름&gt;</em>에 액세스해야 합니다.</p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Action Needed] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>액세스를 요청한 사용자의 이름<br>사용자가 요청하는 액세스 유형입니다<br><strong>[!UICONTROL 부여] &lt;액세스 요청된 액세스 이름&gt; </strong> 및 <strong>[!UICONTROL 다른 액세스 권한 부여]</strong> 단추<br>*보류 중인 액세스 요청 승인의 총 수<br>*<strong>[!UICONTROL 액세스 요청]</strong> 승인에 대한 링크<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>즉시 및 매일</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 문서 업로드를 요청했습니다</strong> </p> <p>문서 요청자는 사용자가 문서를 업로드하라는 요청을 받으면 이메일 알림을 받습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;문서를 요청하는 사용자의 이름&gt; [!UICONTROL에는 [!DNL Workfront]에 사용자의 문서가 필요합니다.]</em></p> <p> <p>참고: 일별 요약 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 문서를 요청하는 사용자의 이름<br>문서를 업로드해야 하는 개체의 이름<br><strong>[!UICONTROL 여기에 첨부]</strong> 링크 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
 </tbody> 
</table>
