---
product-area: projects
navigation-topic: update-work-in-a-project
title: 그룹에 연결된 작업에 상태 적용
description: 프로젝트가 그룹과 연결된 경우 시스템 수준 상태와 해당 그룹과 연결된 사용자 지정 상태를 모두 해당 프로젝트의 프로젝트, 작업 또는 문제에 적용할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 그룹에 연결된 작업에 상태 적용

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

프로젝트가 그룹과 연결된 경우 시스템 수준 상태와 해당 그룹과 연결된 사용자 지정 상태를 프로젝트 또는 해당 프로젝트의 작업 및 문제에 모두 적용할 수 있습니다. Adobe Workfront의 그룹 상태에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

>[!TIP]
>
>프로젝트만 그룹과 연결할 수 있습니다. 문제 및 작업은 해당 그룹이 속한 프로젝트에서 그룹을 상속합니다.

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 그룹 및 상태 업데이트

프로젝트에 대한 그룹을 업데이트할 때 작업, 문제 또는 프로젝트 상태에 사용할 수 있는 옵션이 그룹과 일치하도록 변경됩니다.

1. [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)에 설명된 대로 프로젝트로 이동하거나 새 프로젝트를 만듭니다.
1. **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png)을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. **개요** 섹션 아래쪽에 표시되는 **프로젝트 편집** 상자의 **그룹** 드롭다운 메뉴에서 그룹을 선택합니다.

1. **상태** 드롭다운 메뉴에서 사용자 지정 상태를 선택합니다.

   >[!NOTE]
   >
   >**그룹** 드롭다운 메뉴에서 다른 그룹을 선택하면 **상태** 메뉴의 사용자 지정 상태가 자동으로 변경되어 새 그룹과의 상관 관계를 만듭니다.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >
   >

1. 프로젝트의 상태를 선택합니다. 해당 그룹에 작성 및 적용한 사용자 정의 상태가 목록에 표시됩니다.
