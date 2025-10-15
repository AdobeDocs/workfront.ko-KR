---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 목표 활성화
description: 목표를 만들면 Adobe Workfront 목표가 초안 상태로 목표를 저장합니다. 초안 목표는 목표 관리의 일부가 아닙니다.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# Adobe Workfront 목표에서 목표 활성화

<!--Audited for P&P only: 4/2025-->

목표를 만들면 Adobe Workfront 목표가 초안 상태로 목표를 저장합니다. 초안 목표는 목표 관리의 일부가 아닙니다.

진행 상황을 업데이트하여 목표 달성에 얼마나 근접했는지 추적하려면 목표를 활성화해야 합니다. 상태가 활성으로 변경됩니다.

목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오.

>[!IMPORTANT]
>
>결과 및 활동의 진행 상황을 업데이트하려면 먼저 목표를 활성화해야 합니다.


## 액세스 요구 사항

>[!NOTE]
>
>이전에 이 패키지를 구입한 경우 귀사에서 Adobe Workfront 목표를 계속 사용하도록 선택할 수 있습니다. 자세한 내용은 계정 담당자에게 문의하십시오.
>
>Adobe Workfront 목표를 더 이상 구매할 수 없습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
  <tr>
  <td> <p>Adobe Workfront 패키지</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr>
 <td role="rowheader">액세스 수준 구성</td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
 </tr>
 <tr>
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>시스템 관리자를 포함한 모든 사용자에게는 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 전제 조건

목표를 활성화하려면 목표가 활동, 결과, 프로젝트 등의 진행 표시기와 연결되어 있거나 다른 활성 목표에 맞춰져 있어야 합니다.

목표를 활성화하려면 다음 중 하나 이상을 수행하십시오.

* 목표에 결과 추가

  자세한 내용은 [Adobe Workfront 목표의 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md)를 참조하십시오.

* 목표에 활동 추가

  자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md)를 참조하십시오.

* 목표에 프로젝트 연결

  자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../results-and-activities/connect-projects-to-goals-overview.md)를 참조하십시오.

* 활성화하려는 목표에 다른 목표 정렬

  자세한 내용은 [Adobe Workfront 목표에서 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)을 참조하십시오.

## 목표 활성화

만든 목표나 관리 권한이 있는 목표를 활성화할 수 있습니다.

1. 활성화하려는 목표로 이동합니다. 목표 페이지가 열립니다.

1. 목표 이름 오른쪽에 있는 **자세히** 메뉴 ![자세히 아이콘](../goal-management/assets/more-icon.png)을 클릭한 다음 **활성화**&#x200B;를 클릭합니다.

   ![메뉴가 더 확장됨](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   목표 상태가 활성으로 변경됩니다. 이제 목표에 대한 진행률을 추적할 수 있으며, 목표가 체크인 섹션에 표시되고 Workfront 목표의 그래프 섹션에서 고려됩니다
