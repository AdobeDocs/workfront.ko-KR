---
product-area: projects
navigation-topic: use-the-home-area
title: 에 항목 표시 [!UICONTROL 작업 목록] 홈 영역에서
description: 다음 [!UICONTROL 작업 목록] 다음에서 [!UICONTROL 홈] 영역에는 사용자에게 할당된 모든 작업 항목이 표시됩니다. 에 표시되는 항목을 제어할 수 있습니다. [!UICONTROL 작업 목록], 필터를 사용하고 작업 항목을 그룹화 및 정렬하여.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '1826'
ht-degree: 0%

---

# 에 항목 표시 [!UICONTROL 작업 목록] 다음에서 [!UICONTROL 홈] 영역

<!-- Audited: 1/2024 -->


다음 [!UICONTROL 작업 목록] 다음에서 [!UICONTROL 홈] 영역에는 사용자에게 할당된 모든 작업 항목이 표시됩니다. 에 표시되는 항목을 제어할 수 있습니다. [!UICONTROL 작업 목록], 필터를 사용하고 작업 항목을 그룹화 및 정렬하여.

>[!NOTE]
>
>* 문제를 작업 또는 프로젝트로 전환할 때 문제에 할당된 사용자의 홈 영역에서 문제가 제거됩니다.
>
>* 작업을 프로젝트로 전환할 때 작업이 삭제되고 작업에 할당된 사용자의 홈 영역에서 제거됩니다.


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> <p>신규:</p><ul><li>승인용 [!UICONTROL Contributor]</li> <li>다른 모든 개체의 [!UICONTROL Standard] 이상</li> <p>또는</p> 
  </ul><p>현재:</p><ul><li>승인용 [!UICONTROL Review]</li> <li>다른 모든 개체에 대해 [!UICONTROL Work] 이상</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>프로젝트, 작업, 문제 및 문서에 대한 [!UICONTROL 보기] 이상 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 권한 이상 부여</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 필터 [!UICONTROL 작업 목록]

에서 항목을 필터링할 수 있습니다. [!UICONTROL 작업 목록] 특정 유형의 항목만 표시합니다. 예를 들어 다음을 필터링할 수 있습니다. [!UICONTROL 작업 목록] 문제 또는 요청만 표시합니다.

