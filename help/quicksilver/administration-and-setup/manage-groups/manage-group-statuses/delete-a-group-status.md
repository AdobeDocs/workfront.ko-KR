---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 그룹 상태 삭제
description: 그룹 관리자는 관리한 그룹의 상태를 시스템 수준에서 필수 또는 잠긴 상태로 구성되지 않았거나 계층의 상위 그룹에 대해 삭제할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 그룹 상태 삭제

그룹 관리자는 관리한 그룹의 상태를 시스템 수준에서 필수 또는 잠긴 상태로 구성되지 않았거나 계층의 상위 그룹에 대해 삭제할 수 있습니다.

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

>[!NOTE]
>
>다음을 삭제할 수 없습니다.
>
>* 기본 제공 상태 계획, 현재 및 완료. 이름을 업데이트하고, 색상을 편집하고, 잠그거나 잠금을 해제할 수 있지만 삭제할 수는 없습니다.
>* 그룹 또는 해당 하위 그룹 중 하나와 연관된 하나 이상의 객체에 대해 승인 보류 중인 상태입니다.

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
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 상태 삭제

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.
1. 최상위 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **상태**&#x200B;를 클릭합니다.
1. 표시되는 상태 목록에서 삭제할 상태를 마우스로 가리킨 다음 맨 오른쪽에 나타나면 **삭제**&#x200B;를 클릭합니다.

   ![삭제](assets/hover-click-delete.jpg)

1. 표시되는 상자에서 삭제하려는 상태를 사용하고 있던 객체(프로젝트, 작업, 문제 및 승인 프로세스)에 대한 대체 상태를 지정할 상태를 선택합니다.

   삭제하려는 상태와 동일한 상태만 사용할 수 있습니다. 예를 들어 현재 와 동일한 상태를 삭제하는 경우 현재 와 동일한 상태만 표시됩니다.

   또한 삭제하려는 상태가 잠금 해제되었는지 또는 잠겼는지에 따라 표시되는 상태가 달라집니다.

   * **잠금 해제된 경우**: 숨기지 않은 잠금 및 잠금 해제된 상태를 사용할 수 있습니다.

     하위 그룹에 대해 생성된 상태와 함께 시스템 레벨 및 상위 레벨 그룹에서 상속된 상태가 포함됩니다.

   * **잠겨 있는 경우**: 다음 중 하나가 true입니다.

      * 다른 잠기고 숨겨지지 않은 상태가 있는 경우 해당 상태만 사용할 수 있습니다.
      * 숨김이 아닌 잠김 상태가 없는 경우 기본 Workfront 상태가 숨겨져 있거나 잠금 해제된 경우에도 사용할 수 있습니다.

        기본 Workfront 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 목록 액세스](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [시스템 작업 상태 목록 액세스](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) 및 [시스템 문제 상태 목록 액세스](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)의 4가지 필수 문제 상태에 대한 정보를 참조하십시오.

1. **상태 삭제**&#x200B;를 클릭합니다.

   삭제된 상태가 그룹의 해당 유형에 대한 기본 상태인 경우 교체 상태가 적용됩니다.

   프로젝트 환경 설정에서 삭제된 상태가 기본 프로젝트 상태로 설정된 경우 환경 설정이 이제 교체 상태로 설정됩니다.

## 그룹 삭제 시

그룹을 삭제하고 다른 그룹으로 대체하면 삭제된 그룹에 있던 고유한 상태가 대체 그룹의 상태에 추가됩니다. 자세한 내용은 이동 또는 삭제된 그룹의 [사용자 지정 상태](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md)를 참조하십시오.
