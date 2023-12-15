---
product-area: projects
navigation-topic: use-predecessors
title: 프로젝트 간 전임 작업 만들기
description: 프로젝트 간 전임 작업은 다른 프로젝트의 다른 작업(후속 작업이라고 함)이 종속된 작업입니다. 전임 작업은 종속(후임 작업)보다 우선하는 작업입니다. 예를 들어 종속 작업을 시작하기 전에 전임 작업을 완료로 표시해야 하는 종속성을 만들 수 있습니다.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# 프로젝트 간 전임 작업 만들기

<!--Audited: 12/2023-->

프로젝트 간 전임 작업은 다른 프로젝트의 다른 작업(후속 작업이라고 함)이 종속된 작업입니다. 전임 작업은 종속(후임 작업)보다 우선하는 작업입니다. 예를 들어 종속 작업을 시작하기 전에 전임 작업을 완료로 표시해야 하는 종속성을 만들 수 있습니다.

Adobe Workfront을 사용하면 단일 프로젝트 내에서 전임 작업을 허용하는 것처럼 작업을 다른 프로젝트의 작업에 종속시킬 수 있습니다.

>[!INFO]
>
>예를 들어 굴착 업체는 백호가 1개만 있고, 2개 프로젝트에는 백호를 사용해야 하는 업무가 있다. 프로젝트 관리자는 첫 번째 프로젝트의 작업을 두 번째 프로젝트의 작업의 전임 작업으로 만들 수 있습니다. 이는 첫 번째 프로젝트가 완료될 때 백호우 사용을 시작할 수 있음을 보여 줍니다.

프로젝트 간 전임 작업을 통해 프로젝트를 연결할 때 기본 프로젝트(전임 작업이 있는 프로젝트)의 날짜가 보조 프로젝트(후임 작업이 있는 프로젝트)에 영향을 줍니다.

>[!TIP]
>
>보조 프로젝트에 대해 업데이트된 날짜를 보려면 프로젝트에 대한 타임라인을 다시 계산해야 합니다. 타임라인 다시 계산에 대한 자세한 내용은 다음을 참조하십시오. [프로젝트에 대한 타임라인 재계산 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

전임 작업 관계에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
 <tr> 
  <td role="rowheader">Adobe Workfront 라이센스*</td> 
  <td> <p>새로운 기능: 표준 </p>
 <p>또는</p> 
<p>현재: 플랜 </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 간 전임 작업 만들기

1. 후속 작업이 될 작업(종속 작업)으로 이동합니다.
1. 클릭 **전임 작업** 왼쪽 패널에서
1. 클릭 **전임 작업 추가.**
1. 다음에서 **상위 프로젝트** 필드에서 현재 작업의 전임 작업으로 사용할 작업이 포함된 프로젝트의 이름을 입력합니다.
1. 드롭다운 목록에 표시될 때 이름을 클릭합니다.
1. 다음에서 **작업** 필드에서 현재 작업의 전임 작업으로 사용할 작업의 이름을 입력합니다.
1. 전임 작업과 종속 작업 간의 관계를 정의하기 위해 다음 정보를 지정합니다.

   * **종속성 유형:** 전임 작업이 종속 작업과 가질 관계를 선택합니다. 기본 관계는 &quot;Finish-Start&quot;입니다. 즉, 종속 작업을 시작하려면 먼저 전임 작업을 완료해야 합니다. 다양한 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **지연:** 종속 작업이 시작될 때까지 적용된 전임 작업이 완료된 후 경과해야 하는 시간을 지정합니다. 다양한 유형의 지연에 대한 자세한 내용은 [지연 유형 개요](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **적용됨:** 이 옵션을 선택하면 작업을 일찍 시작하는 사용자가 두 작업 간의 종속성 관계를 우회할 수 없습니다. 예를 들어, 태스크 A와 태스크 B 간의 관계를 집행하는 경우, 태스크 A가 완료될 때까지 태스크 B를 시작할 수 없습니다. 전임 작업을 적용하는 방법에 대한 자세한 내용은 [전임 작업 시행](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     이 옵션을 선택하지 않으면 종속성이 사용자에게 제안처럼 처리됩니다. 예를 들어 사용자는 작업 A가 완료되기 전에 작업 B를 시작할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   프로젝트 간 전임 작업이 있는 작업에는 작업 목록의 전임 작업 열에 전임 작업이 속한 프로젝트의 참조 번호와 작업 번호가 콜론으로 구분되어 표시됩니다.

   ![프로젝트 간 전임 작업](assets/cross-project-predecessor-in-list-view.png)

   전임 작업이 완료된 것으로 표시되면 전임 작업 아이콘이 녹색으로 바뀝니다. 이는 종속 작업이 작업을 수행할 준비가 되었음을 나타냅니다.

   전임 작업, 프로젝트 및 날짜에 대한 자세한 내용을 보려면 이 값 위로 마우스를 가져갑니다. 세부 정보 상자에서 프로젝트 간 전임 작업 을 클릭하여 작업을 엽니다.

   전임 작업 프로젝트에 대한 자세한 내용을 보려면 마우스로 가리키기 창의 상단 근처에 있는 을 클릭합니다.

   클릭 **프로젝트 보기** 을 눌러 전임 작업 프로젝트를 엽니다.

   ![프로젝트 간 전임 작업 세부 정보](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   다음 **프로젝트 보기** 옵션은 프로젝트 간 전임 작업을 볼 때만 표시됩니다.

