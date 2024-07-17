---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 하위 그룹 멤버 보기 및 관리
description: 관리하는 그룹을 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 하위 그룹 멤버 보기 및 관리

관리하는 그룹을 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 관리자(모든 사용자) 옵션을 선택한 상태로 사용자에 대한 액세스 편집</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하세요.

## 그룹 아래의 하위 그룹 구성원 보기 및 관리

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 하위 그룹 구성원을 보거나 관리할 그룹의 이름을 누릅니다.
1. 왼쪽 패널에서 **하위 그룹 구성원**&#x200B;을 클릭합니다.

   이 왼쪽 패널 항목은 그룹에 하위 그룹이 있는 경우에만 사용할 수 있습니다.

1. 다음 중 하나를 수행합니다.

   * 목록에서 구성원을 선택한 다음 ![](assets/edit-icon.png) 편집을 클릭하여 해당 사용자의 사용자 프로필을 수정합니다.

     자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 또는 [사용자 프로필 일괄 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)을 참조하십시오.

   * 목록에서 원하는 수의 구성원을 선택한 다음 ![](assets/comment-icon.png) 업데이트를 클릭하여 사용자 프로필에 주석을 추가합니다.

     사용자 또는 사용자는 댓글이 포함된 이메일 알림과 인앱 알림을 받습니다. 댓글은 사용자 프로필의 업데이트 영역에 표시됩니다.

   * 목록에서 원하는 수의 멤버를 선택한 다음 ![](assets/deactivate-user.png) 비활성화 또는 ![](assets/activate-user.png) 활성화를 클릭합니다.

     자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하십시오.

   * 구성원 목록을 ![](assets/export.png)에 내보냅니다.
