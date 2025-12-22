---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 워크스트림에 반복 만들기
description: 반복은 작업을 완료하기 위해 예약된 설정된 시간입니다. 일부 애자일 팀은 반복을 스프린트로 참조할 수 있습니다.
author: Jenny
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 4%

---

# 작업 스트림에 반복 만들기

>[!IMPORTANT]
>
>작업 스트림은 특정 고객 그룹만 사용할 수 있습니다.

반복은 작업을 완료하기 위해 예약된 설정된 시간입니다. 일부 애자일 팀은 반복을 스프린트로 참조할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

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

## 작업 스트림에 반복 만들기

{{step1-to-boards}}

1. 반복을 추가할 워크스트림을 엽니다. 작업 스트림을 열려면 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭합니다.
1. 다음 방법 중 하나를 사용하여 반복을 만듭니다.

   * 카드 목록 탭의 반복 보기에서 [!UICONTROL **반복 만들기**]&#x200B;를 클릭합니다.
   * 카드 목록 탭의 목록 보기에서 [!UICONTROL **반복 만들기**]&#x200B;를 클릭합니다.
   * 보드 탭에서 [!UICONTROL **보드 추가**]&#x200B;를 클릭하고 [!UICONTROL **반복 프로세스**]&#x200B;를 보드 템플릿으로 선택합니다. 그런 다음 반복 보드를 열고 [!UICONTROL **반복 구성**]&#x200B;을 클릭합니다.

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

   카드를 반복에 추가하려면 [카드 목록 사용](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)을 참조하세요.

## 기존 반복 편집

1. 작업 스트림을 열려면 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭합니다.
1. 다음 방법 중 하나를 사용하여 반복을 엽니다.

   * 카드 목록 탭의 반복 보기에서 [!UICONTROL **반복 세부 정보**] 아이콘 ![반복 세부 정보](assets/iteration-details-button.png)을 클릭합니다.
   * 반복 보드에서 오른쪽 상단의 지표 영역에서 [!UICONTROL **반복 세부 정보**] 아이콘 ![반복 세부 정보](assets/iteration-details-button.png)을 클릭합니다.

1. [!UICONTROL 반복 구성] 패널에서 필요에 따라 반복을 편집합니다.
1. 반복 이름을 변경하려면 [!UICONTROL **반복 세부 정보**]&#x200B;를 확장하세요.

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

1. 작업 스트림에서 [!UICONTROL **카드 목록**] 탭을 클릭하고 반복 보기를 엽니다.
1. 반복 옆에 있는 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.
1. 확인 메시지에서 [!UICONTROL **반복 삭제**]&#x200B;를 클릭합니다.
