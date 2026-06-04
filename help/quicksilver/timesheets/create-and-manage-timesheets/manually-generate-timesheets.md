---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 수동으로 타임시트 생성
description: 타임시트 프로필에 적용한 변경 내용이 현재 타임시트에 반영되도록 하려면 먼저 기존 타임시트를 삭제한 다음 새 타임시트를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 설정의 타임시트 영역 또는 진단 영역에서 타임시트를 수동으로 생성할 수 있습니다.
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
TQID: https://experienceleague.adobe.com/0hU3VlHM8l5TXee6K3lJaV9-W3ZKujDYf9-f1NXH-Nc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 4%

---

# 수동으로 타임시트 생성

타임시트 프로필에 적용한 변경 내용이 현재 타임시트에 반영되도록 하려면 먼저 기존 타임시트를 삭제한 다음 새 타임시트를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 설정의 타임시트 영역 또는 진단 영역에서 타임시트를 수동으로 생성할 수 있습니다.

타임시트 삭제에 대한 지침은 [Adobe Workfront에서 타임시트 삭제](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>Workfront 관리자이거나 그룹에 대한 타임시트 프로필 작업을 하는 경우 그룹 관리자(또는 Workfront 관리자)여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 수동으로 생성된 타임시트에 대한 고려 사항

타임시트를 수동으로 생성하는 경우:

* 사용자와 연결된 타임시트 프로필에 따라 생성됩니다. 타임시트 프로필이 연결되어 있지 않은 사용자는 타임시트를 받지 못합니다.
* 현재 타임시트와 팔로우할 타임시트만 생성됩니다. Workfront은 동일한 기간에 두 개의 타임시트를 생성하지 않습니다. 현재 일정에 대한 타임시트가 이미 있는 경우, 수동 프로세스를 사용하여 타임시트를 생성하는 경우 다른 타임시트가 생성되지 않습니다.

## 타임시트 및 시간 영역에서 수동으로 타임시트 생성

설정의 타임시트 및 시간 영역에서 시스템 수준 또는 그룹 수준 타임시트를 수동으로 생성할 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 시스템 전체에서 사용 중인 타임시트를 생성하는 경우 **타임시트 및 시간을 클릭합니다.**

   또는

   특정 그룹에서 사용하는 타임시트를 생성하는 경우 **그룹**&#x200B;을 클릭한 다음 그룹 이름을 클릭합니다.

1. **타임시트 프로필**&#x200B;을 클릭합니다.
1. 기타 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **타임시트 생성**&#x200B;을 클릭합니다.

1. 타임시트 프로필 목록의 맨 위에서 시스템 수준 타임시트 프로필의 경우 **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png), 그룹 타임시트 프로필의 경우 **자세히**&#x200B;를 클릭한 다음 **타임시트 생성**&#x200B;을 클릭합니다.

   새 타임시트는 타임시트 프로필과 연결된 사용자의 경우 최대 2개 기간 동안 만들어집니다.

## 진단 영역에서 시스템 수준 타임시트를 수동으로 생성

설정의 진단 영역에서 시스템 수준 타임시트를 수동으로 생성할 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **시스템**&#x200B;을 확장한 다음 **진단**&#x200B;을 클릭합니다.

1. **진단 수행**&#x200B;을 클릭합니다.
1. **타임시트 생성**&#x200B;을 클릭합니다.
