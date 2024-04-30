---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표에서 목표 활성화
description: 목표를 만들면 Adobe Workfront 목표가 초안 상태로 목표를 저장합니다. 초안 목표는 목표 관리의 일부가 아닙니다.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Adobe Workfront 목표에서 목표 활성화

목표를 만들면 Adobe Workfront 목표가 초안 상태로 목표를 저장합니다. 초안 목표는 목표 관리의 일부가 아닙니다.

진행 상황을 업데이트하여 목표 달성에 얼마나 근접했는지 추적하려면 목표를 활성화해야 합니다. 상태가 활성으로 변경됩니다.

목표 작성에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>결과 및 활동의 진행 상황을 업데이트하려면 먼저 목표를 활성화해야 합니다.


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
 <p>현재 라이선스: 요청 이상</p> <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">제품*</td>
 <td>
 <p> 다음 중 하나인 새 제품 요구 사항: </p>
<ul>
<li>Select 또는 Prime Adobe Workfront 플랜 및 추가 Adobe Workfront Goals 라이선스.</li>
<li>기본적으로 Workfront 목표를 포함하는 Ultimate Workfront 계획입니다. </li></ul>
 <p>또는</p>
 <p>현재 제품 요구 사항: Workfront 플랜 및 Adobe Workfront 목표에 대한 추가 라이선스. </p> <p>자세한 내용은 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront 목표 사용 요구 사항</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">액세스 수준</td>
 <td> <p>목표에 대한 액세스 편집</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">개체 권한</td>
 <td>
  <div>
  <p>목표에 대한 또는 그 이상의 권한에 대한 보기</p>
  <p>편집할 목표에 대한 권한 관리</p>
  <p>목표 공유에 대한 자세한 내용은 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront 목표에서 목표 공유</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 전제 조건

목표를 활성화하려면 목표가 활동, 결과, 프로젝트 등의 진행 표시기와 연결되어 있거나 다른 활성 목표에 맞춰져 있어야 합니다.

목표를 활성화하려면 다음 중 하나 이상을 수행하십시오.

* 목표에 결과 추가

  자세한 내용은 [Adobe Workfront 목표의 목표에 결과 추가](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* 목표에 활동 추가

  자세한 내용은 [Adobe Workfront 목표의 목표에 활동 추가](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* 목표에 프로젝트 연결

  자세한 내용은 [Adobe Workfront 목표의 목표에 프로젝트 추가](../results-and-activities/connect-projects-to-goals-overview.md).

* 활성화하려는 목표에 다른 목표 정렬

  자세한 내용은 [Adobe Workfront 목표에서 연결하여 목표 정렬](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## 목표 활성화

만든 목표나 관리 권한이 있는 목표를 활성화할 수 있습니다.

1. 활성화하려는 목표로 이동합니다. 목표 페이지가 열립니다.

1. 다음을 클릭합니다. **자세히** 메뉴 ![](../goal-management/assets/more-icon.png) 목표 이름의 오른쪽에 있는 을(를) 클릭합니다. **활성화**.

   ![](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   목표 상태가 활성으로 변경됩니다. 이제 목표에 대한 진행률을 추적할 수 있으며, 목표가 체크인 섹션에 표시되고 Workfront 목표의 그래프 섹션에서 고려됩니다
