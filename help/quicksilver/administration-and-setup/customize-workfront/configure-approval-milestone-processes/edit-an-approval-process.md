---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: 승인 프로세스 편집
description: Adobe Workfront 관리자이거나 승인 프로세스에 대한 관리자 액세스 권한이 있는 경우 시스템에서 모든 승인 프로세스를 보고 편집할 수 있습니다.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 6%

---

# 승인 프로세스 편집

Adobe Workfront 관리자이거나 승인 프로세스에 대한 관리자 액세스 권한이 있는 경우 시스템에서 모든 승인 프로세스를 보고 편집할 수 있습니다.

그룹 관리자라면 관리하는 그룹 또는 그룹과 연관된 승인 프로세스를 보고 편집할 수 있습니다.

승인 프로세스 생성에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* 이미 사용 중인 전역 승인 프로세스를 편집하면 변경 사항이 이미 연관된 시스템 전체에서 모든 객체에 영향을 줍니다.
>* 객체에 이미 시작된 승인 프로세스의 현재 단계에 새 승인자를 추가하는 경우 해당 객체에 대한 프로세스가 재설정되고 승인자는 다시 시작해야 합니다.
>
>  그러나 객체에 대해 이미 시작된 승인 프로세스를 다음과 같이 변경하는 경우 중단 없이 해당 프로세스가 계속됩니다.
>
>* 현재 단계 이상의 단계 추가
>* 현재 단계 앞에 추가 승인자 추가


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시스템 관리자가 아닌 경우 승인 프로세스에 대한 관리자 액세스</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 기존 승인 프로세스 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).
1. (조건부) 시스템 수준 승인 프로세스를 편집하는 경우 **프로세스** > **승인** 왼쪽 패널에 표시됩니다.

   또는

   그룹 수준 승인 프로세스를 편집하는 경우 다음을 수행합니다.

   1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).
   1. 그룹 승인 프로세스를 나열하거나 관리할 그룹의 이름을 누릅니다.
   1. 왼쪽 패널에서 **승인**. 을(를) 클릭하여 **자세히 표시** 먼저

1. 을(를) 클릭합니다. **프로젝트 승인**, **작업 승인**, 또는 **문제 승인** 탭합니다.

1. 편집할 승인 프로세스를 선택한 다음 **편집** 를 클릭합니다. 승인 프로세스 편집 상자가 표시됩니다.

   ![](assets/edit-approval-process-global-area-new.png)

