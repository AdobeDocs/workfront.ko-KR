---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: 승인 프로세스 편집
description: Adobe Workfront 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 경우 시스템의 모든 승인 프로세스를 보고 편집할 수 있습니다.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1955'
ht-degree: 1%

---

# 승인 프로세스 편집

Adobe Workfront 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 경우 시스템의 모든 승인 프로세스를 보고 편집할 수 있습니다.

그룹 관리자인 경우 관리하는 그룹 또는 그룹과 관련된 승인 프로세스를 보고 편집할 수 있습니다.

승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

>[!NOTE]
>
>* 이미 사용 중인 글로벌 승인 프로세스를 편집하면 변경 사항이 이미 연결된 시스템 전체의 모든 오브젝트에 영향을 미칩니다.
>* 객체에서 이미 시작된 승인 프로세스의 현재 단계에 새 승인자를 추가하면 해당 객체에 대한 프로세스가 재설정되고 승인자는 다시 시작해야 합니다.
>
>  그러나 객체에서 이미 시작된 승인 프로세스를 다음과 같이 변경하면 해당 프로세스가 중단 없이 계속됩니다.
>
>* 현재 단계 뒤에 단계 추가
>* 현재 단계 전에 추가 승인자 추가

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시스템 관리자가 아닌 경우 승인 프로세스에 대한 관리 액세스</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 기존 승인 프로세스 편집

{{step-1-to-setup}}

1. (조건부) 시스템 수준 승인 프로세스를 편집하는 경우 왼쪽 패널에서 **프로세스** > **승인**&#x200B;을 클릭합니다.

   또는

   그룹 수준 승인 프로세스를 편집하는 경우 다음을 수행합니다.

   1. 왼쪽 패널에서 **그룹** ![그룹 아이콘](assets/groups-icon.png)을 클릭합니다.
   1. 그룹 승인 프로세스를 나열하거나 관리할 그룹의 이름을 클릭합니다.
   1. 왼쪽 패널에서 **승인**&#x200B;을 클릭합니다. 먼저 **자세히 표시**&#x200B;를 클릭해야 할 수 있습니다.

1. 편집할 승인 프로세스 유형에 따라 **프로젝트 승인**, **작업 승인** 또는 **문제 승인** 탭을 클릭합니다.

1. 편집할 승인 프로세스를 선택한 다음 목록의 맨 위에서 **편집**&#x200B;을 클릭합니다. 승인 프로세스 편집 상자가 표시됩니다.

   ![승인 프로세스 편집](assets/edit-approval-process-global-area-new.png)

