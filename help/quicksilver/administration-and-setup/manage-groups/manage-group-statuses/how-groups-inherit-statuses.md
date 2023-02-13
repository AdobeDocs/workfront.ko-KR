---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 그룹이 상태를 상속하는 방법
description: 그룹에 사용할 수 있는 상태를 나열하면 다음을 볼 수 있습니다
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 그룹이 상태를 상속하는 방법

그룹에 사용할 수 있는 상태를 나열하면 다음을 볼 수 있습니다

* 그룹에 대해 생성된 사용자 지정 상태(예: [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 이 문서에서 설명한 대로 시스템에서 상속되고 그룹 계층 구조의 상위에서 상속된 상태입니다.

## 상태 상속

다음 상황이 발생하면 그룹은 상태를 상속합니다.

* 그룹을 만듭니다.
* 관리자는 상위 수준 그룹에서 상태를 잠급니다.
* 관리자는 다른 그룹을 삭제하고 해당 그룹을 선택할 수 있습니다.

아래 표는 이러한 각 상황을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">그룹을 만들 때</td> 
   <td> <p>새 그룹을 만들면 자동으로 상속됩니다.</p> 
    <ul> 
     <li>새 그룹이 하위 그룹인 경우 그룹의 잠금 해제된 상태가 한 수준 위로 표시됩니다.</li> 
    </ul> 
    <ul> 
     <li>시스템 수준에서 잠긴 상태입니다.</li> 
    </ul> 
     <b>예:</b></span></span> 
     <p>마케팅 이라는 그룹에 마케팅 커뮤니케이션 및 브랜딩이라는 두 개의 하위 그룹이 있다고 가정합니다.</p> 
     <p>마케팅 그룹의 그룹 관리자는 Discovery라는 새로운 사용자 지정 상태를 만듭니다.</p> 
     <p>나중에 마케팅 그룹 아래에 새 하위 그룹을 만들고 광고 라고 합니다.</p> 
     <p>다른 관리자가 잠금 해제된 검색 상태를 만든 후 그룹을 만들었으므로 하위 그룹은 검색 상태를 상속합니다.</p> 
     <p>이 경우 하위 그룹 마케팅 커뮤니케이션 및 브랜딩이 마케팅 그룹 아래에 이미 존재했으므로 잠금 해제된 검색 상태를 상속하지 않습니다.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">관리자가 높은 수준에서 상태를 잠그는 경우</td> 
   <td> <p>Workfront 관리자가 시스템 수준에서 상태를 잠그면 그룹은 시스템의 다른 모든 그룹과 함께 해당 상태를 상속합니다.</p> <p>마찬가지로, 관리자가 그룹 위에 있는 그룹의 상태를 잠글 때 해당 그룹은 상위 그룹 아래에 있는 다른 하위 그룹과 함께 이를 상속합니다.</p> <p><b>참고</b>: 나중에 관리자가 시스템 수준 또는 그룹 위의 그룹에서 이러한 상태 중 하나를 잠금 해제하면 그룹은 이전에 상속한 상태를 유지합니다. 이제 별도의 버전의 상태이며 해당 그룹에 대해서만 사용자 지정할 수 있습니다.</p> 
    <p><b>예:</b></p>
    <p>마케팅 그룹 관리자는 위에 언급된 검색 상태를 잠근 후 3개의 하위 그룹 모두 이 검색 상태를 확인합니다.</p> 
    <p>광고 그룹과 함께, 마케팅 커뮤니케이션 및 브랜딩 그룹은 이제 검색 상태를 갖습니다. 위의 마케팅 그룹에 잠겼을 때 상속되었습니다.</p> 
    <p>그런 다음 마케팅 그룹 관리자가 검색 상태를 잠금 해제하여 세 하위 그룹 모두 검색 상태의 자체 버전을 갖도록 합니다. 이제 사용자와 다른 두 그룹의 관리자는 그룹의 요구 사항에 맞게 검색 상태를 사용자 지정할 수 있습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">관리자가 그룹을 삭제하는 경우</td> 
   <td> <p>관리자가 그룹을 삭제하고 사용자 그룹을 시스템에서 해당 위치로 선택하면 삭제된 그룹의 사용자 지정 상태가 그룹에 아직 없는 경우 해당 그룹은 해당 그룹을 상속합니다.</p> 
   <p><b>예: </b></p>
     <p>Messaging이라는 그룹은 광고 그룹과 병합해야 하므로 Workfront 관리자가 메시징 그룹을 삭제하고 해당 그룹을 대체할 그룹을 선택합니다.</p> 
     <p>메시징 그룹의 고유한 상태는 In Process입니다. 이제 광고 그룹에 해당 상태를 사용할 수 있습니다.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 상태 구성 상속

최상위 그룹을 만들면 시스템 수준에서 다음 구성을 상속합니다. 하위 그룹을 만들면 다음 상위 그룹에서 다음 구성을 상속합니다.

* 기본 상태 구성

   자세한 내용은 [사용자 지정 상태를 기본 상태로 사용](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* 상태 표시 주문 구성

   자세한 내용은 [시스템 수준 및 그룹 상태 순서 조정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

그룹을 만든 후 다른 사용자가 이러한 구성을 변경할 경우 해당 상태는 영향을 받지 않습니다.
