---
title: 레코드 주석 관리
description: 레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 73f339b54985b725f265d582992a43b9f80dbd7c
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# 레코드 주석 관리

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.

레코드의 오른쪽 패널에는 다음 섹션이 표시됩니다.

* **댓글**: 사용자가 레코드에 추가하는 댓글과 답글을 표시합니다.
* **기록**: 사용자가 레코드 필드에 적용한 시스템 기록 변경 내용을 표시합니다. 자세한 내용은 [기록 섹션 개요](/help/quicksilver/planning/records/history-section-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

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
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 기여자, 라이트 또는 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 </a>에 대한 이상의 권한 보기 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드에 댓글을 달 때 고려 사항

* 레코드의 댓글 섹션에서 Workfront Planning의 레코드에 댓글 및 응답을 추가할 수 있습니다.

* 연결된 레코드에 추가된 댓글은 연결하려는 레코드에 표시되지 않습니다. 예를 들어 캠페인 레코드에 연결된 Workfront Planning 제품 레코드에 댓글을 다는 경우 해당 댓글은 Workfront Planning의 제품 레코드에만 표시되고 연결된 캠페인 레코드에는 표시되지 않습니다.

* 레코드와 다른 응용 프로그램의 개체 간의 연결로 생성된 Workfront Planning 레코드에 주석을 추가할 수 있습니다.

  예를 들어 Workfront 프로젝트를 Workfront Planning 레코드와 연결한 후 프로젝트 Workfront Planning 레코드에 주석을 달 수 있습니다. 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 다른 응용 프로그램의 연결된 객체에 추가된 주석은 Workfront Planning에서 표시되지 않으며 Workfront Planning의 연결된 객체에 추가된 주석은 다른 응용 프로그램에서 표시되지 않습니다.

  예를 들어 Workfront의 프로젝트에 추가된 댓글은 Workfront Planning의 캠페인에 연결된 동일한 프로젝트에 표시되지 않으며, Workfront Planning 프로젝트에 추가된 댓글은 Workfront에 표시되지 않습니다.

* 사용자에 태그를 지정하여 업데이트에 주의를 기울일 수 있습니다. 태그가 지정된 사용자가 인앱 알림이나 업데이트에 대한 이메일을 받지 않습니다. <!--this might change??-->

* 사용자에 태그를 지정하여 업데이트에 주의를 기울일 수 있습니다. 태그가 지정된 사용자는 업데이트에 대한 인앱 알림 또는 이메일 알림을 받습니다.

  >[!NOTE]
  >
  >   통합 경험 Adobe과 함께 온보딩된 고객의 사용자만 인앱 알림과 이메일 알림을 모두 받습니다. 회사에서 통합 경험 Adobe을 사용하는지 확인하려면 [Workfront에 통합 경험 Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)를 참조하십시오.

* 레코드에 업데이트를 추가하고 Workfront Planning의 다음 영역에서 변경 내역을 검토할 수 있습니다.

   * 레코드 세부 정보 페이지에서.
   * 보기에서 레코드 세부 정보 상자의

### 레코드에 대한 댓글 관리

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 기록 유형이 카드에 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.
레코드 유형 페이지가 열리고 해당 유형의 모든 레코드가 표시됩니다.

1. **보기** 드롭다운 메뉴에서 표 보기를 선택하십시오.
1. 테이블 보기에서 레코드 이름을 클릭합니다.

   레코드의 **세부 정보** 페이지가 열립니다. 주석(Comments) 영역은 기본적으로 오른쪽 패널에 열립니다.

1. (조건부) 기본적으로 오른쪽 패널이 열리지 않으면 오른쪽 상단의 **댓글 표시** ![](assets/show-comments-icon.png) 아이콘을 클릭하여 [댓글] 섹션을 엽니다.

1. **새 댓글** 상자에 댓글을 입력하세요.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >댓글을 입력하고 제출하기 전에 댓글 섹션에서 다른 곳으로 이동하면 로그오프한 후 다시 로그온한 후에도 페이지에서 댓글이 초안 모드로 유지됩니다. 주석에 추가된 모든 이미지도 초안에 저장됩니다. 초안은 7일 동안 저장되며 이후 삭제되며 복구할 수 없습니다. 초안 주석은 설명을 입력한 사용자만 볼 수 있습니다.

1. (선택 사항) 변경을 실행 취소하거나 재실행하려면 다음 단축키를 사용합니다.
   * 변경 내용을 취소하려면 CTRL+Z(Mac의 경우 ⌘+z)
   * CTRL+Y(Mac의 경우 ⌘+y) 를 눌러 변경 사항을 재실행합니다
1. (선택 사항 및 조건부) Workfront 인스턴스가 통합 경험 Adobe의 일부인 경우 **@**&#x200B;을(를) 추가한 다음 사용자 이름을 추가하여 업데이트에서 사용자를 태그 지정합니다. 자세한 내용은 이 문서의 [레코드 댓글에 대한 고려 사항](#considerations-about-commenting-on-a-record) 섹션을 참조하십시오.

1. (선택 사항) 리치 텍스트 도구 모음의 옵션을 사용하여 텍스트 서식을 지정하고, 업데이트에 이모지, 링크 또는 이미지를 추가하여 콘텐츠를 개선합니다.

1. 레코드에 주석을 계속 추가합니다.

   Workfront Planning 레코드를 포함하여 개체를 업데이트하는 방법에 대한 자세한 내용은 [작업 업데이트](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)를 참조하십시오.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![](assets/new-line-indicator-comments.png)

1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.

   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  

1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
   
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.

1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     

   ![](assets/search-box-for-comments-area.png)
     
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)

1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.

    ![](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
  
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 

    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

1. (선택 사항) 댓글의 오른쪽 상단에 있는 **자세히** 아이콘 ![](assets/more-menu.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭하여 댓글을 삭제합니다.
1. (선택 사항) **댓글 숨기기** 아이콘 ![](assets/hide-comments-icon.png)을 클릭하여 오른쪽 패널을 닫습니다.

## 내역 섹션 개요

레코드의 오른쪽 패널에 있는 [작업 내역] 섹션에서 레코드에 대한 변경 사항을 검토할 수 있습니다.

자세한 내용은 [기록 섹션 개요](/help/quicksilver/planning/records/history-section-overview.md)를 참조하십시오.
