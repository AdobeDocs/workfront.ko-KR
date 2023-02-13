---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 프로젝트 팀 관리
description: 프로젝트 팀은 프로젝트와 연결된 사용자로 구성됩니다. 프로젝트 팀의 멤버가 프로젝트의 사람 섹션에 표시됩니다.
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 프로젝트 팀 관리

프로젝트 팀은 프로젝트와 연결된 사용자로 구성됩니다. 프로젝트 팀의 멤버가 프로젝트의 사람 섹션에 표시됩니다.

## 액세스 요구 사항

<!--drafted for P&P:
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
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>사용자에 대한 액세스 권한 보기 이상</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 팀에 사용자 추가

프로젝트 팀에 사용자를 추가하면 프로젝트에 대한 보기 권한 및 프로젝트의 작업, 문제 및 문서에 대한 권한이 제공됩니다. 자세한 내용은 문서를 참조하십시오 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>프로젝트 팀의 사용자는 프로젝트의 리소스 관리 도구에 자동으로 추가되지 않습니다.

다음과 같은 방법으로 프로젝트 팀에 사용자를 추가할 수 있습니다.

* [프로젝트 팀에 사용자 자동 추가](#automatically-add-users-to-a-project-team)
* [수동으로 프로젝트 팀에 사용자 추가](#manually-add-users-to-a-project-team)

### 프로젝트 팀에 사용자 자동 추가 {#automatically-add-users-to-a-project-team}

프로젝트에서 다음 역할을 수행하는 사용자는 프로젝트 팀에 자동으로 추가되고 프로젝트를 만들 때 사람 섹션에 표시됩니다.

* 프로젝트 작성자
* 프로젝트 소유자
* 프로젝트 후원자

사용자는 다음에 할당되면 프로젝트 팀에도 자동으로 추가됩니다.

* 작업
* 문제

### 수동으로 프로젝트 팀에 사용자 추가 {#manually-add-users-to-a-project-team}

프로젝트에서 역할을 수행하지 않는 사용자가 프로젝트 수명 동안 특정 업데이트 또는 변경 사항에 대한 알림을 받으려는 경우 프로젝트 팀에 수동으로 추가할 수 있습니다.

프로젝트 팀의 사용자에게 어떤 알림을 활성화할 수 있는지에 대한 자세한 내용은 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. 사용자를 추가할 프로젝트로 이동합니다.

1. 클릭 **사람** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시** 먼저

1. 클릭 **사용자 추가**.

   프로젝트 팀에 사용자 추가 대화 상자가 표시됩니다.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 에서 **사용자 추가** 상자에서 프로젝트 팀에 추가할 활성 Workfront 사용자의 이름을 입력하고 드롭다운 목록에 이 이름이 나타나면 이름을 클릭합니다.

   이 단계를 반복하여 프로젝트 팀에 여러 사용자를 추가합니다. 사용자는 프로젝트와 연결된 그룹에 속해야 합니다.

   >[!TIP]
   >
   >* 팀, 그룹, 회사 또는 작업 역할을 추가하여 사용자를 추가할 수 없습니다.
   >* 사용자를 추가하면 아바타, 사용자의 기본 역할 및 이메일 주소를 확인하여 동일한 이름의 사용자를 구별합니다. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.



1. 클릭 **추가**.

   사용자는 프로젝트에 대한 보기 권한을 획득하고 프로젝트 팀의 일부로 프로젝트에 대한 알림을 받습니다.

## 프로젝트 팀에서 사용자 제거

사용자가 프로젝트에서 해당 역할에서 제거되면 해당 사용자는 프로젝트 팀의 일부로 남습니다.

프로젝트 팀에서 사용자를 제거하고 사용자가 프로젝트의 작업이나 문제에 할당되면 완료되지 않은 작업 및 문제에 대해 사용자의 지정이 취소됩니다. 이 경우 작업 및 문제는 작업 로드 밸런서에서 지정되지 않은 작업 영역으로 돌아갑니다.

완료된 작업 및 문제에 지정된 사용자는 프로젝트 팀에서 제거한 후에도 계속 할당됩니다.

프로젝트 팀에서 사용자 제거에 대한 자세한 내용은 [프로젝트에서 사용자 제거](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
