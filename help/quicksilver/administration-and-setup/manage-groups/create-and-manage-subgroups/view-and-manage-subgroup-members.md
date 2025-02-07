---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 하위 그룹 멤버 보기 및 관리
description: 관리하는 그룹을 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 하위 그룹 멤버 보기 및 관리

관리하는 그룹을 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

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
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <img src="assets/gear-icon-settings.png">에서 두 개의 <b>사용자 관리</b> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 아래의 하위 그룹 구성원 보기 및 관리

{{step-1-to-setup}}

1. **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 하위 그룹 구성원을 보거나 관리할 그룹의 이름을 누릅니다.
1. 왼쪽 패널에서 **하위 그룹 구성원**&#x200B;을 클릭합니다.

   이 왼쪽 패널 항목은 그룹에 하위 그룹이 있는 경우에만 사용할 수 있습니다.

1. 다음 중 하나를 수행합니다.

   * 목록에서 구성원을 선택한 다음 편집 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 해당 사용자의 사용자 프로필을 수정합니다.

     자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 또는 [사용자 프로필 일괄 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)을 참조하십시오.

   * 목록에서 원하는 수의 구성원을 선택한 다음 ![댓글 아이콘 업데이트](assets/comment-icon.png)를 클릭하여 사용자 프로필에 댓글을 추가합니다.

     사용자 또는 사용자는 댓글이 포함된 이메일 알림과 인앱 알림을 받습니다. 댓글은 사용자 프로필의 업데이트 영역에 표시됩니다.

   * 목록에서 원하는 수의 구성원을 선택한 다음 ![사용자 비활성화](assets/deactivate-user.png) 또는 ![사용자 활성화](assets/activate-user.png) 활성화를 클릭합니다.

     자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하십시오.

   * 구성원 목록을 ![내보내기](assets/export.png)합니다.
