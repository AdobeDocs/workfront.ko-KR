---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 개체가 삭제 및 복원될 때 시간에 대한 효과 구성
description: 사용자가 시간이 기록되는 프로젝트, 작업 또는 문제를 삭제할 때 시간이 어떻게 되는지 구성할 수 있습니다. 선택하는 옵션은 프로젝트, 작업 또는 문제가 나중에 복원될 경우 시간에 미치는 영향도 결정합니다. Workfront의 항목 복원에 대한 자세한 내용은 삭제된 항목 복원을 참조하십시오.
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 개체가 삭제 및 복원될 때 시간에 대한 효과 구성

사용자가 시간이 기록되는 프로젝트, 작업 또는 문제를 삭제할 때 시간이 어떻게 되는지 구성할 수 있습니다. 선택하는 옵션은 프로젝트, 작업 또는 문제가 나중에 복원될 경우 시간에 미치는 영향도 결정합니다. (Workfront의 항목 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)을 참조하세요.)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 항목 삭제 및 복원 시 시간 관리 방법 구성

{{step-1-to-setup}}

1. **타임시트 및 시간**&#x200B;을 확장한 다음 **환경 설정**&#x200B;을 클릭합니다.

1. **프로젝트, 작업 또는 문제 삭제 환경 설정** 섹션을 찾습니다.
1. (조건부) 프로젝트 삭제 시 시간을 관리하는 방법을 구성하려면 **프로젝트 삭제 시** 섹션에서 다음 옵션 중 하나를 선택합니다.

   * 타임시트에 이미 추가된 기록된 시간을 일반 시간으로 유지(이 프로젝트가 나중에 복원되면 타임시트에 시간이 유지됩니다.)\
     이 옵션은 기본적으로 선택되어 있습니다.
   * 기록된 시간 삭제(이 프로젝트가 나중에 복원되면 기록된 시간이 프로젝트에 복원됨)

1. (조건부) 작업 또는 문제를 삭제할 때 시간을 관리하는 방법을 구성하려면 **작업 또는 문제를 삭제할 때** 섹션에서 다음 옵션 중 하나를 선택하십시오.

   * 기록된 시간을 작업 또는 문제가 있는 프로젝트로 이동합니다(이 작업 또는 문제가 나중에 복원되면 프로젝트에 시간이 남아 있음).\
     이 옵션은 기본적으로 선택되어 있습니다.
   * 기록된 시간 삭제(이 작업 또는 문제가 나중에 복원되면 기록된 시간이 작업 또는 문제에 복원됨)

1. **저장**&#x200B;을 클릭합니다.
