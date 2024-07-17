---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 업무 균형자에서 작업 할당 해제
description: Adobe Workfront 업무 균형자 의 할당된 작업 영역에서 작업 항목에서 사용자 할당을 해제하거나 다른 사용자, 역할 또는 팀에 재할당할 수 있습니다.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# 업무 균형자에서 작업 할당 해제

Adobe Workfront 업무 균형자 의 할당된 작업 영역에서 작업 항목에서 사용자 할당을 해제하거나 다른 사용자, 역할 또는 팀에 재할당할 수 있습니다.

사용자를 수동으로 끌어다 놓거나 일괄적으로 지정하여 작업 항목에서 할당 해제할 수 있습니다. 이 문서에서는 사용자를 수동으로 할당 해제하는 방법을 설명합니다.

끌어다 놓기로 사용자 할당을 취소하는 방법에 대한 자세한 내용은 [끌어다 놓기로 업무 균형자에서 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)을 참조하십시오.

사용자를 일괄 할당 해제하는 방법에 대한 자세한 내용은 [업무 균형자를 사용하여 작업 일괄 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>리소스 조달 영역에서 업무 균형자 를 사용할 때 계획</p>
   <p>팀 또는 프로젝트의 업무 균형자 를 사용할 때 작업</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음에 대한 액세스 권한 편집:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>할당이 포함된 프로젝트, 작업 및 문제에 대한 Contribute 권한 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

 

## 업무 균형자에서 작업 항목 할당 해제

사용자의 항목 할당을 해제하고 할당 해제된 작업 영역으로 이동하거나 다른 사용자에게 재할당할 수 있습니다.

사용자로부터 작업 항목 할당을 취소하려면 다음을 수행합니다.

1. 업무 균형자에서 **할당된 작업** 영역으로 이동하여 사용자를 확장합니다.
1. 다음 중 하나를 수행하십시오.

   * 사용자 영역에서 할당 해제할 항목을 찾아 클릭한 다음 할당 해제된 영역 또는 다른 사용자 영역으로 끌어서 놓습니다.
   * 작업 항목 이름 오른쪽에 있는 **자세히** 아이콘 ![](assets/more-icon-task-list.png)을 클릭하고 **할당 대상**&#x200B;을 클릭한 다음 작업 항목에 할당된 엔터티 이름을 제거하거나 다른 이름을 입력하고 **저장**&#x200B;을 클릭합니다.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   항목이 해당 영역의 필터링 기준과 일치하고 다른 사용자에게 할당되지 않은 경우 미할당 작업 영역에 표시되고 다른 사용자에게 할당된 경우 사용자 영역에 표시됩니다.

   업무 균형자에서 정보를 필터링하는 방법에 대한 자세한 내용은 [업무 균형자에서 정보 필터링](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)을 참조하십시오.
