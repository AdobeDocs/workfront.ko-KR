---
product-area: projects
navigation-topic: use-the-home-area
title: 에 항목 표시 [!UICONTROL 작업 목록] 집 지역에서
description: 다음 [!UICONTROL 작업 목록] 에서 [!UICONTROL 홈] 영역에는 사용자에게 지정된 모든 작업 항목이 표시됩니다. 에 표시되는 항목을 제어할 수 있습니다 [!UICONTROL 작업] 아래에 설명된 대로 나열합니다.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# 에 항목 표시 [!UICONTROL 작업 목록] 집 지역에서

다음 [!UICONTROL 작업 목록] 에서 [!UICONTROL 홈] 영역에는 사용자에게 지정된 모든 작업 항목이 표시됩니다. 에 표시되는 항목을 제어할 수 있습니다 [!UICONTROL 작업] 아래에 설명된 대로 나열합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>승인을 위한 [!UICONTROL Review]</p> <p>다른 모든 개체에 대해 [!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>프로젝트, 작업, 문제 및 문서에 대한 [!UICONTROL 보기] 이상 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 대한 사용 권한 이상을 제공합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 필터 [!UICONTROL 작업 목록]

에서 항목을 필터링할 수 있습니다 [!UICONTROL 작업 목록] 를 클릭하여 특정 유형의 항목만 표시합니다. 예를 들어 [!UICONTROL 작업 목록] 문제 또는 요청만 표시합니다.

>[!NOTE]
>
>필터 옵션은 브라우저에 저장됩니다. 동일한 컴퓨터에서 동일한 브라우저를 일관되게 사용(사이트 데이터를 지우지 않음)하면 선택한 필터가 변경되지 않습니다. 브라우저나 컴퓨터를 전환하면 필터가 모든 필터가 선택 취소된 기본 옵션으로 돌아갑니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 을(를) 클릭합니다. **[!UICONTROL 필터]** ![](assets/filter-nwepng.png) 드롭다운 메뉴
1. 다음 필터 옵션 중에서 선택하여 표시할 항목의 유형을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>모든 항목을 표시하고 선택합니다. 여기에는 작업, 문제, 승인, 개인 작업, 완료된 작업 및 문제가 포함됩니다. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업 작업]</strong></td> 
      <td> <p>작업 중인 작업만 표시합니다. 이러한 작업은 [!UICONTROL Work On It] 단추를 클릭한 사용자에게 할당된 작업입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Ready To Start]</strong></td> 
      <td> 
       <div> 
        <p>시작할 준비가 된 작업만 표시합니다. 다음 문은 모두 true여야 합니다.</p> 
        <ul> 
         <li> <p>일과부모에게는 일과가 되지 않도록 하는 선행 작업이나 작업 제약 조건이 없습니다.</p> </li> 
         <li> <p>작업의 [!UICONTROL 계획된 시작 날짜]가 과거 또는 2주 내에 있습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업이 준비되지 않음]</strong></td> 
      <td> 
       <div> 
        <p>아직 시작할 준비가 되지 않은 작업만 표시합니다. 다음 문 중 하나는 true여야 합니다.</p> 
        <ul> 
         <li> <p>일과부모에게는 일과가 되지 않도록 하는 선행 또는 작업 제약 조건이 있을 수 있습니다.</p> </li> 
         <li> <p>작업에는 향후 2주 이상인 [!UICONTROL 계획 시작 날짜]가 있습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업 문제]</strong></td> 
      <td> <p>현재 작업 중인 문제만 표시합니다. 이는 [!UICONTROL Work On It] 단추를 클릭한 사용자에게 할당된 문제입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Requested]</strong></td> 
      <td>[!UICONTROL Work On It] 단추를 클릭하지 않은 문제만 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>개인</strong></td> 
      <td>개인 작업만 표시합니다. 이 작업은 섹션에 설명된 대로 [!UICONTROL To Do] 작업으로 만드는 작업입니다 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">개인 작업 만들기</a> 기사 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">[!UICONTROL 홈] 영역에서 작업 항목 만들기</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>자신에게 할당되거나 위임된 승인 및 제출한 승인만 표시합니다. 승인에는 작업 항목(프로젝트, 작업 및 문제)에 대한 승인, 문서, 증명, 액세스 요청 및 작업표에 대한 승인이 포함됩니다. 승인에 대한 자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">승인 보기</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">작업 승인</a> </p> </li> 
        </ul> 
        <p>참고: 제출한 승인 및 승인자 중 하나인 경우에도 두 번 계산됩니다.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 완료]</strong></td> 
      <td> <p>완료된 작업, 문제 및 개인 작업만 표시합니다. 완료된 작업은 이전 2주 동안 표시되며 완료된 주에 따라 작업 목록에 그룹화됩니다. 승인이 포함되지 않습니다.</p> <p>이 필터를 선택하지 않으면 완료된 작업은 [!UICONTROL 작업 목록]에 숨겨집니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 필터 옵션은 개체(작업, 문제, 승인, 개인 작업)를 기반으로 합니다.
   >* 작업 및 문제는 작업 준비 상태([!UICONTROL 작업], [!UICONTROL 시작 준비 완료], [!UICONTROL 준비 안 됨] 작업 및 [!UICONTROL 작업] 및 [!UICONTROL 요청] 문제 참조). 작업 또는 문제를 특정 상태로 표시하도록 선택하거나 작업 또는 문제 를 클릭하여 모든 상태를 선택하고 표시할 수 있습니다.
   >* 완료된 항목에 대한 별도의 필터가 있으며 여기에는 작업과 문제가 모두 포함됩니다. 여기에는 승인이 포함되지 않습니다. 다음 [!UICONTROL 완료됨] 필터에 개인 작업이 포함됩니다.
   >* 한 번에 한 상태만 선택할 수 있습니다. 예를 들어 만 표시할 수 있습니다 [!UICONTROL 작업] 작업 및 전용 [!UICONTROL 요청] 문제.
   >* 팀 중 하나에 할당된 항목에 대해서는 필터를 적용할 수 없으며 직접 할당된 항목에 포함되지 않습니다.



