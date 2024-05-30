---
title: 레코드 주석 관리
description: 레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# 레코드 주석 관리

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.

레코드의 오른쪽 패널에는 다음 섹션이 표시됩니다.

* **댓글**: 사용자가 레코드에 추가하는 댓글 및 답글을 표시합니다.
* **기록**: 사용자가 레코드 필드에 적용한 시스템 기록 변경 사항을 표시합니다. 자세한 내용은 [내역 섹션 개요](/help/quicksilver/maestro/records/history-section-overview.md).

## 레코드에 댓글을 달 때 고려 사항

* 레코드의 댓글 섹션에서 Workfront Planning의 레코드에 댓글 및 응답을 추가할 수 있습니다.

* 연결된 레코드에 추가된 댓글은 연결하려는 레코드에 표시되지 않습니다. 예를 들어 캠페인 레코드에 연결된 Workfront Planning 제품 레코드에 댓글을 다는 경우 해당 댓글은 Workfront Planning의 제품 레코드에만 표시되고 연결된 캠페인 레코드에는 표시되지 않습니다.

* 레코드와 다른 응용 프로그램의 개체 간의 연결로 생성된 Workfront Planning 레코드에 주석을 추가할 수 있습니다.

  예를 들어 Workfront 프로젝트를 Workfront Planning 레코드와 연결한 후 프로젝트 Workfront Planning 레코드에 주석을 달 수 있습니다. 자세한 내용은 [레코드 연결](/help/quicksilver/maestro/records/connect-records.md).

* 다른 응용 프로그램의 연결된 객체에 추가된 주석은 Workfront Planning에서 표시되지 않으며 Workfront Planning의 연결된 객체에 추가된 주석은 다른 응용 프로그램에서 표시되지 않습니다.

  예를 들어 Workfront의 프로젝트에 추가된 댓글은 Workfront Planning의 캠페인에 연결된 동일한 프로젝트에 표시되지 않으며, Workfront Planning 프로젝트에 추가된 댓글은 Workfront에 표시되지 않습니다.

* 사용자에 태그를 지정하여 업데이트에 주의를 기울일 수 있습니다. 태그가 지정된 사용자가 인앱 알림이나 업데이트에 대한 이메일을 받지 않습니다. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/maestro/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* 레코드에 업데이트를 추가하고 Workfront Planning의 다음 영역에서 변경 내역을 검토할 수 있습니다.

   * 레코드 세부 정보 페이지에서.
   * 보기에서 레코드 세부 정보 상자의

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront Planning에는 액세스 수준 제어가 없습니다. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 이상의 권한 보기</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### 레코드에 대한 댓글 관리

{{step1-to-maestro}}

마지막으로 액세스한 작업 공간은 기본적으로 열립니다.
1. 다음에서 표 보기 선택 **보기** 드롭다운 메뉴.
1. 테이블 보기에서 레코드 이름을 클릭합니다.

   레코드는 **세부 사항** 페이지가 열립니다. 주석(Comments) 영역은 기본적으로 오른쪽 패널에 열립니다.

1. (조건부) 기본적으로 오른쪽 패널이 열리지 않으면 **댓글 표시** ![](assets/show-comments-icon.png) 오른쪽 위 모서리에 있는 아이콘을 클릭하여 주석 섹션을 엽니다.

1. 에 주석 입력 시작 **새 댓글** 상자.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >댓글을 입력하고 제출하기 전에 댓글 섹션에서 다른 곳으로 이동하면 로그오프한 후 다시 로그온한 후에도 페이지에서 댓글이 초안 모드로 유지됩니다. 주석에 추가된 모든 이미지도 초안에 저장됩니다. 초안은 7일 동안 저장되며 이후 삭제되며 복구할 수 없습니다. 초안 주석은 설명을 입력한 사용자만 볼 수 있습니다.

1. (선택 사항) 변경을 실행 취소하거나 재실행하려면 다음 단축키를 사용합니다.
   * 변경 내용을 취소하려면 CTRL+Z(Mac의 경우 ⌘+z)
   * CTRL+Y(Mac의 경우 ⌘+y) 를 눌러 변경 사항을 재실행합니다
