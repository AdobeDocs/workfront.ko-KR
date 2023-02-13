---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront 목표 펄스 섹션에서 목표 검토
description: 소유자가 누구인지에 관계없이 조직의 모든 목표를 볼 수 있습니다. 목표 만들기에 대한 자세한 내용은 Adobe Workfront 목표에서 목표 만들기 를 참조하십시오.
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Adobe Workfront 목표 펄스 섹션에서 목표 검토

>[!IMPORTANT]
> 
>이 문서에 설명된 기능은 23.1 릴리스부터 Workfront에서 제거되었습니다.\
>이 문서는 2023년 초에 23.1 릴리스 직후 제거됩니다. 지금은 이에 따라 책갈피를 업데이트하는 것이 좋습니다.


소유자가 누구인지에 관계없이 조직의 모든 목표를 볼 수 있습니다. 목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).

Adobe Workfront 목표의 펄스 섹션을 공동 작업 도구로 사용할 수 있습니다. 이 도구를 통해 사용자, 팀, 그룹 또는 조직에 속한 현재 목표에 대한 업데이트 스트림을 검토하고 참여하며 해당 목표를 최신 상태로 유지할 수 있습니다. Workfront 목표는 펄스 섹션에서 목표별로 진행 상태 업데이트, 댓글 및 편집 내역을 그룹화합니다.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> <p>이 문서에 설명된 기능에 액세스하려면 Adobe Workfront 목표에 대한 추가 라이센스를 구매해야 합니다. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>목표에 대한 액세스 권한 보기 이상</p> <p>참고:  <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 보기 이상</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하려면 먼저 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 펄스 섹션에서 목표 업데이트 및 주석 관리 

>[!TIP]
>
>적어도 한 번 이상 체크 인된 목표만 [펄스] 섹션에 표시됩니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 화면 오른쪽 상단 모서리에서 을(를) 클릭합니다.

   이렇게 하면 Workfront 목표 영역이 열립니다.

   기본적으로 모든 목표가 표시됩니다.

1. 클릭 **펄스** 왼쪽 패널에 표시됩니다.

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   목표 목록이 표시됩니다. 목록에는 각 목표에 대한 정보가 있는 다음 열이 포함되어 있습니다.

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">목표</td> 
         <td>목표 이름.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">소유자</td> 
         <td>목표 소유자의 이름입니다.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">기간</td> 
         <td>목표가 예약된 기간입니다.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">진행</td> 
         <td>일반적으로 백분율 값인 목표에 대한 진행률 표시기입니다.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>상태(정렬 아이콘 포함)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>목표 상태는 다음 중 하나일 수 있습니다.</p> 
         <ul> 
         <li>활성</li> 
         <li>초안</li> 
         <li>비활성</li> 
         <li>마감됨</li> 
         </ul> <p>정렬 아이콘은 다른 목표에 정렬된 목표에 나타납니다. 목표 정렬에 대한 자세한 내용은 <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Adobe Workfront 목표에 연결하여 목표 정렬</a>.</p>

   <p>상태 열에는 목표에 체크인된 각 결과 또는 활동에 대한 증분 업데이트가 포함됩니다.</p>

   예를 들어, 목표에 하나의 수동 진행률 표시줄 활동이 있고, 목표에 대해 체크인하고 활동을 50%로 업데이트하는 경우 상태 열에는 해당 목표의 활동에 대한 50%가 표시됩니다. 나중에 동일한 활동을 60%로 업데이트할 수 있습니다. 이 경우 활동의 진행 상태에 10%를 추가했으므로, 10%의 동일한 활동에 대해 동일한 목표 아래에 새 줄이 표시됩니다.
   </td>
   </tr> 
      </tbody> 
      </table>

1. (선택 사항) [펄스] 섹션의 오른쪽 위 모서리에서 필터를 업데이트하여 표시할 정보 유형을 선택합니다.

   펄스 목록에는 선택한 필터의 기준과 일치하는 목표 및 업데이트된 기록이 표시됩니다.

   필터링 목표에 대한 자세한 내용은 [Adobe Workfront 목표에서 정보 필터링](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 목표를 확장하고 각 목표에 대한 업데이트에 대한 추가 정보를 보려면 목표 이름 왼쪽의 오른쪽 화살표를 클릭합니다.

   다음 정보는 각 목표 아래의 펄스 섹션에 표시됩니다.

   * 결과 이름 및 소유자. 결과에 대한 자세한 내용은 [Adobe Workfront 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * 활동 이름 및 소유자. 활동에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * 결과 및 활동 진행률 표시줄 및 진행률 상태. Workfront 목표가 목표 진행률을 계산하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 및 조건 개요](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. 클릭 **댓글 추가** 목표에 대한 설명을 추가하려면 **Post**. 주석은 체크인 영역과 목표 세부 정보 패널의 업데이트 탭에 표시됩니다. 펄스 섹션을 사용하여 한동안 업데이트되지 않은 목표에 대해 설명하고 목표 소유자에게 업데이트를 요청하는 것이 좋습니다.

1. (선택 사항) **모든 업데이트 표시** 목표 업데이트를 모두 표시합니다. 그러면 오른쪽의 목표 세부 사항 패널에서 업데이트 탭이 열립니다.
1. 목표 이름을 클릭하여 **목표 세부 사항** 오른쪽의 패널에서는 목표에 대한 자세한 정보를 검토하고, 목표와 그 결과 및 활동을 관리할 수 있습니다. 개별 목표 검토에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 세부 사항 섹션에서 목표 업데이트](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (선택 사항 및 조건부) **정렬 아이콘** ![](assets/align-icon.png) 목표를 다른 목표에 맞게 정렬한 경우 목표 정렬 섹션에서 이 목표를 엽니다.

1. (선택 사항) **페이지당 목표** 드롭다운 메뉴에서 다음 옵션 중에서 선택하여 추가 목표를 표시합니다.

   * 20. 기본 선택 사항입니다.
   * 50
   * 100


