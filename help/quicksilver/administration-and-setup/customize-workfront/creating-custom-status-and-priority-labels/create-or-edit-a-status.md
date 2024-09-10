---
title: 상태 만들기 또는 편집
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Adobe Workfront 관리자는 프로젝트, 작업 및 문제에 대한 사용자 정의 상태를 만들 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 2%

---

# 상태 만들기 또는 편집

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront 관리자는 프로젝트, 작업 및 문제에 대한 사용자 정의 상태를 만들 수 있습니다. 전체 Workfront 시스템 또는 특정 그룹이나 하위 그룹의 사용자용일 수 있습니다. 상태에 대한 자세한 내용은 [상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)를 참조하십시오.

>[!NOTE]
>
>그룹 관리자는 자신의 그룹에서만 사용할 수 있도록 자신의 그룹 상태를 만들 수도 있습니다. 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)을 참조하세요.

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

## 사용자 지정 상태 만들기 또는 편집

전체 조직 또는 단일 그룹에서 사용할 사용자 지정 상태를 추가할 수 있습니다.

전체 조직에 대한 사용자 지정 상태를 만들 때 시스템의 모든 그룹이 편집하지 않고 사용할 수 있도록 구성할 수 있습니다. 또는 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)에 설명된 대로 그룹 관리자가 그룹의 상태를 수정할 수 있도록 구성할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **상태**&#x200B;를 클릭합니다.

1. (조건부) 시스템 전체에서 사용할 상태를 만들거나 편집하는 경우 오른쪽 상단의 상자에서 **시스템 상태**&#x200B;가 선택되어 있는지 확인하십시오.

   ![](assets/system-statuses-in-upper-rt-corner-new.jpg)

   또는

   그룹 또는 하위 그룹의 상태일 경우 오른쪽 상단 모서리에 그룹 이름을 입력한 다음 표시될 때 선택합니다.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 상태와 연결할 개체 유형(**프로젝트**, **작업** 또는 **문제**)의 탭을 선택하십시오.

1. 새 상태를 만드는 경우 **새 상태 추가**&#x200B;를 클릭하세요.

   또는

   기존 상태를 편집하는 경우 해당 상태를 마우스로 가리킨 다음 맨 오른쪽에 표시되는 **편집** 아이콘을 클릭합니다.

   ![](assets/custom-status-edit.png)

1. 다음 옵션을 사용하여 상태를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">상태 이름</td> 
      <td> <p>상태 이름을 입력합니다. 필수 필드입니다.</p> <p>상태 이름을 만들 때는 시스템의 다른 사용자가 같은 이름으로 상태를 만들 수 있습니다. Workfront에서 상태를 선택할 때 혼동을 피하기 위해 고유한 이름을 사용하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>(선택 사항) 상태에 대한 설명을 입력합니다. 이것은 그것의 목적을 이용하는 사람들에게 전달한다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>색상 필드를 클릭하고 견본 패널에서 색상을 선택하여 상태의 색상을 사용자 정의합니다. 필드에 16진수를 입력할 수도 있습니다.</p> <p>사용자가 개체를 볼 때 Workfront의 오른쪽 위 모서리에 상태 색상이 표시됩니다.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">같음</td> 
      <td> <p>목록에서 상태의 기능을 가장 잘 설명하는 옵션 중 하나를 선택합니다. 예를 들어 상태 이름이 완료인 경우 이 이름과 동일한 옵션은 완료여야 합니다.</p> <p>모든 상태는 이러한 옵션 중 하나와 동일해야 합니다. 이렇게 하면 상태의 작동 방식이 결정되기 때문입니다.</p> <p>상태를 만든 후에는 이 옵션을 수정할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">키</td> 
      <td> <p>새 상태를 만드는 경우 해당 상태에 대한 코드나 약어를 입력하거나 생성된 약어를 사용하십시오. 이 키는 보고 목적으로 사용할 수 있으므로 Workfront에서 고유해야 합니다. 시스템에서 이미 사용 중인 키를 지정하려고 하면 필드가 빨간색으로 바뀝니다.</p> <p>이를 사용할 사람이 인식할 수 있는 약어를 사용하는 것이 유용할 수 있습니다.</p> <p>상태를 만든 후에는 이 옵션을 수정할 수 없습니다.</p> <p>계획, 현재 및 완료 상태에 대한 키 코드는 변경할 수 없습니다. 이는 텍스트 모드에서 보고서를 작성하는 경우에 중요합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">상태 숨기기</td> 
      <td> <p>(프로젝트 및 작업 상태만 해당)</p> <p>사용자에게 상태를 숨기려면 이 옵션을 활성화합니다. 이 옵션이 비활성화되면(기본 설정) 시스템의 모든 사용자가 상태를 사용할 수 있습니다.</p> <p>4가지 문제 유형(버그 보고서, 순서 변경, 문제, 요청) 모두에 대해 이 옵션을 비활성화하면 문제 상태를 숨길 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 그룹에 대해 잠금</td> 
      <td>
       <p>상태가 잠겨 있으면 시스템 전체의 사용자가 이를 보고 사용할 수 있으며 그룹 관리자는 자신의 그룹에 대해 상태를 사용자 정의할 수 없습니다.</p> 
       <p>상태가 잠금 해제되면 그룹 관리자는 개별 그룹에 대해 상태를 사용자 지정할 수 있습니다.</p>

   <div>
       <p>시스템 승인 프로세스에서 잠김 및 잠금 해제 상태를 모두 사용할 수 있습니다. 잠금 해제된 시스템 상태의 시스템 승인 프로세스를 생성하는 경우 시스템 전체의 사용자는 승인 프로세스를 시스템의 프로젝트, 작업 또는 문제에 첨부할 수 있습니다.</p>
       <p> 다음 시나리오에서는 사용자와 사용자가 상태 잠금 해제 결과를 이해하는 데 도움이 되는 경고 메시지가 표시됩니다.</p>
       <ul>
       <li>관리자가 승인 프로세스에 사용되는 시스템 수준 상태를 잠금 해제합니다. 그룹에 대해 잠금 해제 상태를 삭제할 수 있다는 경고가 표시됩니다. 이렇게 하면 그룹 구성원이 그룹에 할당된 오브젝트에 대해 해당 승인 프로세스를 제대로 사용할 수 없게 됩니다.</li>
       <li>사용자가 잠금 해제 상태를 사용하는 승인 프로세스 편집을 시작합니다. 잠금 해제된 상태에 대해 경고하는 메시지가 표시되어 다시 잠그거나 바꾸는 것이 좋은지 평가할 수 있습니다.</li>
       <li>잠금 해제 상태의 시스템 수준 승인 프로세스가 오브젝트에 첨부되고 해당 오브젝트에 할당된 그룹에 대한 상태가 삭제되었습니다. 그룹 멤버가 객체의 승인 섹션으로 이동하면 객체에 대해 승인 프로세스를 시작할 수 없다는 메시지가 표시됩니다.</li>
       </ul>
       <p>잠금 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">잠김 및 잠금 해제된 시스템 수준 상태</a>를 참조하십시오.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

   이 상태를 기본 상태로 만드는 방법에 대한 지침은 [사용자 지정 상태를 기본 상태로 사용](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md)을 참조하세요.

그룹 상태 순서 조정에 대한 자세한 내용은 [시스템 수준 및 그룹 상태 순서 조정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md)을 참조하십시오.
