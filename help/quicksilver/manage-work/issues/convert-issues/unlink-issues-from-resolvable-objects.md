---
product-area: projects
navigation-topic: convert-issues
title: 해결 오브젝트에서 문제 연결 해제
description: 문제를 프로젝트 또는 작업으로 변환하여 프로젝트 또는 작업을 만들 때 원래 문제를 유지할 수 있는 옵션이 있습니다. 문제를 전환하는 동안 이 옵션을 사용하려면 Adobe Workfront 관리자가 이 환경 설정을 활성화해야 합니다. 문제를 프로젝트 및 작업으로 변환하는 방법에 대한 자세한 내용은 Adobe Workfront의 문제 변환 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# 해결 오브젝트에서 문제 연결 해제

<!--Audited: 08/2025-->

문제를 프로젝트 또는 작업으로 변환하여 프로젝트 또는 작업을 만들 때 원래 문제를 유지할 수 있는 옵션이 있습니다. 문제를 전환하는 동안 이 옵션을 사용하려면 Adobe Workfront 관리자가 이 환경 설정을 활성화해야 합니다.\
문제를 프로젝트 및 작업으로 변환하는 방법에 대한 자세한 내용은 [Adobe Workfront의 문제 변환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

프로젝트 또는 작업으로 전환된 문제를 유지하기로 결정하면 문제 해결은 프로젝트 또는 작업과 연결됩니다. 문제가 프로젝트 또는 작업의 해결 가능한 오브젝트가 됩니다. 프로젝트 또는 작업이 문제의 해결 개체입니다.

문제를 다른 문제에 수동으로 연결할 수도 있습니다. 두 번째 문제는 첫 번째 문제(이 경우)에 대한 해결 중 오브젝트가 됩니다.\
개체 확인에 대한 자세한 내용은 [해결 및 해결 가능한 개체 개요](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)를 참조하십시오.

>[!TIP]
>
>문제 상태는 해결 중 오브젝트의 상태에 따라 자동으로 변경되므로 변경할 수 없습니다.

문제에서 프로젝트, 작업 또는 문제를 제거하여 프로젝트, 작업 또는 문제의 해결에서 연결을 해제할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>작업 및 프로젝트에 대한 액세스 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>작업 또는 프로젝트에 대한 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 프로젝트, 작업 또는 문제에서 문제 연결 해제

1. 프로젝트, 작업 또는 문제에 연결된 문제로 이동합니다.
1. **문제 세부 정보** 섹션을 클릭합니다.
1. **문제 세부 정보** 섹션의 **개요** 영역으로 이동합니다.
1. **해결한 사람** 필드에서 해결 가능한 개체 유형을 제거합니다.\
   문제는 프로젝트, 작업 또는 문제로 해결될 수 있습니다.

   이렇게 하면 해결 중인 오브젝트가 문제에서 제거됩니다.

1. **저장** **변경 내용**&#x200B;을 클릭합니다.\
   이 문제는 더 이상 프로젝트, 작업 또는 문제와 연결되지 않으며 이제 독립적으로 문제를 해결할 수 있습니다.
