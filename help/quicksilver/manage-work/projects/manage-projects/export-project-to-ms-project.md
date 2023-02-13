---
product-area: projects
navigation-topic: manage-projects
title: Microsoft 프로젝트로 프로젝트 내보내기
description: Adobe Workfront 프로젝트를 Microsoft 프로젝트로 내보낼 수 있습니다.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft 프로젝트로 프로젝트 내보내기

Adobe Workfront 프로젝트를 Microsoft 프로젝트로 내보낼 수 있습니다. 

>[!IMPORTANT]
>
>* 일부 Workfront 필드가 Microsoft 프로젝트 파일에 전송되지 않습니다.\
   >  Workfront과 Microsoft 프로젝트 간의 필드 호환성에 대한 자세한 내용은 문서를 참조하십시오 [Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* 한 애플리케이션에서 다른 애플리케이션으로 프로젝트를 전송하는 횟수를 제한하는 것이 좋습니다. 
>


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
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 보기 이상의 액세스 권한</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 보기 이상</p> <p>프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## Workfront에서 Microsoft 프로젝트로 프로젝트 내보내기

프로젝트 페이지 또는 프로젝트 목록 또는 보고서에서 Workfront에서 프로젝트를 내보낼 수 있습니다.

1. 내보낼 프로젝트로 이동하고 **자세히** 아이콘 ![](assets/qs-more-menu.png) 프로젝트 이름의 오른쪽에 있습니다.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   또는

   프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택한 다음 자세히 아이콘을 클릭합니다 ![](assets/qs-more-menu.png) 를 클릭합니다.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 클릭 **MS 프로젝트 내보내기**.

   프로젝트는 컴퓨터에 XML 파일로 다운로드되므로 Microsoft Project로 가져올 수 있습니다. 
