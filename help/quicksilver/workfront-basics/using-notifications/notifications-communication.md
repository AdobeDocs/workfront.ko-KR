---
content-type: reference
navigation-topic: notifications
title: '알림: 통신'
description: 다음 알림은 사용자와 관련된 작업 항목에서 발생하는 업데이트 댓글과 같은 커뮤니케이션에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 고유한 이벤트 알림 활성화 또는 비활성화를 참조하십시오.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 2af2a1f7d1a4d0b06cf4e7bfd2b9997ff8b9a6bf
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 4%

---

# 알림: 통신

다음 알림은 사용자와 관련된 작업 항목에서 발생하는 업데이트 댓글과 같은 커뮤니케이션에 대해 알려줍니다. 수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>이러한 알림은 특정 항목에 게시된 모든 주석에 대해 알려줍니다. 이러한 이유로 모든 알림을 동시에 선택하거나 선택 취소하여 일별 다이제스트 이메일로 전달해야 합니다. 특정 댓글이 발생할 때만 알림을 받으려면 개별 알림을 즉시 전송할 수 있습니다.

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
   <td> <p><strong>누군가가 지시된 업데이트에 나를 포함시킵니다.</strong> </p> <p>지정 업데이트는 다음에 설명된 대로 사용자가 특히 업데이트에 다른 사용자를 포함하는 경우입니다. <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL 다른 사용자에게 태그 지정] 업데이트</a>.</p> <p>이 경우 지정 업데이트에 포함된 사용자는 업데이트에 대한 이메일 알림을 받습니다.</p> <p>전자 메일 알림은 사용자에게 객체에 대한 액세스 권한이 있는 경우에만 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL에서 사용자가 알고 싶어함]</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다. <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 업데이트가 수행된 개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지정 업데이트에 포함된 모든 사용자 및 팀의 이름<br>업데이트가 수행된 날짜 및 시간<br>지정 업데이트 텍스트<br><strong>[!UICONTROL Comment]</strong> 버튼<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜<br></td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 내 요청에 답글을 달았습니다.</strong> </p> <p>사용자가 작업 요청을 제출하고 다른 사용자가 해당 작업 요청에 응답하면 요청을 제출한 사용자가 이메일 알림을 받습니다.</p> <p>다음의 경우 이메일 알림이 전송되지 않습니다.</p> 
    <ul> 
     <li> <p>답장하는 사용자는 요청을 한 동일한 사용자입니다</p> </li> 
     <li> <p>사용자에게 메모를 볼 수 있는 액세스 권한이 없습니다</p> </li> 
    </ul><strong>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;request name=""&gt; on &lt;project name=""&gt; (참조#) &lt;request reference="" number=""&gt;)</em></strong> 일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자의 이름입니다<br>댓글을 작성한 날짜 및 시간<br>요청에 대한 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜<br></td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 요청에 댓글이 게시되었습니다.</strong> </p> <p>문제에 대한 기본 연락처는 [!UICONTROL Help Desk] 요청에 댓글이 게시될 때 해당 문제에 대한 기본 연락처도 아닌 전자 메일 알림을 받습니다.</p> <p>주석에 직접 포함된 모든 사용자도 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;request name=""&gt; on &lt;project name=""&gt; (참조#) &lt;request reference="" number=""&gt;)</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 요청 이름<br>프로젝트 이름<br>참조 번호<br>요청에 응답한 사용자의 이름입니다<br>댓글을 작성한 날짜 및 시간<br>요청에 대한 댓글 텍스트<br>*받은 총 댓글 수<br>*각 요청에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜<br></td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>내 문서에 댓글이 추가되었습니다.</strong> </p> <p>에 있는 문서의 소유자 [!DNL Adobe Workfront] 댓글을 게시한 사용자도 문서 소유자일 수 없는 한 문서에 댓글을 게시하면 전자 메일 알림을 받습니다.</p> <p>주석에 직접 포함된 모든 사용자도 이메일 알림을 받습니다.</p> <p>프로젝트 상태가 [!UICONTROL Current]인 경우에만 알림이 전송됩니다. </p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;request name=""&gt; on &lt;project name=""&gt; (참조#) &lt;request reference="" number=""&gt;)</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>문서 이름<br>프로젝트, 작업 또는 문제 이름<br>참조 번호<br>요청에 응답한 사용자의 이름입니다<br>댓글을 작성한 날짜 및 시간<br>문서에 대한 주석 텍스트</td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내가 속한 스레드에 주석을 남김</strong> </p> <p>스레드의 참여자와 직접 메시지에 포함된 사용자는 사용자가 스레드에 댓글을 달 때 이메일 알림을 받게 됩니다.</p> <p>알림을 받으려면 사용자에게 [!UICONTROL 보기] 액세스 권한이 있어야 합니다.</p> <p>다음 사용자는 알림을 받지 않습니다.</p> 
    <ul> 
     <li>직접 메시지에 포함된 팀</li> 
     <li>메모의 소유자</li> 
     <li>기본 연락처</li> 
    </ul> <p><strong>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL RE: 댓글 on] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;(참조#) &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> 일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> 개체 이름<br>상위 개체 이름<br>스레드에 댓글을 달았던 사용자의 이름입니다<br>스레드에서 만들어진 주석 텍스트입니다<br>댓글을 작성한 날짜 및 시간<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가 내 작업 항목 중 하나에 댓글을 남겼습니다.</strong> </p> <p>작업 항목의 할당자는 사용자가 작업 항목에 업데이트를 추가할 때마다 전자 메일 알림을 받습니다. 단, 업데이트를 추가하는 사용자가 할당자이기도 합니다. </p> <p>요청에 댓글이 게시되면 문제 주요 연락처에 이메일로 보냅니다.</p> <p>문제에 대한 기본 연락처는 댓글을 게시한 사용자도 문제에 대한 기본 연락처가 아닌 한, 요청에 댓글을 게시하면 이메일 알림을 받습니다.</p> <p>주석에 직접 포함된 모든 사용자도 이메일 알림을 받습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>[!UICONTROL Comment on] &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 작업 항목 이름<br>프로젝트 이름<br>작업 항목 참조 번호<br>작업 항목에 주석을 표시한 사용자의 이름입니다<br>작업 항목에 대한 설명 텍스트<br>댓글을 작성한 날짜 및 시간<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>누군가가 지시된 업데이트에 내 팀을 포함시킵니다.</strong> </p> <p>지정 업데이트는 다음에 설명된 대로 사용자가 특히 업데이트에 다른 사용자를 포함하는 경우입니다. <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">업데이트에 다른 사용자에게 태그 지정</a>.</p> <p>이 경우 지정 업데이트에 포함된 팀의 구성원은 업데이트에 대한 이메일 알림을 받습니다.</p> <p>전자 메일 알림은 객체에 대한 액세스 권한이 있는 사용자에게만 전송됩니다.</p> <p>지정 업데이트를 보내는 사용자가 포함될 팀의 구성원인 경우 업데이트를 보내는 사용자는 이메일 알림을 받지 않습니다.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. [!UICONTROL Comment on] &lt;object name=""&gt; on &lt;parent object="" name=""&gt; (참조#) &lt;object reference="" number=""&gt;)</p> <p> 일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>개체 이름<br>상위 개체 이름<br>개체 참조 번호<br>지정 업데이트를 수행한 사용자의 이름입니다<br>지정 업데이트에 포함된 모든 팀 및 사용자의 이름입니다<br>지정 업데이트가 수행된 날짜 및 시간<br>지정 업데이트 텍스트<br><strong>[!UICONTROL Comment]</strong> 버튼<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*프로젝트 이름<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜 </p> </td> 
   <td><strong>일별</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>사용자에게 댓글이 추가되었을 때</strong> </p> <p>사용자 개체의 [!UICONTROL 업데이트] 탭에서 사용자에게 주석을 달 수 있습니다. 사용자의 설정을 편집할 때 사용자에게 주석을 달 수도 있습니다. 댓글이 작성되는 사용자는 이 댓글에 대해 알리는 이메일을 받게 됩니다. </p> <p>사용자의 [!UICONTROL Updates] 탭에 업데이트를 입력하려면 사용자에게 최소 [!UICONTROL 보기]에 대한 권한이 있어야 합니다. 사용자의 설정을 편집하려면 사용자에게 [!UICONTROL 편집] 권한이 있어야 합니다. </p> <p>업데이트 탭에서 사용자에 대한 의견을 작성하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">작업 업데이트</a>.</p> <p>사용자의 설정을 편집할 때 사용자에게 주석을 입력하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>.</p> <p>인스턴트 알림 이메일의 제목은 다음과 같습니다. <em>&lt;user name=""&gt; [!UICONTROL에서 사용자가 알고 싶어함]</em></p> <p>일별 다이제스트 알림의 주제는 다음과 같습니다.<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 사용자 이름<br>댓글을 추가한 사용자의 이름입니다<br>주석의 텍스트<br>댓글을 작성한 날짜 및 시간<br>*받은 총 댓글 수<br>*각 개체에 대해 받은 댓글 수<br>*<strong>[!UICONTROL 모든 알림 보기]</strong> 버튼<br>*일별 다이제스트 날짜 </td> 
   <td> <p><strong>인스턴트</strong> </p> <p><strong>및 일별</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
