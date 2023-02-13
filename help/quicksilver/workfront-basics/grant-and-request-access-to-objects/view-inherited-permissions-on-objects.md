---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 객체에 대한 상속된 권한 보기
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 개체를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여할 수 있습니다. 자세한 내용은 프로젝트에 대한 액세스 권한 부여 를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: 7025f097-ea99-41bf-965e-617b0f532ff7
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 객체에 대한 상속된 권한 보기

Adobe Workfront 관리자는 액세스 수준을 할당할 때 개체를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여할 수 있습니다. 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

사용자에게 부여된 액세스 레벨과 함께, 공유 액세스 권한이 있는 특정 객체에 권한을 부여할 수도 있습니다. 액세스 수준 및 권한에 대한 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방법](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

개체는 Adobe Workfront의 상위 개체에서 권한을 상속합니다.

Workfront의 객체 계층 구조에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p>
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access on the objects you want to view permissions for</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the objects you want to view permissions for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용 권한을 보려는 개체에 대한 보기 또는 더 높은 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>사용 권한을 보려는 개체에 대한 보기 또는 더 높은 사용 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 객체에 대한 상속된 권한 보기

상속된 사용 권한을 보는 것은 모든 객체에 대해 동일합니다.

프로젝트에 대한 상속된 권한을 보려면

1. 공유 권한을 보려는 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **공유**.

1. 를 확장합니다. **상속된 권한** 목록.

   이 목록에는 프로젝트가 속한 포트폴리오나 프로그램에 액세스할 수 있고 프로젝트에 대한 권한이 있는 사용자 이름이 표시됩니다.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

1. (선택 사항) 객체에서 상속된 권한을 제거하려면 다음을 참조하십시오 [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   >[!NOTE]
   >
   >상속된 권한을 제거하려면 객체에 대한 관리 권한이 있어야 합니다.

 

 
