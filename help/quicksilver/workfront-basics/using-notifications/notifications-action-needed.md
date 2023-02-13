---
content-type: reference
navigation-topic: notifications
title: '알림: 필요한 작업'
description: 다음 알림은 작업 항목에 대해 작업을 수행해야 할 경우 사용자에게 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 고유한 이벤트 알림 활성화 또는 비활성화를 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '2446'
ht-degree: 4%

---

# 알림: [!UICONTROL 필요한 작업]

다음 알림은 작업 항목에 대해 작업을 수행해야 할 경우 사용자에게 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>새 작업 요청을 받습니다.</strong> </p> <p>작업 항목의 할당자는 요청을 하는 사용자도 할당자가 아닌 경우 이메일 알림을 받습니다. </p> <p>작업 상태가 [!UICONTROL Complete]이거나 문제 상태가 [!UICONTROL Closed]인 경우에는 알림이 전송되지 않습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 새 작업 요청]: &lt;request name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다. <em>[!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>작업 이름</p> <p>[!UICONTROL 계획된 완료 날짜]</p> <p>상위</p> <p>할당자:</p> <p>할당 대상:</p> <p>[!UICONTROL 상태]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View] 단추<br>일별 다이제스트에 추가하는 옵션</p> <br> </td> 
   <td><strong>인스턴트 및</strong> <strong>일별</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>문서 승인이 필요합니다</strong> </p> <p>문서의 승인자는 승인자로 나열되면 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL에서 문서를 승인하도록 요청했습니다. [!DNL Adobe Workfront].]</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>승인을 제출한 사용자의 이름입니다<br>문서 이름<br>문서 참조 번호<br>승인 요청 날짜 및 시간<br>문서 세부 정보(형식, 크기, 버전 번호)<br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 대기 중인 문서 승인 수<br>*링크 대상 <strong>[!UICONTROL Document Approvals</strong>*<strong>모든 승인 참조]</strong> 버튼<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트를 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되어 있는지 여부에 따라 달라집니다. <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>). </p> <p><strong>이 옵션이 활성화되어 있으면</strong>를 입력하면 승인과 연관된 작업 역할이 있는 시스템의 모든 사용자에게 이메일 알림이 전송됩니다. </p> <p><strong>이 옵션을 비활성화한 경우</strong>를 설정하는 경우 승인 프로세스와 연관된 작업 역할을 가진 프로젝트 팀 멤버만 이메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자는 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Project Pending Approval]: &lt;project name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>승인을 제출한 사용자의 이름<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>프로젝트 우선 순위<br>승인 단계 승인 보류 중<br>승인을 기다리는 의사 결정 수<br>승인자 이름(사용자만 해당)<br>[!UICONTROL Project Planning 완료 날짜] <br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 대기 중인 프로젝트 승인 수 <br>*링크 대상 <strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL 모든 승인 보기]</strong> 버튼<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작업을 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되어 있는지 여부에 따라 달라집니다. <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>). </p> <p><strong>이 옵션이 활성화되어 있으면</strong>를 입력하면 승인과 연관된 작업 역할이 있는 시스템의 모든 사용자에게 이메일 알림이 전송됩니다. </p> <p><strong>이 옵션을 비활성화한 경우</strong>를 설정하는 경우 승인 프로세스와 연관된 작업 역할을 가진 프로젝트 팀 멤버만 이메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자는 알림을 받습니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Task Pending Approval]: &lt;task name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>작업 이름<br>프로젝트 이름<br>승인을 제출한 사용자의 이름입니다<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>작업 우선 순위<br>승인 단계 이름<br>승인자 이름<br>[!UICONTROL 작업 계획된 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 보류 중인 작업 승인 수<br>*링크 대상<strong>[!UICONTROL 작업 승인 *모든 승인 참조]</strong> 버튼<strong></strong>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>타임시트를 승인해야 합니다</strong> </p> <p>작업표를 제출한 사용자도 작업표 승인자가 아닌 경우, 승인자가 승인해야 하는 작업표를 제출하면 전자 메일 알림을 받습니다.</p> <p>작업표의 상태가 [!UICONTROL Submitted]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 제출됨]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 승인을 위해 작업표를 제출한 사용자의 이름입니다<br>작업표를 제출한 날짜 및 시간<br>작업표의 상태<br>작업표의 시작 및 종료 날짜<br>작업표에 기록된 시간<br>작업표에 기록된 초과 시간 수<br><strong>[!UICONTROL Review]</strong> 및 <strong>[!UICONTROL Approve]</strong> 버튼<br>*보류 중인 총 작업표 승인 수<br>*링크 대상 <strong>[!UICONTROL 작업표 승인]</strong><br><strong>[!UICONTROL *모든 승인 참조]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td><strong>인스턴트 및</strong> <strong>일별</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>문제를 승인해야 합니다</strong> </p> <p>작업 역할 승인의 경우 이 이벤트에 대한 전자 메일 알림을 받는 사용자는 '[!UICONTROL 승인자가 프로젝트 팀(역할을 포함하는 승인 프로세스의 경우)]' 설정이 활성화되어 있는지 여부에 따라 달라집니다. <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL 전역 승인 구성] 설정</a>). </p> <p><strong>이 옵션이 활성화되어 있으면</strong>를 입력하면 승인과 연관된 작업 역할이 있는 시스템의 모든 사용자에게 이메일 알림이 전송됩니다. </p> <p><strong>이 옵션을 비활성화한 경우</strong>를 설정하는 경우 승인 프로세스와 연관된 작업 역할을 가진 프로젝트 팀 멤버만 이메일 알림을 받습니다.</p> <p>승인이 사용자와 연관되어 있으면 해당 사용자는 알림을 받습니다. </p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Issue Pending Approval]: &lt;issue name=""&gt;</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다. <em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>승인을 위해 문제를 제출한 사용자의 이름입니다<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>문제 우선순위<br>승인 단계<br>승인자 이름<br>[!UICONTROL Issue 계획된 완료 날짜]<br>[!UICONTROL 기본 연락처]<br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 보류 중인 문제 승인 수<br>*링크 대상 <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *모든 승인 참조]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td><strong>인스턴트 및</strong> <strong>일별</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 위임한 프로젝트 승인을 검토해야 합니다.</strong> </p> <p>프로젝트 승인이 위임되었으므로 검토해야 합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Delegated Project Approval - 검토] &lt;project name=""&gt;</em></p> <p><em>일별 다이제스트 알림의 주제는 다음과 같습니다. [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>승인을 요청한 사용자의 이름입니다<br>프로젝트를 승인하는 사용자의 이름입니다<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>프로젝트 우선 순위<br>승인 단계<br>승인자 이름<br>[!UICONTROL Project Planning 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 대기 중인 프로젝트 승인 수<br>*링크 대상 <strong>[!UICONTROL Project Approvals *모든 승인 참조]</strong> 버튼 <br>*일별 다이제스트 날짜 </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내게 위임된 작업 승인을 검토해야 합니다.</strong> </p> <p>작업 승인이 사용자에게 위임되었으므로 검토해야 합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 위임된 작업 승인 - 검토]&lt;task name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>승인을 요청한 사용자의 이름입니다<br>작업을 승인하는 사용자의 이름입니다<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>작업 우선 순위<br>승인 단계<br>승인자 이름<br>[!UICONTROL 작업 계획된 완료 날짜]<br><strong>[!UICONTROL 승인 결정]</strong> 버튼 <br>*총 보류 중인 작업 승인 수<br>*링크 대상 <strong>[!UICONTROL 작업 승인 *모든 승인 참조]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 위임한 문제 승인을 검토해야 합니다.</strong> </p> <p>문제 승인이 위임되었으므로 검토해야 합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 위임된 문제 승인 - 검토] &lt;issue name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>승인을 요청한 사용자의 이름입니다<br>문제를 승인하는 사용자의 이름입니다<br>승인 보류 중 상태<br>승인 요청 날짜 및 시간<br>문제 우선순위<br>승인 단계<br>승인자 이름<br>출고 계획 완료 일자<br>기본 연락처<br><strong>[!UICONTROL 승인 결정]</strong> 버튼<br>*총 보류 중인 문제 승인 수<br>*링크 대상 <strong>[!UICONTROL Issue Approvals]</strong><br><strong>[!UICONTROL *모든 승인 참조]</strong> 버튼<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>나에게 문제가 할당되었습니다.</strong> </p> <p>문제 할당자가 전자 메일 알림을 받습니다. 문제 할당자가 문제 상태가 [!UICONTROL Closed]와 일치하거나 인 경우 이메일을 받지 않습니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 새 작업 요청]: &lt;issue name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>문제 이름<br>프로젝트 이름<br>[!UICONTROL Issue Reference Number]<br>사용자 이름<br>발행 기한([!UICONTROL 계획된 완료 날짜])<br>문제를 자신에게 할당한 사용자의 이름입니다<br><strong>[!UICONTROL Work On It]</strong> 버튼<br>*총 할당 수<br>*사용자에게 할당된 총 작업 및 문제 수<br>*링크 대상 <strong>[!UICONTROL Work Requests]</strong><br>*일별 다이제스트 날짜<br></p> </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>나는 작업의 기본 피할당자로 설정되었습니다.</strong> </p> <p>할당자가 할당한 사용자가 아닌 경우 임무 할당자가 해당 작업의 주요 할당자로 지정된 경우 이메일 통지를 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 작업이 [!UICONTROL Complete]로 표시되지 않으면 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 또는 [!UICONTROL Requestor] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 새 작업 요청]: &lt;task name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>사용자 이름<br>작업 기한([!UICONTROL 계획된 완료 날짜])<br>작업을 자신에게 할당한 사용자의 이름<br><strong>[!UICONTROL Work On It]</strong> 버튼<br>*사용자에게 할당된 총 작업 및 문제 수<br>*링크 대상 <strong>[!UICONTROL Work Requests]</strong>*일별 다이제스트 날짜 </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 팀이 새 작업 요청을 받습니다.</strong> </p> <p>팀이 새 작업 요청을 받으면 팀 구성원이 전자 메일 알림을 받습니다. (요청을 제출한 사용자가 팀의 구성원이면 알림을 받지 않습니다.)</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 작업 요청 상태가 [!UICONTROL New]인 경우에만 알림이 전송됩니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자가 알림을 받지 않습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 새 작업 요청]: &lt;request name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다. <em>[!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> 문제 이름<br>프로젝트 이름(요청 큐 이름)<br>문제 참조 번호<br>팀 이름<br>발행 만기 일자(계획 완료 일자)<br>요청을 제출한 사용자의 이름입니다<br><strong>[!UICONTROL Work On It]</strong> 버튼<br>*팀에 할당된 총 요청 수</p> <p>*작업 요청 이름</p> <p>[!UICONTROL *계획된 완료 날짜]</p> <p>*요청을 제출한 사용자의 이름입니다<br>*링크 대상 <strong>[!UICONTROL Team Requests]</strong><br>*일별 다이제스트 날짜 </p> <p><span class="preview">*팀 지정</span> </p> </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 다시 열렸습니다.</strong> </p> <p>작업표를 다시 연 사용자가 작업표 소유자도 아닌 경우 작업표 소유자가 작업표를 다시 열면 전자 메일 알림을 받습니다.</p> <p>작업표 상태가 [!UICONTROL Open]인 경우에만 전자 메일 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 작업표 다시 열림]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> 작업표를 다시 연 사용자의 이름입니다<br>작업표를 다시 연 날짜 및 시간<br>작업표 상태([!UICONTROL 다시 열림])<br>작업표에 기록된 총 시간<br>작업표에 기록된 초과 시간 수<br><strong>[!UICONTROL Review]</strong> 버튼 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 타임시트가 거부되었습니다.</strong> </p> <p>작업표를 거부한 사용자도 소유자가 아닌 경우 작업표가 거부되면 작업표 소유자가 전자 메일 알림을 받습니다.</p> <p>작업표 상태가 [!UICONTROL 거부됨]인 경우에만 전자 메일 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 작업표 거부됨]:&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </td> 
   <td> 작업표를 거부한 사용자의 이름입니다<br>작업표 상태([!UICONTROL 거부됨])<br>작업표가 거부된 날짜 및 시간<br><strong>[!UICONTROL Review]</strong> 버튼 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 액세스 권한을 요청했습니다.</strong> </p> <p>나한테 뭘 하라고 하니 켜라.</p> <p>프로젝트를 만드는 사람이 프로젝트에 액세스할 수 있습니다.</p> <p>사용자가 액세스를 요청할 때 알림을 받게 되는 이유입니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL은에 액세스해야 함] &lt;object name=""&gt;</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL 필요한 작업 다이제스트] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>액세스를 요청한 사용자의 이름<br>사용자가 요청하는 액세스 유형<br><strong>[!UICONTROL Grant] &lt;name of="" the="" access="" requested=""&gt; 액세스</strong> 및 <strong>[!UICONTROL 다른 액세스 권한 부여]</strong> 버튼<br>*총 대기 중인 액세스 요청 승인 수<br>*링크 대상 <strong>[!UICONTROL Access Request]</strong> 승인<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>인스턴트 및 일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 문서 업로드를 요청했습니다.</strong> </p> <p>사용자가 문서 업로드 요청을 받으면 문서 요청이 이메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [!UICONTROL은에서 제공하는 문서가 필요합니다. [!DNL Workfront].]</em></p> <p> <p>참고: 일별 다이제스트 이메일에 대해 이 알림을 구성할 수 없습니다.</p> </p> </td> 
   <td> 문서를 요청하는 사용자의 이름<br>문서를 업로드할 객체의 이름입니다<br><strong>[!UICONTROL 여기에 연결]</strong> 링크 </td> 
   <td><strong>인스턴트</strong> </td> 
  </tr> 
 </tbody> 
</table>
