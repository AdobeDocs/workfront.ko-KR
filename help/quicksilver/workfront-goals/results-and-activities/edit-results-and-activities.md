---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront 목표에서 결과 및 활동 편집
description: Adobe Workfront 관리자가 Adobe Workfront 목표에 대한 올바른 액세스 권한을 부여하면 목표, 결과 및 활동을 만들고 편집할 수 있습니다.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---

# Adobe Workfront 목표에서 결과 및 활동 편집

Adobe Workfront 관리자가 Adobe Workfront 목표에 대한 올바른 액세스 권한을 부여하면 목표, 결과 및 활동을 만들고 편집할 수 있습니다.

목표, 결과 및 활동 작성에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront 목표에서 결과 및 활동 시작](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Adobe Workfront 목표의 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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
  <ul><li>궁극적인 플랜 </li>
  또는
  <li>Prime 또는 Select Adobe Workfront 플랜에 대한 Adobe Workfront Goals에 대한 추가 라이센스입니다. </li></ul> </p>
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
 <td> <p>목표에 대한 액세스 편집</p> </td>
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

## 결과 및 활동 편집 시 고려 사항

<!--
According to Vazgen, access levels will add more considerations.)
-->

* 만든 목표나 관리 권한이 있는 목표에 속하는 결과 및 활동을 편집할 수 있습니다.
* Workfront 목표의 활동으로 목표에 연결된 프로젝트의 진행률을 편집할 수 없습니다. 프로젝트의 작업이 완료되면 프로젝트 진행률이 업데이트됩니다. 프로젝트의 연결을 해제하여 목표에서 프로젝트를 제거할 수 있습니다. 자세한 내용은 문서 [Adobe Workfront 목표의 목표에서 결과, 활동 및 프로젝트 제거](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)의 &quot;프로젝트 연결 끊기&quot; 섹션을 참조하십시오.

  >[!NOTE]
  >
  >다음 프로젝트 정보가 프로젝트 수준에서 업데이트되면 Workfront 목표가 목표 수준에서 자동으로 업데이트합니다.
  >
  >   
  >   
  >   * 프로젝트 소유자
  >   * 프로젝트 이름
  >   * 프로젝트 완료율
  >   
  >   
  >목표에 프로젝트를 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)를 참조하십시오.

* 결과 및 활동이 목표 진행률과 더 이상 관련이 없는 경우 목표에서 삭제할 수 있습니다. 삭제된 결과 및 활동은 복구할 수 없습니다. 결과 및 활동 삭제에 대한 자세한 내용은 [Adobe Workfront 목표의 목표에서 결과, 활동 및 프로젝트 제거](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)를 참조하십시오.
* 과거를 포함하여 모든 기간의 목표와 연관된 결과 및 활동을 편집할 수 있습니다.
* 결과 및 활동을 편집하면 설정이 업데이트되고 진행률이 업데이트되지 않습니다. 결과 및 활동의 진행 상황을 업데이트해야 합니다. 목표, 결과 및 활동에 대한 진행 상황 업데이트에 대한 자세한 내용은 [Adobe Workfront 목표의 목표 진행 상황 업데이트](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)를 참조하십시오.

## 결과 편집

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. **주 메뉴** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.
1. 목표 목록에서 목표 이름을 클릭하여 목표 페이지를 엽니다.
1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.
1. 진행 상태 표시기 목록에서 결과를 선택하고 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

   결과 편집(Edit Result) 상자가 열립니다.

   ![](assets/edit-result-box-unshimmed.png)

1. 다음 정보를 편집합니다.
   * **결과 이름**: 결과의 이름입니다. 목표를 달성하기 위해 어떤 결과를 얻어야 하는지를 보여 주는 수사적 이름을 사용하십시오.
   * **결과 소유자**: 결과의 소유자입니다. 소유자는 활성 Workfront 사용자여야 합니다.
   * **값 형식**: 결과의 진행 상황을 측정하는 방법.
   * **초기 값**: 결과의 원래 값입니다.
   * **대상 값**: 결과가 완료되면 원하는 값입니다.
결과 필드에 대한 자세한 내용은 [목표에 결과 추가](../results-and-activities/add-results-to-goals.md)를 참조하십시오.
1. **저장**&#x200B;을 클릭합니다.

## 활동 편집

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. **주 메뉴** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **목표**&#x200B;를 클릭합니다.
1. 목표 목록에서 목표 이름을 클릭하여 목표 페이지를 엽니다.
1. 왼쪽 패널에서 **진행률 표시기**&#x200B;를 클릭합니다.
1. 진행 상태 표시기 목록에서 활동을 선택하고 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

   활동 편집 상자가 열립니다.

   ![](assets/edit-activity-box-unshimmed.png)

1. 다음 정보를 편집합니다.
   * **활동 이름**: 활동의 이름입니다. 목표가 완료되었음을 나타내기 위해 수행해야 하는 활동을 설명하는 수사적 이름을 사용합니다.
   * **활동 소유자:** 활동의 소유자입니다. 소유자는 활성 Workfront 사용자여야 합니다.\
     활동 필드에 대한 자세한 내용은 [목표에 활동 추가](../results-and-activities/add-activities-to-goals.md)를 참조하십시오.
1. **저장**&#x200B;을 클릭합니다.


