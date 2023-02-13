---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 작업표 수동으로 생성
description: 작업표 프로필에 적용된 변경 사항을 현재 작업표에 반영하려면 먼저 기존 작업표를 삭제한 다음 새 작업표를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 작업표 영역 또는 설정의 진단 영역에서 작업표를 수동으로 생성할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 작업표 수동으로 생성

작업표 프로필에 적용된 변경 사항을 현재 작업표에 반영하려면 먼저 기존 작업표를 삭제한 다음 새 작업표를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 작업표 영역 또는 설정의 진단 영역에서 작업표를 수동으로 생성할 수 있습니다.

작업표 삭제에 대한 지침은 [Adobe Workfront에서 작업표 삭제](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자이거나 그룹의 작업표 프로필에 대해 작업하는 경우 그룹 관리자(또는 Workfront 관리자)여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a>.</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 수동으로 생성된 작업표에 대한 고려 사항

작업표를 수동으로 생성하는 경우:

* 사용자와 연결된 작업표 프로필에 따라 생성됩니다. 작업표 프로필이 연결되어 있지 않은 사용자는 작업표를 받지 않습니다. 
* 현재 작업표와 팔로우할 작업표만 생성됩니다. Workfront에서 같은 기간 동안 작업표를 두 개 생성하지 않습니다. 특정 기간에 대한 작업표가 이미 있는 경우 수동 프로세스를 사용하여 작업표를 생성할 때 다른 작업표가 생성되지 않습니다.

## 작업표 및 시간 영역에서 작업표를 수동으로 생성합니다

Setup의 작업표 및 시간 영역에서 시스템 레벨 또는 그룹 레벨 작업표를 수동으로 생성할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 시스템 전체에서 사용 중인 작업표를 생성하는 경우 **작업표 및 시간**

   또는

   특정 그룹에서 사용하는 작업표를 생성하는 경우 **그룹**&#x200B;를 클릭한 다음 그룹 이름을 클릭합니다.

1. 클릭 **작업표 프로필**.
1. 클릭 **자세히**, 그런 다음 **작업표 생성**.

   작업표 프로필과 관련된 사용자의 경우 최대 두 기간 동안 새 작업표를 만듭니다.

## 진단 영역에서 시스템 수준 작업표를 수동으로 생성합니다.

설치 프로그램의 진단 영역에서 시스템 수준 작업표를 수동으로 생성할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 확장 **시스템**&#x200B;를 클릭한 다음 **진단**.

1. 클릭 **진단 수행**. 
1. 클릭 **작업표 생성**.