1. 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스 이름</td> 
      <td>승인 프로세스에 대한 수사적 이름을 입력합니다. <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결</a>에 설명된 대로 사용자에게 승인 프로세스를 오브젝트에 적용할 때 이 이름이 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>승인 프로세스에 대한 설명을 입력합니다. 승인 프로세스 이름 옆에 있는 <b>설정</b> 영역의 <b>승인</b> 섹션에 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>다른 사용자가 만드는 프로젝트, 작업 및 문제에 승인 프로세스를 첨부할 수 있도록 하려면 이 옵션을 활성화한 상태로 유지하십시오. </p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p>팁: 승인 프로세스를 비활성으로 표시하는 것은 조직에서 승인 프로세스를 더 이상 사용할 필요는 없지만 사용 기록 정보를 유지하려는 경우 유용합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이 승인 진행을 사용할 수 있는 대상자: </td> 
      <td> <p>특정 그룹에만 속하는 프로젝트, 작업, 문제 및 템플릿에 대해 승인 프로세스를 사용할 수 있도록 하려면 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> 
       <ul> 
        <li>시스템 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 경우 이름을 입력하면 시스템에서 그룹을 볼 수 있습니다. 기본적으로 <b>모든 그룹</b>이 선택됩니다. </li> 
        <li>승인 프로세스에 대한 관리 액세스 권한이 없는 그룹 관리자인 경우 그룹 이름을 입력할 때 관리하는 그룹에 승인 프로세스를 지정할 수 있습니다. <b>모든 그룹</b> 옵션을 사용할 수 없습니다.</li> 
       </ul> <p>이 옵션은 일회용 승인 프로세스에는 사용할 수 없습니다.</p> <p><b>경고</b>: 그룹별 승인 프로세스를 변경할 때 이미 작업 항목과 연결된 기존 승인 프로세스가 변경될 수 있습니다. 이러한 변경 사항에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경 사항이 할당된 승인 프로세스에 미치는 영향</a>을 참조하십시오.</p> <p>그룹 페이지에서 그룹 승인 프로세스를 나열하고 관리하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">그룹 수준 승인 프로세스</a>를 참조하십시오. </p> <p>승인 프로세스에 대한 관리 액세스 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 사용자 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음 옵션을 사용하여 승인 프로세스의 경로를 구성합니다.

   경로는 승인 프로세스에서 수행해야 할 작업을 지정하는 곳입니다. 경로에서 단계를 만들어 승인 작업을 수행해야 할 사람과 순서를 나타냅니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">상태가 설정되면 승인 프로세스 시작</p> </td> 
      <td> <p>작업 항목에 대한 승인 프로세스를 트리거할 상태를 선택합니다. 누군가가 작업 항목을 이 상태로 업데이트하면 승인 프로세스가 시작됩니다. </p> <p>여러 승인 프로세스 경로에 대해 동일한 상태를 선택할 수 없습니다.</p> <p>사용 가능한 상태는 옵션 <b>에서 선택한 항목을 기반으로 합니다. 이 승인은 </b>에서 사용할 수 있습니다(위 표에 설명).</p> 
      <ul> 
      <li> <b>모든 그룹</b>을 선택하면 시스템 전체에서 잠긴 상태만 사용할 수 있습니다. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>특정 그룹을 선택하면 해당 그룹에 사용 가능한 상태만 사용할 수 있습니다</p> </li> 
      </ul> <p>승인 프로세스가 상태로 작동하는 방법에 대한 자세한 내용은 문서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>에서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">승인 프로세스가 상태를 사용하는 방법</a> 섹션을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 이름</td> 
      <td>(선택 사항) 경로의 첫 번째 단계를 설명하는 이름을 입력합니다. 단계 이름을 지정하지 않으면 기본 이름은 <b>단계 1</b>입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인자</td> 
      <td> <p>이 단계의 승인자로 지정할 사용자, 팀 또는 작업 역할의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다. 활성 사용자, 작업 역할 및 팀만 추가할 수 있습니다. </p>

   <p><b>팁</b>:</p>

   <p>사용자를 승인자로 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 동일한 이름을 가진 사용자를 구별하는지 확인하십시오. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.</p>
      <p>사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">사용자에게 액세스 권한 부여</a>를 참조하십시오.</p>.

   <p><b>참고</b>:

   사용자, 팀 또는 역할을 승인자로 추가해도 해당 승인과 연관된 오브젝트에 대한 권한이 자동으로 부여되지 않습니다. 이 사용자는 승인 단계가 트리거될 때 오브젝트에 대한 권한을 받습니다. 그렇지 않으면 승인 결정을 내리기 전에 객체를 공유해야 합니다. </p>
   <p>개인의 역할을 지정하여 개인을 승인자로 지정할 수도 있습니다. 예를 들어 프로젝트 소유자, 프로젝트 스폰서, Portfolio 소유자, 프로그램 소유자 또는 관리자를 승인자로 지정할 수 있습니다. 이러한 옵션은 입력을 시작할 때 자동으로 나타납니다.</p> 
      <p><b>중요</b>:  
      <ul> 
      <li> 프로젝트 스폰서에게 승인을 할당하고 아무도 프로젝트의 스폰서로 지정되지 않으면 승인은 프로젝트 소유자에게 재지정됩니다. 아무도 프로젝트의 소유자로 지정되지 않은 경우 승인이 Workfront 관리자에게 할당됩니다. </li> 
      <li> 역할에 승인을 할당하고 <b>프로젝트 팀에 속해 있지 않아도 되는 승인자</b> 옵션을 사용할 수 없지만 프로젝트 팀의 역할이 승인에 대한 역할과 일치하지 않으면 승인이 프로젝트 소유자에게 다시 할당됩니다. 승인 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>을 참조하세요.
      </li> 
      <li>프로젝트 소유자에게 승인을 할당하고 아무도 프로젝트 소유자로 지정되지 않으면, 승인 권한은 설정 영역의 고객 정보 섹션에 표시된 대로 기본 Workfront 관리자에게 재할당됩니다. 자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">시스템에 대한 기본 정보 구성</a>을 참조하십시오.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>승인자로 작업 역할을 할당하면 프로젝트 팀에 있는 해당 작업 역할과 연결된 모든 사용자가 승인에 대해 의사 결정을 내릴 수 있습니다. </p> 
      <p>팀을 승인자로 할당하면 해당 팀의 모든 사용자가 승인에 대한 결정을 내릴 수 있습니다. </p> 
      <p>프로젝트 팀에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>를 참조하십시오. 작업 승인에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">작업 승인 </a>을(를) 참조하십시오.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">필요한 결정은 단 하나입니다.</td> 
      <td>(단계에 여러 승인자를 추가하는 경우에만 표시됨) 단계에 있는 승인자 중 한 명이 이 단계에서 작업 항목을 승인하거나 거부할 수 있는 경우 이 옵션을 선택합니다. 이 작업을 수행하면 작업 항목이 스테이지를 떠날 수 있습니다.  
      <p>이 옵션을 선택하지 않으면 식별된 모든 승인자는 항목이 단계를 떠나기 전에 단계를 임의의 순서로 승인 또는 거부해야 합니다. 승인자 중 한 명이 단계를 거부하면 프로세스는 필요한 변경을 수행할 수 있도록 을 중단하고 다시 시작합니다. 그러면 승인자는 단계를 다시 한 번 승인하거나 거부할 수 있습니다.</p> 
      <p>팀을 승인자로 지정하면 팀의 모든 구성원이 단계를 부여하거나 거부할 수 있습니다.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">단계 추가</p> </td> 
      <td>(선택 사항) 위의 세 행에 설명된 옵션을 사용하여 경로에 다른 단계를 추가합니다. 경로에 필요한 만큼 단계를 추가할 수 있습니다.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> 승인이 거부될 때 수행할 작업 선택</td> 
      <td> <p>경로의 모든 단계에서 작업 항목이 거부되는 경우 수행할 작업을 선택합니다.</p> 
      <ul> <li><strong>문제 만들기</strong>: (프로젝트 및 작업 승인 프로세스에만 사용 가능) 승인 프로세스가 실행 중인 프로젝트 또는 작업에 문제가 만들어집니다. 작업에 할당된 기본 리소스 또는 프로젝트 소유자가 문제에 할당됩니다. 기본적으로 만들어지는 문제의 이름은 <strong>승인 거부됨(프로젝트 또는 작업 이름)</strong>입니다. 거부가 발생한 승인 프로세스에 따라 작업 또는 프로젝트에 입력한 거부 문제입니다.</li> 
      <li> <p><strong>상태를 </strong>(으)로 설정: 다음 중 하나를 선택하십시오.</p> 
      <ul> <li><strong>이전 상태</strong>: 거부된 프로젝트, 작업 또는 문제가 승인 프로세스를 활성화하는 상태 이전의 상태로 되돌아갑니다.</li> 
      <li> <p><strong>목록의 다른 상태</strong>: 거부된 개체가 보류 중과 같이 선택한 상태로 이동합니다. Workfront 시스템에 추가한 기본 상태 또는 사용자 지정 상태 중 하나를 선택할 수 있습니다.</p> <p>승인 프로세스와 연결된 상태를 승인 경로에 대한 거부 상태로 선택하면 거부된 오브젝트가 선택된 상태로 이동하고 "승인 대기 중"으로 표시됩니다.</p>
      <p>예를 들어 거부 상태에서 보류 중 을 선택하고 보류 중 상태가 승인 프로세스와 연결된 경우 거부된 오브젝트는 "보류 중 - 승인 대기 중" 상태에 배치되어 승인이 필요합니다.</p>    <p>시스템 전체 승인 프로세스의 경우 시스템 전체 상태만 사용할 수 있습니다.</p> <p>그룹별 승인 프로세스의 경우 모든 그룹 상태를 사용할 수 있습니다. 여기에는 그룹 관리자가 그룹에 대해 특별히 만든 사용자 지정 상태와 시스템 전체 상태가 포함됩니다. </p> <p>승인 프로세스가 상태로 작동하는 방법에 대한 자세한 내용은 문서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>에서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">승인 프로세스가 상태를 사용하는 방법</a> 섹션을 참조하십시오.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **경로 추가**&#x200B;를 클릭하여 이전 단계의 옵션 목록을 참조하여 승인 프로세스에 다른 경로를 추가합니다.

   새 경로는 다른 상태와 연결되어 있어야 합니다. 이 상태를 표시하도록 항목이 업데이트되면 경로가 트리거됩니다. 동일한 상태에 대해 두 개의 경로를 가질 수 없습니다.

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)에 설명된 대로 승인 프로세스를 시스템 전체에서 특정 프로젝트, 작업 또는 문제와 연결합니다.
   * [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)에 설명된 대로 Workfront 외부에서 사용자에게 승인 프로세스를 사용하여 프로젝트, 작업 또는 문제를 연결할 수 있음을 알립니다.
   * 이 승인 프로세스가 거부되고 항목이 다른 상태에 있을 경우 트리거되는 다른 승인 프로세스를 만듭니다. 이렇게 하면 승인 프로세스를 서로 연결할 수 있습니다.
