---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Workfront 목표에서 목표 공유
description: 목표를 공유할 때 목표를 만들지 않은 사람에게 목표에 대한 관리 권한을 제공합니다.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Adobe Workfront 목표에서 목표 공유

목표를 공유할 때 목표를 만들지 않은 사람에게 목표에 대한 관리 권한을 제공합니다.

## 액세스 요구 사항

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>
-->

다음 항목이 있어야 합니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>목표 이상에 대한 액세스 편집</p> <p><b>메모</b><p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 다음을 참조하십시오.</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront 목표에 대한 액세스 권한 부여</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <div> 
     <p>목표에 대한 권한 관리</p> 
     <p>목표 공유에 대한 자세한 내용은 <a href="#" class="MCXref xref selected">Workfront 목표에서 목표 공유</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿.

## 목표 공유에 대한 고려 사항

* 사용자에게 목표에 대해 다음 권한을 가질 수 있습니다.

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
      <p>사용자는 목표를 볼 수 있는 권한이 있지만 목표에 대한 정보를 편집할 수는 없으며 결과 또는 활동에 대한 정보를 추가 또는 편집할 수 없거나, 상태를 업데이트하거나, 목표를 삭제할 수 없습니다.</p>      
      <p>기본적으로 목표에 액세스할 수 있는 모든 사용자는 시스템의 모든 목표를 볼 수 있습니다. 액세스 수준에서 목표에 대한 편집 액세스 권한이 있는 경우 목표를 복사할 수 있습니다.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>관리</p></td> 
      <td> <p>사용자는 결과나 삭제 등의 활동을 포함하여 목표에 대한 모든 정보를 편집할 수 있습니다.</p> 
      <p>목표에 대한 관리 권한이 특별히 부여된 목표 생성자나 사용자만 목표를 관리할 수 있습니다.</p> 
      목표에 대한 관리 권한이 있는 사용자만 목표를 다른 사용자와 공유하여 목표에 대한 관리 권한을 제공할 수 있습니다. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 다음 유형의 목표를 다른 사용자와 공유할 수 있습니다.

   * 사용자가 만든 목표
   * 관리 권한이 부여된 다른 사람이 만든 목표입니다.

* 목표에 대한 관리 권한이 있는 경우 목표 작성자에 대한 목표에 대한 권한을 변경할 수 있습니다. 기본적으로 목표를 만들 때 관리 권한이 있지만, 권한을 보기로 변경할 수 있습니다.

## 목표 공유

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) > **목표** 오른쪽 상단 모서리에서

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   목표 목록이 표시됩니다.

1. 목록에서 목표 이름을 클릭합니다. 목표 페이지가 열립니다.

1. 을(를) 클릭합니다. **자세히 아이콘** 목표 이름 옆에 있는 을 클릭합니다. **공유**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   목표 액세스 상자가 표시됩니다.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 다음 중 하나를 수행하십시오.

   * 을(를) 선택합니다 **시스템 전체 관리** 액세스 수준에서 목표에 대한 편집 액세스 권한이 있는 시스템 모든 사용자에게 관리 권한을 제공하는 설정. 이 옵션은 모든 새로운 목표에 대해 기본적으로 선택 취소되어 있습니다.
   * 에서 관리 권한을 부여할 사용자 이름을 입력합니다 **관리 액세스 권한 부여** 상자. 목록에 표시될 이름을 선택합니다.

      >[!TIP]
      >
      >목표를 다른 사용자와만 공유할 수 있습니다. 그룹, 팀 또는 회사와 목표를 공유할 수 없습니다.

1. 클릭 **공유**.

   목표는 지정한 사용자와 공유됩니다. 목표에 대한 관리 권한이 있는 사용자 이름 또는 &quot;시스템 전체&quot; 레이블은 목표 세부 정보 패널의 관리 액세스 필드에 표시됩니다.

## 목표 권한 옵션

다음 표에는 목표를 공유할 때 부여할 수 있는 권한이 나와 있습니다. 라이센스를 기반으로 하는 액세스 사용자에 대한 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>액션</strong> </p> </th> 
   <th> <p><strong>관리</strong> </p> </th> 
   <th> <p><strong></strong> 보기 </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>목표 보기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>결과 또는 활동 보기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>목표 복사* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>결과 또는 활동을 다른 목표로 변환*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>활동으로 추가된 프로젝트 보기** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>목표 편집</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>결과 또는 활동 편집</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>목표에 대한 결과 또는 활동 추가</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트를 목표에 활동으로 연결**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>목표 삭제</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>결과 또는 활동 삭제</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>목표에서 프로젝트 연결 끊기</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*결과와 활동을 목표로 전환하려면 액세스 수준에서 목표에 대한 편집 액세스 권한이 있어야 합니다.

**추가된 프로젝트에 대한 프로젝트 보기 및 보기 권한에 대한 액세스 권한이 있거나 목표에 추가하여 볼 수 있어야 합니다.

프로젝트 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

프로젝트 권한에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
