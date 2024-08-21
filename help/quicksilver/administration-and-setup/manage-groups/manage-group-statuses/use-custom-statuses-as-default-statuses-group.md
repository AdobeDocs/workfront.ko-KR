---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 사용자 지정 상태를 그룹의 기본 상태로 사용
description: 그룹 관리자는 사용자 지정 상태를 관리하는 그룹 또는 하위 그룹의 기본 상태로 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# 사용자 지정 상태를 그룹의 기본 상태로 사용

그룹 관리자는 사용자 지정 상태를 관리하는 그룹 또는 하위 그룹의 기본 상태로 구성할 수 있습니다. 이 기능은 시스템이 프로젝트, 작업 또는 문제에 Workfront 상태를 자동으로 할당해야 할 때 유용합니다. 프로젝트, 작업 또는 문제는 항상 해당하는 Workfront 상태를 표시하는 대신 기본 상태로 설정한 사용자 지정 상태를 표시합니다.

구성하는 상태는 그룹에 대해 만들어지거나, 그룹 위의 그룹에서 상속되거나, 시스템 수준에서 상속되는 모든 사용자 지정 상태일 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

>[!INFO]
>
>**예:** 완료 라는 사용자 지정 상태를 만들고 이를 Workfront 완료 상태와 동등한 기본 상태로 설정할 수 있습니다.
>
>그런 다음 100%에 도달하면 완료 상태로 변경되도록 설정된 작업의 경우 상태가 완료 대신 완료됨으로 표시됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

+++

## 문제 상태

사용자 지정 상태가 문제 상태인 경우 네 가지 문제 유형(버그 보고서, 순서 변경, 문제 및 요청)을 모두 활성화해야 합니다. 예를 들어 아래에 표시된 문제 상태에서 주문 변경 문제 유형이 선택되지 않았으므로 다시 열림 상태를 기본 상태로 사용할 수 없습니다.

![](assets/all-4-issue-types-enabled.png)

## 사용자 지정 상태를 그룹의 기본 상태로 설정

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭한 다음 상태를 만들거나 사용자 지정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **상태** ![](assets/gear-icon-settings.png)를 클릭합니다.
1. 기본 상태로 설정할 상태 유형에 따라 **프로젝트**, **작업** 또는 **문제** 탭을 엽니다.
1. 오른쪽 상단 근처에 있는 **기본 상태 설정**&#x200B;을 클릭합니다.
1. 표시되는 드롭다운 영역에서 기본 상태를 설정할 상태 옆에 설정할 기본 상태를 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

   이제 상태를 그룹과 연결된 프로젝트에 사용할 기본 상태로 사용할 수 있습니다.

1. 사용자 정의 상태를 사용하려는 프로젝트와 연결합니다.

   상태가 있는 그룹을 프로젝트와 연관시켜 상태와 프로젝트를 연관시킵니다. 상태가 있는 그룹이 프로젝트와 연결되어 있는 경우에만 사용자 정의 상태를 사용할 수 있습니다.

   >[!NOTE]
   >
   >프로젝트를 다른 그룹에 할당하면 프로젝트 상태가 다시 로드되고 변경될 수 있습니다.

   1. 사용자 지정 상태를 사용할 프로젝트로 이동합니다.
   1. 기타 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **편집**&#x200B;을 클릭합니다.
   1. **프로젝트 연결** 아래의 **그룹** 필드에 표시되는 **프로젝트 편집** 상자에서 사용자 지정 상태와 연결된 그룹을 선택합니다.

   1. **변경 내용 저장**&#x200B;을 클릭합니다.

## 그룹은 기본 상태 구성 상속

Workfront 관리자가 사용자 지정 상태를 기본 상태로 구성한 후 새로 만든 그룹은 해당 구성을 상속합니다.

마찬가지로 그룹 관리자가 사용자 지정 상태를 기본 상태로 설정한 후에는 그룹 바로 아래에 만들어진 새 하위 그룹이 해당 구성을 상속합니다.

자세한 내용은 [그룹이 상태를 상속하는 방법](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md)을 참조하세요.

## 기본 상태가 숨겨져 있는 경우

기본 상태를 숨기면(해당 상태 숨기기 옵션을 활성화하여), 시스템에서 동등 유형의 다른 상태를 기본값으로 설정하려고 시도합니다.

해당 형식의 사용 가능한 상태가 없으면 상태 형식은 **숨김**&#x200B;으로 표시되며 작업 항목에 사용할 수 없습니다.

![](assets/when-hide-default-status-no-equivalent.png)