1. 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스 이름</td> 
      <td>승인 프로세스를 설명하는 이름을 입력합니다. 사용자는 객체에 승인 프로세스를 적용할 때 <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">신규 또는 기존 승인 프로세스를 작업물과 연결</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>승인 프로세스에 대한 설명을 입력합니다. 다음 화면에 표시됩니다. <b>승인</b> 의 섹션 <b>설정</b> 승인 프로세스의 이름 옆에 있는 영역입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>다른 사용자가 만든 프로젝트, 작업 및 문제에 승인 프로세스를 첨부할 수 있도록 하려면 이 옵션을 활성화하십시오. </p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p>팁: 승인 프로세스를 비활성 상태로 표시하는 것은 조직에서 더 이상 승인 프로세스를 사용할 필요가 없지만 사용 내역 정보를 보존하려는 경우에 유용합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이 승인 진행을 사용할 수 있는 대상자: </td> 
      <td> <p>특정 그룹에만 속하는 프로젝트, 작업, 문제 및 템플릿에 대해 승인 프로세스를 사용할 수 있도록 하려면 그룹 이름을 입력한 다음 그룹 이름이 나타나면 이름을 선택합니다.</p> 
       <ul> 
        <li>시스템 관리자이거나 승인 프로세스에 대한 관리자 액세스 권한이 있는 경우 이름을 입력할 때 시스템에서 모든 그룹을 볼 수 있습니다. <b>모든 그룹</b> 기본적으로 선택되어 있습니다. </li> 
        <li>승인 프로세스에 대한 관리자 액세스 권한이 없는 그룹 관리자인 경우 이름을 입력할 때 관리하는 그룹에 승인 프로세스를 지정할 수 있습니다. 다음 <b>모든 그룹</b> 옵션을 사용할 수 없습니다.</li> 
       </ul> <p>이 옵션은 단일 사용 승인 프로세스에 사용할 수 없습니다.</p> <p><b>경고</b>: 그룹별 승인 프로세스를 변경하면 작업 항목과 이미 연관된 기존 승인 프로세스가 변경될 수 있습니다. 이러한 변경 사항에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경이 지정된 승인 프로세스에 미치는 영향</a>.</p> <p>그룹 페이지에서 그룹의 승인 프로세스를 나열하고 관리하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">그룹 수준 승인 프로세스</a>. </p> <p>승인 프로세스에 대한 관리 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음 옵션을 사용하여 승인 프로세스에 대한 경로를 구성합니다.

   경로는 승인 프로세스에서 수행해야 하는 작업을 지정하는 위치입니다. 경로에 단계를 만들어 승인 작업을 수행해야 하는 대상과 순서를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">상태가 설정되면 승인 프로세스 시작</p> </td> 
      <td> <p>작업 항목에 대한 승인 프로세스를 트리거할 상태를 선택합니다. 작업 항목을 이 상태로 업데이트하면 승인 프로세스가 시작됩니다. </p> <p>여러 승인 프로세스 경로에 대해 동일한 상태를 선택할 수 없습니다.</p> <p>사용 가능한 상태는 옵션 아래에서 선택한 상태에 따라 달라집니다 <b>이 승인은</b> (위의 표에 설명되어 있음).</p> 
      <ul> 
      <li> If <b>모든 그룹</b> 이(가) 선택되면 시스템 전체에 잠긴 상태만 사용할 수 있습니다. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>특정 그룹을 선택하면 해당 그룹에 사용할 수 있는 상태만 사용할 수 있습니다</p> </li> 
      </ul> <p>승인 프로세스가 상태로 작동하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">승인 프로세스가 상태에 의존하는 방식</a> 기사 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 이름</td> 
      <td>(선택 사항) 경로의 첫 번째 단계를 설명하는 이름을 입력합니다. 스테이지 이름을 지정하지 않으면 기본 이름은 <b>1단계</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인자</td> 
      <td> <p>이 단계의 승인자로 지정할 사용자, 팀 또는 작업 역할의 이름을 입력하고 드롭다운 목록에 표시될 때 이름을 클릭합니다. 활성 사용자, 작업 역할 및 팀만 추가할 수 있습니다. </p>

   <p><b>팁</b>:</p>

   <p>사용자를 승인자로 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.</p>

   <p><b>메모</b>:

   승인자로서 사용자, 팀 또는 역할을 추가하면 해당 승인과 연관된 객체에 대한 권한이 자동으로 부여되지 않습니다. 이들은 승인 단계가 트리거되면 개체에 대한 권한을 받습니다. 그렇지 않으면 승인 결정을 내리기 전에 객체를 공유해야 합니다. </p>
   <p>개인의 역할을 지정하여 개인을 승인자로 지정할 수도 있습니다. 예를 들어, 프로젝트 소유자, 프로젝트 스폰서, Portfolio 소유자, 프로그램 소유자 또는 관리자를 승인자로 지정할 수 있습니다. 이러한 옵션은 입력을 시작하면 자동으로 나타납니다.</p> 
      <p><b>중요 사항</b>:  
      <ul> 
      <li> 프로젝트 스폰서에 승인을 지정하고 어느 누구도 프로젝트의 스폰서로 지정되지 않으면 승인이 프로젝트 소유자에게 재지정됩니다. 프로젝트 소유자로 지정된 사람이 없는 경우 Workfront 관리자에게 승인이 할당됩니다. </li> 
      <li> 역할 및 옵션에 승인을 지정하는 경우 <b>승인자가 프로젝트 팀에 있을 필요가 없습니다.</b> 이 비활성화되어 있지만 프로젝트 팀의 역할이 승인 시 역할과 일치하지 않으면 승인이 프로젝트 소유자에게 재지정됩니다. 승인 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>.
      </li> 
      <li>프로젝트 소유자에게 승인을 지정하고 아무도 프로젝트 소유자로 지정되지 않으면 설정 영역의 고객 정보 섹션에 표시된 대로 기본 Workfront 관리자에게 승인이 재할당됩니다. 자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">시스템에 대한 기본 정보 구성</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>작업 역할을 승인자로 지정하면 프로젝트 팀에도 있는 해당 작업 역할과 연관된 모든 사용자가 승인을 결정할 수 있습니다. </p> 
      <p>팀을 승인자로 지정하면 해당 팀의 모든 사용자가 승인에 대해 결정을 내릴 수 있습니다. </p> 
      <p>프로젝트 팀에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>. 작업 승인에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">작업 승인 </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">필요한 결정은 단 하나입니다.</td> 
      <td>(스테이지에 여러 승인자를 추가하는 경우에만 표시) 스테이지의 승인자 중 한 사람이 이 단계 동안 작업 항목을 승인하거나 거부할 수 있는 경우 이 옵션을 선택합니다. 이 작업을 수행하면 작업 항목이 스테이지를 나갈 수 있습니다.  
      <p>이 옵션을 선택하지 않은 경우, 식별된 모든 승인자는 항목이 스테이지를 떠나기 전에 단계를 승인 또는 거부해야 합니다(임의의 순서로). 승인자 중 한 사람이 단계를 거부하면 프로세스가 중단되고 다시 시작되므로 필요한 변경이 가능합니다. 그러면 승인자가 단계를 다시 승인하거나 거부할 수 있습니다.</p> 
      <p>팀이 승인자로 지정되면 팀의 구성원이 스테이지를 부여하거나 거부할 수 있습니다.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">단계 추가</p> </td> 
      <td>(선택 사항) 위의 세 행에 설명된 옵션을 사용하여 경로에 다른 스테이지를 추가합니다. 경로에 필요한 만큼 단계를 추가할 수 있습니다.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> 승인이 거부될 때 수행할 작업 선택</td> 
      <td> <p>경로의 어느 단계에서든 작업 항목이 거부되면 수행할 작업을 선택합니다.</p> 
      <ul> <li><strong>문제 만들기</strong>: (프로젝트 및 태스크 승인 프로세스에만 사용 가능) 승인 프로세스가 실행 중인 프로젝트나 태스크에서 문제가 생성됩니다. 작업에 할당된 기본 자원이나 프로젝트 소유자가 문제에 할당됩니다. 기본적으로 생성되는 문제 이름은 입니다 <strong>승인 거부(프로젝트 또는 작업 이름)</strong>. 거부가 발생한 승인 프로세스에 따라 태스크 또는 프로젝트에 입력된 거부 문제입니다.</li> 
      <li> <p><strong>상태를 로 설정</strong>: 다음 중 하나를 선택합니다.</p> 
      <ul> <li><strong>이전 상태</strong>: 거부된 프로젝트, 작업 또는 문제는 승인 프로세스를 활성화하는 상태 이전의 상태로 되돌아갑니다.</li> 
      <li> <p><strong>목록의 다른 모든 상태</strong>: 거부된 객체가 선택한 상태(예: 보류 중)로 이동합니다. 기본 상태 또는 Workfront 시스템에 추가한 사용자 지정 상태 중 하나를 선택할 수 있습니다.</p> <p>승인 프로세스와 연결된 상태를 승인 경로에 대한 거부 상태로 선택하면 거부된 오브젝트가 선택된 상태로 이동하고 “승인 대기 중”으로 표시됩니다. </p>
      <p>예를 들어 거부 상태에서 보류 중을 선택하고 보류 중 상태가 승인 프로세스와 연결된 경우 거부된 오브젝트는 “보류 중 - 승인 대기 중” 상태에 배치되어 승인이 필요합니다.</p>    <p>시스템 전체 승인 프로세스의 경우 시스템 전체 상태만 사용할 수 있습니다.</p> <p>그룹별 승인 프로세스의 경우 모든 그룹 상태를 사용할 수 있습니다. 여기에는 그룹 관리자가 그룹을 위해 특별히 만든 사용자 지정 상태와 시스템 전체 상태가 포함됩니다. </p> <p>승인 프로세스가 상태로 작동하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">승인 프로세스가 상태에 의존하는 방식</a> 기사 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **경로 추가** 승인 프로세스에 다른 경로를 추가하려면 이전 단계의 옵션 목록을 참조하십시오.

   새 경로는 다른 상태와 연결되어야 합니다. 이 상태를 표시하도록 항목이 업데이트되면 경로가 트리거됩니다. 동일한 상태에 대해 두 개의 경로를 가질 수 없습니다.

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * 에 설명된 대로 승인 프로세스를 시스템 전체에서 특정 프로젝트, 작업 또는 문제와 연결합니다. [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Workfront 외부에서 다음에 설명된 대로 승인 프로세스를 사용하여 프로젝트, 작업 또는 문제와 연결할 수 있음을 사용자에게 알립니다 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 이 승인 프로세스가 거부되고 품목이 다른 상태를 취하는 경우 트리거되는 다른 승인 프로세스를 생성합니다. 이렇게 하면 승인 프로세스를 함께 연결하는 방법이 제공됩니다.
