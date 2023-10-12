---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드에서 연결된 카드 사용
description: Workfront의 기존 작업 및 문제에 연결된 카드를 보드에 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 99e985642fff751ac67a9de562908bd2156b3812
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---

# 보드에서 연결된 카드 사용

{{preview-and-fast-release}}

의 기존 작업 및 문제에 연결된 카드를 보드에 추가할 수 있습니다. [!DNL Workfront].

한 위치에서 카드에 대해 다음 세부 정보 중 하나가 업데이트되면 다른 위치에서 자동으로 업데이트됩니다.

* [!UICONTROL 이름]
* [!UICONTROL 설명]
* [!UICONTROL 할당자]
* [!UICONTROL 상태]
* [!UICONTROL 계획된 완료 일자]
* [!UICONTROL 예상] / [!UICONTROL 스토리 포인트]
* <span class="preview">[!UICONTROL 하위 작업]</span>
* <span class="preview">[!UICONTROL 문서]</span>

>[!NOTE]
>
>연결된 단일 작업 또는 문제는 보드당 한 번만 추가할 수 있습니다. 동일한 작업 또는 문제를 여러 보드에 연결할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td>
   <td><p>작업 및 문제에 대한 [!UICONTROL 보기] 이상 액세스</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>개체 권한</strong></td>
   <td><p>Workfront 작업 또는 문제에 대한 [!UICONTROL 보기] 이상 권한</p></td>
  </tr>
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 연결된 카드 추가

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 게시판]**.
1. 보드에 액세스합니다. 자세한 내용은 [보드 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md).
1. 클릭 **[!UICONTROL 카드 추가] > [!UICONTROL 연결된 카드]**.
1. 프로젝트를 선택한 다음 보드에 카드로 추가할 작업 또는 문제를 선택하십시오.

   여러 개체를 선택할 수 있으며, 이 개체는 모두 별도의 카드로 추가됩니다.

   >[!NOTE]
   >
   >* 사용 권한이 있는 개체만 검색 결과에서 사용할 수 있습니다. 항목이 흐리게 표시되면 보드에 이미 추가된 것입니다.
   >* 필터링 기준: **[!UICONTROL 내가 소유한 프로젝트]** 또는 **[!UICONTROL 내가 진행 중인 프로젝트]**, 완료, 중단 또는 거부됨 상태와 동일한 프로젝트는 포함되지 않습니다. 를 사용하여 해당 프로젝트를 계속 검색할 수 있습니다. **[!UICONTROL 모두]** 필터.

1. 클릭 **[!UICONTROL 추가]**.

   ![연결할 작업 또는 문제 검색](assets/boards-tasksissues-350x94.png)

   카드가 맨 왼쪽 열 하단에 추가됩니다. 연결됨 [!DNL Workfront] 객체와 해당 할당자가 카드에 표시됩니다.

   ![연결된 카드](assets/boards-connected-card-first-added.png)

1. 클릭 ![작업 또는 문제 열기](assets/boards-launch-icon.png) 을(를) 열려면 [!DNL Workfront] 새 브라우저 탭의 작업 또는 문제
1. 카드 세부 사항을 편집하려면 카드 이름 대신 카드를 클릭합니다.

   또는

   다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 카드에서 다음을 선택합니다. **[!UICONTROL 편집]**.

