---
product-area: projects
navigation-topic: plan-a-project
title: 역할 할당 패널에서 프로젝트 계획 시간 보기
description: 프로젝트의 역할 할당 패널에서 프로젝트의 작업 항목에 할당된 모든 작업 역할에 대한 역할 할당을 볼 수 있습니다.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 역할 할당 패널에서 프로젝트 계획 시간 보기

프로젝트의 역할 할당 패널에서 프로젝트의 작업 항목에 할당된 모든 작업 역할에 대한 역할 할당을 볼 수 있습니다.

>[!NOTE]
>
>이 문서에서는 프로젝트의 작업 및 문제와 관련된 작업 역할과 프로젝트의 역할 할당 패널에서 할당된 계획된 시간을 보는 것을 말합니다. Adobe Workfront 시나리오 플래너를 사용할 때 역할 할당 패널을 사용하여 계획된 시간을 이니셔티브 시간과 조정하는 방법에 대한 자세한 내용은 다음을 참조하십시오.
>
>* [작업 목록에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [업무 균형자에서 프로젝트 및 이니셔티브에 대한 역할 할당 표시](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  역할 할당 패널에서 이니셔티브 시간을 보려면 시나리오 플래너 라이선스가 있어야 합니다. 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 시작](../../../scenario-planner/get-started-with-scenario-planning.md) 을 참조하십시오.
>

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

다음 항목이 있어야 합니다.

* 작업 역할이나 작업 역할과 연관된 사용자에게 할당된 작업 또는 문제입니다.

  >[!TIP]
  >
  >작업 또는 문제가 할당 해제되거나, 팀에 할당되거나, 작업 역할이 없는 사용자에게 할당된 경우 역할 할당 패널에서 프로젝트의 계획된 시간이 0입니다.

* 기간이 0보다 큰 작업 및 문제

## 역할 할당 패널에서 프로젝트 계획 시간 보기

1. Adobe Workfront의 오른쪽 상단에 있는 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **프로젝트**&#x200B;를 클릭합니다.
1. 액세스할 프로젝트의 이름을 클릭합니다. 프로젝트 페이지가 열립니다.
1. 왼쪽 패널에서 다음 중 하나를 클릭합니다.

   * **작업**
   * **워크로드 밸런서**

1. **역할 할당 표시** 아이콘 ![](assets/show-role-allocation-icon.png)을 클릭합니다.

   역할 할당 패널이 표시됩니다.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. **역할 할당** 패널에서 다음 정보를 검토하십시오.
|필드 | 설명|
|—|—|
| **작업 역할** |프로젝트의 작업 및 문제에 할당된 작업 역할입니다. 작업 및 문제에 직접 할당된 작업 역할이거나 프로젝트의 작업 및 문제에 할당된 사용자와 연관된 작업 역할일 수 있습니다.  |
| **계획된 시간** |프로젝트의 작업 역할과 연결된 사용자 또는 작업 역할에 할당된 작업 및 문제의 총 계획된 시간 수입니다.  |



