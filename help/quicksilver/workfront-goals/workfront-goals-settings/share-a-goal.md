---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Workfront 목표에서 목표 공유
description: 목표를 공유하면 목표를 만들지 않은 사람에게 목표에 대한 관리 권한을 부여합니다.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---

# Adobe Workfront 목표에서 목표 공유

목표를 공유하면 목표를 만들지 않은 사람에게 목표에 대한 관리 권한을 부여합니다.

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
 <p>현재 라이선스: 요청 이상</p> </td>
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
 <td role="rowheader">액세스 수준</td>
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

## 목표 공유에 대한 고려 사항

* 사용자는 목표에 대해 다음과 같은 권한을 가질 수 있습니다.

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>목표 권한</b></p></td> 
      <td>
      <p><b>설명</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>보기</p></td> 
      <td>
      <p>사용자는 목표를 볼 수 있는 권한이 있지만 목표에 대한 정보를 편집할 수 없으며 결과 또는 활동에 대한 정보를 추가 또는 편집하거나 상태를 업데이트하거나 목표를 삭제할 수 없습니다.</p>      
      <p>기본적으로 목표에 대한 액세스 권한이 있는 모든 사용자는 시스템의 모든 목표를 볼 수 있습니다. 사용자가 자신의 액세스 수준에 있는 목표에 대한 편집 액세스 권한이 있는 경우 목표를 복사할 수 있습니다.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>관리</p></td> 
      <td> <p>사용자는 결과를 포함하여 목표에 대한 모든 정보 또는 삭제를 포함하여 활동에 대한 모든 정보를 편집할 수 있습니다.</p> 
      <p>목표에 대한 관리 권한이 특별히 부여된 목표 작성자 또는 사용자만 목표를 관리할 수 있습니다.</p> 
      목표에 대한 관리 권한이 있는 사용자만 목표를 다른 사용자와 공유하여 목표에 대한 관리 권한을 부여할 수 있습니다. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 다음 유형의 목표를 다른 사용자와 공유할 수 있습니다.

   * 목표를 만들었습니다.
   * 관리할 권한이 있는 다른 사용자가 만든 목표입니다.

* 목표에 대한 관리 권한이 있는 경우 목표 작성자에 대한 목표에 대한 권한을 변경할 수 있습니다. 기본적으로 목표를 생성할 때 관리 권한이 있지만, 해당 권한을 보기로 변경할 수 있습니다.

## 목표 공유

1. 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표**&#x200B;를 클릭합니다.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   목표 목록이 표시됩니다.

1. 목록에서 목표의 이름을 클릭합니다. 목표 페이지가 열립니다.

1. 목표 이름 옆에 있는 **자세히 아이콘**&#x200B;을 클릭한 다음 **공유**&#x200B;를 클릭합니다.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   목표 액세스 상자가 표시됩니다.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 다음 중 하나를 수행하십시오.

   * **시스템 전체 관리** 설정을 선택하여 액세스 수준의 목표에 대한 편집 액세스 권한이 있는 시스템의 모든 사용자에게 관리 권한을 부여합니다. 기본적으로 모든 새 목표에 대해 선택 취소됩니다.
   * **관리 액세스 권한 부여** 상자에서 관리 권한을 부여할 사용자의 이름을 입력하세요. 목록에 표시되면 이름을 선택합니다.

     >[!TIP]
     >
     >다른 사용자와 목표를 공유할 수만 있습니다. 그룹, 팀 또는 회사와 목표를 공유할 수 없습니다.

1. **공유**&#x200B;를 클릭합니다.

   목표를 지정한 사용자와 공유합니다. 목표에 대한 관리 권한이 있는 사용자의 &quot;시스템 전체&quot; 레이블 또는 이름이 목표 세부 정보 패널의 관리에 대한 액세스 필드에 표시됩니다.

## 목표 권한 옵션

다음 표에는 목표를 공유할 때 부여할 수 있는 권한이 나열되어 있습니다. 사용자가 라이선스를 기반으로 하는 액세스 권한에 대한 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)를 참조하십시오.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>관리</strong> </p> </th> 
   <th> <p><strong>보기</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>목표 보기</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
  </tr> 
  <tr> 
   <td> <p>결과 또는 활동 보기</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
  </tr> 
  <tr> 
   <td>목표 복사* </td> 
   <td>✓ 덧신 </td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>결과 또는 활동을 다른 목표로 변환*</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td>활동으로 추가된 프로젝트 보기** </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td>목표 편집</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>결과 또는 활동 편집</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>목표에 대한 결과 또는 활동 추가</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트를 목표에 대한 활동으로 연결합니다**</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>목표 삭제</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>결과 또는 활동 삭제</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>목표에서 프로젝트 연결 해제</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*결과 및 활동을 목표로 전환하려면 액세스 수준에서 목표에 대한 편집 액세스 권한이 있어야 합니다.

**추가된 프로젝트 또는 보기 목표에 추가하려는 프로젝트에 대한 프로젝트 보기 및 보기 권한에 대한 액세스 권한이 있어야 합니다.

프로젝트 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

프로젝트 권한에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.

 