>[!NOTE]
>
>필터 옵션은 브라우저에 저장됩니다. 동일한 컴퓨터에서 동일한 브라우저를 일관되게 사용하고 사이트 데이터를 지우지 않으면 선택한 필터가 변경되지 않습니다. 브라우저나 컴퓨터를 전환하면 모든 필터가 선택 해제된 기본 옵션으로 필터가 되돌아갑니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 다음을 클릭합니다. **[!UICONTROL 필터]** ![](assets/filter-nwepng.png) 드롭다운 메뉴. 필터를 선택한 경우 아이콘 대신 선택한 필터의 수가 표시됩니다.
1. 다음 필터 옵션 중에서 선택하여 표시할 항목 유형을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>모든 항목을 표시하고 선택합니다. 여기에는 작업, 문제, 승인, 개인 작업 및 완료된 작업 및 문제가 포함됩니다. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업: 처리 중]</strong></td> 
      <td> <p>현재 작업 중인 작업만 표시합니다. 이는 [!UICONTROL Work On It] 버튼을 클릭한 사용자에게 할당된 작업입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업: 시작할 준비 완료]</strong></td> 
      <td> 
       <div> 
        <p>시작할 준비가 된 작업만 표시합니다. 다음 문은 모두 true여야 합니다.</p> 
        <ul> 
         <li> <p>과제와 그 부모에게는 작업을 할 수 없는 전임자나 과업 제한이 없다.</p> </li> 
         <li> <p>작업의 [!UICONTROL 계획된 시작 일자]가 과거 또는 최대 2주 후입니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 작업: 준비되지 않음]</strong></td> 
      <td> 
       <div> 
        <p>아직 시작할 준비가 되지 않은 작업만 표시합니다. 다음 문 중 하나가 true여야 합니다.</p> 
        <ul> 
         <li> <p>작업 및 상위 사용자에게 작업을 수행할 수 없는 선행 작업 또는 작업 제한이 있을 수 있습니다.</p> </li> 
         <li> <p>작업에 앞으로 2주 이상 소요되는 [!UICONTROL 계획된 시작 일자]가 있습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 문제: 처리 중]</strong></td> 
      <td> <p>현재 진행 중인 문제만 표시합니다. 이는 [!UICONTROL Work On It] 버튼을 클릭한 사용자에게 할당된 문제입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 문제: 요청됨]</strong></td> 
      <td>나에게 할당되었지만 [!UICONTROL Work On It] 단추를 클릭하지 않은 문제만 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>개인</strong></td> 
      <td>개인 작업만 표시합니다. 섹션에 설명된 대로 [!UICONTROL 할 일] 작업으로 만드는 작업입니다 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">개인 작업 만들기</a> 이 문서에서 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">[!UICONTROL Home] 영역에서 작업 항목 만들기</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>귀하에게 할당되거나 위임된 승인 및 귀하가 제출한 승인만 표시합니다. 승인에는 작업 항목(프로젝트, 작업 및 문제)에 대한 승인과 문서, 증명, 액세스 요청 및 타임시트에 대한 승인이 포함됩니다. 승인에 대한 자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">승인 보기</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">작업 승인</a> </p> </li> 
        </ul> 
        <p>참고: 제출한 승인과 승인자 중 하나인 승인은 두 번 계산됩니다.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 위임됨: 내가 위임함]</strong></td> 
      <td> 
       <div> 
        <p>다른 사용자에게 위임한 작업 항목만 표시합니다.</p> 
        <p>작업 위임에 대한 자세한 내용은 <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">다른 사용자에게 작업 및 문제 위임</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 위임됨: 내게 위임됨]</strong></td> 
      <td> 
       <div> 
        <p>다른 사용자가 일시적으로 귀하에게 위임한 작업 항목만 표시합니다.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 완료]</strong></td> 
      <td> <p>완료된 작업, 문제 및 개인 작업만 표시합니다. 완료된 작업이 이전 2주 동안 표시되고 완료된 주에 따라 작업 목록에 그룹화됩니다. 승인이 포함되지 않습니다.</p> <p>이 필터를 선택하지 않으면 완료된 작업이 [!UICONTROL 작업 목록]에 표시되지 않습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 필터 옵션은 개체(작업, 문제, 승인, 개인 작업)를 기반으로 합니다.
   >* 작업 및 문제는 작업 준비도( )와 관련하여 해당 상태별로 추가로 필터링됩니다.[!UICONTROL 작업 중], [!UICONTROL 시작할 준비 완료], [!UICONTROL 준비 안 됨] 작업 및 [!UICONTROL 작업 중] 및 [!UICONTROL 요청됨] 문제)에 대해 설명합니다. 을(를) 선택하여 특정 상태의 작업 또는 문제를 표시하거나 작업 또는 문제를 클릭하여 모든 상태를 선택하고 표시할 수 있습니다.
   >* 완료된 항목에 대한 별도의 필터가 있으며 여기에는 작업과 문제가 모두 포함됩니다. 여기에는 승인이 포함되지 않습니다. 다음 [!UICONTROL 완료됨] 필터에는 개인 작업이 포함됩니다.
   >* 한 번에 하나의 상태만 표시하도록 선택할 수 있습니다. 예를 들어, [!UICONTROL 작업 중] 작업 및 전용 [!UICONTROL 요청됨] 문제. 한 번에 여러 상태를 선택할 수도 있습니다.
   >* 팀 중 하나에 할당된 항목에 필터를 적용할 수 없으며 팀 할당은 사용자에게 직접 할당된 항목에 포함되지 않습니다.


1. (선택 사항) [!UICONTROL 작업 목록]섹션에 설명된 대로 [날짜, 프로젝트 및 우선 순위별로 그룹화 및 정렬](#group-and-sort-by-date-project-and-priority) 이 문서에서.

## 그룹화 및 정렬 기준 [!UICONTROL 날짜], [!UICONTROL 프로젝트], 및 [!UICONTROL 우선 순위]

다음을 그룹화 및 정렬할 수 있습니다. [!UICONTROL 작업 목록] 작성자: [!UICONTROL 계획된 완료 일자], [!UICONTROL 커밋 일자], [!UICONTROL 프로젝트], 또는 [!UICONTROL 내 우선 순위]. 선택하는 옵션은 항목을에서 그룹화하는 방법을 결정합니다 [!UICONTROL 작업 목록].

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 다음을 클릭합니다. **[!UICONTROL 그룹화 기준]** ![그룹화 기준](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) 드롭다운 메뉴.

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 계획된 완료]</strong></td> 
      <td> <p> 항목은 [!UICONTROL 계획된 완료 일자]에 따라 [!UICONTROL 작업 목록]에서 다음 그룹화로 표시됩니다(각 그룹화에 포함된 항목 수는 제목 옆에 괄호로 표시됨).</p> 
       <ul> 
        <li> <p>[!UICONTROL 지연]</p> </li> 
        <li> <p>[!UICONTROL 계획된 완료 일자 없음]</p> </li> 
        <li> <p>[!UICONTROL This Week]</p> <p>이 그룹화는 기본적으로 확장되어 있습니다.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned] 다음에 여러 [!UICONTROL Planned Completion Dates](여러 그룹화)가 옵니다.</p> </li> 
        <li> <p>[!UICONTROL 완료]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 계획 시작]</strong></td> 
      <td> <p>항목은 [!UICONTROL 계획된 시작 일자]에 따라 [!UICONTROL 작업 목록]에서 다음 그룹화로 표시됩니다(각 그룹화에 포함된 항목 수는 제목 옆에 괄호로 표시됨).</p> 
       <ul> 
        <li> <p>[!UICONTROL 지연]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>이 그룹화는 기본적으로 확장되어 있습니다.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned] 다음에 여러 [!UICONTROL Planned Start Dates](여러 그룹화)가 옵니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 커밋 일자]</strong></td> 
      <td> <p>항목은 [!UICONTROL 작업 목록]에서 다음 그룹화로 표시됩니다(각 그룹화 내에 포함된 항목의 수는 제목 옆에 괄호로 표시됨).</p> 
       <ul> 
        <li> <p>[!UICONTROL 커밋 일자 없음]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 프로젝트]</strong></td> 
      <td>항목은 프로젝트에 따라 그룹화되고 프로젝트는 [!UICONTROL 작업 목록]에 알파벳순으로 표시됩니다. 각 그룹화 내에 포함된 항목의 수는 제목 제목 옆에 괄호로 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 내 우선 순위]</strong></td> 
      <td>선택한 순서대로 항목이 표시됩니다. 자세한 내용은 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">[!UICONTROL Home] 영역에서 작업의 우선 순위 지정</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>기본 정렬은 오름차순입니다. 정렬을 내림차순으로 변경하면 선택한 정렬 옵션이 브라우저에 저장됩니다. 동일한 컴퓨터에서 동일한 브라우저를 일관되게 사용하고 사이트 데이터를 지우지 않으면 정렬이 변경되지 않지만 브라우저나 컴퓨터를 전환하면 정렬이 기본 정렬로 변경됩니다.

