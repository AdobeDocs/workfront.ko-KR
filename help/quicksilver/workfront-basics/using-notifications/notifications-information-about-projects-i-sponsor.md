---
content-type: reference
navigation-topic: notifications
title: '알림: 내가 후원하는 프로젝트에 대한 정보'
description: 다음 알림은 후원 중인 프로젝트에서 발생하는 활동에 대해 경고합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 0%

---

# 알림: 내가 후원하는 프로젝트에 대한 정보

다음 알림은 후원 중인 프로젝트에서 발생하는 활동에 대해 경고합니다.

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
   <td> <p><strong>내가 후원하는 프로젝트에 문서가 추가됨</strong> </p> <p>문서가 프로젝트에 추가되면 프로젝트 스폰서가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]이고 문서가 [!UICONTROL Private]이 아닌 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문서가 &lt;프로젝트 이름&gt;</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Projects] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문서 참조 번호<br>문서를 추가한 사용자의 이름<br>문서 이름<br>날짜에 추가됨<br>문서 세부 정보(형식, 크기, 버전 번호)<br>문서 썸네일<br><strong>[!UICONTROL 미리 보기]</strong> 및 <strong>[!UICONTROL 다운로드]</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문서 수<br>*문서 이름<br>*문서를 추가한 사용자의 이름<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트에서 마일스톤 작업이 완료되었습니다</strong> </p> <p>프로젝트 스폰서는 자신이 후원하는 프로젝트에서 마일스톤 작업이 완료되면 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]: &lt;프로젝트 이름&gt;</em>의 &lt;작업 이름&gt;입니다.</p> <p>참고: 작업이 [!UICONTROL Complete]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL Complete]"가 표시됩니다.<br></p> <p>일별 요약 알림의 제목은 <em> 후원하는 프로젝트의 요약 &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>새 작업 상태<br>작업이 완료된 날짜 및 시간<br>이전 작업 상태<br><strong>[!UICONTROL 자세한 정보 보기]</strong> 단추 <br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트가 늦어지고 있습니다</strong> </p> <p>프로젝트가 지연되면 프로젝트 스폰서가 이메일 알림을 받습니다. 진행 상태가 "[!UICONTROL At Risk]" 또는 "[!UICONTROL In Trouble]"일 때 프로젝트가 일정보다 늦습니다.</p> <p>[!UICONTROL Review] 라이센스가 있는 사용자는 알림을 받지 못합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 프로젝트 진행 상황 변경]: &lt;프로젝트 이름&gt;</em>입니다.</p> <p>일별 요약 알림의 주제는 <em>[!UICONTROL Digest of Projects] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 진행 상태<br>프로젝트 [!UICONTROL 계획된 시작 일자]<br>프로젝트 [!UICONTROL 계획된 완료 일자]<br>프로젝트 [!UICONTROL 예상 시작 일자]<br>프로젝트 [!UICONTROL 예상 완료 일자]<br>프로젝트 완료율<br>프로젝트 상태<br>프로젝트 소유자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트 진행 상태<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트에서 작업이 완료되었습니다</strong> </p> <p>프로젝트 스폰서가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]: &lt;프로젝트 이름&gt;</em>의 &lt;작업 이름&gt;입니다.</p> <p> <p>참고: 작업이 [!UICONTROL Complete]와 동일한 상태로 변경되면 전자 메일의 제목에 여전히 "[!UICONTROL Complete]"가 표시됩니다.</p> </p> <p>일별 요약 알림의 제목은 <em> 후원하는 프로젝트의 요약 &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>작업을 완료한 사용자의 이름<br>작업 상태<br>작업 상태가 변경된 날짜와 시간<br>이전 작업 상태<br><strong>자세한 내용 보기</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 작업 수<br>*작업 이름<br>*작업을 완료한 사용자의 이름<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트의 작업이 지연되고 있습니다</strong> </p> <p>프로젝트의 작업이 지연되면 프로젝트 스폰서가 이메일 알림을 받습니다. 진행 상태가 "[!UICONTROL At Risk]" 또는 "[!UICONTROL Behind]" 또는 "[!UICONTROL Late]"일 때 작업이 지연되고 있습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 작업 진행 상황 변경]입니다. &lt;작업 이름&gt;</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Projects] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 이름<br>프로젝트 이름<br>작업 참조 번호<br>새 작업 진행 상태<br>작업 [!UICONTROL 계획된 시작 일자]<br>작업 [!UICONTROL 계획된 완료 일자]<br>작업 [!UICONTROL 예상 시작 일자]<br>작업 [!UICONTROL 예상 완료 일자]<br>작업 완료율<br>작업 상태<br>이름으로 할당<br>이름으로 입력<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*일정 뒤에 있는 총 작업 수<br>*작업 이름<br> 작업을 입력한 사용자의 이름<br>*일별 요약 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트에 문제가 추가됨</strong> </p> <p>프로젝트에 문제가 추가되면 프로젝트 스폰서가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL 문제가 &lt;프로젝트 이름&gt;</em></p> <p>일별 요약 알림의 주제는 <em>[!UICONTROL Digest of Projects] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름<br>문제 이름<br>문제 유형<br>날짜 입력<br>문제 우선 순위<br>이름 <br>문제 상태<br>기본 담당자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*프로젝트에 추가된 총 문제 수<br>*문제 이름<br>*문제에 할당된 사용자의 이름<br>*일일 다이제스트 날짜<br><br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트에서 문제가 완료되었습니다</strong> </p> <p>프로젝트 스폰서가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 완료]: &lt;프로젝트 이름&gt;</em>의 &lt;문제 이름&gt;입니다.</p> <p>일별 요약 알림의 제목은 <em> 후원하는 프로젝트의 요약 &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 문제 이름<br>프로젝트 이름<br>문제 참조 번호<br>문제를 완료한 사용자의 이름<br>문제 상태<br>문제가 완료된 날짜 및 시간<br>이전 문제 상태<br><strong>자세한 정보 보기</strong> 단추<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*완료된 총 문제 수<br>*문제 이름<br>*문제에 할당된 사용자의 이름<br>*일일 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 후원하는 프로젝트에 할당 해제된 문제가 추가됨</strong> </p> <p>미할당 문제가 프로젝트에 추가되면 프로젝트 스폰서가 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current] 또는 [!UICONTROL Planning]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL [&lt;프로젝트 이름&gt;]에서 이 새로운 문제를 누구에게 할당하시겠습니까?</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Projects] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 프로젝트 이름<br>Portfolio 이름<br>문제 참조 번호<br>문제를 추가한 사용자의 이름<br>문제 이름<br>문제 유형<br>날짜 입력<br>문제 우선 순위<br>이름 할당(빈)<br>문제 상태<br>기본 담당자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*추가된 총 문제 수<br>*문제 이름<br>*문제를 추가한 사용자의 이름<br>*일일 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트의 스폰서로 설정되었습니다</strong> </p> <p>프로젝트 스폰서가 프로젝트의 스폰서로 설정되면 이메일 알림을 받습니다.<br></p> <p>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL 프로젝트 스폰서]입니다. &lt;프로젝트 이름&gt;</em></p> <p>이메일 알림의 본문에는 다음 텍스트가 포함되어 있습니다.</p> <p><em>[!UICONTROL Hi] &lt;사용자 이름&gt;,</em> </p> <p><em>&lt;사용자를 프로젝트 스폰서로 할당한 사용자 이름&gt; [!UICONTROL이 사용자를] &lt;프로젝트 이름&gt;의 스폰서로 만들었습니다. [!UICONTROL 프로젝트 스폰서로서 프로젝트 활동에 대한 추가 이메일 알림을 받거나 프로젝트와 관련된 작업 승인에 참여할 수 있습니다. 즐거운 시간 보내세요.]</em> </p> <p>일별 요약 알림의 제목은 <em>후원하는 프로젝트의 요약 &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>프로젝트 이름<br>Portfolio 이름<br>프로젝트 참조 번호<br>프로젝트 계획 완료 일자<br>*프로젝트 이름<br>*프로젝트 참조 번호<br>*일별 다이제스트 날짜</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
 </tbody> 
</table>