1. 다음에서 **[!UICONTROL 카드 세부 정보]** 상자에서 다음 정보를 추가하거나 업데이트합니다.

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 이름]</strong></td> 
      <td>이름을 변경하면 연결된 에서도 이름이 변경됩니다 [!DNL Workfront] 개체.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 설명]</strong></td> 
      <td>설명을 변경하면 연결된 항목에 대한 설명도 변경됩니다 [!DNL Workfront] 개체. 설명에 URL을 추가할 수 있으며 카드가 저장되면 클릭할 수 있는 링크가 됩니다.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 열]</strong></td>
      <td>카드 열을 선택합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상태]</strong></td>
      <td><p>카드 상태를 선택합니다. 기본값은 [!UICONTROL New], [!UICONTROL In Progress] 및 [!UICONTROL Complete]이지만 의 항목에 대해 정의된 모든 사용자 지정 상태입니다. [!DNL Workfront] 사용할 수도 있습니다.</p>
      <p>필드 값을 업데이트하기 위해 열 정책을 활성화한 경우 카드의 상태를 변경하면 카드가 자동으로 해당 열로 이동합니다. 자세한 내용은 문서의 "열 설정 및 정책 정의"를 참조하십시오 <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">보드 열 관리</a>.</p>
      <p>다음을 클릭: <strong>[!UICONTROL Mark Complete]</strong> 카드 상단에서 상태가 자동으로 완료로 변경됩니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 계획된 완료]</strong></td>
      <td>이 날짜를 변경하면 연결된 의 계획된 완료 날짜도 변경됩니다. [!DNL Workfront] 개체.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>카드를 완료할 시간입니다.</p><p>추정을 변경하면 연결된 항목의 스토리 포인트 값도 변경됩니다 [!DNL Workfront] 개체.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>카드에 더 많은 사람 또는 팀을 할당하려면 <strong>[!UICONTROL 할당 추가]</strong> 검색 필드에 이름을 입력하십시오. 그런 다음 결과 목록에 표시될 때 선택합니다. 개인 사용자와 팀을 모두 추가할 수 있습니다. 연결된 카드에는 팀 할당이 하나만 허용됩니다.</p>
      <p>선택한 모든 피할당자도 의 작업 또는 문제에 할당됩니다. [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 태그]</strong></td>
      <td><p>카드에 대한 태그를 검색하고 선택합니다.</p>
      <p>새 태그 만들기에 대한 내용은 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">태그 추가</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 사용자 정의 필드]</strong></td>
      <td><p>추가한 모든 사용자 정의 필드가 이 영역에 표시됩니다.</p>
      <p>자세한 내용은 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">카드에 표시할 필드 사용자 지정</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[!UICONTROL 하위 작업]</strong></span></td>
      <td><span class="preview"><p>작업에 대한 기존 하위 작업이 이 섹션에 표시됩니다. 클릭 <strong>[!UICONTROL 하위 작업 추가]</strong> 을 눌러 새 하위 작업을 추가합니다.</p>
      <p>섹션 맨 위에 있는 카운터는 완료된 하위 작업 수와 총 하위 작업 수를 보여 줍니다.</p>
      <p>하위 작업에 대한 자세한 내용은 <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">보드에서 하위 작업 관리</a>.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 검사 목록]</strong></td>
      <td><p>클릭 <strong>[!UICONTROL 체크리스트 항목 추가]</strong>. 그런 다음 항목의 제목을 입력하고 Enter 키를 누릅니다. 다른 항목이 자동으로 추가됩니다. 제목을 계속 입력하여 더 많은 항목을 추가합니다.</p>
      <p>체크리스트 상단의 카운터는 완료된 품목 수와 전체 품목 수를 보여준다.</p> <p>체크리스트 항목에 대한 자세한 내용은 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">카드의 체크리스트 항목 관리</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[!UICONTROL 문서]</strong></span></td>
      <td><span class="preview">기존 문서의 경우 문서 축소판 위로 마우스를 가져간 다음 <strong>미리 보기</strong> 브라우저에서 파일을 보려면 <strong>다운로드</strong> 를 클릭하여 파일을 컴퓨터에 다운로드합니다. 새 문서에 대해서는 다음을 참조하십시오. <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">카드에 문서 추가</a>.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 시간]</strong></td>
      <td>아래의 "연결된 카드에 시간 기록"을 참조하십시오.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>을(를) 클릭합니다. <strong>[!UICONTROL 새 주석]</strong> 필드에 댓글을 입력합니다. 서식 도구를 사용하여 텍스트 서식을 지정하고 <strong>첨부 파일 추가</strong> 아이콘 <img src="assets/attachment-icon.png" alt="첨부 파일 아이콘"> 파일을 주석에 첨부합니다. 사용자 또는 팀에 태그를 지정하려면 댓글 영역 하단에 있는 검색 상자를 사용합니다. 사용자는 보드에서 멤버일 필요가 없습니다. 연결된 카드에 태그가 지정된 사용자는 이메일 알림을 받게 됩니다.</p><p>클릭 <strong>[!UICONTROL Submit]</strong> 주석을 카드에 추가합니다.</p>
      <p><strong>참고:</strong> 카드의 주석 달기 영역에서는 새로운 Adobe Workfront 주석 달기 경험을 사용합니다. 자세한 내용은 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">작업 업데이트</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p>다음을 보유한 경우: <strong>시스템 활동</strong> 카드 섹션으로 활성화되면 활동이 이 영역에 표시됩니다.</p> <p>자세한 내용은 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">카드에 표시할 필드 사용자 지정</a> 및 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">시스템 추적 업데이트</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   왼쪽 탐색 패널을 사용하여 카드 세부 정보에서 필드의 섹션 사이를 이동합니다.

