---
title: 레코드 댓글 관리
description: 레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Systems Workfront Planning 레코드에 대해 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대한 다른 변경 사항과 시스템에 의해 기록된 변경 사항도 볼 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 0%

---

# 레코드 댓글 관리

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Systems Workfront Planning 레코드에 대해 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대한 다른 변경 사항과 시스템에 의해 기록된 변경 사항도 볼 수 있습니다.

레코드의 오른쪽 패널에는 다음 섹션이 표시됩니다.

* **댓글**: 사용자가 레코드에 추가한 댓글 및 답글을 표시합니다.
* **기록**: 사용자가 레코드 필드에 대해 수행하는 시스템 기록 변경 사항을 표시합니다. 자세한 내용은 기록 섹션 개요를[ 참조하세요](/help/quicksilver/planning/records/history-section-overview.md).

## 액세스 요구 사항

+++ 액세스 요구 사항을 보려면 확장합니다.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 제품</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td> 
   <td> 
<p>어떤 </p> 
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩되어 있어야 합니다.</p> 
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td> 
   <td><p> Contributor 이상 라이선스</p>
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Systems Workfront Planning에 대한 액세스 수준 컨트롤은 없습니다</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 사용 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류에 대한 보기 이상의 권한</a> </p>  
   <p>시스템 관리자는 자신이 생성하지 않은 작업 영역을 포함하여 모든 작업 공간에 대한 권한을 갖습니다</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> Light 또는 Contributor 라이센스가 있는 사용자에게는 Planning이 포함된 레이아웃 템플릿 정보가 지정되어야 합니다.
   <p>표준 사용자 및 시스템 관리자는 기본적으로 계획 영역을 사용하도록 설정되어 있습니다.</p></div></li></ul>

</td>
  </tr>
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## 레코드에 주석 달기에 대한 고려 사항

* Workfront Planning의 레코드에 있는 [Comments] 섹션에서 레코드에 댓글 및 회신을 추가할 수 있습니다.

* 연결된 레코드에 추가된 설명은 연결하려는 원본 레코드에는 표시되지 않습니다. 예를 들어, Campaign 레코드에 연결된 Workfront Planning 제품 레코드에 주석을 추가하는 경우 해당 주석은 Workfront Planning의 제품 레코드에만 표시되고 연결 중인 Campaign 레코드에는 표시되지 않습니다.

* 레코드와 다른 애플리케이션의 개체 간의 연결의 결과로 생성된 Workfront Planning 레코드에 댓글 추가할 수 있습니다.

  예를 들어, Workfront 프로젝트를 Workfront Planning 레코드와 연결한 후 Project Workfront Planning 레코드에 주석을 달 수 있습니다. 자세한 내용은 레코드[ 연결을 참조하세요](/help/quicksilver/planning/records/connect-records.md).

* 다른 응용 프로그램에서 연결된 개체에 추가된 설명은 Workfront Planning에 표시되지 않으며 Workfront Planning에서 연결된 개체에 추가된 댓글은 다른 응용 프로그램에 표시되지 않습니다.

  예를 들어, Workfront의 프로젝트에 추가된 댓글은 Workfront Planning의 캠페인에 연결된 동일한 프로젝트에 표시되지 않으며, 프로젝트 Workfront Planning 레코드에 추가된 댓글은 Workfront에 표시되지 않습니다.

* 사용자 또는 팀이 업데이트에 주의를 기울이도록 태그 지정할 수 있습니다. 개별적으로 태그가 지정된 사용자와 태그 지정됨 팀의 사용자 모두 인앱 알림 및 업데이트에 대한 이메일을 받습니다.

  >[!NOTE]
  >
  >   Adobe Systems 통합 경험으로 온보딩한 고객의 사용자만 인앱 알림과 이메일 알림을 모두 받습니다. 회사에서 Adobe Systems Unified Experience를 사용하고 있는지 확인하려면 Adobe Systems Unified Experience for Workfront[를 참조하십시오](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* 레코드에 업데이트를 추가하고 Workfront Planning의 다음 영역에서 변경 내역을 검토할 수 있습니다.

   * 레코드 세부 정보 페이지에서.
   * 보기에서 레코드 세부 정보 상자에서.

### 레코드에 대한 댓글 관리

{{step1-to-planning}}

1. 작업 영역 카드 클릭

   작업 영역 영역이 열리고 레코드 종류가 카드에 표시됩니다.

1. 레코드 종류 카드 클릭
레코드 유형 페이지 가 열리고 해당 유형의 모든 레코드가 표시됩니다.

1. [보기&#x200B;**] 드롭다운 메뉴에서 테이블 보기를**&#x200B;선택합니다.
1. 테이블 뷰에서 레코드의 이름을 클릭합니다.

   레코드의 **세부 정보** 페이지 페이지가 열립니다. [주석] 영역은 기본적으로 오른쪽 패널에서 열립니다.

1. (조건부) 오른쪽 패널이 기본적으로 열리지 않으면 오른쪽 상단 모서리에 있는 주석&#x200B;****&#x200B;보기 보기 댓글 표시 아이콘![ 아이콘을 클릭하여 ](assets/show-comments-icon.png)주석 섹션을 엽니다.

1. 시작 새로 만들기 설명&#x200B;**상자에 설명을**&#x200B;입력합니다.

   ![레코드의 빈 주석 상자](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >주석 입력을 마치고 제출하기 전에 주석 섹션에서 벗어나면 로그오프했다가 다시 로그온한 후 페이지 주석이 초안 모드로 균일 유지됩니다. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (선택 사항) 변경을 실행 취소하거나 재실행하려면 다음 바로 가기 키를 사용합니다.
   * CTRL + Z(⌘Mac의 경우 +z)를 사용하여 변경 사항을 실행 취소합니다.
   * CTRL + Y(⌘Mac의 경우 +y)를 눌러 변경 사항을 다시 실행합니다.
1. (선택 사항 및 조건부) Workfront 인스턴스가 Adobe Systems Unified Experience의 일부인 경우 @**다음에 사용자 또는 팀 이름을 추가하여**&#x200B;업데이트에서 태그 지정합니다. 자세한 내용은 이 문서의 레코드[에 주석을 달 때 고려 사항 섹션을 ](#considerations-about-commenting-on-a-record)참조하세요.

1. (선택 사항) 리치 텍스트 도구 모음의 옵션을 사용하여 텍스트를 포맷하거나, 이모티콘을 추가하거나, 업데이트에 대한 링크를 추가하여 컨텐츠 향상시킬 수 있습니다.

   >[!TIP]
   >
   >레코드 댓글에는 이미지를 추가할 수 없습니다.


1. 레코드에 댓글 추가 계속.

   Workfront Planning 레코드를 포함한 객체 업데이트에 대한 자세한 내용은 작업[ 업데이트 섹션을 참조하세요](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (선택 사항) **댓글의 오른쪽 상단 모서리에 있는 자세히** 아이콘 ![더 메뉴를](assets/more-menu.png) 클릭한 다음 삭제를&#x200B;**클릭하여**&#x200B;댓글을 삭제합니다.
1. (선택 사항) **[댓글** 숨기기] 아이콘 ![[댓글 숨기기] 아이콘을](assets/hide-comments-icon.png) 클릭하여 오른쪽 패널을 닫습니다.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## 기록 섹션 개요

레코드의 오른쪽 패널에 있는 [작업 내역] 섹션에서 레코드에 대한 변경 사항을 검토할 수 있습니다.

자세한 내용은 기록 섹션 개요를[ 참조하세요](/help/quicksilver/planning/records/history-section-overview.md).
