---
product-area: projects
navigation-topic: manage-issues
title: 문제 할당
description: 사용자, 역할 및 팀에 문제를 할당하여 문제를 완료할 책임이 있는 사용자를 나타낼 수 있습니다. 문제 지정에 대한 일반적인 정보는 문제 지정 수정 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 0%

---

# 문제 할당

사용자, 역할 및 팀에 문제를 할당하여 문제를 완료할 책임이 있는 사용자를 나타낼 수 있습니다. 문제 지정에 대한 일반적인 정보는 [문제 지정 수정 개요](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
>
>사용자, 작업 역할 또는 팀이 비활성화되기 전에 지정된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
>
>* 작업 항목을 활성 자원에 재지정합니다.
>* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


이 문서 외에 문제 지정에 대한 자세한 내용은 다음 문서를 읽는 것이 좋습니다.

* [문제 지정 수정 개요](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)
* [목록의 여러 문제에 대한 사용자 할당 수정](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [스마트 할당 만들기](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [작업 로드 밸런서에서 작업 할당 개요](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

개별 문제 수준에서 하나 또는 여러 리소스에 문제를 할당하거나 여러 리소스를 한 번에 여러 문제에 할당할 수 있습니다.

문제 및 작업을 할당하는 것은 Adobe Workfront과 유사합니다. 작업 지정에 대한 일반적인 정보는 [작업 지정 수정 개요](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 이상의 액세스 권한</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>문제를 추가하는 기능으로 문제를 복사하는 항목에 권한을 부여합니다.</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## Job 역할, 팀 및 사용자에게 여러 지정 고려 사항

여러 리소스를 작업 항목에 할당할 때 다음 사항을 고려하십시오.

* 사용자는 프로필과 연결된 두 개 이상의 작업 역할을 가질 수 있습니다. 사용자와 작업 역할 연결에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 작업 또는 문제는 일반적으로 하나 이상의 작업 역할이나 팀에 먼저 할당됩니다. 프로젝트를 시작할 준비가 되면 사용자에게 할당해야 할 수도 있습니다.

   작업 또는 문제가 하나 이상의 역할에 할당되어 있고 그 다음 사용자도 할당하면 Adobe Workfront에서 다음 규칙에 따라 추가 사용자(있는 경우)와 연결할 작업 역할을 결정합니다.

   * 할당된 작업 역할이 하나만 있고 사용자의 기본 역할과 일치하는 경우 해당 작업이나 문제는 기본 역할을 수행하는 사용자만 할당됩니다.
   * 여러 개의 역할이 할당되고 역할 중 하나 이상이 사용자의 보조 역할과 일치하는 경우 해당 작업이나 문제가 다른 역할 중 하나를 수행하는 사용자에게 할당됩니다. 즉, Workfront에서 일치하는 항목이 여러 개 있으면 무작위로 선택합니다. 또한 할당된 추가 역할과 해당 역할 중 하나 이상이 할당됩니다.
   * 하나 이상의 작업 역할이 할당되어 있고 사용자의 역할에 일치하는 항목이 없는 경우 해당 작업이나 문제는 사용자뿐만 아니라 역할이나 역할 모두에 할당됩니다.

* 작업이나 문제가 팀에 할당되어 있고 사용자도 할당하면 작업이나 문제가 팀과 사용자 모두에 할당된 상태로 유지됩니다.

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

1. 할당하려는 문제로 이동합니다.
1. 클릭 **할당 대상** 문제 헤더의 오른쪽 위 모서리에서 **지정** 영역

   또는

   문제가 이미 지정된 경우 현재 할당의 이름을 누릅니다.

   ![](assets/nwe-assign-to-button-in-header-350x77.png)

1. 다음 중 하나를 수행하십시오.

   * 할당할 사용자, 역할 또는 팀의 이름을 입력하고 목록에 표시되면 클릭합니다.

      ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

   * (조건부) **제안된 지정** list
   * 클릭&#x200B;**나에게 할당** 그것을 직접 할당하다
   * 클릭 **고급**

      고급 할당을 만드는 것은 작업 및 문제와 유사합니다. 고급 할당 방법에 대한 자세한 내용은 [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

      >[!TIP]
      >
      >사용자 지정을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.


1. 클릭 **저장** 문제 지정을 완료하려면
1. (선택 사항) **X 아이콘** 문제 헤더의 지정 영역 내의 지정 이름 옆에 발령을 제거합니다.

## 목록에 문제 지정

목록 보기에서 지정 필드가 표시될 때 목록이나 보고서에 문제를 지정할 수 있습니다. 문제를 할당하는 더 빠른 방법입니다.

뷰에 표시되는 필드에 따라 문제에 다음 엔티티를 할당할 수 있습니다.

| 옵션 | 할당된 엔터티 |
|---|---|
| **할당 대상** | 사용자 한 명 할당 |
| **할당됨** | 사용자 한 명 할당 |
| **할당** | 사용자, 작업 역할 또는 팀을 할당합니다. |

목록에 문제를 할당하려면

1. 뷰의 지정 대상, 지정 또는 지정 필드가 있는 문제 목록으로 이동합니다.
1. 문제를 할당하려면 다음 중 하나를 수행합니다.

   * 의 내부를 클릭합니다. **지정 대상** 또는 **할당됨** 필드를 작성하고 문제에 지정할 활성 사용자 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

      ![](assets/assigned-to-field-task-list-nwe.png)

   * 의 내부를 클릭합니다. **지정** 필드를 입력하고 문제에 지정할 활성 사용자, 작업 역할 또는 활성 팀의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

      ![](assets/assignments-field-task-list-nwe.png)
   >[!TIP]
   >
   >사용자 지정을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.


1. (조건부) 지정 필드에 표시되면 **사람 아이콘** ![](assets/teams.png) 지정 상자의 오른쪽 상단 모서리에서 고급 지정 상자를 열고 고급 지정을 생성합니다. 자세한 내용은 [고급 할당 만들기](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >지정 대상 또는 지정 필드에서 고급 지정을 수행할 수 없습니다.

1. 문제에 담당자를 추가한 후 Enter 키를 누르거나 페이지의 아무 곳이나 클릭하여 변경 내용을 저장합니다.

## 일괄 처리 문제 할당

1. 일괄 할당할 문제 목록으로 이동합니다.
1. 목록에서 몇 가지 문제를 선택합니다.
1. 을(를) 클릭합니다. **편집 아이콘** ![](assets/qs-edit-icon.png).

   다음 **문제 편집** 대화 상자가 열립니다.

1. 에서 **지정** 영역을 선택하고 **할당자** 그런 다음 모든 문제에 지정할 사용자, 작업 역할 또는 팀의 이름을 입력합니다.

   >[!IMPORTANT]
   >
   >문제가 이미 할당되어 있는 경우, 여기에서 표시하는 리소스는 문제에 대한 기존 리소스를 대체하는 대신 문제에 추가됩니다.

1. (선택 사항) **문제 소유자** 열에 두 개 이상의 자원을 문제에 할당할 때 주요 할당자 또는 문제 소유자를 나타내는 열이 있습니다. 팀에는 사용할 수 없습니다.
1. (선택 사항) 사용자가 **역할 선택** 드롭다운 메뉴에서 **할당자의 역할** 열에 있는 문제를 해결했습니다. 역할을 선택하지 않으면 Workfront은 자동으로 사용자의 기본 역할을 선택합니다.

1. (선택 사항) 모든 문제에서 기존 담당자를 제거하려면 다음 중 하나를 수행합니다.

   1. 문제에 제거할 사용자, 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 선택한 다음 를 클릭합니다 **할당자 제거** 제거할 추가 담당자를 추가하려면
   1. 클릭 **기존 할당 모두 제거** 을 눌러 선택한 모든 문제에서 모든 지정자를 제거합니다.

1. 클릭 **변경 내용 저장**.
1. (선택 사항 및 조건부) 문제 목록에 지정 대상 또는 지정 필드가 표시되면 문제에 대해 이러한 열 중 하나를 클릭한 다음 **X 아이콘** 문제로부터 제거할 담당자 이름 옆에 있습니다.