1. 클릭 **[!UICONTROL 닫기]** 게시판으로 돌아갑니다.
카드에 연결된 객체, 담당자, 태그, 기한, 체크리스트 카운터, 예상 시간, 상태 등이 표시됩니다.

   ![보드에 추가된 카드](assets/boards-connected-card-details-110922.png)

## 연결된 카드 분리

연결된 카드를 해당 Workfront 개체에서 연결 해제할 수 있으며 카드는 편집할 수 있는 임시 카드로 보드에 남아 있습니다.

보드 수준에서 연결을 끊으려면:

1. 보드에 액세스합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 연결된 카드에서 **[!UICONTROL 연결 해제]**.
1. 클릭 **[!UICONTROL 연결 해제]** 확인 메시지 표시.

카드 수준에서 연결을 끊으려면:

1. 보드에 액세스하여 연결된 카드를 엽니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![기타 메뉴](assets/more-icon-spectrum.png) 카드 세부 정보의 연결 영역에서 을(를) 선택한 다음 **[!UICONTROL 연결 해제]**.
1. 클릭 **[!UICONTROL 연결 해제]** 확인 메시지 표시.

## Ad Hoc 카드를 연결된 카드로 변환

Ad Hoc 카드를 만든 후 연결된 카드로 변환할 수 있습니다. 임시 카드에 대한 자세한 내용은 [보드에 애드혹 카드 추가](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. 보드에 액세스하고 Ad Hoc 카드를 엽니다.
1. 카드의 이름과 설명을 확인합니다. 이 사용자들은 사용자가 만드는 작업 또는 문제에 추가됩니다. [!DNL Workfront].
1. 다음에서 [!UICONTROL 연결] 카드 세부 정보 영역에서 **[!UICONTROL Workfront과 연결]**.
1. 다음에서 [!UICONTROL 카드 연결] 창에서 작업을 생성할지 문제를 생성할지 선택합니다.
1. 작업 또는 문제를 추가할 프로젝트를 검색하고 선택합니다.

   >[!NOTE]
   >
   >* 사용 권한이 있는 개체만 검색 결과에서 사용할 수 있습니다.
   >* 필터링 기준: **[!UICONTROL 내가 소유한 프로젝트]** 또는 **[!UICONTROL 내가 진행 중인 프로젝트]**, 와 동일한 프로젝트 [!UICONTROL 완료], [!UICONTROL 중단], 또는 [!UICONTROL 거부됨] 상태는 포함되지 않습니다. 를 사용하여 해당 프로젝트를 계속 검색할 수 있습니다. **[!UICONTROL 모두]** 필터.

1. 클릭 **[!UICONTROL 연결]**.

   ![Ad Hoc 카드를 Workfront에 연결](assets/boards-connect-ad-hoc-card.png)

   프로젝트 이름은 카드 세부 정보의 연결 영역에 표시됩니다.

1. 클릭 **[!UICONTROL 닫기]** 게시판으로 돌아갑니다.

## 연결된 카드에 시간 기록

연결된 작업 또는 문제에 시간을 기록하려면 올바른 권한이 있어야 합니다.

시간 로깅 필드는 기본적으로 연결된 카드에 표시되지 않습니다. 다음을 활성화해야 합니다. [!UICONTROL **시간**] 다음에서 [!UICONTROL 구성] 아래 지역 [!UICONTROL 카드]. 자세한 내용은 [카드에 표시할 필드 사용자 지정](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 작업 또는 문제의 시간 수를 입력합니다.
1. 선택 [!UICONTROL 시간 유형] 드롭다운 메뉴에서 ( 기본 값과 다른 경우) 을 선택합니다.
1. 클릭 [!UICONTROL **로그 시간**].

   ![카드에 시간 기록](assets/log-hours-on-card.png)

   카드에 기록된 시간도 연결된 작업 또는 문제에 저장됩니다.

카드의 로깅 시간은 작업 또는 문제의 로깅 시간과 동일합니다. 자세한 내용은 문서의 &quot;프로젝트, 작업 또는 문제에 시간 기록&quot;을 참조하십시오 [로그 시간](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

