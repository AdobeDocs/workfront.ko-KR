---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 수동으로 타임시트 생성
description: 타임시트 프로필에 적용한 변경 내용이 현재 타임시트에 반영되도록 하려면 먼저 기존 타임시트를 삭제한 다음 새 타임시트를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 설정의 타임시트 영역 또는 진단 영역에서 타임시트를 수동으로 생성할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# 수동으로 타임시트 생성

타임시트 프로필에 적용한 변경 내용이 현재 타임시트에 반영되도록 하려면 먼저 기존 타임시트를 삭제한 다음 새 타임시트를 수동으로 생성해야 합니다. 이 문서에 설명된 대로 설정의 타임시트 영역 또는 진단 영역에서 타임시트를 수동으로 생성할 수 있습니다.

타임시트 삭제에 대한 지침은 [Adobe Workfront에서 타임시트 삭제](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)를 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자이거나 그룹에 대한 타임시트 프로필 작업을 하는 경우 그룹 관리자(또는 Workfront 관리자)여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a>를 참조하세요.</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

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
1. **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png), **타임시트 생성**&#x200B;을 클릭합니다.

   새 타임시트는 타임시트 프로필과 연결된 사용자의 경우 최대 2개 기간 동안 만들어집니다.

## 진단 영역에서 시스템 수준 타임시트를 수동으로 생성

설정의 진단 영역에서 시스템 수준 타임시트를 수동으로 생성할 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **시스템**&#x200B;을 확장한 다음 **진단**&#x200B;을 클릭합니다.

1. **진단 수행**&#x200B;을 클릭합니다. 
1. **타임시트 생성**&#x200B;을 클릭합니다.
