---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 작업 스트림에 반복 만들기
description: 반복은 작업을 완료하기 위해 예약된 설정된 시간입니다. 일부 애자일 팀은 반복을 스프린트로 지칭할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 0ca3428d7442564a9753db04790fd40839ae24ea
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 1%

---

# 작업 스트림에 반복 만들기

반복은 작업을 완료하기 위해 예약된 설정된 시간입니다. 일부 애자일 팀은 반복을 스프린트로 지칭할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

## 작업 스트림에 반복 만들기

{{step1-to-boards}}

1. 반복을 추가할 워크스트림을 엽니다. 작업 스트림을 열려면 다음을 클릭합니다. [!UICONTROL **작업 스트림 보기**].
1. 다음 방법 중 하나를 사용하여 반복을 만듭니다.

   * 카드 목록 탭의 반복 보기에서 [!UICONTROL **반복 만들기**].
   * 카드 목록 탭의 목록 보기에서 [!UICONTROL **반복 만들기**].
   * 보드 탭에서 [!UICONTROL **보드 추가**] 및 선택 [!UICONTROL **반복 프로세스**] 게시판 템플릿으로 사용됩니다. 그런 다음 반복 보드를 열고 를 클릭합니다. [!UICONTROL **반복 구성**].

1. 반복 세부 정보 대화 상자에서 다음 정보를 추가합니다.

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL 반복 이름]</strong></td> 
      <td>반복의 이름(예: "Sprint 1").</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL 반복 길이]</strong></td> 
      <td>반복 길이(일, 주 또는 월 단위)입니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 시작 날짜]</strong></td> 
      <td>반복이 시작되는 날짜입니다. 종료 날짜는 반복 길이에 따라 자동으로 입력됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   이제 카드 목록의 반복 보기와 반복 보드의 지표 영역에 반복이 표시됩니다.

   카드를 반복에 추가하려면 다음을 참조하십시오. [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## 기존 반복 편집

1. 작업 스트림을 열려면 다음을 클릭합니다. [!UICONTROL **작업 스트림 보기**].
1. 다음 방법 중 하나를 사용하여 반복을 엽니다.

   * 카드 목록 탭의 반복 보기에서 [!UICONTROL **반복 세부 정보**] 아이콘 ![반복 세부 정보](assets/iteration-details-button.png).
   * 반복 보드에서 [!UICONTROL **반복 세부 정보**] 아이콘 ![반복 세부 정보](assets/iteration-details-button.png) 오른쪽 상단의 지표 영역에서 을 참조하십시오.

1. 다음에서 [!UICONTROL 반복 구성] 패널을 열고 필요에 따라 이터레이션을 편집합니다.
1. 반복 이름을 변경하려면 를 확장합니다. [!UICONTROL **반복 세부 정보**].

   반복이 시작되면 일자 또는 반복 길이가 아닌 반복 이름만 변경할 수 있습니다.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## 반복 삭제

1. 다음을 클릭합니다. [!UICONTROL **카드 목록**] 을(를) 작업 스트림에서 탭하고 반복 보기를 엽니다.
1. 다음을 클릭합니다. **삭제** 아이콘 ![삭제 아이콘](assets/delete.png) 를 클릭합니다.
1. 클릭 [!UICONTROL **반복 삭제**] 확인 메시지 표시.
