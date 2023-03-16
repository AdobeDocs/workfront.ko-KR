---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 드래그 앤 드롭으로 작업 로드 밸런서에서 작업 할당
description: 작업 항목을 올바른 사용자에게 끌어다 놓아 Adobe Workfront 작업 로드 밸런서를 사용하여 작업 항목을 할당할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 1%

---

# 드래그 앤 드롭으로 작업 로드 밸런서에서 작업 할당

<!--remove production and preview preferences at release-->

작업 항목을 올바른 사용자에게 끌어다 놓아 Adobe Workfront 작업 로드 밸런서를 사용하여 작업 항목을 할당할 수 있습니다.

작업 로드 밸런서를 사용하여 사용자에게 작업을 지정하는 방법에 대한 일반적인 정보는 [작업 로드 밸런서에서 작업 할당 개요](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>리소스 영역에서 작업 로드 밸런서에서 작업을 할당하도록 계획합니다.</p>
   <p>작업하여 팀 또는 프로젝트의 작업 로드 밸런서에서 작업을 할당합니다</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>다음에 대한 액세스 편집:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>지정 작업을 포함하는 프로젝트, 작업 및 문제에 대한 권한 이상의 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 드래그 앤 드롭으로 항목 할당

지정되지 않은 작업 영역의 품목을 사용자에게 지정하거나 지정된 작업 영역의 다른 사용자에게 이미 지정된 품목을 재지정할 수 있습니다.

1. 작업을 할당하려는 작업 로드 밸런서로 이동합니다.

   자원 조정 영역, 프로젝트 또는 팀 레벨에서 작업 로드 밸런서를 사용하여 사용자에게 작업을 할당할 수 있습니다. 작업 로드 밸런서가 Workfront에 있는 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (선택 사항) 로 이동합니다. **할당되지 않은 작업** 영역 및 필터를 적용하여 사용자에게 할당되지 않은 작업 및 문제를 봅니다

   또는

   로 이동합니다. **지정된 작업 시간** 항목을 재할당하려는 경우 해당 항목에 지정된 작업 항목을 볼 수 있도록 영역을 확장하고 사용자 이름을 확장합니다.

1. (조건부) 프로젝트의 작업 로드 밸런서에서 **모든 사용자 표시** 아이콘 ![](assets/show-all-users-icon-project-workload-balancer.png) 모든 Workfront 사용자를 표시합니다.

   여기에는 볼 수 있는 액세스 권한이 있는 모든 사용자가 표시됩니다.

   프로젝트 팀에도 속하고 프로젝트의 항목에 이미 할당된 사용자는 지정된 작업 영역에서 이름 오른쪽에 프로젝트 아이콘이 있습니다.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* 모든 사용자 표시 옵션은 프로젝트의 작업 로드 밸런서에서만 사용할 수 있습니다.
   >* 필터를 사용하여 본인에게 중요한 사용자만 표시할 수 있습니다. 예를 들어 필터를 사용하여 팀 또는 그룹의 사용자만 표시할 수 있습니다.




1. 계획된 타임라인이나 예상 타임라인을 나타내는 작업 항목의 막대를 클릭하고 **할당됨** 영역.

   마우스로 가리키면 작업 항목이 강조 표시됩니다.

   >[!TIP]
   >
   >마우스로 작업 품목의 일별 계획 시간 수를 사용하여 실시간으로 갱신하는 사용자의 계획 시간 을 사용하여 신규 품목 추가의 영향을 전체 할당에 나타낼 수 있습니다.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 준비가 되면 선택한 작업 항목을 지정된 영역에서 사용자 이름과 동일한 라인에 놓습니다. 품목이 지정되고 할당된 계획 시간은 작업 항목의 새 시간을 사용하여 사용자에 대해 갱신됩니다.

   사용자가 이행할 수 없는 작업 역할에 항목이 지정된 경우, 지정된 작업 영역에 사용자 이름 아래에 항목이 표시되고, 연관된 작업 역할이 아직 사용자에 의해 대체되지 않았음을 나타내는 [지정되지 않은 작업] 영역에도 표시됩니다.

   >[!TIP]
   >
   >* 설정 영역에서 프로젝트별 그룹 을 활성화한 경우 지정된 작업이 해당 프로젝트 아래에 표시됩니다. 설정이 비활성화되면 지정된 작업이 사용자 영역에 표시됩니다.
      >
      >
      >     작업 항목 정렬에 대한 작업 로드 밸런서 기준에 따라 항목이 표시됩니다. 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* 프로젝트의 작업 로드 밸런서에 있는 모든 사용자 표시 및 프로젝트의 항목에 이전에 할당되지 않은 사용자에게 할당된 항목을 활성화하면 사용자가 프로젝트 팀에 추가됩니다. 자세한 내용은 [프로젝트 팀 관리](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (선택 사항) 할당된 작업 영역에서 사용자의 이름으로 작업 항목의 막대를 클릭한 다음, 해당 작업 항목을 할당되지 않은 작업 영역 위로 끌어 놓습니다. 항목이 사용자로부터 지정되지 않지만 작업 역할에 지정될 수 있으며, 이 경우 미지정 작업 영역에 표시됩니다. 항목이 다른 사용자에게 지정된 경우 여전히 지정된 사용자의 이름 아래에 지정된 작업 영역 내에 남아 있습니다.
1. (선택 사항) **할당 표시 아이콘** ![](assets/show-allocations-icon-small.png)를 클릭한 다음 **추가 메뉴** ![](assets/qs-more-menu.png) > **할당 편집**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   또는

   일별 또는 주별 할당을 두 번 눌러 사용자가 작업 항목에 할당되는 시간을 수정합니다.

   작업 로드 밸런서에서 사용자 할당 수정에 대한 자세한 내용은 문서의 &quot;사용자 할당 수정&quot; 섹션을 참조하십시오 [작업 로드 밸런서에서 사용자 할당 관리](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   작업 로드 밸런서를 사용하여 작업 항목에서 지정을 제거하는 방법에 대한 자세한 내용은 [작업 로드 밸런서에서 작업 할당 취소](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

