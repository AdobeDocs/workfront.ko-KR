---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 업무 균형자 를 사용하여 수동으로 작업 할당
description: Adobe Workfront 업무 균형자 를 사용하여 사용자에게 작업 항목을 수동으로 할당할 수 있습니다.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 1%

---

# 업무 균형자 를 사용하여 수동으로 작업 할당

Adobe Workfront 업무 균형자 를 사용하여 사용자에게 작업 항목을 수동으로 할당할 수 있습니다.

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
       <p>현재: 리소스 조달 영역에서 업무 균형자 사용 시 계획;</br>
       팀 또는 프로젝트의 업무 균형자 를 사용할 때 작업</p></td>
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
   <td>할당이 포함된 프로젝트, 작업 및 문제에 대한 Contribute 권한 이상</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 업무 균형자에서 수동으로 작업 할당

사용자에게 아직 할당되지 않은 작업 항목을 할당하거나 업무 균형자에서 사용자에게 할당된 항목을 재할당할 수 있습니다.

1. 작업을 할당할 업무 균형자로 이동합니다.

   리소스 영역, 프로젝트 또는 팀 수준에서 업무 균형자 를 사용하여 사용자에게 작업을 할당할 수 있습니다. Workfront에서 업무 균형자 위치에 대한 자세한 내용은 [업무 균형자 찾기](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)를 참조하십시오.

1. (선택 사항) **할당 해제된 작업** 영역으로 이동하여 필터를 적용하여 작업 또는 문제를 봅니다

   또는

   해당 항목을 다시 할당하려면 **할당된 작업** 영역으로 이동하여 할당된 작업 항목을 볼 사용자 이름을 확장하세요.

1. 작업 항목 이름 왼쪽의 **추가 메뉴** ![](assets/qs-more-menu.png)을(를) 클릭한 다음 **할당 대상**&#x200B;을 클릭합니다.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >다음 단축키를 사용하여 작업 또는 문제를 할당할 수도 있습니다.
   >
   >* Windows의 경우: CTRL 키를 누른 상태에서 작업 또는 문제 표시줄 클릭
   >* Mac에서 CMD+작업 또는 문제 표시줄을 클릭합니다.

1. 다음 중 하나를 수행하십시오.

   * **사람, 역할 또는 팀 검색** 필드에 항목에 할당할 사용자, 작업 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 선택한 다음 **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >사용자를 추가할 때 아바타, 사용자의 기본 역할 및 이메일 주소에 따라 이름이 동일한 사용자를 구별해야 합니다.
   >
   >사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
   >
   > 사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Workfront 또는 그룹 관리자가 사용자 환경에서 위임을 활성화한 경우 할당 탭을 사용하여 사용자를 작업 또는 문제에 할당합니다. 위임 탭을 사용하여 작업 항목에 위임된 사용자를 봅니다. 작업 위임에 대한 자세한 내용은 [작업 및 문제 위임](../../manage-work/delegate-work/how-to-delegate-work.md)을 참조하세요.


   지정된 할당자에게 작업 항목을 할당하거나 재할당합니다.

   팀이나 작업 역할에만 항목을 할당하면 해당 항목이 미할당 작업 영역에만 표시됩니다. 업무 균형자의 할당된 작업 영역에 표시하려면 사용자에게 작업 항목을 할당해야 합니다.

   >[!TIP]
   >
   >여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >
   >비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
   >
   >   
   >   
   >   * 작업 항목을 활성 리소스에 재할당합니다.
   >   * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.
   >   
   >

   * 고급 할당에 액세스하려면 **고급**&#x200B;을 클릭하세요.

     고급 할당에 대한 자세한 내용은 [고급 할당 만들기](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)를 참조하십시오.

1. (선택 사항) **할당 표시 아이콘** ![](assets/show-allocations-icon-small.png)을 클릭한 다음 **추가 메뉴** ![](assets/qs-more-menu.png) > **할당 편집**&#x200B;을 클릭합니다.

   또는

   일별 또는 주별 할당을 두 번 클릭하여 사용자가 작업 항목에 할당된 시간을 수정합니다.

   업무 균형자에서 사용자 할당을 수정하는 방법에 대한 자세한 내용은 문서 [업무 균형자에서 사용자 할당 관리](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)의 &quot;사용자 할당 수정&quot; 섹션을 참조하십시오.

   업무 균형자를 사용하여 작업 항목에서 할당을 제거하는 방법에 대한 자세한 내용은 [업무 균형자에서 작업 할당 해제](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)를 참조하십시오.

    
