---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 그룹이 상태를 상속하는 방법
description: 그룹에 사용할 수 있는 상태를 나열하면 다음과 같이 표시됩니다
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 그룹이 상태를 상속하는 방법

그룹에 사용할 수 있는 상태를 나열하면 다음과 같이 표시됩니다

* [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)에 설명된 대로 그룹에 대해 만들어진 사용자 지정 상태입니다.
* 이 문서에 설명된 대로 시스템 및 그룹 계층 구조에서 상위에서 상속된 상태.

## 상태 상속

그룹은 다음과 같은 일이 발생할 때 상태를 상속합니다.

* 그룹을 만듭니다.
* 관리자는 상위 수준 그룹의 상태를 잠급니다.
* 관리자가 다른 그룹을 삭제하고 해당 그룹을 선택하여 대체할 수 있습니다.

아래 표는 이러한 각 상황을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">그룹을 만들 때</td> 
   <td> <p>새 그룹을 만들 때 자동으로 상속됩니다.</p> 
    <ul> 
     <li>새 그룹이 하위 그룹인 경우 그룹 내 잠금 해제된 상태 한 레벨 위로</li> 
    </ul> 
    <ul> 
     <li>시스템 수준에서 잠긴 상태.</li> 
    </ul> 
     <b>예:</b></span></span> 
     <p>Marketing 이라는 그룹에 Marketing Communications and Branding 이라는 두 개의 하위 그룹이 있다고 가정해 봅시다.</p> 
     <p>마케팅 그룹의 그룹 관리자는 검색이라는 새 사용자 지정 상태를 만듭니다.</p> 
     <p>나중에 마케팅 그룹 아래에 새 하위 그룹을 만들고 이를 Advertising라고 합니다.</p> 
     <p>다른 관리자가 잠금 해제된 검색 상태를 만든 후에 그룹을 만들었으므로 하위 그룹이 검색 상태를 상속합니다.</p> 
     <p>이러한 경우 하위 그룹 마케팅 커뮤니케이션 및 브랜딩이 마케팅 그룹 아래에 이미 존재했으므로 이 하위 그룹은 잠금 해제된 검색 상태를 상속하지 않습니다.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">관리자가 상위 수준에서 상태를 잠그는 경우</td> 
   <td> <p>Workfront 관리자가 시스템 수준에서 상태를 잠그면 그룹이 시스템의 다른 모든 그룹과 함께 상태를 상속합니다.</p> <p>마찬가지로 관리자가 그룹 위의 그룹에 대한 상태를 잠그면 그룹은 상위 그룹 아래의 다른 하위 그룹과 함께 상속됩니다.</p> <p><b>참고</b>: 나중에 관리자가 시스템 수준이나 그룹 위의 그룹에서 이러한 상태 중 하나를 잠금 해제하면 그룹이 이전에 상속된 상태를 유지합니다. 이제 별도의 상태 버전이며 그룹에 대해서만 사용자 지정할 수 있습니다.</p> 
    <p><b>예:</b></p>
    <p>마케팅 그룹 관리자는 위에 언급된 검색 상태를 잠가서 3개의 하위 그룹 모두가 검색되었는지 확인합니다.</p> 
    <p>이제 Advertising 그룹과 함께 마케팅 커뮤니케이션 및 브랜딩 그룹이 검색 상태를 갖습니다. 상위 마케팅 그룹에서 잠겼을 때 상속되었습니다.</p> 
    <p>그런 다음 마케팅 그룹 관리자는 3개의 모든 하위 그룹이 자체 버전의 검색 상태를 갖도록 검색 상태 잠금을 해제합니다. 이제 사용자와 다른 두 그룹의 관리자는 그룹의 요구 사항에 맞게 검색 상태를 사용자 정의할 수 있습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">관리자가 그룹을 삭제하는 경우</td> 
   <td> <p>관리자가 그룹을 삭제하고 시스템 내에서 처리하기로 선택하면 그룹에 삭제된 그룹의 사용자 지정 상태가 존재하지 않는 경우 해당 그룹이 해당 상태를 상속합니다.</p> 
   <p><b>예: </b></p>
     <p>메시징이라는 그룹은 Advertising 그룹과 병합해야 하므로 Workfront 관리자는 메시징 그룹을 삭제하고 그룹을 선택하여 해당 그룹을 대체합니다.</p> 
     <p>메시징 그룹에 처리 중이라는 고유한 상태가 있습니다. 이제 Advertising 그룹에서 해당 상태를 사용할 수 있습니다.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 상태 구성 상속

최상위 그룹을 만들면 시스템 수준에서 다음 구성을 상속합니다. 하위 그룹을 만들면 그 다음 상위 그룹에서 다음 구성을 상속합니다.

* 기본 상태 구성

  이에 대한 자세한 내용은 [사용자 지정 상태를 기본 상태로 사용](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md)을 참조하세요.

* 상태 표시 순서 구성

  자세한 내용은 [시스템 수준 및 그룹 상태 순서 바꾸기](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md)를 참조하십시오.

그룹을 만든 후 누군가가 이러한 구성을 변경할 경우 해당 상태는 영향을 받지 않습니다.
