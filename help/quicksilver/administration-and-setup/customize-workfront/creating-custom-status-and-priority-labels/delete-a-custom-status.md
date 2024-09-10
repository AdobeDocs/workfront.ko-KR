---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 사용자 지정 상태 삭제
description: 사용자 정의 시스템 상태가 더 이상 조직에 유용하지 않은 경우 삭제할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---

# 사용자 지정 상태 삭제

사용자 정의 시스템 상태가 더 이상 조직에 유용하지 않은 경우 삭제할 수 있습니다.

상태가 잠겨 있는지 또는 잠금 해제되었는지 여부에 따라 시스템의 모든 그룹에 대해 상태가 삭제되는지 여부가 결정됩니다.

* 현재 잠긴 시스템 상태를 삭제하면 그룹의 이름이 변경되었는지 여부에 관계없이 시스템의 모든 그룹에 대해 상태가 제거됩니다.
* 반대로 현재 잠금 해제된 시스템 상태를 삭제하면 시스템의 모든 그룹에 대해 상태가 유지됩니다.


>[!NOTE]
>
>다음을 삭제할 수 없습니다.
>
>* 시스템에 있는 하나 이상의 객체에 대해 현재 승인 보류 중인 시스템 승인 프로세스에 사용되는 잠금 또는 잠금 해제된 시스템 상태입니다.
>
>  그러나 현재 승인 보류 중인 일회용 또는 그룹 수준 승인 프로세스에 사용되는 잠금 해제된 시스템 상태를 삭제할 수 있습니다.
>
>  보고서를 실행하여 개체를 찾고 보류 중인 승인을 해결한 다음 상태를 다시 삭제할 수 있습니다. 지침은 [특정 상태를 사용하여 승인 보류 중인 개체 나열](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md)을 참조하세요.
>
>* 시스템에서 하나 이상의 객체에 대해 현재 승인 보류 중인 승인 프로세스에 사용되는 상태.

그룹 상태 삭제에 대한 지침은 [그룹 상태 삭제](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md)를 참조하세요.

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
     <p>새로운 기능: 표준</p>
     <p>또는</p>
     <p>현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 시스템 상태 삭제

{{step-1-to-setup}}

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **상태**&#x200B;를 클릭합니다.

1. 전체 시스템(개별 그룹의 경우 포함)에서 상태를 삭제하려면 상태를 마우스로 가리킨 다음 **편집**&#x200B;을 클릭한 다음 **모든 그룹의 경우 잠금**&#x200B;을 선택하십시오. **저장**&#x200B;을 클릭합니다.

   또는

   시스템 상태를 삭제하지만 개별 그룹에 대해 유지하려면 상태를 마우스로 가리키고 **편집**&#x200B;을 클릭한 다음 **모든 그룹에 대해 잠금**&#x200B;을 선택하지 않았는지 확인하십시오. **저장**&#x200B;을 클릭합니다.

1. 삭제할 상태를 마우스로 가리킨 다음 **삭제**&#x200B;를 클릭합니다.
1. 표시되는 메시지에서 **상태 삭제**&#x200B;를 클릭합니다.
1. 표시되는 **상태 삭제** 상자에서 **현재 이 상태의 모든 프로젝트를 다음으로 설정**&#x200B;이라는 필드의 상태를 선택합니다.

   삭제 중인 상태를 사용 중인 프로젝트가 선택한 상태로 설정됩니다.

   삭제 중인 상태와 동일한 상태와 동일한 경우에만 드롭다운 목록에서 상태를 사용할 수 있습니다.

   예를 들어, 현재 상태와 같은 상태를 삭제하는 경우 현재 상태와 같은 상태만 선택할 수 있습니다.

1. **상태 삭제**&#x200B;를 클릭합니다.