1. (선택 사항) 추가 구성 [!UICONTROL 작업 목록]섹션에 설명된 대로 [날짜, 프로젝트 및 우선 순위를 기준으로 그룹화 및 정렬](#group-and-sort-by-date-project-and-priority) 참조하십시오.

## 그룹화 및 정렬 기준 [!UICONTROL 날짜], [!UICONTROL 프로젝트], 및 [!UICONTROL 우선순위]

을(를) 그룹화하고 정렬할 수 있습니다 [!UICONTROL 작업 목록] by [!UICONTROL 계획 완료 일자], [!UICONTROL 커밋 날짜], [!UICONTROL 프로젝트], 또는 [!UICONTROL 내 우선 순위]. 선택한 옵션에 따라 항목이 [!UICONTROL 작업 목록].

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 을(를) 클릭합니다. **[!UICONTROL 그룹화 기준]** 드롭다운 메뉴

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 계획된 완료]</strong></td> 
      <td> <p> 항목이 [!UICONTROL 작업 목록]의 [!UICONTROL 계획 완료 날짜]에 따라 다음 그룹화에 표시됩니다(각 그룹핑 내에 포함된 항목 수는 제목 옆에 괄호로 표시).</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL 계획된 완료 날짜 없음]</p> </li> 
        <li> <p>[!UICONTROL 이번 주]</p> <p>이 그룹은 기본적으로 확장됩니다.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL 계획됨], 그 다음에 다양한 [!UICONTROL 계획 완료 날짜](여러 그룹화)가 옵니다.</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 계획된 시작]</strong></td> 
      <td> <p>항목이 [!UICONTROL 작업 목록]의 [!UICONTROL 계획 시작 날짜]에 따라 다음 그룹화에 표시됩니다(각 그룹 내에 포함된 항목 수는 제목 옆에 괄호 안에 표시됩니다.).</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL 이번 주] </p> <p>이 그룹은 기본적으로 확장됩니다.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL 계획됨], 그 다음에 다양한 [!UICONTROL 계획됨 시작 날짜](여러 그룹화)가 옵니다</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 커밋 날짜]</strong></td> 
      <td> <p>[!UICONTROL 작업 목록]의 다음 그룹화에 항목이 표시됩니다(각 그룹화에 포함된 항목 수는 제목 옆에 괄호로 표시).</p> 
       <ul> 
        <li> <p>[!UICONTROL 커밋 날짜 없음]</p> </li> 
        <li> <p>[!UICONTROL 다음 주에 커밋됨]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>항목은 프로젝트에 따라 그룹화되고 프로젝트는 [!UICONTROL 작업 목록]에 알파벳순으로 표시됩니다. (각 그룹화 내에 포함된 항목 수는 제목 제목 옆에 괄호로 표시됩니다.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>선택한 순서대로 항목이 표시됩니다. 자세한 내용은 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">[!UICONTROL Home] 영역에서 작업 우선 순위 지정</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>기본 정렬은 오름차순입니다. 정렬을 내림차순으로 변경하면 선택한 정렬 옵션이 브라우저에 저장됩니다. 동일한 컴퓨터에서 동일한 브라우저를 일관되게 사용(사이트 데이터를 지우지 않음)하면 정렬이 변경되지 않지만 브라우저나 컴퓨터를 전환하면 정렬이 기본 정렬로 변경됩니다.

## 지연 항목 보기

[!DNL Adobe Workfront] 작업 요청이 지연되었는지 여부를 판별하려면 다음 날짜를 사용합니다.

* **작업**: [!UICONTROL 계획 완료 일자]
* **문제**: [!UICONTROL 계획 완료 일자]
* **문서**: [!UICONTROL 제출일]
* **작업표**: [!UICONTROL 제출일]
* **승인**: [!UICONTROL 제출일]
* **증명 승인**: [!UICONTROL 증명 최종 기한]

## 검색 [!UICONTROL 작업 목록]

를 검색할 때 [!UICONTROL 작업 목록]에 지정된 모든 항목이 검색 시 반환됩니다(화면에 현재 로드되지 않은 항목도). 만약 [!UICONTROL 완료 표시] 옵션을 선택하면 지난 2주 내에 완료로 표시한 모든 항목이 반환됩니다.

또한 작업 항목의 이름만 검색됩니다(작업 항목 내의 정보는 검색되지 않으며 작업 항목이 상주하는 프로젝트의 이름도 검색되지 않음).

를 검색하려면 [!UICONTROL 작업 목록]:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. (선택 사항) [!UICONTROL 작업 목록]에 설명된 대로 [필터 [!UICONTROL 작업 목록]](#filter-the-work-list) 및 [날짜, 프로젝트 및 우선 순위를 기준으로 그룹화 및 정렬](#group-and-sort-by-date-project-and-priority).

1. (선택 사항) 이미 완료된 작업 항목을 검색하는 경우 다음을 구성해야 합니다 [!UICONTROL 작업 목록] 검색하기 전에 완료된 항목을 표시합니다.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. 검색할 항목 이름의 이름을 입력합니다.\
   다음 [!UICONTROL 작업 목록] 은 이름이 일치하는 항목을 포함하도록 자동으로 필터링됩니다.

## 작업 목록 크기 변경

크기를 변경할 수 있습니다 [!UICONTROL 작업 목록] 그래서 그것은 Home 지역의 약 4분의 1에서 약 1/2까지 어느 곳에서든 소비되도록 합니다 [!UICONTROL 홈] 영역.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 마우스 오른쪽 가장자리 [!UICONTROL 작업 목록]을 누른 다음 작업 목록 이 원하는 크기가 될 때까지 왼쪽 또는 오른쪽으로 드래그합니다.

## 그룹화 축소 및 확장

의 항목 [!UICONTROL 작업 목록] 는 그룹화 내에 표시됩니다. 그룹을 축소하고 확장하여 지정된 시간에 페이지에 표시되는 정보의 양을 제어할 수 있습니다.

내 그룹화를 축소하고 확장할 수 있습니다 [!UICONTROL 작업 목록] 표시되는 정보를 보다 효과적으로 제어할 수 있습니다.\
기본적으로 [!UICONTROL 이번 주] 그룹이 확장되고 다른 모든 그룹이 축소됩니다. 변경한 내용은 다음에 홈 영역에 액세스할 때 기억됩니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 을(를) 클릭합니다. **[!UICONTROL 확장]** 또는 **[!UICONTROL 축소]** 확장하거나 축소할 그룹 옆의 화살표.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   또는\
   모든 그룹을 동시에 확장하거나 축소하려면 **[!UICONTROL 확장]** 또는 **[!UICONTROL 축소]** 그룹 옆의 화살표를 누른 채 [!UICONTROL Shift] 키.
