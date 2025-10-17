---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 보드에 Ad Hoc 카드 추가
description: Ad Hoc 카드를 보드에 빠르게 추가하고 보드에 있는 멤버에게 할당할 수 있습니다. 카드는 작업, 문제, 개인, 그룹 또는 보드에 포함할 모든 유형의 항목을 나타낼 수 있습니다.
author: Jenny
feature: Agile
exl-id: 9bc1f92a-85b0-44fd-b5de-09a69af6def5
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 보드에 애드혹 카드 추가

보드에 카드를 빠르게 추가하고 보드에 있는 멤버에게 카드를 할당할 수 있습니다. 카드는 작업, 문제, 개인, 그룹 또는 보드에 포함할 모든 유형의 항목을 나타낼 수 있습니다.

>[!NOTE]
>
>보드에 있는 임시 카드가 [!DNL Adobe Workfront]의 작업 항목에 연결되어 있지 않습니다. 연결된 카드에 대한 자세한 내용은 [보드에 연결된 카드 사용](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전체 세부 정보가 포함된 애드혹 카드 추가

임시 카드가 [!DNL Adobe Workfront]의 작업 항목에 연결되어 있지 않습니다.

{{step1-to-boards}}

1. 보드에 액세스합니다. 자세한 내용은 [게시판 만들기 또는 편집](../../agile/get-started-with-boards/create-edit-board.md)을 참조하세요.
1. **[!UICONTROL 카드 추가] > [!UICONTROL 새 카드]**&#x200B;를 클릭합니다.

   [!UICONTROL 카드 세부 정보] 상자가 나타납니다.

   >[!NOTE]
   >
   >이름 필드 외부를 클릭하면 Ad Hoc 카드가 맨 왼쪽 열 하단에 자동으로 &quot;제목 없음&quot;으로 저장됩니다. 카드를 저장하지 않고 종료하려면 [!UICONTROL **카드 세부 정보**] 상자의 아무 곳이나 클릭하지 않고 [!UICONTROL 취소]를 클릭해야 합니다.

1. **[!UICONTROL 카드 세부 정보]** 상자에 다음 정보를 추가하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 이름]</strong> </td> 
      <td>카드의 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 설명]</strong> </td> 
      <td>카드에 대한 설명. 설명에 URL을 추가할 수 있으며 카드가 저장되면 클릭할 수 있는 링크가 됩니다.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 열]</strong> </td> 
      <td>카드 열을 선택합니다. <strong>[!UICONTROL Column]</strong> 필드를 비워 두면 카드가 보드 왼쪽의 첫 번째 열에 배치됩니다.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 상태]</strong> </td> 
      <td>카드 상태를 선택합니다. 카드 상단에서 <strong>[!UICONTROL Mark Complete]</strong>을(를) 클릭하면 상태가 자동으로 [!UICONTROL Complete] (으)로 변경됩니다.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 기한]</strong></td> 
      <td>카드의 기한을 선택하십시오. </td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td> 
      <td>카드를 완료할 예상 시간을 입력합니다. 수동 입력만 가능합니다.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong> </td> 
      <td>카드를 할당하려면 <strong>[!UICONTROL 할당 추가]</strong>를 클릭하고 검색 필드에 이름을 입력하세요. 그런 다음 결과 목록에 표시될 때 선택합니다. 개인 및 팀을 모두 추가할 수 있으며 한 카드에 둘 이상의 개인 또는 팀을 할당할 수 있습니다.</td>
     </tr>     
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 태그]</strong></td> 
      <td>카드에 대한 태그를 검색하고 선택합니다. 새 태그를 만드는 방법에 대한 자세한 내용은 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">태그 추가</a>를 참조하십시오.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 연결]</strong> </td>
      <td>임시 카드를 [!DNL Workfront] 작업 또는 문제에 연결할 수 있습니다. 자세한 내용은 문서 <a href="/help/quicksilver/agile/get-started-with-boards/connected-cards.md">보드에서 연결된 카드 사용</a>에서 "Ad Hoc 카드를 연결된 카드로 변환"을 참조하십시오.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 검사 목록]</strong> </td> 
      <td> <p><strong>[!UICONTROL 체크리스트 항목 추가]</strong>를 클릭합니다. 그런 다음 항목의 제목을 입력하고 Enter 키를 누릅니다. 다른 항목이 자동으로 추가됩니다. 제목을 계속 입력하여 더 많은 항목을 추가합니다.</p> <p>체크리스트 상단의 카운터는 완료된 품목 수와 전체 품목 수를 보여준다.</p> <p>검사 목록 항목에 대한 자세한 내용은 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">카드의 검사 목록 항목 관리</a>를 참조하십시오.</p> </td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p><strong>[!UICONTROL New comment]</strong> 필드를 클릭하고 설명을 입력하십시오. 서식 도구를 사용하여 텍스트 서식을 지정합니다. (이미지는 임시 카드의 주석에서 사용할 수 없습니다.) 사용자 또는 팀에 태그를 지정하려면 댓글 영역 하단에 있는 검색 상자를 사용합니다. 사용자는 보드에서 멤버일 필요가 없습니다.</p><p><strong>참고:</strong> 현재 Ad Hoc Card에서 댓글을 태그 지정한 사용자가 전자 메일 알림을 받지 않습니다.
      </p><p>카드에 주석을 추가하려면 <strong>[!UICONTROL Submit]</strong>을(를) 클릭합니다.</p>
      <p>댓글에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">작업 업데이트</a>를 참조하세요.</p></td>
     </tr>
    </tbody> 
   </table>

   ![임시 카드 세부 정보](assets/ad-hoc-card-details-with-comments.png)

   왼쪽 탐색 패널을 사용하여 카드 세부 정보에서 필드의 섹션 사이를 이동합니다.

