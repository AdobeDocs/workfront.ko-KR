---
content-type: reference
navigation-topic: notifications
title: '알림: 통신'
description: 다음 알림은 관련된 작업 항목에서 발생하는 업데이트 댓글 등의 통신에 대해 경고합니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 4%

---

# 알림: 커뮤니케이션

다음 알림은 관련된 작업 항목에서 발생하는 업데이트 댓글 등의 통신에 대해 경고합니다. 수신하는 알림 구성에 대한 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>이러한 알림은 특정 항목에 게시된 모든 댓글에 대해 알려줍니다. 따라서 일별 요약 이메일로 배달할 모든 알림을 동시에 선택하거나 선택 해제해야 합니다. 특정 댓글이 발생할 때만 알림을 받으려면 개별 알림을 즉시 전달하도록 지정할 수 있습니다.

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
   <td> <p><strong>누군가가 지시된 업데이트에 나를 포함시킵니다.</strong> </p> <p>지시된 대로, 사용자가 업데이트에 다른 사용자를 구체적으로 포함하는 것입니다. <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL] 업데이트에 다른 사용자 태그 지정</a>.</p> <p>이 경우, 지시된 업데이트에 포함된 사용자는 업데이트에 대한 이메일 알림을 수신한다.</p> <p>사용자에게 오브젝트에 대한 액세스 권한이 있는 경우에만 이메일 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL이 귀하가 알기를 원했습니다]</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다. <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 업데이트가 이루어진 개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지시된 업데이트에 포함된 모든 사용자 및 팀의 이름<br>업데이트 날짜 및 시간<br>방향성 업데이트 텍스트<br><strong>[!UICONTROL Comment]</strong> 단추<br>*받은 총 댓글 수<br>*각 오브젝트에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜<br></td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 내 요청에 답글을 달았습니다.</strong> </p> <p>사용자가 작업 요청을 제출하고 다른 사용자가 해당 작업 요청에 응답하면 요청을 제출한 사용자가 이메일 알림을 받습니다.</p> <p>다음과 같은 경우에는 이메일 알림이 전송되지 않습니다.</p> 
    <ul> 
     <li> <p>답글을 달 사용자는 요청을 한 사용자와 동일합니다</p> </li> 
     <li> <p>사용자에게 메모 보기 액세스 권한이 없습니다.</p> </li> 
    </ul><strong>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 댓글] &lt;request name=""&gt; 날짜 &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> 일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자의 이름<br>댓글이 작성된 날짜 및 시간<br>요청에 대한 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 요청에 댓글이 게시되었습니다.</strong> </p> <p>댓글을 게시한 사용자가 문제에 대한 기본 연락처이기도 하지 않는 한 문제에 대한 기본 연락처는 [!UICONTROL 헬프 데스크] 요청에 댓글이 게시될 때 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 댓글] &lt;request name=""&gt; 날짜 &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자의 이름<br>댓글이 작성된 날짜 및 시간<br>요청에 대한 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜<br></td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 문서에 댓글이 추가되었습니다.</strong> </p> <p>의 문서 소유자 [!DNL Adobe Workfront] 문서에 댓글을 게시한 사용자가 문서 소유자도 아닌 한, 문서에 댓글이 게시되면 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다. </p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 댓글] &lt;request name=""&gt; 날짜 &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>문서 이름<br>프로젝트, 작업 또는 문제 이름<br>참조 번호<br>요청에 응답한 사용자의 이름<br>댓글이 작성된 날짜 및 시간<br>문서에 작성된 댓글의 텍스트</td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내가 속한 스레드에 주석을 남김</strong> </p> <p>스레드의 참여자와 다이렉트 메시지에 포함된 사용자는 사용자가 스레드에서 댓글을 달면 이메일 알림을 받습니다.</p> <p>알림을 받으려면 사용자에게 [!UICONTROL 보기] 액세스 권한이 있어야 합니다.</p> <p>다음 사용자는 알림을 받지 않습니다.</p> 
    <ul> 
     <li>다이렉트 메시지에 포함된 팀</li> 
     <li>메모 소유자</li> 
     <li>기본 담당자</li> 
    </ul> <p><strong>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL RE: Comment on] &lt;object name=""&gt;&lt;object type=""&gt; 날짜 &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> 일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> 개체 이름<br>상위 개체 이름<br>스레드에 주석을 단 사용자의 이름<br>스레드에 대한 댓글 텍스트<br>댓글이 작성된 날짜 및 시간<br>*받은 총 댓글 수<br>*각 오브젝트에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내 작업 항목 중 하나에 댓글을 남겼습니다.</strong> </p> <p>작업 항목에 업데이트를 추가하는 사용자가 할당자도 아닌 경우 작업 항목의 할당자는 사용자가 작업 항목에 업데이트를 추가할 때마다 이메일 알림을 받습니다. </p> <p>요청에 댓글이 게시되면 문제 기본 담당자에게 이메일을 보내십시오.</p> <p>댓글을 게시한 사용자가 문제에 대한 기본 연락처이기도 하지 않는 한, 문제에 대한 기본 연락처는 요청에 댓글이 게시될 때 이메일 알림을 받습니다.</p> <p>댓글에 직접 포함된 모든 사용자에게는 이메일 알림도 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL 댓글] &lt;work item="" name=""&gt; 날짜 &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> 일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 항목 이름<br>프로젝트 이름<br>작업 항목 참조 번호<br>작업 항목에 주석을 단 사용자의 이름<br>작업 항목에 대한 댓글의 텍스트<br>댓글이 작성된 날짜 및 시간<br>*받은 총 댓글 수<br>*각 오브젝트에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 지시된 업데이트에 내 팀을 포함시킵니다.</strong> </p> <p>지시된 대로, 사용자가 업데이트에 다른 사용자를 구체적으로 포함하는 것입니다. <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자 태그 지정</a>.</p> <p>이 경우 지시된 업데이트에 포함된 팀의 모든 구성원이 업데이트에 대한 이메일 알림을 받습니다.</p> <p>이메일 알림은 오브젝트에 대한 액세스 권한이 있는 사용자에게만 전송됩니다.</p> <p>지시된 업데이트를 전송하는 사용자가 포함된 팀의 멤버인 경우 업데이트를 전송하는 사용자가 이메일 알림을 받지 못합니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. [!UICONTROL Comment on] &lt;object name=""&gt; 날짜 &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> 일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지시된 업데이트를 수행한 사용자의 이름<br>지시된 업데이트에 포함된 모든 팀 및 사용자의 이름<br>지시된 업데이트를 수행한 날짜 및 시간입니다<br>지시된 업데이트의 텍스트<br><strong>[!UICONTROL Comment]</strong> 단추<br>*받은 총 댓글 수<br>*각 오브젝트에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜 </p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>사용자에게 댓글이 추가되었을 때</strong> </p> <p>사용자 개체의 [!UICONTROL 업데이트] 탭에서 사용자에 대한 댓글을 달 수 있습니다. 사용자의 설정을 편집할 때 사용자에 대한 댓글을 달 수도 있습니다. 댓글이 작성되는 사용자는 이 댓글을 알리는 이메일을 받게 됩니다. </p> <p>사용자의 [!UICONTROL 업데이트] 탭에 업데이트를 입력하려면 적어도 [!UICONTROL 보기]에 대한 권한이 있어야 합니다. 사용자 설정을 편집하려면 사용자에 대한 [!UICONTROL 편집] 권한이 있어야 합니다. </p> <p>업데이트 탭에서 사용자에게 댓글을 다는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">작업 업데이트</a>.</p> <p>사용자 설정을 편집할 때 사용자에 대한 설명을 입력하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;user name=""&gt; [!UICONTROL이 귀하가 알기를 원했습니다]</em></p> <p>일별 요약 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 사용자 이름<br>댓글을 추가한 사용자의 이름<br>주석 텍스트<br>댓글을 작성한 날짜와 시간<br>*받은 총 댓글 수<br>*각 오브젝트에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 단추<br>*일별 요약 날짜 </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
