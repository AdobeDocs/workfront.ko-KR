---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 이동 또는 삭제된 그룹의 사용자 지정 상태
description: 이 문서에서는 그룹을 이동하거나 삭제할 때 사용자 지정 상태를 그룹화하는 방법에 대해 설명합니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# 이동 또는 삭제된 그룹의 사용자 지정 상태

이 문서에서는 그룹을 이동하거나 삭제할 때 사용자 지정 상태를 그룹화하는 방법에 대해 설명합니다.

## 이동되는 그룹의 사용자 지정된 상태

한 그룹을 다른 그룹 아래의 새 위치로 이동할 때 사용자 지정 상태를 그룹화하는 상황을 설명하는 다음 시나리오를 고려하십시오.

그룹 이동에 대한 자세한 내용은 [그룹 이동](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">다른 그룹 아래로 그룹을 이동할 때 </td> 
   <td> <p>이동된 그룹의 모든 상태는 계속 유지됩니다. 그룹의 새 상위 그룹 상태에 추가되지 않습니다.</p> <p>하지만 이동된 그룹은 그룹 또는 그룹의 잠긴 상태를 상속합니다. 그룹 또는 그룹은 이제 그룹 계층에서 더 높은 상태를 갖습니다. 그리고 지금부터 관리자가 계층 구조에서 더 높은 상태를 잠그는 경우 이동된 그룹은 해당 상태를 상속합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">두 그룹의 상태에 키가 같지만 특성이 다른 경우</td> 
   <td> <p>두 개의 다른 하위 그룹이 상위 그룹에서 잠금 해제된 동일한 상태를 상속한다고 가정합니다. 그런 다음 두 그룹의 그룹 관리자는 다양한 방법으로 그룹의 상태를 사용자 지정합니다.</p> <p>나중에 두 그룹 중 하나가 다른 그룹 아래로 이동됩니다. 이제 둘 다 키가 같은 상태이지만, 두 그룹의 특성이 다릅니다.</p> <p>이 경우 다음 중 하나가 true입니다.</p> 
    <ul> 
     <li>새 상위 그룹의 상태 잠금이 해제되면 이동된 그룹의 상태는 이동의 영향을 받지 않고 속성을 유지합니다.</li> 
     <li>새 상위 그룹의 상태가 잠긴 경우 상위 그룹의 상태 속성은 이동된 그룹의 상태를 덮어씁니다.</li> 
    </ul> <p>상태 키에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>이동된 그룹의 상태가 이전 상위 그룹에서 상속된 경우 </td> 
   <td> <p>이전 상위 그룹에서 상속된 모든 사용자 지정 상태는 이동된 그룹과 함께 제공되며 자신의 사용자 지정 상태가 됩니다. 더 이상 이전 상위 그룹과 연결되지 않습니다.</p> 
    <ul> 
     <li>이전 상위 그룹이 이동 후 잠긴 사용자 정의 상태를 편집하면 변경 사항이 이동된 하위 그룹의 상태에 영향을 주지 않습니다.</li> 
     <li>이전 상위 그룹이 그룹을 이동할 때 잠금이 해제된 사용자 지정 상태를 잠그는 경우 이동된 하위 그룹의 상태는 잠기지 않습니다.</li> 
     <li>이동된 그룹은 이제 이전 상위 그룹에서 상속되었을 때 잠긴 상태의 잠금을 해제할 수 있습니다.</li> 
    </ul> 
     <p><b>예:</b><p> 
     <p>마케팅 그룹의 그룹 관리자인 올리비아는 그룹에 대해 두 개의 상태를 만듭니다. 그녀는 키 ABC와 함께 하나의 First Review의 이름을 지정하고 잠급니다. 이 설명서는 키 XYZ를 사용하여 다른 최종 리뷰의 이름을 지정하고 이 리뷰를 잠기지 않습니다.</p> 
     <p>또한 제품 마케팅이라는 마케팅 그룹 아래에 하위 그룹을 만듭니다. 만들어진 즉시 마케팅 그룹의 첫 번째 검토와 최종 검토를 모두 자동으로 상속합니다.</p> 
     <p>나중에 Olivia가 제품 그룹 아래에 제품 마케팅 하위 그룹을 이동합니다. 첫 번째 검토와 최종 검토 모두 제품 마케팅 그룹과 함께 제품 그룹 아래에 있는 새 위치로 이동합니다.</p> 
     <p>이동 전에 첫 번째 검토가 잠겼지만, 제품 마케팅 그룹 관리자는 이제 해당 검토가 상위 그룹에서 제어하는 상속된 상태가 아니므로 편집할 수 있습니다.</p> 
     <p>Final Review는 잠금 해제되어 있으며 항상 그래왔던 대로 편집할 수 있습니다.</p> 
     <p>마케팅 그룹의 경우, Olivia는 첫 번째 검토 및 최종 검토의 색상을 변경하고 첫 번째 검토-편집됨 및 마지막 검토-편집됨 이름을 변경합니다. 그녀는 최종 리뷰-편집도 잠금한다. 한편 제품 마케팅 그룹에서 첫 번째 검토 및 최종 검토 상태의 색상 및 이름은 변경되지 않습니다.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 삭제된 그룹에서 사용자 지정된 상태

그룹이나 하위 그룹을 삭제하면 해당 사용자 지정된 상태를 포함하여 연관된 정보를 다른 그룹이나 하위 그룹에 재할당합니다. 삭제된 그룹의 상태가 대상 그룹의 상태에 추가됩니다.

삭제된 그룹의 상태 중 하나를 대상 그룹에서도 사용하고 있고(두 그룹의 상태는 키가 동일함) 대상 그룹이 다른 방식으로 상태를 사용자 지정한 경우 대상 그룹의 버전 설정은 이동된 그룹 버전의 설정을 덮어씁니다.

>[!INFO]
>
>**예:**
>
>그룹 A의 그룹 관리자는 그룹의 잠금 해제된 시스템 수준 상태를 변경합니다. 그룹 B의 그룹 관리자도 그룹 이름을 변경합니다. 상태는 두 그룹에서 다른 이름을 가지지만 키가 동일합니다.
>
>나중에 그룹 A가 삭제되고 모든 정보가 그룹 B에 재할당됩니다.
>
>* 상태 그룹 B 버전의 이름은 그룹 A 버전의 이름을 무시합니다.
>* 해당 그룹이 삭제되기 전에 그룹 A의 어떤 사람이 객체에 상태를 적용한 경우 객체의 상태 이름이 그룹 B에서 사용하는 상태의 이름으로 업데이트됩니다.
>
>상태 키에 대한 자세한 내용은 다음 문서의 표를 참조하십시오. [사용자 지정 상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [그룹의 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>그룹 삭제에 대한 자세한 내용은 [그룹 삭제](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
