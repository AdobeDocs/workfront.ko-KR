---
title: 작업 역할에 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 통해 Workfront에서 작업 역할에 대한 사용자의 액세스 권한을 정의할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a5ba79da-37f3-43f8-a7e2-4ccd75b56fef
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 5%

---

# 작업 역할에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 사용자의 액세스 수준을 통해 작업 역할에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

작업 역할에 대한 자세한 내용은 [작업 역할 만들기 및 관리](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 액세스 수준을 사용하여 작업 역할 편집에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 작업 역할 오른쪽의 ![](assets/gear-icon-settings.png)보기&#x200B;**또는**&#x200B;편집&#x200B;**단추에서 톱니바퀴 아이콘**&#x200B;을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   >[!NOTE]
   >
   >**보기**&#x200B;는 작업 역할의 기본 액세스입니다.

   ![작업 역할 액세스 미세 조정](assets/job-role-access-view-fine-tune.png)

   **보기** 액세스 권한이 있는 사용자는 기존 작업 역할을 보고 선택적으로 다음을 수행할 수 있습니다.

   * 작업 역할에 대한 청구 요금 보기
   * 작업 역할에 대한 원가율 보기
   * 작업 역할의 일반 재무 필드 보기(청구 또는 비용 요금과 관련이 없음)

   **편집** 액세스 권한이 있는 사용자는 기존 작업 역할을 보고 편집할 수 있으며 선택적으로 다음을 수행할 수 있습니다.

   * 새 작업 역할 만들기
   * 작업 역할 삭제
   * 작업 역할의 청구 요금 편집
   * 작업 역할의 비용 비율 편집
   * 작업 역할의 일반 재무 필드 편집(청구 또는 비용 요금과 관련이 없음)
   * 작업 역할 청구 요금, 비용 요금 및 일반 재무 필드 보기

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나(예: [작업에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md))를 계속 사용하십시오.
1. 완료되면 **저장**&#x200B;을 클릭하세요.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

## 라이선스 유형별 작업 역할에 액세스

각 액세스 수준의 사용자가 작업 역할로 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#job-roles)의 [작업 역할](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md) 섹션을 참조하십시오.
