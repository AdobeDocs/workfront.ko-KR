---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서에서 작업 할당 취소
description: Adobe Workfront 작업 로드 밸런서의 할당된 작업 영역 내의 작업 항목에서 사용자 할당을 취소하거나 다른 사용자, 역할 또는 팀에 재지정할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# 작업 로드 밸런서에서 작업 할당 취소

Adobe Workfront 작업 로드 밸런서의 할당된 작업 영역 내의 작업 항목에서 사용자 할당을 취소하거나 다른 사용자, 역할 또는 팀에 재지정할 수 있습니다.

수동으로 또는 끌어다 놓거나 대량으로 작업 항목에서 사용자 할당을 취소할 수 있습니다. 이 문서에서는 수동으로 사용자 할당을 취소하는 방법에 대해 설명합니다.

드래그 앤 드롭으로 사용자 할당 해제에 대한 자세한 내용은 [드래그 앤 드롭으로 작업 로드 밸런서에서 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

사용자 일괄 할당 해제에 대한 자세한 내용은 [작업 로드 밸런서를 사용하여 일괄 작업 할당](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음에 대한 액세스 편집:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>지정 작업을 포함하는 프로젝트, 작업 및 문제에 대한 권한 이상의 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

 

## 작업 로드 밸런서에서 작업 항목 할당 취소

사용자로부터 품목을 할당 취소하고 미지정 작업 영역으로 이동하거나 다른 사용자에게 재지정할 수 있습니다.

사용자로부터 작업 항목을 할당 취소하려면

1. 작업 로드 밸런서에서 **지정된 작업 시간** 영역을 확장하고 사용자를 확장합니다.
1. 다음 중 하나를 수행하십시오.

   * 사용자 영역에서 할당을 취소할 항목을 찾아 클릭한 다음 [지정되지 않음] 영역 또는 다른 사용자 영역에 끌어서 놓습니다.
   * 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/more-icon-task-list.png) 작업 항목 이름의 오른쪽에 있는 **여기에 지정**&#x200B;를 클릭한 다음 작업 항목에 할당된 엔티티의 이름을 제거하거나 다른 이름을 입력한 다음 **저장**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   해당 영역에 대한 필터링 기준과 일치하고 다른 사용자에게 할당되지 않은 경우 또는 다른 사용자에게 할당된 경우 사용자 영역에 표시되는 경우 [지정되지 않은 작업 영역]에 항목이 표시됩니다.

   작업 로드 밸런서의 필터링 정보에 대한 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
