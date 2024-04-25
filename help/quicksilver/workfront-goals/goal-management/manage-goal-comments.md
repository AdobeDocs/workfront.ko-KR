---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 주석 관리
description: Adobe Workfront 목표에서 볼 수 있는 모든 목표에 주석을 추가할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Adobe Workfront 목표의 목표 주석 관리

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Adobe Workfront 목표에서 볼 수 있는 모든 목표에 주석을 추가할 수 있습니다.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront 플랜</td>
 <td>
 <p>임의</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront 라이선스</td>
 <td>
 <p>임의</td>
 </tr>
 <tr>
 <td role="rowheader">제품*</td>
 <td>
 <p> 새 제품 요구 사항: Select 또는 Prime Adobe Workfront 플랜이 있는 경우 추가 Adobe Workfront Goals 라이센스도 구입해야 합니다. Workfront 목표는 Ultimate Workfront 플랜에 포함되어 있습니다.</p>
 또는
 <p>현재 제품 요구 사항: 이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 목표에 대한 추가 라이선스를 구입해야 합니다. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">액세스 수준 구성</td>
 <td> <p>목표에 대한 보기 또는 상위 액세스</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 권한 보기 이상</p>
  <p>기본적으로 사용자는 목표에 대한 액세스 권한이 없습니다 </p>
 <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

시작하려면 먼저 다음 항목이 있어야 합니다.

* 메인 메뉴에 목표 영역을 포함하는 레이아웃 템플릿입니다.

## 목표 댓글 관리

목표 페이지의 업데이트 섹션에서 목표에 주석을 추가할 수 있습니다.

이 영역에서 귀하 또는 다른 사람이 추가한 댓글에 답글을 달거나 댓글을 달도록 할 수 있습니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) 오른쪽 상단 또는 **메인 메뉴** 아이콘 ![](assets/lines-main-menu.png) 왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **목표**.
이렇게 하면 목표 목록이 열립니다.
1. 주석을 추가할 목표를 찾은 다음 해당 이름을 클릭하여 목표 페이지를 엽니다.
1. 클릭  **업데이트** 왼쪽 패널에서
1. (선택 사항) 기존 설명을 찾으려면 키워드 입력을 시작합니다 <!--or a user's name--> 다음에서 **검색** 의 오른쪽 위 모서리에 있는 상자 **댓글** 탭.

   ![](assets/search-field-in-updates-tab-goals.png)

   키워드 <!--or user--> 을 검색하면 강조 표시되고 이 검색어가 포함된 주석이 업데이트 섹션의 맨 위에 표시됩니다.

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >댓글이나 답글에 포함된 단어를 검색해야 합니다. 태그가 지정된 사용자 또는 팀은 검색할 수 없습니다.

   자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. 다음을 클릭합니다. **x** 아이콘을 클릭하여 검색 결과를 지우고 전체 업데이트로 돌아갑니다.
1. 다음을 클릭합니다. **댓글** 업데이트 영역의 왼쪽 상단 모서리에 있는 탭입니다.
1. 에 주석 입력 시작 **새 댓글** 상자.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >댓글을 입력하고 제출하기 전에 업데이트 섹션에서 다른 곳으로 이동하면 로그오프했다가 다시 로그온한 후에도 페이지에서 댓글이 초안 모드로 유지됩니다. 주석에 추가된 모든 이미지도 초안에 저장됩니다. 초안은 7일 동안 저장되며 이후 삭제되며 복구할 수 없습니다. 초안 주석은 설명을 입력한 사용자만 볼 수 있습니다.

1. (선택 사항) 변경을 실행 취소하거나 재실행하려면 다음 단축키를 사용합니다.
   * 변경 내용을 취소하려면 CTRL+Z(Mac의 경우 ⌘+z)
   * CTRL+Y(Mac의 경우 ⌘+y) 를 눌러 변경 사항을 재실행합니다
