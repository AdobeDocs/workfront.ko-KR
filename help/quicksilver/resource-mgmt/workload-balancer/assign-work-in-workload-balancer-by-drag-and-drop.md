---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 드래그 앤 드롭으로 업무 균형자에서 작업 할당
description: 작업 항목을 올바른 사용자에게 끌어다 놓아 Adobe Workfront 업무 균형자를 사용하여 작업 항목을 할당할 수 있습니다.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 69ac06c36440d9fbbf0c8c9f3e019374da2e2f91
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---

# 드래그 앤 드롭으로 업무 균형자에서 작업 할당

{{preview-fast-release-general}}

작업 항목을 올바른 사용자에게 끌어다 놓아 Adobe Workfront 업무 균형자를 사용하여 작업 항목을 할당할 수 있습니다.

업무 균형자를 사용하여 사용자에게 작업을 할당하는 방법에 대한 일반 정보는 [업무 균형자에서 작업 할당 개요](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 리소스 조달 영역의 업무 균형자에서 작업을 할당하도록 계획합니다.</br>
       팀 또는 프로젝트의 업무 균형자에서 작업을 할당하려면 작업</p></td>
  </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음에 대한 액세스 권한 편집:</p> 
    <ul> 
     <li>리소스 관리</li> 
     <li>프로젝트</li> 
     <li>작업</li> 
     <li>문제</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>할당이 포함된 프로젝트, 작업 및 문제에 권한 이상 기여</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 드래그 앤 드롭하여 항목 할당

미할당 작업 영역에서 사용자에게 품목을 지정하거나 이미 할당된 항목을 할당된 작업 영역의 다른 사용자에게 재할당할 수 있습니다.

1. 작업을 할당할 업무 균형자로 이동합니다.

   리소스 영역, 프로젝트 또는 팀 수준에서 업무 균형자 를 사용하여 사용자에게 작업을 할당할 수 있습니다. Workfront에서 업무 균형자 위치에 대한 자세한 내용은 [업무 균형자 찾기](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)를 참조하십시오.

1. (선택 사항) **할당 해제된 작업** 영역으로 이동하여 필터를 적용하여 사용자에게 할당되지 않은 작업, 문제, <span class="preview">및 역할 할당</span>을 봅니다

   또는

   해당 항목을 다시 할당하려면 **할당된 작업** 영역으로 이동하여 할당된 작업 항목을 볼 사용자 이름을 확장하세요.

   >[!NOTE]
   >
   ><span class="preview">역할 할당 표시 설정을 사용하면 할당 해제된 작업 영역의 작업 항목 아래에 역할 할당이 표시됩니다. 자세한 내용은 [업무 균형자 이동](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view)에서 [보기 사용자 지정](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)을 참조하십시오.</span>

1. (조건부) 프로젝트의 업무 균형자에서 **모든 사용자 표시** 아이콘 ![모든 사용자 표시](assets/show-all-users-icon-project-workload-balancer.png)를 클릭하여 모든 Workfront 사용자를 표시합니다.

   보기 액세스 권한이 있는 모든 사용자가 표시됩니다.

   프로젝트 팀에 속해 있고 프로젝트의 항목에 이미 할당된 사용자에게는 할당된 작업 영역에서 이름 오른쪽에 프로젝트 아이콘이 표시됩니다.

   프로젝트의 ![사용자](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)

   >[!TIP]
   >
   >* 모든 사용자 표시 옵션은 프로젝트의 업무 균형자에서만 사용할 수 있습니다.
   >* 필터를 사용하여 자신에게 중요한 사용자만 표시합니다. 예를 들어 필터를 사용하여 팀이나 그룹의 사용자만 표시할 수 있습니다.

1. 계획된 또는 예상 타임라인을 나타내는 작업 항목 <span class="preview">또는 역할 할당</span>의 표시줄을 클릭하고 **할당됨** 영역에서 사용자 이름으로 끌어서 놓습니다.

   작업 항목을 놓기 위해 마우스를 가져다 대는 사용자가 강조 표시됩니다.

   <span class="preview">역할 할당을 끌어다 놓을 때 현재 역할이 역할 할당과 일치하지 않으면 주황색으로 강조 표시됩니다. 역할이 일치하지 않아도 사용자에게 작업을 할당할 수 있습니다.</span>

   >[!TIP]
   >
   >마우스로 가리키고 있는 사용자의 계획된 시간은 작업 항목에서 매일 계획된 시간의 수로 실시간으로 업데이트되어, 전체 할당에 새 항목을 추가할 때 어떤 영향이 있을 수 있는지 나타냅니다.

   <span class="preview">미리 보기 환경의 샘플 이미지:</span>
   ![사용자에게 할당할 항목 삭제](assets/wb-drag-drop-role-or-task-to-user.png)

   프로덕션 환경의 샘플 이미지:
   ![사용자에게 할당할 항목 삭제](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 준비가 되면 선택한 작업 항목 <span class="preview">이나 역할 할당</span>을(를) 할당된 영역의 사용자 이름과 같은 줄에 놓습니다. 항목이 할당되고 할당된 계획 시간이 작업 항목의 새 시간과 함께 사용자에 대해 업데이트됩니다.

   <span class="preview">역할 할당 표시 설정이 활성화되지 않은 경우</span> 작업 항목이 사용자가 이행할 수 없는 작업 역할에 할당되면 항목이 할당된 작업 영역의 사용자 이름 아래에 표시됩니다. 또한 미할당 작업 영역에 남아 있어 관련된 작업 역할이 아직 사용자에 의해 대체되지 않았음을 나타냅니다.

   >[!TIP]
   >
   >* 설정 영역에서 프로젝트별 그룹을 활성화한 경우 할당된 작업이 해당 프로젝트 아래에 표시됩니다. 이 설정을 사용하지 않으면 할당된 작업이 사용자 영역에 표시됩니다.
   >
   >
   >     작업 항목을 정렬하기 위한 업무 균형자 기준에 따라 항목이 표시됩니다. 자세한 내용은 [업무 균형자 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)을 참조하십시오.
   >
   >
   >* 프로젝트의 업무 균형자에 모든 사용자 표시를 활성화하고 프로젝트의 항목에 이전에 할당되지 않은 사용자에게 항목을 할당한 경우 사용자는 프로젝트 팀에 추가됩니다. 자세한 내용은 [프로젝트 팀 관리](../../manage-work/projects/planning-a-project/manage-project-team.md)를 참조하십시오.


1. (선택 사항) 할당된 작업 영역에서 사용자 이름 아래에 있는 작업 항목의 막대를 클릭하고 드래그한 다음 미할당 작업 영역에 놓아 할당을 취소합니다. 사용자에게서 항목의 할당이 해제되었지만, 여전히 작업 역할에 할당될 수 있으며, 이 경우 할당 해제된 작업 영역에 표시됩니다. 항목이 다른 사용자에게 할당된 경우 여전히 할당된 사용자의 이름으로 할당된 작업 영역에 유지됩니다.
1. (선택 사항) **할당 표시 아이콘** ![할당 표시 아이콘](assets/show-allocations-icon-small.png)을 클릭한 다음 **추가 메뉴** ![추가 메뉴](assets/qs-more-menu.png) > **할당 편집**&#x200B;을 클릭합니다.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   또는

   일별 또는 주별 할당을 두 번 클릭하여 사용자가 작업 항목에 할당된 시간을 수정합니다.

   업무 균형자에서 사용자 할당을 수정하는 방법에 대한 자세한 내용은 문서 [업무 균형자에서 사용자 할당 관리](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)의 &quot;사용자 할당 수정&quot; 섹션을 참조하십시오.

   업무 균형자를 사용하여 작업 항목에서 할당을 제거하는 방법에 대한 자세한 내용은 [업무 균형자에서 작업 할당 해제](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)를 참조하십시오.

