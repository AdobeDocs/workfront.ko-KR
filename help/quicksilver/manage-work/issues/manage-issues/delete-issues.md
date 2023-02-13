---
product-area: projects
navigation-topic: manage-issues
title: 문제 삭제
description: 올바른 액세스 권한 및 요청이 있는 경우 Adobe Workfront에서 문제 또는 요청을 삭제할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 문제 삭제

올바른 액세스 권한 및 요청이 있는 경우 Adobe Workfront에서 문제 또는 요청을 삭제할 수 있습니다.

>[!TIP]
>
>&quot;문제&quot; 및 &quot;요청&quot;은 Workfront에서 서로 교환하여 사용됩니다. 프로젝트 및 작업 모두에 문제를 기록하여 해결해야 하는 예상치 못한 작업을 나타낼 수 있습니다. 요청 큐로 지정된 프로젝트에서 문제로 기록된 요청을 제출할 수도 있습니다.

## 액세스 요구 사항

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
   <td> <p>요청 이상</p> <p>프로젝트의 Issues 섹션에서 문제를 삭제하려면 해당 이상의 라이센스를 검토하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>프로젝트 또는 작업에 대한 기여 또는 더 높은 권한</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제 삭제 고려 사항

* Workfront 관리자나 그룹 관리자는 프로젝트 환경 설정 영역에서 완료 상태인 프로젝트의 삭제 문제를 활성화해야 합니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 문제가 기록되면 Workfront 관리자나 그룹 관리자가 Workfront 인스턴스에서 작업 및 문제 환경 설정을 구성하여 이러한 문제를 삭제할 수 있도록 허용해야 합니다. 이 기능은 로그온하는 시간 문제가 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   시간이 기록되는 문제의 삭제를 활성화하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 삭제 문제의 영향

문제를 삭제하면 문제에 연결된 다른 개체가 영향을 받습니다.

문제를 삭제하면 문제에 첨부된 다음 개체도 삭제됩니다.

* 문서

   체크 아웃된 문서가 첨부된 문제는 삭제할 수 없습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md).

* 메모
* 승인

Workfront 또는 그룹 관리자가 **작업표 및 시간 기본 설정** Workfront 인스턴스에서 문제에 대해 기록된 시간은 문제를 삭제할 때 다음 방법 중 하나로 처리됩니다.

* 나중에 문제가 복원되면 프로젝트로 이동하며 문제가 복원되지 않습니다.
* 문제가 나중에 복원되면 삭제되고 문제에 대해 복원됩니다.

   이 기능은 로그온한 시간이 있는 작업이 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   로그온한 시간 동안의 삭제 환경 설정 구성에 대한 자세한 내용은 다음을 참조하십시오 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 문제 또는 문제 승인에 지정된 사용자는 프로젝트 팀에 유지됩니다.\
   프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 문제 삭제

* [프로젝트에서 동시에 여러 문제 삭제](#delete-multiple-issues-in-a-project-simultaneously)
* [단일 문제 삭제](#delete-a-single-issue)

### 프로젝트에서 동시에 여러 문제 삭제  {#delete-multiple-issues-in-a-project-simultaneously}

1. 로 이동합니다. **기본 메뉴**.
1. 클릭 **프로젝트**.
1. 삭제할 문제가 포함된 프로젝트 이름을 클릭합니다.
1. 클릭 **문제** 왼쪽 패널에 표시됩니다.
1. 문제를 선택한 다음 **삭제** 아이콘 ![](assets/delete.png) 를 클릭합니다.

1. 삭제를 허용하는 경우 **예, 삭제합니다.**.\
   Workfront 관리자는 시간이 기록되는 문제를 삭제하지 못할 수 있습니다.\
   문제를 삭제하는 데 필요한 액세스 및 권한에 대한 자세한 내용은 [문제 삭제](#access-and-permissions-needed).

### 단일 문제 삭제 {#delete-a-single-issue}

1. 을(를) 클릭합니다. **기본** 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **프로젝트**.
1. 삭제할 문제가 포함된 프로젝트 이름을 클릭합니다.
1. 클릭 **문제** 왼쪽 패널에 표시됩니다.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 삭제할 문제 이름을 클릭합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 아래의 제품에서 사용할 수 있습니다.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. 클릭 **삭제**.
1. 삭제를 허용하는 경우 **예, 삭제합니다.**.

   Workfront 관리자는 시간이 기록되는 문제를 삭제하지 못할 수 있습니다.\
   문제를 삭제하는 데 필요한 액세스 및 권한에 대한 자세한 내용은 [문제 삭제](#access-and-permissions-needed).

## 삭제된 문제 복원

Workfront 또는 그룹 관리자는 삭제된 후 30일 이내에 문제를 복원할 수 있습니다. Workfront에서 항목 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