1. (선택 사항) 업데이트, 하이퍼링크 또는 이미지에 서식 있는 텍스트 서식을 추가하려면 서식 있는 텍스트 도구 모음이나 옆에 있는 아이콘을 사용하십시오. 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (선택 사항) **사람 또는 팀에 태그 지정** 영역에 이 댓글에 포함할 사용자 또는 팀의 이름 또는 이메일을 입력한 다음 목록에 표시될 때 선택합니다.
1. 다음 항목 선택 **내 회사에 비공개** 회사 내 사용자에게만 댓글이 표시되도록 전환합니다.

   >[!TIP]
   >
   >업데이트 영역에서 이 옵션을 사용하려면 프로필에 회사를 지정해야 합니다.

1. 클릭 **제출**.

   >[!TIP]
   >
   >다른 사용자가 업데이트하고 있는 동일한 항목에 주석을 제출하는 경우 새로운 주석을 알려주는 &quot;New&quot; 표시기가 있는 빨간색 라인과 새 주석의 수를 표시하는 화면 하단에 파란색 알림이 있습니다.
   >
   >표시기는 항목에 대한 댓글이 제출된 후에만 표시되며 댓글이 아직 작성된 경우에는 표시되지 않습니다.
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. (선택 사항) 주석을 편집하려면 **자세히** 메뉴 ![](assets/more-icon.png) 좋아요 아이콘 오른쪽에 있는 **편집**.
1. 주석의 정보를 편집하거나, 이미지를 추가 또는 제거하거나, 태그 지정된 사용자를 제거합니다.
의견을 제출하고 15분 이내에 편집할 수 있습니다. 댓글이 업데이트될 때 표시되는 날짜 스탬프 왼쪽에 &quot;편집됨&quot; 표시기가 추가됩니다.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 원본 업데이트를 제출한 경우에만 사용자에게 업데이트를 알리는 이메일이 생성됩니다. 업데이트를 편집한 후 이메일이 생성되지 않습니다.
   >
   > * 날짜 스탬프는 원래 댓글의 날짜이며 최신 업데이트 날짜는 아닙니다.

1. (선택 사항) **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음, 다음 옵션 중 하나를 클릭하여 댓글의 정보를 클립보드나 새 회신에 복사합니다.

   * **링크 복사** 를 클릭하여 회신 없이 업데이트 링크를 복사합니다.
   * **본문 복사** 를 클릭하여 업데이트 텍스트를 복사합니다.
   * **견적 회신** 원래 댓글이 새 회신에서 인용되고 블록 인용으로 표시되는 새 댓글 상자를 엽니다.

     자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (선택 사항) **자세히** 메뉴 ![](assets/more-icon.png) 주석의 오른쪽에 있는 을(를) 클릭한 다음 **삭제** 주석을 삭제하려면 다음을 수행하십시오. 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (선택 사항) **답변** 기존 댓글에 회신하려면 위의 5-9단계를 따르십시오. 업데이트 회신에 대한 자세한 내용은 [업데이트에 대한 회신](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. (조건부 및 선택 사항) 다른 사용자가 업데이트 섹션의 표시 영역 외부에 표시되는 주석을 추가한 경우 **보기** 파란색 안쪽에 **새 댓글 배너** 이 설명을 표시하려면 이 단추를 클릭하십시오.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   추가 주석이 화면 하단에 표시됩니다.
1. (선택 사항) **좋아요** 아이콘![](assets/like-icon.png) 다른 사용자가 추가한 댓글을 좋아하도록 하는 것입니다. 아이콘이 좋아요 수로 업데이트됩니다.

1. (선택 사항) **시스템 활동** 시스템에 의해 기록된 업데이트를 보려면 탭하십시오. 목표가 업데이트되면 Workfront에서는 해당 업데이트에 대한 메모를 생성하고 시스템 활동 탭에 표시합니다. Workfront은 결과, 활동 또는 프로젝트가 목표에 추가되거나 업데이트될 때도 시스템 업데이트를 기록합니다. <!--ensure the casing on the tab has not changed-->


