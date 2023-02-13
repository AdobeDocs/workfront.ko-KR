---
product-area: projects
navigation-topic: use-predecessors
title: 프로젝트 간 선행 작업 만들기
description: 상호 프로젝트 전임자는 다른 프로젝트의 다른 작업(후속 작업이라고 함)이 종속되는 작업입니다. 전임자는 종속(후속) 작업보다 우선하는 과제입니다. 예를 들어 종속 작업을 시작하기 전에 선행 작업이 완료 로 표시되어야 하는 종속성을 만들 수 있습니다.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 프로젝트 간 선행 작업 만들기

프로젝트 간 전임자는 다른 프로젝트의 다른 작업(후속 작업이라고 함)이 종속되는 작업입니다. 전임자는 종속(후속) 작업보다 우선하는 과제입니다. 예를 들어 종속 작업을 시작하기 전에 선행 작업이 완료 로 표시되어야 하는 종속성을 만들 수 있습니다.

단일 프로젝트 내의 이전 작업처럼 Adobe Workfront에서는 다른 프로젝트의 작업에 따라 작업이 달라질 수 있습니다.

**예**

굴착회사에 하나의 백호만 있고 두 개의 동시 프로젝트에 백호우 사용이 필요한 작업이 있는 경우, 프로젝트 관리자는 제 2 프로젝트의 작업에 따라 제 1 프로젝트의 작업을 수행하여 이전 프로젝트가 백호우를 포기할 때 굴착이 시작될 수 있음을 알 수 있습니다.
프로젝트 간 선행 작업을 통해 프로젝트를 연결할 때 기본 프로젝트의 날짜(이전 작업이 있는 날짜)는 보조 프로젝트(후속 작업이 있는 날짜)에 영향을 줍니다.

>[!TIP]
>
>보조 프로젝트에 대해 업데이트된 날짜를 보려면 프로젝트의 타임라인을 다시 계산해야 합니다. 타임라인 재계산에 대한 자세한 내용은 [프로젝트에 대한 타임라인 재계산 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

이전 관계에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 액세스 요구 사항

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 간 이전 버전 만들기

1. 후임자가 될 과목으로 이동하십시오.
1. 클릭 **선행 작업** 왼쪽 패널에 표시됩니다.
1. 클릭 **선행 작업을 추가합니다.**
1. 에서 **상위 프로젝트** 필드에서 현재 작업에 종속될 작업이 포함된 프로젝트의 이름을 입력합니다.
1. 드롭다운 목록에 이 이름이 표시되면 이름을 클릭합니다.
1. 에서 **작업** 필드에서 현재 작업에 종속될 작업의 이름을 입력합니다.
1. 선행 작업과 종속 작업 간의 관계를 정의하는 데 사용할 다음 정보를 지정합니다.

   * **종속성 유형:** 작업에 종속된 태스크와 관계를 선택합니다. 기본 관계는 &quot;완료 시작&quot;입니다. 즉, 종속 작업을 시작하려면 선행 작업이 완료되어야 합니다. 다양한 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **지연:** 종속 작업을 시작할 때까지 강제 선행 작업이 완료된 후 경과해야 하는 시간을 지정합니다. 다양한 유형의 지연에 대한 자세한 내용은 [지연 유형 개요](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **강제 적용:** 이 옵션을 선택하면 사용자가 작업을 일찍 시작하여 두 작업 간의 종속성 관계를 우회할 수 없습니다. 예를 들어, 작업 A와 작업 B 간의 관계를 적용하는 경우 작업 A가 완료될 때까지 작업 B를 시작할 수 없습니다. 이전 버전 실행에 대한 자세한 내용은 [선행 작업 적용](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      이 옵션을 선택하지 않으면 종속성은 사용자에게 제안으로 처리됩니다. 예를 들어, 사용자는 작업 A가 완료되기 전에 작업 B를 시작할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   상호 프로젝트 선행 작업이 있는 작업은 선행 작업이 속한 프로젝트의 참조 번호와 작업 목록의 선행 작업 열에 콜론으로 구분되는 작업 수를 표시합니다.

   ![크로스 프로젝트 전임자](assets/cross-project-predecessor-in-list-view.png)

   선행 작업이 완료된 것으로 표시되면 선행 작업 아이콘이 녹색으로 바뀝니다. 종속 작업이 작업을 수행할 준비가 되었음을 나타냅니다.

   이 값을 마우스로 가리키면 이전 버전, 프로젝트 및 날짜에 대한 자세한 정보가 표시됩니다. 세부 정보 상자에서 프로젝트 간 선행 작업을 클릭하여 작업을 엽니다. 클릭 **프로젝트 를 참조하십시오** 교차 프로젝트를 엽니다.

   ![프로젝트 간 이전 세부 정보](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   다음 **프로젝트 를 참조하십시오** 옵션은 프로젝트 간 전임자를 볼 때만 표시됩니다.

