---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront 목표의 목표에 결과 추가
description: 결과는 목표의 진행 상황을 측정합니다. 결과, 활동을 연관시키거나 목표에 목표를 정렬하지 않으면 목표를 활성화할 수 없으며 목표에 대한 진행률을 기록할 수 없습니다.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 3%

---

# Adobe Workfront 목표의 목표에 결과 추가

결과는 목표의 진행 상황을 측정합니다. 결과, 활동을 연관시키거나 목표에 목표를 정렬하지 않으면 목표를 활성화할 수 없으며 목표에 대한 진행률을 기록할 수 없습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> 
   <p>새 플랜 및 라이선스 구조의 경우:
  <ul><li>궁극적인 플랜 </li></ul>
   </p>
<p>현재 플랜 및 라이선스 구조의 경우: 
<ul><li> Pro 이상 </li>
  <li>Workfront 라이선스 외에 Adobe Workfront Goals 라이선스.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront 라이센스*</td>
 <td>
 <p>새 라이선스: 기여자 이상</p>
 또는
 <p>현재 라이선스: 요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>를 참조하십시오.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">제품*</td>
 <td>
 <p> 다음 중 하나인 새 제품 요구 사항: </p>
<ul>
<li>Select 또는 Prime Adobe Workfront 플랜 및 추가 Adobe Workfront Goals 라이선스.</li>
<li>기본적으로 Workfront 목표를 포함하는 Ultimate Workfront 계획입니다. </li></ul>
 <p>또는</p>
 <p>현재 제품 요구 사항: Workfront 플랜 및 Adobe Workfront 목표에 대한 추가 라이선스. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표를 사용하기 위한 요구 사항</a>을 참조하십시오. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>액세스 수준</p></td>
 <td> <p>목표에 대한 액세스 편집</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>를 참조하십시오. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 전제 조건

시작하려면 먼저 다음 항목이 있어야 합니다.

* 메인 메뉴에 목표 영역을 포함하는 레이아웃 템플릿입니다.
* 기존 목표입니다.

  목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오.

>[!IMPORTANT]
>목표는 총 1000개를 초과하는 활동, 결과, 프로젝트 또는 정렬된 목표를 가질 수 없습니다.

## 목표에 결과 추가

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. 기본 메뉴 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.

1. **목표 목록**&#x200B;에서 목표 페이지를 열 목표 이름을 클릭합니다.
1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.
1. **새 진행률 표시기** 드롭다운 메뉴를 확장한 다음 **결과 만들기**&#x200B;를 클릭합니다.

   새 결과(New result) 상자가 열립니다.

   ![](assets/new-result-box-unshimmed.png)

1. **결과 이름** 필드에 결과 이름을 입력하십시오. 필수 필드입니다.
1. (선택 사항) 다른 사용자에게 결과를 할당하려면 **결과 소유자** 필드에서 이름을 제거합니다. 기본적으로 사용자가 만드는 활동의 소유자입니다.

   >[!NOTE]
   >
   >팀, 그룹 또는 회사를 결과 소유자로 할당할 수 없습니다.

1. **에서 결과를 어떻게 측정하시겠습니까?** 영역에서 다음 정보를 지정하십시오.
   * **값 형식**: 결과의 진행률을 측정하는 방법을 나타냅니다. 진행률을 백분율로 측정하거나 통화 금액을 사용하여 수치로 측정할 수 있습니다.

     다음 표에 나열된 옵션에서 값 유형을 선택합니다.

     | 값 유형 | 설명 |
     |---------------------------------------------------------|------------------|
     | 숫자 | 숫자 값 |
     | % | 백분율 값 |
     | CN, DKK,KR,Mex$, R, R$, ze우, 파운드 , € , ₹, ฿, MYR, ₪, $ | 통화 값 |

   * **초기 값**: 결과가 진행률이 기록되기 전에 시작 부분에 있는 값입니다.
   * **목표 값**: 완료된 것으로 간주될 때 결과의 목표 값입니다.
1. **결과 만들기**&#x200B;를 클릭합니다.

   결과는 목표 페이지의 진행 표시기 섹션(결과 그룹화 아래)에 표시됩니다.

   목표를 활성화하면 결과의 진행 상황을 업데이트할 때 목표의 진행 상황이 자동으로 업데이트됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../goal-management/activate-goals.md)를 참조하십시오.