1. (선택 사항) 추가 **@** 뒤에 업데이트의 사용자를 태깅할 사용자 이름이 옵니다.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (선택 사항) 리치 텍스트 도구 모음의 옵션을 사용하여 텍스트 서식을 지정하고, 업데이트에 이모지, 링크 또는 이미지를 추가하여 콘텐츠를 개선합니다. 자세한 내용은 이 문서의 &quot;Workfront 업데이트에서 리치 텍스트 사용&quot; 섹션을 참조하십시오 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >다른 사용자가 업데이트하고 있는 동일한 항목에 주석을 제출하는 경우 새로운 주석을 알려주는 &quot;신규&quot; 표시기가 있는 빨간색 줄이 있습니다.
   >
   >표시기는 항목에 대한 댓글이 제출된 후에만 표시되며 댓글이 아직 작성된 경우에는 표시되지 않습니다.
   >
   >![](assets/new-line-indicator-comments.png)

1. 클릭 **제출** 를 클릭하여 레코드에 업데이트를 추가합니다.
1. (선택 사항) 주석을 편집하려면 **자세히** 메뉴 ![](assets/more-menu.png) 주석의 오른쪽 상단 모서리에서 을(를) 클릭한 다음 을(를) 클릭합니다 **편집**.

   >[!IMPORTANT]
   >
   >의견을 제출한 후 15분 이내에만 편집할 수 있습니다.

1. 주석의 정보를 편집하거나, 이미지를 추가 또는 제거하거나, 태그 지정된 사용자를 제거합니다. &quot;편집됨&quot; 표시기가 댓글 왼쪽에 추가됩니다.

   >[!TIP]
   >
   >현재 연도의 주석은 날짜 스탬프에 연도를 표시하지 않습니다. 타임스탬프를 마우스로 가리키면 연도를 포함한 전체 날짜가 표시됩니다.

1. (선택 사항 및 조건부) 기존 댓글을 검색하려면 의 오른쪽 위 모서리에 있는 검색 상자에 키워드를 입력하십시오. **댓글** 영역입니다.

   ![](assets/search-box-for-comments-area.png)

1. (선택 사항) **답변** 또는에서 댓글을 입력해 보십시오. **회신 추가...** 영역을 클릭하여 기존 댓글에 응답한 다음 위의 4-8단계를 수행합니다. <!--(**************accurate??***********)-->

1. (조건부 및 선택 사항) 다른 사용자가 주석을 추가하는 동안 주석 섹션의 표시 영역 외부에 표시되는 주석을 추가한 경우 **보기** 의 내부 **새 댓글 배너** 이 설명을 표시하려면 이 단추를 클릭하십시오.

   ![](assets/new-comments-banner-on-record.png)

   추가 주석이 화면 하단에 표시됩니다.

1. (선택 사항) **좋아요** 아이콘을 클릭하여 업데이트를 좋아하거나 읽은 것을 확인합니다. 아이콘이 좋아요 수로 업데이트됩니다.
1. (조건부 및 선택 사항) 댓글에 다른 사람을 포함한 경우 업데이트에 포함된 사용자의 아바타를 클릭하여 댓글이 공유된 사용자 목록을 표시합니다.
1. (선택 사항) **자세히** 아이콘 ![](assets/more-menu.png) 주석의 오른쪽 상단 모서리에서 다음 옵션 중 하나를 클릭하여 주석의 정보를 복사합니다.

   * **링크 복사**: 댓글에 대한 링크를 클립보드에 복사합니다.
   * **본문 복사**: 주석 텍스트가 클립보드에 복사됩니다.
   * **견적 회신**: 댓글의 콘텐츠를 새 회신에 복사합니다. 이미지는 복사된 응답에 포함되지 않습니다.

   자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (선택 사항) **자세히** 아이콘 ![](assets/more-menu.png) 주석의 오른쪽 상단 모서리에서 을(를) 클릭한 다음 을(를) 클릭합니다 **삭제** 주석을 삭제하려면 다음 작업을 수행하십시오.
1. (선택 사항) **댓글 숨기기** 아이콘 ![](assets/hide-comments-icon.png) 오른쪽 패널을 닫습니다.

## 내역 섹션 개요

레코드의 오른쪽 패널에 있는 [작업 내역] 섹션에서 레코드에 대한 변경 사항을 검토할 수 있습니다.

자세한 내용은 [내역 섹션 개요](/help/quicksilver/maestro/records/history-section-overview.md).
