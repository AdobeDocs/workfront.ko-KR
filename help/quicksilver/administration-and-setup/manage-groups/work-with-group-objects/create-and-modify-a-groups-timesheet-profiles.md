---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 작업표 프로필 만들기 및 관리
description: 그룹 영역에서 관리하는 그룹을 볼 때는 그룹 관리자 또는 해당 하위 그룹 중 한 명이 관리자 액세스 권한이 있는 작업표 프로필을 보고 작업할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 그룹의 작업표 프로필 만들기 및 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

그룹 영역에서 관리하는 그룹을 볼 때는 그룹 관리자 또는 해당 하위 그룹 중 한 명이 관리자 액세스 권한이 있는 작업표 프로필을 보고 작업할 수 있습니다.

관리하는 그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>그룹의 그룹 관리자여야 합니다.</p>  <p>작업표에 대한 관리자 액세스 권한도 있어야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p>  <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 그룹 수준 작업표 프로필 만들기 및 편집

관리하는 그룹에서 사용할 작업표 프로필을 만들고 편집할 수 있습니다. 자세한 내용은 [작업표 프로필 만들기, 편집 및 할당](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 그룹 수준 작업표 프로필 삭제

관리하는 그룹에서 사용 중인 작업표 프로필을 삭제할 수 있습니다. 자세한 내용은 [작업표 프로필 삭제](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## 수동으로 그룹 작업표 생성

작업표 프로필을 그룹화하여 현재 그룹 작업표에 반영하도록 변경하려면 먼저 기존 작업표를 삭제한 다음 새 작업표를 수동으로 생성해야 합니다. 자세한 내용은 [작업표 및 시간 영역에서 작업표를 수동으로 생성합니다](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [작업표 수동으로 생성](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

그룹 작업표 삭제에 대한 자세한 내용은 [Adobe Workfront에서 작업표 삭제](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 그룹 수준 작업표 프로필 내보내기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).
1. 클릭 **그룹**.

   표시되는 목록에서 관리하는 그룹과 해당 그룹의 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 내보내려는 작업표 프로필이 있는 그룹 이름을 클릭합니다.
1. 클릭 **작업표 프로필**.
1. 클릭 **내보내기** 그룹에 대한 작업표 프로필 목록을 내보내려면
