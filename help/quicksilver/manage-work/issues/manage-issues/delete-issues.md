---
product-area: projects
navigation-topic: manage-issues
title: 문제 삭제
description: 올바른 액세스 및 권한이 있는 경우 Adobe Workfront에서 문제 또는 요청을 삭제할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# 문제 삭제

<!--Audited: 05/2025-->

올바른 액세스 및 권한이 있는 경우 Adobe Workfront에서 문제 또는 요청을 삭제할 수 있습니다.

>[!TIP]
>
>Workfront에서 &quot;문제&quot;와 &quot;요청&quot;은 서로 교환하여 사용됩니다. 프로젝트와 작업 모두에 문제를 기록하여 해결해야 하는 예기치 않은 작업을 표시할 수 있습니다. 요청 대기열로 지정된 프로젝트에 문제로 기록된 요청을 제출할 수도 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 기여자 이상</p>
   <p>현재: 요청 이상</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 또는 상위 액세스 권한</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>프로젝트 또는 작업에 대한 기여 또는 더 높은 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문제 삭제 시 고려 사항

* Workfront 관리자 또는 그룹 관리자는 프로젝트 환경 설정 영역에서 완료 상태의 프로젝트 삭제 문제를 활성화해야 합니다.

  프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

* 문제가 시간을 기록한 경우 Workfront 관리자 또는 그룹 관리자는 Workfront 인스턴스에서 작업 및 문제 환경 설정을 구성하여 이러한 문제를 삭제할 수 있도록 허용해야 합니다. 이 설정은 시간이 기록되는 문제가 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

  시간이 기록된 문제의 삭제를 활성화하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)의 &quot;삭제&quot; 섹션을 참조하십시오.


## 문제 삭제의 영향

문제를 삭제하면 해당 문제에 연결된 다른 오브젝트에 영향을 줍니다.

문제를 삭제하면 문제에 첨부된 다음 개체도 삭제됩니다.

* 문서

  체크 아웃된 문서가 첨부된 문제는 삭제할 수 없습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

* 메모
* 승인

Workfront 또는 그룹 관리자가 Workfront 인스턴스의 **타임시트 및 시간 환경 설정**&#x200B;에서 프로젝트, 작업 또는 문제 삭제 환경 설정을 구성하는 방법에 따라, 문제를 삭제할 때 문제에 기록된 시간이 다음 중 한 방법으로 처리됩니다.

* 프로젝트로 이동하고 나중에 문제가 복원되는 경우 해당 문제에 대해 복원되지 않습니다.
* 나중에 문제가 복원되면 을 삭제하고 문제에 대해 복원합니다.

  시간이 기록된 작업이 있는 프로젝트를 삭제하려고 할 때도 적용됩니다.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  문제에 기록된 시간에 대한 삭제 환경 설정을 구성하는 방법에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.

* 문제 또는 문제 승인에 할당된 사용자가 프로젝트 팀에 남아 있습니다.\
  프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md)를 참조하십시오.

## 문제 삭제

### 프로젝트에서 여러 문제를 동시에 삭제  {#delete-multiple-issues-in-a-project-simultaneously}

1. **주 메뉴**(으)로 이동합니다.
1. **프로젝트**&#x200B;를 클릭합니다.
1. 삭제할 문제가 포함된 프로젝트 이름을 클릭합니다.
1. 왼쪽 패널에서 **문제**&#x200B;를 클릭합니다.

   선택한 프로젝트와 관련된 문제 목록이 오른쪽에 표시됩니다.
1. 목록에서 하나 이상의 문제를 선택한 다음 목록 맨 위에 있는 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.

1. 삭제가 허용되는 경우 **삭제**&#x200B;를 클릭하십시오.

   Workfront 관리자는 시간이 기록되는 문제의 삭제를 허용하지 않을 수 있습니다.\
   문제를 삭제하는 데 필요한 액세스 및 권한에 대한 자세한 내용은 이 문서의 [문제 삭제 고려 사항](#considerations-for-deleting-issues) 섹션을 참조하십시오.

### 단일 문제 삭제 {#delete-a-single-issue}

{{step1-to-projects}}

1. 삭제할 문제가 포함된 프로젝트 이름을 클릭합니다.
1. 왼쪽 패널에서 **문제**&#x200B;를 클릭합니다.

   왼쪽 패널의 ![문제 섹션](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 삭제할 문제의 이름을 클릭합니다.
1. 문제 이름 오른쪽에 있는 **자세히** 메뉴를 클릭합니다.

   ![추가 문제 메뉴](assets/qs-issue-more-menu-highlighted-350x469.png)

1. **문제 삭제**&#x200B;를 클릭합니다.
1. **삭제**&#x200B;를 클릭하여 삭제하십시오.

   >[!NOTE]
   >
   >  Workfront 관리자는 시간이 기록되는 문제의 삭제를 허용하지 않을 수 있습니다.\
   >  문제를 삭제하는 데 필요한 액세스 및 권한에 대한 자세한 내용은 이 문서의 [문제 삭제 고려 사항](#considerations-for-deleting-issues) 섹션을 참조하십시오.

## 삭제된 문제 복원

Workfront 또는 그룹 관리자는 문제를 삭제한 후 30일 이내에 복원할 수 있습니다.

Workfront에서 항목을 복원하는 방법에 대한 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)을 참조하십시오.