1. 보드에 카드를 추가하려면 **[!UICONTROL 닫기]**&#x200B;를 클릭하십시오.

   담당자, 태그, 만기일, 체크리스트 카운터, 예상 시간 및 상태가 카드에 표시됩니다.

## 애드혹 카드의 빠른 추가

제목만 있는 임시 카드를 추가하여 보드를 빠르게 채울 수 있습니다.

1. 카드를 추가할 보드에 액세스합니다.
1. 카드를 추가하려는 열에서 **[!UICONTROL 추가]** 아이콘 ![카드 추가](assets/addicon-spectrum.png)를 클릭합니다.
1. 카드 이름을 입력하고 Enter 키를 누릅니다.

   새 카드 아래에 다른 카드가 자동으로 추가됩니다.

1. 카드 이름을 계속 입력하여 카드를 더 추가합니다.
1. 카드 추가를 중지하려면 열 바깥쪽을 클릭합니다.
1. 자세한 내용을 추가하려면 카드를 편집해야 합니다. 자세한 내용은 이 문서에서 [기존 카드 편집](#edit-an-existing-card)을 참조하십시오.

## 기존 카드 편집 {#edit-an-existing-card}

1. 보드에 액세스합니다.
1. 이름을 편집하려면 카드 이름을 클릭합니다.
1. 카드 세부 사항을 편집하려면 카드 이름 대신 카드를 클릭합니다.

   또는

   카드에서 **[!UICONTROL 기타]** 메뉴 ![[!UICONTROL 기타 메뉴]](assets/more-icon-spectrum.png)를 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. [!UICONTROL 카드 세부 정보] 상자에서 필요에 따라 정보를 업데이트한 다음 **[!UICONTROL 닫기]**&#x200B;를 클릭하여 게시판으로 돌아갑니다.

   필드 값을 업데이트하기 위해 열 정책을 활성화한 경우 카드의 상태를 변경하면 카드가 자동으로 해당 열로 이동합니다. 자세한 내용은 문서 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)에서 &quot;열 설정 및 정책 정의&quot;를 참조하십시오.