## 지연 항목 보기

[!DNL Adobe Workfront] 은 다음 일자를 사용하여 작업 요청이 늦어졌는지 확인합니다.

* **작업**: [!UICONTROL 계획된 완료 일자]
* **문제**: [!UICONTROL 계획된 완료 일자]
* **문서**: [!UICONTROL 제출 날짜]
* **타임시트**: [!UICONTROL 제출 날짜]
* **승인**: [!UICONTROL 제출 날짜]
* **증명 승인**: [!UICONTROL 증명 기한]

## 검색 [!UICONTROL 작업 목록]

검색할 때 [!UICONTROL 작업 목록]에 할당된 모든 항목은 검색에서 반환됩니다(현재 화면에 로드되지 않은 항목도). 다음과 같은 경우 [!UICONTROL 완료 표시] 옵션이 선택되어 있으면 지난 2주 이내에 완료로 표시한 모든 항목도 반환됩니다.

또한 작업 항목의 이름만 검색됩니다(작업 항목 내의 정보는 검색되지 않으며 작업 항목이 있는 프로젝트의 이름도 검색되지 않음).

을 검색하려면 [!UICONTROL 작업 목록]:

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. (선택 사항) 다음을 필터링하고 그룹화합니다. [!UICONTROL 작업 목록]에 설명된 대로 [필터 [!UICONTROL 작업 목록]](#filter-the-work-list) 및 [날짜, 프로젝트 및 우선 순위별로 그룹화 및 정렬](#group-and-sort-by-date-project-and-priority).

1. (선택 사항) 이미 완료된 작업 항목을 검색하는 경우 다음을 구성해야 합니다 [!UICONTROL 작업 목록] 검색 전에 완료된 항목을 표시합니다.

1. 검색 아이콘 클릭 ![검색](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. 검색 중인 항목 이름의 이름을 입력하십시오.\
   다음 [!UICONTROL 작업 목록] 이름이 일치하는 항목을 포함하도록 자동으로 필터링됩니다.

## 작업 목록 크기 변경

크기 변경 가능 [!UICONTROL 작업 목록] 따라서 홈 영역의 약 1/4~의 절반 정도를 사용합니다. [!UICONTROL 홈] 영역입니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 마우스로 오른쪽 가장자리 [!UICONTROL 작업 목록]을 클릭한 다음 작업 목록 이 원하는 크기가 될 때까지 왼쪽 또는 오른쪽으로 드래그합니다.

## 그룹화 축소 및 확장

의 항목 [!UICONTROL 작업 목록] 그룹화 내에 표시됩니다. 그룹화를 축소 및 확장하여 주어진 시간에 페이지에 표시되는 정보의 양을 제어할 수 있습니다.

내에서 그룹화를 축소하고 확장할 수 있습니다. [!UICONTROL 작업 목록] 표시되는 정보를 보다 효과적으로 제어할 수 있습니다.\
기본적으로 [!UICONTROL 이번 주] 그룹화가 확장되고 다른 모든 그룹화가 축소됩니다. 변경한 내용은 다음에 홈 영역에 액세스할 때 기억됩니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 다음을 클릭합니다. **[!UICONTROL 확장]** 또는 **[!UICONTROL 접기]** 확장하거나 축소할 그룹화 옆에 있는 화살표.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   또는\
   모든 그룹화를 동시에 확장하거나 축소하려면 **[!UICONTROL 확장]** 또는 **[!UICONTROL 접기]** 을 누르고 있는 동안 모든 그룹화 옆에 있는 화살표 [!UICONTROL Shift] 키.
