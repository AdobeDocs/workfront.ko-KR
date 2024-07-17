---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 타임시트 프로필 만들기 및 관리
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹 또는 그 하위 그룹 중 하나의 관리자가 관리 액세스 권한을 가지는 타임시트 프로필을 보고 작업할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 그룹의 타임시트 프로필 만들기 및 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

그룹 영역에서 관리하는 그룹을 볼 때 그룹 또는 그 하위 그룹 중 하나의 관리자가 관리 액세스 권한을 가지는 타임시트 프로필을 보고 작업할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>그룹의 그룹 관리자여야 합니다.</p>  <p>타임시트에 대한 관리 액세스 권한도 있어야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.</p>  <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 그룹 수준 타임시트 프로필 만들기 및 편집

관리하는 그룹에서 사용할 타임시트 프로필을 만들고 편집할 수 있습니다. 지침은 [타임시트 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

## 그룹 수준 타임시트 프로필 삭제

관리하는 그룹에서 사용 중인 타임시트 프로필을 삭제할 수 있습니다. 지침은 [타임시트 프로필 삭제](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)를 참조하십시오.

## 수동으로 그룹 타임시트 생성

현재 그룹 타임시트에 반영하도록 그룹 타임시트 프로필에 적용한 변경 사항을 활성화하려면 먼저 기존 타임시트를 삭제한 다음 새 타임시트를 수동으로 생성해야 합니다. 지침은 [타임시트 및 시간 영역에서 수동으로 타임시트 생성](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)([타임시트 수동으로 생성](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md))을 참조하십시오.

그룹 타임시트 삭제에 대한 자세한 내용은 [Adobe Workfront에서 타임시트 삭제](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)를 참조하십시오.

## 그룹 수준 타임시트 프로필 내보내기

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.
1. **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 내보낼 타임시트 프로필이 있는 그룹의 이름을 클릭합니다.
1. **타임시트 프로필**&#x200B;을 클릭합니다.
1. 그룹에 대한 타임시트 프로필 목록을 내보내려면 **내보내기**&#x200B;를 클릭하십시오.
