---
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 소유자 및 스폰서 업데이트
description: Adobe Workfront에서 프로젝트를 만들면 자동으로 프로젝트의 프로젝트 소유자로 설정됩니다. 이 필드를 다른 사용자와 업데이트할 수 있습니다. 프로젝트의 프로젝트 스폰서 필드를 업데이트할 수도 있습니다.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 프로젝트 소유자 및 스폰서 업데이트

Adobe Workfront에서 프로젝트를 만들면 자동으로 프로젝트의 프로젝트 소유자로 설정됩니다. 이 필드를 다른 사용자와 업데이트할 수 있습니다. 프로젝트의 프로젝트 스폰서 필드를 업데이트할 수도 있습니다.

프로젝트 소유자 및 스폰서에 대한 자세한 내용은 [프로젝트 소유자 및 스폰서 개요](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>템플릿의 소유자 및 스폰서를 식별할 수 있습니다. 해당 템플릿에서 프로젝트를 생성하면 템플릿 소유자가 프로젝트 소유자가 되고 템플릿 스폰서가 프로젝트 스폰서가 됩니다. 템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>&nbsp;</p> </td> 
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
   <td> <p>Edit permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>모든</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트의 프로젝트 소유자 업데이트

사용자를 프로젝트의 프로젝트 소유자로 추가하면 Workfront이 자동으로 사용자에게 프로젝트를 볼 수 있는 권한을 제공합니다.

1. 업데이트할 프로젝트로 이동합니다.
1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **편집** 아이콘 ![](assets/qs-edit-icon.png) 프로젝트 세부 사항 영역의 오른쪽 위 모서리에서 **개요**.

1. 사용자 이름을 지정합니다. **프로젝트 소유자** 필드.

   활성 사용자만 프로젝트 소유자로 지정할 수 있습니다.

1. 클릭 **변경 내용 저장**.

   프로젝트 소유자는 프로젝트 헤더와 프로젝트 상세내역 영역에서 업데이트됩니다.

![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## 프로젝트의 프로젝트 스폰서 업데이트

사용자를 프로젝트의 프로젝트 스폰서로 추가하면 Workfront이 해당 사용자에게 프로젝트를 볼 수 있는 권한을 자동으로 제공합니다.

>[!TIP]
>
>프로젝트 스폰서로 추가하는 사용자가 시스템 관리자인 경우 프로젝트 공유 목록에 추가되지 않습니다.

1. 업데이트할 프로젝트로 이동합니다.
1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **편집** 아이콘 ![](assets/qs-edit-icon.png) 프로젝트 세부 사항 영역의 오른쪽 위 모서리에서 **개요**.

1. 사용자 이름을 지정합니다. **프로젝트 스폰서** 필드.

   활성 사용자만 프로젝트 스폰서로 지정할 수 있습니다.

1. 클릭 **변경 내용 저장**.

   프로젝트 상세내역 영역의 프로젝트 스폰서 업데이트.

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
