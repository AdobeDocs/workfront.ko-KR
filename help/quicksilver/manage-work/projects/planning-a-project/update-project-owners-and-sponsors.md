---
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트 소유자 및 스폰서 업데이트
description: Adobe Workfront에서 프로젝트를 만들면 프로젝트의 프로젝트 소유자로 자동 설정됩니다. 다른 사용자로 이 필드를 업데이트할 수 있습니다. 프로젝트의 프로젝트 스폰서 필드도 업데이트할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 프로젝트 소유자 및 스폰서 업데이트

Adobe Workfront에서 프로젝트를 만들면 프로젝트의 프로젝트 소유자로 자동 설정됩니다. 다른 사용자로 이 필드를 업데이트할 수 있습니다. 프로젝트의 프로젝트 스폰서 필드도 업데이트할 수 있습니다.

프로젝트 소유자 및 스폰서에 대한 자세한 내용은 [프로젝트 소유자 및 스폰서 개요](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md)를 참조하십시오.

>[!TIP]
>
>템플릿에 대한 소유자와 스폰서를 식별할 수 있습니다. 해당 템플릿에서 프로젝트를 만들면 템플릿 소유자 가 프로젝트 소유자 가 되고 템플릿 스폰서 가 프로젝트 스폰서 가 됩니다.
>
>템플릿에 소유자가 없으면 팀플레이트에서 프로젝트를 만드는 사용자가 프로젝트 소유자가 됩니다.
>
>템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>  </p> </td> 
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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> <p>  </p> </td> 
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
   <td> <p>프로젝트에 대한 권한 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트의 프로젝트 소유자 업데이트

사용자를 프로젝트의 프로젝트 소유자로 추가하면 Workfront에서 자동으로 사용자에게 프로젝트를 볼 수 있는 권한을 부여합니다.

1. 업데이트할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.
1. 프로젝트 세부 정보 영역의 오른쪽 상단에 있는 **편집** 아이콘 ![](assets/qs-edit-icon.png)을(를) 클릭한 다음 **개요**&#x200B;를 클릭합니다.

1. **프로젝트 소유자** 필드에 대한 사용자 이름을 지정하십시오.

   활성 사용자만 프로젝트 소유자로 지정할 수 있습니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   프로젝트 소유자 는 프로젝트 헤더 및 프로젝트 세부 정보 영역에서 업데이트됩니다.

![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## 프로젝트의 프로젝트 스폰서 업데이트

사용자를 프로젝트의 프로젝트 스폰서로 추가하면 Workfront에서 자동으로 사용자에게 프로젝트를 볼 수 있는 권한을 부여합니다.

>[!TIP]
>
>프로젝트 스폰서로 추가하는 사용자가 시스템 관리자인 경우 프로젝트의 공유 목록에 추가되지 않습니다.

1. 업데이트할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.
1. 프로젝트 세부 정보 영역의 오른쪽 상단에 있는 **편집** 아이콘 ![](assets/qs-edit-icon.png)을(를) 클릭한 다음 **개요**&#x200B;를 클릭합니다.

1. **프로젝트 스폰서** 필드에 대한 사용자 이름을 지정하십시오.

   활성 사용자만 프로젝트 스폰서로 지정할 수 있습니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   프로젝트 스폰서는 프로젝트 세부 정보 영역에서 업데이트됩니다.

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
