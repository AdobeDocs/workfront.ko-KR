---
title: Adobe Workfront 목표에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront 목표에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8639da14-d545-4f9a-894b-12c29699b0db
source-git-commit: 6948f9462c59bad9e6db67d6169e5f9dec4157fe
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Adobe Workfront 목표에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 액세스 수준을 사용하여 Adobe Workfront 목표에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

사용자에게 Workfront 목표에 대한 액세스 권한을 부여하려면 다음 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 패키지</td> 
   <td> <p>Workfront Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 액세스 수준이 있어야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Goals <p>Contact your Workfront account manager to learn about a Workfront Goals license. </p> <p>Workfront Goals is available only in the new Adobe Workfront experience.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>You must have the System Administrator access level.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 사용자 정의 액세스 수준을 사용하여 Workfront 목표에 대한 액세스 권한 부여

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 이 액세스 수준에 사용할 **목표** 오른쪽에 있는 옵션을 클릭합니다.


   >[!NOTE]
   >
   >외부 라이선스 유형에서는 Workfront 목표에 대한 보기 또는 편집 액세스를 허용하지 않습니다.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

## 라이선스 유형별 Workfront 목표에 액세스

Workfront 관리자는 액세스 수준을 사용하여 다음 라이선스를 가진 사용자에게 Workfront 목표에 대한 액세스 권한을 부여할 수 있습니다.

* 표준, 라이트, 기여자
* 플랜, 작업, 요청 또는 검토 라이선스.

Workfront 목표에 액세스하는 방법에 대한 자세한 내용은 [Workfront 목표 사용 요구 사항](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)을 참조하십시오.
