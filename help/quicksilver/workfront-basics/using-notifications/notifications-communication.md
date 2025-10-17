---
content-type: reference
navigation-topic: notifications
title: '알림: 커뮤니케이션'
description: 다음 알림은 관련된 작업 항목에서 발생하는 업데이트 댓글 등의 통신에 대해 경고합니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# 알림: 커뮤니케이션

다음 알림은 관련된 작업 항목에서 발생하는 업데이트 댓글 등의 통신에 대해 경고합니다. 받는 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

>[!NOTE]
>
>이러한 알림은 특정 항목에 게시된 모든 댓글에 대해 알려줍니다. 따라서 일별 요약 이메일로 배달할 모든 알림을 동시에 선택하거나 선택 해제해야 합니다. 특정 댓글이 발생할 때만 알림을 받으려면 개별 알림을 즉시 전달하도록 지정할 수 있습니다.

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
   <td> <p><strong>누군가가 지시된 업데이트에 나를 포함시킵니다.</strong> </p> <p><a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] updates</a>에 설명된 대로 사용자가 업데이트에 다른 사용자를 특별히 포함하는 것이 지시된 업데이트입니다.</p> <p>이 경우, 지시된 업데이트에 포함된 사용자는 업데이트에 대한 이메일 알림을 수신한다.</p> <p>사용자에게 오브젝트에 대한 액세스 권한이 있는 경우에만 이메일 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;업데이트에 귀하를 포함한 사용자 이름&gt; [!UICONTROL 이 귀하가 알기를 원했습니다]</em></p> <p>일별 요약 알림의 주제는 <em>[!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 업데이트가 이루어진 개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지정 업데이트에 포함된 모든 사용자 및 팀의 이름<br>업데이트가 이루어진 날짜 및 시간<br>지정 업데이트의 텍스트<br><strong>[!UICONTROL 댓글]</strong> 단추<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜<br></td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내 요청에 답글을 남김</strong> </p> <p>사용자가 작업 요청을 제출하고 다른 사용자가 해당 작업 요청에 응답하면 요청을 제출한 사용자가 이메일 알림을 받습니다.</p> <p>다음과 같은 경우에는 이메일 알림이 전송되지 않습니다.</p> 
    <ul> 
     <li> <p>답글을 달 사용자는 요청을 한 사용자와 동일합니다</p> </li> 
     <li> <p>사용자에게 메모 보기 액세스 권한이 없습니다.</p> </li> 
    </ul><strong>인스턴트 알림 전자 메일의 제목은 <em>[!UICONTROL Comment on] &lt;Project Name&gt;(ref# &lt;Request Reference Number&gt;)의 &lt;Request Name&gt;</em></strong>입니다. 일별 요약 알림의 제목은 <em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em>입니다.</td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자 이름<br>댓글이 작성된 날짜와 시간<br>요청에 대해 작성된 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 요청에 댓글이 게시되었습니다</strong> </p> <p>댓글을 게시한 사용자가 문제에 대한 기본 연락처이기도 하지 않는 한 문제에 대한 기본 연락처는 [!UICONTROL 헬프 데스크] 요청에 댓글이 게시될 때 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;Project Name&gt;(ref# &lt;Request Reference Number&gt;)</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자 이름<br>댓글이 작성된 날짜와 시간<br>요청에 대해 작성된 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜<br></td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 문서에 댓글이 추가되었습니다</strong> </p> <p>[!DNL Adobe Workfront]의 문서 소유자는 댓글을 게시한 사용자가 문서 소유자가 아닌 한 문서에 댓글이 게시될 때 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다. </p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;Project Name&gt;(ref# &lt;Request Reference Number&gt;)</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td>문서 이름<br>프로젝트, 작업 또는 문제 이름<br>참조 번호<br>요청에 응답한 사용자 이름<br>의견이 작성된 날짜 및 시간<br>문서에 작성된 의견 텍스트</td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내가 있는 스레드에 누군가 댓글을 남겼습니다</strong> </p> <p>스레드의 참여자와 다이렉트 메시지에 포함된 사용자는 사용자가 스레드에서 댓글을 달면 이메일 알림을 받습니다.</p> <p>알림을 받으려면 사용자에게 [!UICONTROL 보기] 액세스 권한이 있어야 합니다.</p> <p>다음 사용자는 알림을 받지 않습니다.</p> 
    <ul> 
     <li>다이렉트 메시지에 포함된 팀</li> 
     <li>메모 소유자</li> 
     <li>기본 담당자</li> 
    </ul> <p><strong>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL RE: Comment on] &lt;Object Name&gt;&lt;Object Type&gt; on &lt;Project Name&gt;(ref# &lt;Object Reference Number&gt;</em>)</strong> </p> <p><strong> 일별 요약 알림의 제목:<em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em></strong> </p> </td> 
   <td> 개체 이름<br>상위 개체 이름<br>스레드에 주석을 단 사용자의 이름<br>스레드에 주석을 단 사용자의 이름<br>주석을 단 날짜 및 시간<br>*총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내 작업 항목 중 하나에 댓글을 남겼습니다</strong> </p> <p>작업 항목에 업데이트를 추가하는 사용자가 할당자도 아닌 경우 작업 항목의 할당자는 사용자가 작업 항목에 업데이트를 추가할 때마다 이메일 알림을 받습니다. </p> <p>요청에 댓글이 게시되면 문제 기본 담당자에게 이메일을 보내십시오.</p> <p>댓글을 게시한 사용자가 문제에 대한 기본 연락처이기도 하지 않는 한, 문제에 대한 기본 연락처는 요청에 댓글이 게시될 때 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;Project Name(ref# &lt;Work Item Reference Number&gt;)</em></p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 작업 항목 이름<br>프로젝트 이름<br>작업 항목 참조 번호<br>작업 항목에 댓글을 단 사용자의 이름<br>작업 항목에 대한 댓글의 텍스트<br>댓글이 작성된 날짜와 시간<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 표시]</strong> 단추<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 지시된 업데이트에 내 팀을 포함시킵니다</strong> </p> <p><a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자 태그 지정</a>에 설명된 대로 사용자가 특별히 업데이트에 다른 사용자를 포함하는 경우 지정 업데이트가 수행됩니다.</p> <p>이 경우 지시된 업데이트에 포함된 팀의 모든 구성원이 업데이트에 대한 이메일 알림을 받습니다.</p> <p>이메일 알림은 오브젝트에 대한 액세스 권한이 있는 사용자에게만 전송됩니다.</p> <p>지시된 업데이트를 전송하는 사용자가 포함된 팀의 멤버인 경우 업데이트를 전송하는 사용자가 이메일 알림을 받지 못합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. [!UICONTROL Comment on] &lt;Object name&gt; on &lt;Parent Object Name&gt;(ref# &lt;Object Reference Number&gt;)</p> <p> 일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> <p>개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지정 업데이트를 수행한 사용자의 이름<br>지정 업데이트에 포함된 모든 팀 및 사용자의 이름<br>지정 업데이트가 수행된 날짜 및 시간<br>지정 업데이트의 텍스트<br><strong>[!UICONTROL 댓글]</strong> 단추<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜 </p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>댓글이 사용자에 추가되었을 때</strong> </p> <p>사용자 개체의 [!UICONTROL 업데이트] 탭에서 사용자에 대한 댓글을 달 수 있습니다. 사용자의 설정을 편집할 때 사용자에 대한 댓글을 달 수도 있습니다. 댓글이 작성되는 사용자는 이 댓글을 알리는 이메일을 받게 됩니다. </p> <p>사용자의 [!UICONTROL 업데이트] 탭에 업데이트를 입력하려면 적어도 [!UICONTROL 보기]에 대한 권한이 있어야 합니다. 사용자 설정을 편집하려면 사용자에 대한 [!UICONTROL 편집] 권한이 있어야 합니다. </p> <p>업데이트 탭에서 사용자에 대한 댓글을 작성하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">작업 업데이트</a>를 참조하십시오.</p> <p>사용자의 설정을 편집할 때 사용자에 대한 댓글을 입력하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>을 참조하십시오.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>&lt;사용자 이름&gt; [!UICONTROL 이 알기를 원했습니다]</em></p> <p>일별 요약 알림의 주제는 <em> [!UICONTROL Digest of Communication] &lt;일별 요약 날짜&gt;</em>입니다.</p> </td> 
   <td> 사용자 이름<br>댓글을 추가한 사용자의 이름<br>댓글이 작성된 날짜와 시간<br>댓글이 작성된 날짜와 시간<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 다이제스트 날짜 </td> 
   <td> <p><strong>즉시</strong> </p> <p><strong>및 매일</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
