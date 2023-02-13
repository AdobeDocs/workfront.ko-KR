---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서를 사용하여 수동으로 작업 할당
description: Adobe Workfront 작업 로드 밸런서를 사용하여 사용자에게 작업 항목을 수동으로 할당할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 2%

---

# 작업 로드 밸런서를 사용하여 수동으로 작업 할당

Adobe Workfront 작업 로드 밸런서를 사용하여 사용자에게 작업 항목을 수동으로 할당할 수 있습니다.

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
   <td> <p>팀 또는 자원 영역에서 작업 로드 밸런서를 사용할 계획 </p>
   <p>프로젝트의 작업 로드 밸런서를 사용할 때 작업 </p>
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

## 작업 로드 밸런서에서 수동으로 작업 할당

사용자에게 아직 할당되지 않은 작업 항목을 할당하거나 작업 로드 밸런서에서 사용자에게 할당된 항목을 재할당할 수 있습니다.

1. 작업을 할당하려는 작업 로드 밸런서로 이동합니다.

   자원 조정 영역, 프로젝트 또는 팀 레벨에서 작업 로드 밸런서를 사용하여 사용자에게 작업을 할당할 수 있습니다. 작업 로드 밸런서가 Workfront에 있는 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (선택 사항) 로 이동합니다. **할당되지 않은 작업** 영역 및 필터를 적용하여 작업 또는 문제 보기

   또는

   로 이동합니다. **지정된 작업 시간** 항목을 재할당하려는 경우 해당 항목에 지정된 작업 항목을 볼 수 있도록 영역을 확장하고 사용자 이름을 확장합니다.

1. 을(를) 클릭합니다. **추가 메뉴** ![](assets/qs-more-menu.png) 작업 항목 이름의 왼쪽에 있는 **여기에 지정**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >다음 단축키를 사용하여 작업이나 문제를 할당할 수도 있습니다.
   >
   >* Windows에서: 작업 또는 문제 표시줄을 Ctrl+클릭합니다.
   >* Mac에서: CMD를 클릭한 채 작업 또는 문제 표시줄을 클릭합니다.


1. 다음 중 하나를 수행하십시오.

   * 의 항목에 할당할 사용자, 작업 역할 또는 팀의 이름을 입력합니다. **사람, 역할 또는 팀 검색** 필드를 선택한 다음 목록에 표시될 때 선택한 다음 **저장**.
   >[!TIP]
   >
   >사용자를 추가할 때 아바타, 사용자의 기본 역할 및 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Workfront 또는 그룹 관리자가 사용자 환경에서 위임을 활성화한 경우 지정 탭을 사용하여 사용자를 작업이나 문제에 지정합니다. 위임 탭을 사용하여 작업 항목에 위임된 사용자를 봅니다. 작업 위임에 대한 자세한 내용은 [작업 및 문제 위임 관리](../../manage-work/delegate-work/how-to-delegate-work.md).


   이렇게 하면 지정된 담당자에게 작업 항목이 할당되거나 재지정됩니다.

   팀 또는 작업 역할에만 품목을 지정하면 해당 품목이 미지정 작업 영역에만 표시됩니다. 작업 로드 밸런서의 지정된 작업 영역 내에 표시하려면 작업 항목을 사용자에게 지정해야 합니다.

   >[!TIP]
   >
   >여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >
   >사용자, 작업 역할 또는 팀이 비활성화되기 전에 할당된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
   >
   >   
   >   
   >   * 작업 항목을 활성 자원에 재지정합니다.
   >   * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


   * 클릭 **고급** 고급 지정에 액세스하려면

      고급 지정 만들기에 대한 자세한 내용은 [고급 할당 만들기](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. (선택 사항) **할당 표시 아이콘** ![](assets/show-allocations-icon-small.png)를 클릭한 다음 **추가 메뉴** ![](assets/qs-more-menu.png) > **할당 편집**.

   또는

   일별 또는 주별 할당을 두 번 눌러 사용자가 작업 항목에 할당되는 시간을 수정합니다.

   작업 로드 밸런서에서 사용자 할당 수정에 대한 자세한 내용은 문서의 &quot;사용자 할당 수정&quot; 섹션을 참조하십시오 [작업 로드 밸런서에서 사용자 할당 관리](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   작업 로드 밸런서를 사용하여 작업 항목에서 지정을 제거하는 방법에 대한 자세한 내용은 [작업 로드 밸런서에서 작업 할당 취소](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
