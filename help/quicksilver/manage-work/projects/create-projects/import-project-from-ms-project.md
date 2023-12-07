---
product-area: projects
navigation-topic: create-projects
title: Microsoft 프로젝트에서 프로젝트 가져오기
description: Microsoft Project에서 Adobe Workfront으로 프로젝트를 가져오고 하나의 애플리케이션에서 모든 프로젝트를 관리할 수 있습니다. Microsoft 프로젝트에서 프로젝트를 가져올 때마다 Workfront에 새 프로젝트가 만들어집니다.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# Microsoft 프로젝트에서 프로젝트 가져오기

Microsoft Project에서 Adobe Workfront으로 프로젝트를 가져오고 하나의 애플리케이션에서 모든 프로젝트를 관리할 수 있습니다. Microsoft 프로젝트에서 프로젝트를 가져올 때마다 Workfront에 새 프로젝트가 만들어집니다.

>[!IMPORTANT]
>
>일부 Microsoft 프로젝트 필드는 Workfront으로 전송되지 않습니다.
>
>Workfront과 Microsoft Project 간의 필드 호환성에 대한 자세한 내용은 [Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## 액세스 요구 사항

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
   <td> <p>새 라이선스: Standard </p> 
   또는
   <p>현재 라이선스: 플랜 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받습니다 </p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## MS 프로젝트에서 프로젝트 만들기

주 메뉴의 프로젝트 영역이나 포트폴리오 또는 프로그램의 프로젝트 영역에서 프로젝트를 만들 수 있습니다.

1. Microsoft 프로젝트로 이동한 다음 Workfront에서 가져올 프로젝트를 엽니다.
1. 클릭 **파일**, 그런 다음 **다른 이름으로 저장** 프로젝트를 .xml 파일로 저장합니다.

1. Workfront에 로그인.
1. 다음 중 하나를 수행하십시오.

   * 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-icon.png), 클릭 **프로젝트**, 다음 확장 **새 프로젝트**.
   * 포트폴리오로 이동한 다음 를 확장합니다. **새 프로젝트**.
   * 프로그램으로 이동한 다음 를 확장합니다 **새 프로젝트**.
   * 그룹 관리자는 관리하는 그룹의 프로젝트 섹션에서 프로젝트를 만들 수도 있습니다. 자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 다음을 선택합니다. **MS 프로젝트 가져오기** 옵션을 선택합니다.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 클릭 **파일 선택**&#x200B;그런 다음 Microsoft 프로젝트에서 내보낸 컴퓨터에서 .xml 파일을 찾습니다.
1. 선택한 파일을 가져옵니다.

   Workfront은 가져오기 프로세스를 시작하고 Microsoft 프로젝트에서 내보낸 파일을 기반으로 새 프로젝트를 만듭니다.

   가져오기 프로세스가 완료되면 가져오기가 성공적으로 완료되었음을 확인하는 메시지가 표시되는 새 프로젝트 페이지로 이동합니다.

   >[!NOTE]
   >
   >Workfront의 파일 업로드 시간은 15분으로 제한됩니다. 파일 업로드가 이보다 오래 걸리는 경우 프로젝트를 더 작은 프로젝트로 분류하여 별도로 가져오는 것이 좋습니다. 작업을 Workfront으로 가져온 다음에는 작업을 한 프로젝트에서 다른 프로젝트로 이동하여 한 프로젝트로 결합합니다. 작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (선택 사항) Workfront에서 프로젝트를 계속 편집합니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

   템플릿에서 생성된 새 프로젝트의 상태는 프로젝트 환경 설정 영역에서 Workfront 관리자 또는 그룹 프로젝트 환경 설정 영역에서 그룹 관리자가 정의한 상태에 해당합니다. 프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
