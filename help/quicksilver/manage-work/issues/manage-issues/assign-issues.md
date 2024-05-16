---
product-area: projects
navigation-topic: manage-issues
title: 문제 할당
description: 사용자, 역할 및 팀에 문제를 할당하여 문제 완료에 대한 책임 주체를 나타낼 수 있습니다. 문제 할당에 대한 일반적인 내용은 문제 할당 수정 개요를 참조하십시오.
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 0%

---

# 문제 할당

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경 또는 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">현재 릴리스에 대한 자세한 내용은 [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

사용자, 역할 및 팀에 문제를 할당하여 문제 완료에 대한 책임 주체를 나타낼 수 있습니다. 문제 지정에 대한 일반적인 내용은 [문제 할당 수정 개요](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
>
>비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
>
>* 작업 항목을 활성 리소스에 재할당합니다.
>* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.

이 문서 외에도 문제 할당에 대한 자세한 내용은 다음 문서를 읽는 것이 좋습니다.

* [문제 할당 수정 개요](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)
* [목록의 여러 문제에 대한 사용자 할당 수정](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [업무 균형자에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

개별 문제 수준에서 하나 또는 여러 리소스에 문제를 할당하거나, 여러 리소스를 여러 문제에 한 번에 할당할 수 있습니다.

문제 및 작업 할당은 Adobe Workfront에서 유사합니다. 작업 할당에 대한 일반적인 내용은 [작업 할당 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 또는 상위 액세스 권한</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. 액세스 수준의 문제에 대한 액세스와 관련된 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>문제를 복사하는 항목에 문제를 추가할 수 있는 권한과 함께 권한을 제공하십시오.</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 역할, 팀 및 사용자에 대한 여러 할당 고려 사항

작업 항목에 여러 리소스를 할당할 때 다음 사항을 고려하십시오.

* 사용자는 프로필과 연결된 작업 역할을 두 개 이상 가질 수 있습니다. 사용자를 작업 역할과 연결하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업 또는 문제는 일반적으로 하나 이상의 작업 역할 또는 팀에 먼저 할당됩니다. 프로젝트를 시작할 준비가 되면 사용자에게 할당해야 할 수도 있습니다.

  작업 또는 문제가 하나 이상의 역할에 할당된 다음 사용자도 할당하는 경우, Adobe Workfront은 다음 규칙에 따라 추가 사용자와 연결할 작업 역할(있는 경우)을 결정합니다.

   * 할당된 작업 역할이 하나뿐이고 사용자의 기본 역할과 일치하는 경우 작업 또는 문제는 기본 역할을 수행하는 사용자에게만 할당됩니다.
   * 여러 개의 역할이 할당되고 하나 이상의 역할이 사용자의 보조 역할과 일치하는 경우 작업 또는 문제는 다른 역할(여러 개의 일치하는 역할이 있는 경우 Workfront에서 임의로 선택) 중 하나를 이행하는 사용자와 할당된 추가 역할에 할당됩니다.
   * 하나 이상의 작업 역할이 할당되고 사용자의 역할에 일치하는 항목이 없는 경우 작업 또는 문제는 사용자뿐만 아니라 역할이나 역할 모두에 할당됩니다.

* 작업 또는 문제가 팀에 할당되고 사용자도 할당되면 작업 또는 문제는 팀과 사용자 모두에게 할당된 상태로 유지됩니다.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## 단일 문제 할당

1. 할당할 문제로 이동합니다.
1. 클릭 **할당 대상** 문제 헤더의 오른쪽 상단 모서리에서 **할당** 영역

   또는

   문제가 이미 할당된 경우 현재 할당의 이름을 클릭합니다.

   ![할당 대상 단추](assets/assign-to-button-in-header.png)

1. 다음 중 하나를 수행하십시오.

   * 할당하려는 사용자, 역할 또는 팀의 이름을 입력한 다음 목록에 나타나면 클릭합니다.

     프로덕션 환경의 샘플 이미지:
     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

     <span class="preview">미리보기 환경의 샘플 이미지:</span>
     ![할당 검색](assets/assignments-expanded-in-task-issue-header.png)

   * (조건부) **제안된 할당** 목록
   * 클릭 **나에게 할당** 자신에게 할당하기
   * 클릭 **고급**.

     고급 할당 생성은 작업 및 문제와 유사합니다. 고급 할당 방법에 대한 자세한 내용은 다음을 참조하십시오. [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다.
     >
     >사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
     >
     >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)


1. 클릭 **저장** 을 눌러 문제 할당을 완료합니다.
1. (선택 사항) **X 아이콘** 문제 머리글의 할당 영역에 있는 할당 이름 옆에 있는 할당을 제거합니다.

## 목록에서 문제 할당

지정 필드가 목록 보기에 표시되면 목록이나 보고서에서 문제를 할당할 수 있습니다. 문제를 더 빠르게 할당하는 방법입니다.

보기에 표시되는 필드에 따라 다음 엔티티를 문제에 할당할 수 있습니다.

| 옵션 | 할당된 엔티티 |
|---|---|
| **할당 대상** | 사용자 1명 할당 |
| **할당됨** | 사용자 1명 할당 |
| **할당** | 사용자, 작업 역할 또는 팀을 할당합니다. |

목록에서 문제를 할당하려면 다음을 수행하십시오.

1. 보기에 할당 대상, 할당 또는 할당 필드가 있는 문제 목록으로 이동합니다.
1. 문제를 할당하려면 다음 중 하나를 수행하십시오.

   * 내부를 클릭합니다. **할당 대상** 또는 **할당됨** 필드에 문제에 할당할 활성 사용자의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

     ![](assets/assigned-to-field-task-list-nwe.png)

   * 내부를 클릭합니다. **할당** 필드에 문제에 할당할 활성 사용자, 작업 역할 또는 활성 팀의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

     프로덕션 환경의 샘플 이미지:
     ![](assets/assignments-field-task-list-nwe.png)

     <span class="preview">미리보기 환경의 샘플 이미지:</span>
     ![할당 필드](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다.
   >
   >사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
   >
   >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. (조건부) 지정 필드에 표시되면 **사람 아이콘** ![](assets/teams.png) 지정(assignments) 상자의 오른쪽 상단 모서리에서 고급 지정(Advanced Assignments) 상자를 열고 고급 지정을 생성합니다. 자세한 내용은 [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >할당 대상 또는 할당 대상 필드에서 고급 할당을 수행할 수 없습니다.

1. 문제에 피할당자를 추가한 후 Enter 키를 누르거나 페이지의 아무 곳이나 클릭하여 변경 사항을 저장합니다.

## 일괄 문제 할당

1. 일괄 할당할 문제 목록으로 이동합니다.
1. 목록에서 몇 가지 문제를 선택하십시오.
1. 다음을 클릭합니다. **편집 아이콘** ![](assets/qs-edit-icon.png).

   다음 **문제 편집** 대화 상자가 열립니다.

1. 다음에서 **할당** 영역을 선택하고 **할당자** 그런 다음 모든 문제에 지정할 사용자, 작업 역할 또는 팀의 이름을 입력하십시오.

   >[!IMPORTANT]
   >
   >문제가 이미 할당된 경우 문제에 대한 기존 리소스를 대체하는 대신 여기에 표시하는 리소스가 문제에 추가됩니다.

1. (선택 사항) **문제 소유자** 문제에 둘 이상의 리소스를 할당할 때 문제가 발생하는 기본 담당자 또는 소유자인 리소스를 나타내는 열입니다. 이 기능은 팀에 사용할 수 없습니다.
1. (선택 사항) 사용자가에서 문제에 대해 충족해야 하는 역할을 선택합니다 **역할 선택** 드롭다운 메뉴 **피할당자의 역할** 문제에 사용자를 할당할 때 열을 표시합니다. 역할을 선택하지 않으면 Workfront에서 자동으로 사용자의 기본 역할을 선택합니다.

1. (선택 사항) 모든 문제에서 기존 피할당자를 제거하려면 다음 중 하나를 수행하십시오.

   1. 문제에서 제거할 사용자, 역할 또는 팀의 이름을 입력한 다음 목록에 표시될 때 선택하고 **피할당자 제거** 제거할 추가 피할당자를 추가합니다.
   1. 클릭 **기존 할당자 모두 제거** 을 눌러 선택한 모든 문제에서 모든 피할당자를 제거합니다.

1. 클릭 **변경 내용 저장**.
1. (선택 사항 및 조건부) 할당 대상 또는 할당 필드가 문제 목록에 표시되면 문제에 대해 이러한 열 중 하나를 클릭한 다음 **X 아이콘** 을(를) 피할당자의 이름 옆에 배치하여 문제에서 제거합니다.
