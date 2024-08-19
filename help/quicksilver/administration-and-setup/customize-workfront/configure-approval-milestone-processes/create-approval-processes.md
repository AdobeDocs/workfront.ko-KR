---
title: 작업 항목에 대한 승인 프로세스 만들기
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 사용자가 작업 항목(프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업), 문서 또는 증명에 첨부할 수 있는 승인 프로세스를 만들 수 있습니다. 승인 프로세스를 통해 시스템에서 객체를 진행하기 전에 객체에 지정된 임무 책임자가 특정 변경 사항을 검토하도록 할 수 있습니다.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '2174'
ht-degree: 1%

---

# 작업 항목을 위한 승인 프로세스 만들기

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

사용자가 작업 항목(프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업), 문서 또는 증명에 첨부할 수 있는 승인 프로세스를 만들 수 있습니다. 승인 프로세스를 통해 시스템에서 객체를 진행하기 전에 객체에 지정된 임무 책임자가 특정 변경 사항을 검토하도록 할 수 있습니다.

이 문서에서는 작업 항목(프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업)에 대한 시스템 수준 또는 그룹 수준의 글로벌 승인 프로세스를 만드는 방법에 대해 설명합니다.

문서 또는 증명과 관련된 승인에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [문서 승인 요청](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [자동화된 워크플로우 개요](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>사용자는 관리 권한이 있는 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업에 대해 일회용 승인 프로세스를 만들 수도 있습니다.
>
>이 문서에서는 &quot;글로벌 승인 프로세스&quot;라는 용어를 사용하여 일회용 승인 프로세스와 구별합니다. 글로벌 승인 프로세스를 반복적으로 사용할 수 있습니다.
>
>그룹 수준에서 글로벌 승인 프로세스는 그룹에 속하는 작업 항목 및 상태로 제한됩니다.
>
>일회용 승인 프로세스에 대한 자세한 내용은 [승인 프로세스 개요](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) 및 [새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새 플랜: 표준 </p>
 <p>또는</p> 
<p>현재 플랜: 플랜 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 경우 시스템 수준 승인 프로세스나 특정 그룹에 대한 그룹 수준 승인 프로세스를 만들 수 있습니다.</p> 
   <p>그룹 관리자인 경우 관리하는 그룹에 대해 그룹 수준 승인 프로세스를 만들 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 항목에 대한 시스템 수준 또는 그룹 수준의 글로벌 승인 프로세스 만들기

{{step-1-to-setup}}

1. (조건부) 시스템 수준 승인 프로세스를 만드는 경우 왼쪽 패널에서 **프로세스** > **승인**&#x200B;을 클릭합니다.

   또는

   그룹 수준 승인 프로세스를 만드는 경우 **그룹** ![](assets/groups-icon.png)을 클릭하고 그룹 이름을 클릭한 다음 **승인**&#x200B;을 클릭합니다.

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. **프로젝트 승인**, **작업 승인** 또는 **문제 승인** 탭을 선택하십시오.

1. **새 승인 프로세스**&#x200B;를 클릭합니다.
1. 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스 이름</td> 
      <td><p>승인 프로세스에 대한 수사적 이름을 입력합니다. <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결</a>에 설명된 대로 사용자에게 승인 프로세스를 오브젝트에 적용할 때 이 이름이 표시됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td><p>승인 프로세스에 대한 설명을 입력합니다. 승인 프로세스 이름 옆에 있는 <b>설정</b> 영역의 <b>승인</b> 섹션에 표시됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">활성화됨</td> 
      <td> <p>다른 사용자가 만드는 프로젝트, 작업 및 문제에 승인 프로세스를 첨부할 수 있도록 하려면 이 옵션을 활성화한 상태로 유지하십시오. </p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p> 팁: 승인 프로세스를 비활성으로 표시하는 것은 조직에서 승인 프로세스를 더 이상 사용할 필요는 없지만 사용 기록 정보를 유지하려는 경우 유용합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">이 승인 진행을 사용할 수 있는 대상자: </td> 
      <td> <p>특정 그룹에만 속하는 프로젝트, 작업, 문제 및 템플릿에 대해 승인 프로세스를 사용할 수 있도록 하려면 그룹 이름을 입력한 다음 표시될 때 이름을 선택합니다.</p> 
       <ul> 
       <li>시스템 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 경우 이름을 입력하면 시스템에서 그룹을 볼 수 있습니다. 기본적으로 <b>모든 그룹</b>이 선택됩니다. </li> 
       <li>승인 프로세스에 대한 관리 액세스 권한이 없는 그룹 관리자인 경우 그룹 이름을 입력할 때 관리하는 그룹에 승인 프로세스를 지정할 수 있습니다. <b>모든 그룹</b> 옵션을 사용할 수 없습니다.</li> 
       </ul> 
       <p>이 옵션은 일회용 승인 프로세스에는 사용할 수 없습니다.</p> 
       <p><b>경고</b>: 그룹별 승인 프로세스를 변경할 때 이미 작업 항목과 연결된 기존 승인 프로세스가 변경될 수 있습니다. 이러한 변경 사항에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경 사항이 할당된 승인 프로세스에 미치는 영향</a>을 참조하십시오.</p> 
       <p>그룹 페이지에서 그룹 승인 프로세스를 나열하고 관리하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">그룹 수준 승인 프로세스</a>를 참조하십시오. </p> 
       <p>승인 프로세스에 대한 관리 액세스 권한에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 사용자 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
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
       <li> <b>모든 그룹</b>을(를) 선택하면 시스템 전체 상태만 사용할 수 있습니다.
       <li> <p>특정 그룹을 선택하면 해당 그룹에 사용 가능한 상태만 사용할 수 있습니다</p> </li> 
       </ul> <p>승인 프로세스가 상태로 작동하는 방법에 대한 자세한 내용은 문서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>에서 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">승인 프로세스가 상태를 사용하는 방법</a> 섹션을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">단계 이름</td> 
      <td>(선택 사항) 경로의 첫 번째 단계를 설명하는 이름을 입력합니다. 단계 이름을 지정하지 않으면 기본 이름은 <b>단계 1</b>입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인자</td> 
      <td> <p>이 단계의 승인자로 지정할 사용자, 팀 또는 작업 역할의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다. 활성 사용자, <span>작업 역할</span> 및 팀만 추가할 수 있습니다. </p>

   <p><b>팁</b>:</p>

   <p>사용자를 승인자로 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 동일한 이름을 가진 사용자를 구별하는지 확인하십시오. 사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.</p>
      <p>사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">사용자에게 액세스 권한 부여</a>를 참조하십시오. </p>

   <p><b>참고</b>:

   사용자, 팀 또는 역할을 승인자로 추가해도 해당 승인과 연관된 오브젝트에 대한 권한이 자동으로 부여되지 않습니다. 이 사용자는 승인 단계가 트리거될 때 오브젝트에 대한 권한을 받습니다. 그렇지 않으면 승인 결정을 내리기 전에 객체를 공유해야 합니다. </p> <p>개인의 역할을 지정하여 개인을 승인자로 지정할 수도 있습니다. 예를 들어 프로젝트 소유자, 프로젝트 스폰서, Portfolio 소유자, 프로그램 소유자 또는 관리자를 승인자로 지정할 수 있습니다. 이러한 옵션은 입력을 시작할 때 자동으로 나타납니다.</p>

   <p><b>중요</b>:  
       <ul> 
       <li> <p>프로젝트 스폰서에게 승인을 할당하고 아무도 프로젝트의 스폰서로 지정되지 않으면 승인은 프로젝트 소유자에게 재지정됩니다. 아무도 프로젝트의 소유자로 지정되지 않은 경우 승인이 Workfront 관리자에게 할당됩니다. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>역할에 승인을 할당하고 <b>승인자가 프로젝트 팀에 속해 있지 않아도 됩니다(역할이 포함된 승인 프로세스의 경우)</b>이(가) 비활성화되었지만 프로젝트 팀에 승인에 대한 역할과 일치하는 역할이 없으면 승인이 프로젝트 소유자에게 다시 할당됩니다. 승인 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">전역 승인 설정 구성</a>을 참조하세요.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>프로젝트 소유자에게 승인을 할당하고 아무도 프로젝트 소유자로 지정되지 않으면, 승인 권한은 설정 영역의 고객 정보 섹션에 표시된 대로 기본 Workfront 관리자에게 재할당됩니다. 자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">시스템에 대한 기본 정보 구성</a>을 참조하십시오.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>이 프로세스를 반복하여 단계에 여러 승인자를 추가할 수 있습니다. 단일 단계에는 승인자로 사용자, 팀 및 작업 역할의 조합이 포함될 수 있습니다. 단계에 추가할 수 있는 승인자 수에는 제한이 없습니다.</p> <p><b>중요</b>:  <p>승인자로 작업 역할을 할당하면 프로젝트 팀에 있는 해당 작업 역할과 연결된 모든 사용자가 승인에 대해 의사 결정을 내릴 수 있습니다. </p> <p>팀을 승인자로 할당하면 해당 팀의 모든 사용자가 승인에 대한 결정을 내릴 수 있습니다. </p> <p>프로젝트 팀에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a>를 참조하십시오. 작업 승인에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">작업 승인 </a>을(를) 참조하십시오.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br> <br> 결정은 하나만 필요합니다. 여러 승인자를 단계에 추가하는 경우에만 표시됩니다. </td> 
      <td> <p>단계의 승인자 중 한 명이 이 단계 중에 작업 항목을 승인하거나 거부할 수 있는 경우 이 옵션을 선택합니다. 이 작업을 수행하면 작업 항목이 스테이지를 떠날 수 있습니다. </p> <p>이 옵션을 선택하지 않으면 식별된 모든 승인자는 항목이 단계를 떠나기 전에 단계를 임의의 순서로 승인 또는 거부해야 합니다. 승인자 중 한 명이 단계를 거부하면 프로세스는 필요한 변경을 수행할 수 있도록 을 중단하고 다시 시작합니다. 그러면 승인자는 단계를 다시 한 번 승인하거나 거부할 수 있습니다.</p> <p>팀을 승인자로 지정하면 팀의 모든 구성원이 단계를 부여하거나 거부할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">단계 추가</p> </td> 
      <td><p>(선택 사항) 위의 세 행에 설명된 옵션을 사용하여 경로에 다른 단계를 추가합니다. 경로에 필요한 만큼 단계를 추가할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인이 거부될 때 수행할 작업 선택</p> </td> 
      <td> <p>경로의 모든 단계에서 작업 항목이 거부되는 경우 수행할 작업을 선택합니다.</p> 
       <ul> 
       <li><b>문제 만들기</b>: (프로젝트 및 작업 승인 프로세스에만 사용 가능) 승인 프로세스가 실행 중인 프로젝트 또는 작업에 문제가 만들어집니다. 작업에 할당된 기본 리소스 또는 프로젝트 소유자가 문제에 할당됩니다. 기본적으로 만들어지는 문제의 이름은 <b>승인 거부됨(&lt;프로젝트 또는 작업 이름&gt;)</b>입니다. 거부가 발생한 승인 프로세스에 따라 작업 또는 프로젝트에 입력한 거부 문제입니다.</li> 
       <li> <p><b>상태를 </b>(으)로 설정: 다음 중 하나를 선택하십시오.</p> 
       <ul> 
       <li><b>이전 상태</b>: 거부된 프로젝트, 작업 또는 문제가 승인 프로세스를 활성화하는 상태 이전의 상태로 되돌아갑니다.</li> 
       <li><p><b>목록의 다른 상태</b>: 거부된 개체가 보류 중과 같이 선택한 상태로 이동합니다. Workfront 시스템에 추가한 기본 상태 또는 사용자 지정 상태 중 하나를 선택할 수 있습니다.</p>
       <p>승인 프로세스와 연결된 상태를 거부 상태로 선택하면 거부된 오브젝트가 선택된 상태로 이동하고 "승인 보류 중"으로 표시됩니다.</p> 
       <p> 예를 들어 거부 상태에서 보류 중 을 선택하고 보류 중 상태가 승인 프로세스와 연결된 경우 거부된 오브젝트는 "보류 중 - 승인 대기 중" 상태에 배치되어 승인이 필요합니다.</p>

   </tr> 
    </tbody> 
   </table>

1. (선택 사항) **경로 추가**&#x200B;를 클릭하여 이전 단계의 옵션 목록을 참조하여 승인 프로세스에 다른 경로를 추가합니다.

   새 경로는 다른 상태와 연결되어 있어야 합니다. 이 상태를 표시하도록 항목이 업데이트되면 경로가 트리거됩니다. 동일한 상태에 대해 두 개의 경로를 가질 수 없습니다.

1. **저장**&#x200B;을 클릭합니다.
1. 이제 승인 프로세스가 생성되었으므로 다음 중 하나를 사용하여 계속합니다.

   * [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)에 설명된 대로 승인 프로세스를 시스템 전체에서 특정 프로젝트, 작업 또는 문제와 연결합니다.
   * [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)에 설명된 대로 Workfront 외부에서 사용자에게 승인 프로세스를 사용하여 프로젝트, 작업 또는 문제를 연결할 수 있음을 알립니다.
   * 이 승인 프로세스가 거부되고 항목이 다른 상태에 있을 경우 트리거되는 다른 승인 프로세스를 만듭니다. 이렇게 하면 승인 프로세스를 서로 연결할 수 있습니다.

승인 프로세스 편집에 대한 자세한 내용은 [승인 프로세스 편집](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)을 참조하십시오.

## 승인 프로세스를 작업 항목과 연결

작업 항목(프로젝트, 작업 또는 문제)에 대한 승인 프로세스를 만들려면

1. 먼저 승인 프로세스를 만듭니다.
1. 작업 항목 만들기
1. 승인 프로세스를 작업 항목과 연결

승인 프로세스를 작업 항목과 연결하는 방법에 대한 지침은 [새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

>[!NOTE]
>
>프로젝트, 작업 또는 문제에 대한 관리 권한이 있는 모든 Workfront 사용자는 자신이 생성된 오브젝트에서만 사용할 수 있도록 일회용 승인 프로세스를 만들 수 있습니다. 자세한 내용은 [새 승인 프로세스 또는 기존 승인 프로세스와 작업 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 사용자가 단일 작업 항목에 대한 글로벌 승인 프로세스를 수정할 수 있도록 설정

기본적으로 프로젝트, 작업 및 문제에 대한 관리 권한이 있는 사용자는 프로젝트, 작업 및 문제에 대한 일회용 승인 프로세스를 만들 수 있습니다. 단일 사용 승인 프로세스를 프로젝트, 작업 및 문제에 추가하는 방법에 대한 자세한 내용은 문서 [새 승인 프로세스 또는 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)의 [단일 사용 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) 섹션을 참조하십시오.

작업 항목과 연결된 글로벌 승인 프로세스에 대한 설정을 변경할 수도 있습니다. 이러한 변경 사항은 시스템 수준 승인 프로세스와 연결된 프로젝트, 작업 또는 문제에만 영향을 줍니다. 자세한 내용은 문서 [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md))의 [특정 개체에서 사용할 전역 승인 프로세스 수정](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) 섹션을 참조하십시오.
