---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 객체를 삭제하고 복원할 때 시간에 영향을 구성
description: 사용자가 프로젝트, 작업 또는 시간이 기록되는 문제를 삭제할 때 발생하는 시간을 구성할 수 있습니다. 선택하는 옵션은 프로젝트, 작업 또는 문제가 나중에 복원될 경우 시간이 어떻게 될지 결정합니다. Workfront에서 항목을 복원하는 방법에 대한 자세한 내용은 삭제된 항목 복원 을 참조하십시오.
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 객체를 삭제하고 복원할 때 시간에 영향을 구성

사용자가 프로젝트, 작업 또는 시간이 기록되는 문제를 삭제할 때 발생하는 시간을 구성할 수 있습니다. 선택하는 옵션은 프로젝트, 작업 또는 문제가 나중에 복원될 경우 시간이 어떻게 될지 결정합니다. (Workfront에서 항목 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md))

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 항목을 삭제하고 복원할 때 관리 시간을 구성합니다

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 확장 **작업표 및 시간**&#x200B;를 클릭한 다음&#x200B;**기본 설정**.

1. 을(를) 찾습니다 **프로젝트, 작업 또는 문제 삭제 환경 설정** 섹션을 참조하십시오.
1. (조건부) 프로젝트를 삭제할 때 시간 관리 방법을 구성하려면 **프로젝트 삭제 시** 섹션:

   * 기록표에 이미 추가된 시간을 일반 시간으로 유지합니다. 이 프로젝트를 나중에 복원하면 작업표에 시간이 남아 있습니다.\
      이 옵션은 기본적으로 선택되어 있습니다.
   * 로그된 시간 삭제(이 프로젝트가 나중에 복원되면 기록된 시간이 프로젝트에 복원됨)

1. (조건부) 작업이나 문제가 삭제될 때 시간이 관리되는 방식을 구성하려면 **작업 또는 문제 삭제 시** 섹션:

   * 로그된 시간을 작업이나 문제가 있는 프로젝트로 이동(이 작업이나 문제가 나중에 복원되면 해당 시간이 프로젝트에 남아 있음)\
      이 옵션은 기본적으로 선택되어 있습니다.
   * 로그된 시간 삭제(이 작업이나 문제가 나중에 복원되면 로그된 시간이 작업 또는 문제로 복원됨)

1. **저장**&#x200B;을 클릭합니다.
