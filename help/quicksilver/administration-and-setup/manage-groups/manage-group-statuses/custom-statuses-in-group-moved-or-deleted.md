---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 이동 또는 삭제된 그룹의 사용자 지정 상태
description: 이 문서에서는 그룹을 이동하거나 삭제할 때 그룹 사용자 정의 상태가 어떻게 되는지에 대해 설명합니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# 이동 또는 삭제된 그룹의 사용자 지정 상태

이 문서에서는 그룹을 이동하거나 삭제할 때 그룹 사용자 정의 상태가 어떻게 되는지에 대해 설명합니다.

## 이동된 그룹에서 사용자 지정된 상태

한 그룹을 다른 그룹 아래의 새 위치로 이동할 때 그룹 사용자 정의 상태가 어떻게 되는지를 설명하는 다음 시나리오를 고려하십시오.

그룹 이동에 대한 자세한 내용은 [그룹 이동](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)을 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">그룹을 다른 그룹으로 이동할 때 </td> 
   <td> <p>이동된 그룹의 모든 상태가 그대로 유지됩니다. 그룹의 새 상위 그룹 상태에 추가되지 않습니다.</p> <p>그러나 이동된 그룹은 이제 계층 구조에서 더 높은 위치에 있는 그룹의 잠긴 상태를 상속합니다. 또한 이제부터 관리자가 계층 구조에서 상위 상태를 잠그면 이동된 그룹이 해당 상태를 상속합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">두 그룹의 상태에 동일한 키가 있지만 속성이 다른 경우</td> 
   <td> <p>두 개의 서로 다른 하위 그룹이 상위 그룹에서 동일한 잠금 해제 상태를 상속한다고 가정해 봅시다. 그런 다음 두 그룹의 그룹 관리자는 다른 방식으로 그룹의 상태를 사용자 정의합니다.</p> <p>나중에 두 그룹 중 하나가 다른 그룹 아래로 이동됩니다. 이제 둘 다 동일한 키를 가진 상태를 갖지만 두 그룹에서 속성이 다릅니다.</p> <p>이 경우 다음 중 하나가 적용됩니다.</p> 
    <ul> 
     <li>새 상위 그룹의 상태 잠금이 해제된 경우 이동된 그룹의 상태는 이동의 영향을 받지 않고 속성을 유지합니다.</li> 
     <li>새 상위 그룹의 상태가 잠겨 있으면 상위 그룹의 상태 속성이 이동된 그룹의 상태 속성을 재정의합니다.</li> 
    </ul> <p>상태 키에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td>이동된 그룹에 이전 상위 그룹에서 상속된 상태가 있는 경우 </td> 
   <td> <p>이전 상위 그룹에서 상속된 모든 사용자 지정 상태는 이동된 그룹과 함께 제공되며 고유한 사용자 지정 상태가 됩니다. 이전 상위 그룹과 더 이상 연결되지 않습니다.</p> 
    <ul> 
     <li>이동 후 이전 상위 그룹이 잠긴 사용자 지정 상태를 편집하는 경우 변경 사항은 이동된 하위 그룹의 상태에 영향을 주지 않습니다.</li> 
     <li>이전 상위 그룹이 그룹을 이동할 때 잠금 해제된 사용자 지정 상태를 잠그는 경우, 이동한 하위 그룹의 상태는 잠기지 않습니다.</li> 
     <li>이동된 그룹은 이제 이전 상위 그룹에서 상속할 때 잠긴 상태를 잠금 해제할 수 있습니다.</li> 
    </ul> 
     <p><b>예:</b><p> 
     <p>마케팅 그룹의 그룹 관리자인 Olivia는 그룹에 대해 두 가지 상태를 만듭니다. 그녀는 키 ABC가 있는 첫 번째 리뷰를 지명하고, 잠근다. She names the other Final Review, with key XYZ, and doesn't lock it.</p> 
     <p>또한 제품 마케팅이라는 마케팅 그룹 아래에 하위 그룹을 만듭니다. 작성된 즉시 마케팅 그룹의 첫 번째 검토 및 최종 검토 모두를 자동으로 상속합니다.</p> 
     <p>나중에 Olivia는 제품 그룹 아래의 제품 마케팅 하위 그룹을 이동합니다. 첫 번째 검토와 마지막 검토 모두 제품 마케팅 그룹과 함께 제품 그룹 아래의 새 위치로 이동합니다.</p> 
     <p>이동 전에 첫 번째 검토가 잠겼지만, 제품 마케팅 그룹 관리자는 이제 이 검토를 편집할 수 있습니다. 상위 그룹에서 제어하는 상속된 상태가 아니기 때문입니다.</p> 
     <p>최종 검토(Final Review)는 잠금이 해제되고 평상시처럼 편집할 수 있습니다.</p> 
     <p>마케팅 그룹의 경우 Olivia는 First Review와 Final Review의 색상을 변경하고 First Review-Edited와 Final Review-Edited의 이름을 바꿉니다. 그녀는 또한 최종 검토-편집된 것을 잠급니다. 한편 제품 마케팅 그룹에서 첫 번째 검토 및 최종 검토 상태의 색상 및 이름은 변경되지 않습니다.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 삭제된 그룹의 사용자 지정 상태

그룹이나 하위 그룹을 삭제하면 사용자 정의된 상태를 포함하여 연관된 정보가 다른 그룹이나 하위 그룹에 재할당됩니다. 삭제된 그룹의 상태가 대상 그룹의 상태에 추가됩니다.

삭제된 그룹 상태 중 하나를 대상 그룹에서도 사용하고 있었고(두 그룹의 상태가 동일한 키를 가지고 있음) 대상 그룹이 상태를 다른 방식으로 사용자 지정한 경우, 대상 그룹 버전의 설정은 이동된 그룹 버전의 설정을 덮어씁니다.

>[!INFO]
>
>**예:**
>
>그룹 A의 그룹 관리자는 자신의 그룹에 대해 잠금 해제된 시스템 수준 상태의 이름을 바꿉니다. 그룹 B의 그룹 관리자는 자신의 그룹에 대해 해당 상태의 이름도 바꿉니다. 두 그룹의 상태 이름이 다르지만 동일한 키를 갖습니다.
>
>나중에 그룹 A가 삭제되고 모든 정보가 그룹 B로 재할당됩니다.
>
>* 상태의 그룹 B 버전 이름은 그룹 A 버전 이름을 무시합니다.
>* 그룹 A의 누군가가 해당 그룹을 삭제하기 전에 해당 객체에 상태를 적용했다면 객체의 상태 이름은 그룹 B에서 사용하는 상태의 이름으로 업데이트됩니다.
>
>상태 키에 대한 자세한 내용은 [사용자 지정 상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create)의 이 문서에서 표를 참조하십시오.
>
>그룹 삭제에 대한 자세한 내용은 [그룹 삭제](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)를 참조하십시오.
