---
user-type: administrator
product-area: system-administration;user-management
keywords: 관리,하위 그룹,편집
navigation-topic: create-and-manage-subgroups
title: 하위 그룹 관리
description: 하위 그룹의 그룹 관리자는 하위 그룹을 생성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다. 상위 그룹에서 하위 그룹을 제거하여 최상위 그룹을 만들 수도 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# 하위 그룹 관리

하위 그룹의 그룹 관리자는 하위 그룹을 생성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다.

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹을 만들 수도 있습니다.

그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

하위 그룹에 대한 자세한 내용은 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 하위 그룹 만들기, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 또는 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

   표시되는 목록에서 관리하는 그룹과 해당 그룹의 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 작업할 하위 그룹이 포함된 그룹의 이름을 클릭합니다.

   또는

   하나 이상의 하위 그룹을 이동하는 경우 대상 그룹의 이름을 클릭합니다. 나중에 이동할 하위 그룹을 지정합니다.

1. 왼쪽 메뉴에서 **하위 그룹**.

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">새 하위 그룹 만들기</td> 
      <td> <p>보고 있는 그룹에서 한 수준 아래로 새 하위 그룹을 만들려면 <strong>하위 그룹 추가</strong>.</p> <p>또는 목록의 다른 하위 그룹 아래에 새 하위 그룹을 만들려면 해당 하위 그룹을 선택하고 <strong>추가 s</strong><strong>하위 그룹</strong>.</p> <p>하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">하위 그룹 만들기</a>.</p> <p>그룹 계층은 15개 수준을 초과할 수 없지만, 단일 레벨에는 병렬 그룹의 수가 제한되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 이동 </td> 
      <td> <p>관리하는 다른 그룹 아래에서 기존 하위 그룹을 이동할 수 있습니다.</p> <p>그룹 계층은 15개 수준을 초과할 수 없지만, 단일 레벨에는 병렬 그룹의 수가 제한되지 않습니다.</p> 
       <ol> 
        <li value="1"> <p>(선택 사항) 하위 그룹을 선택하여 대상 그룹으로 만듭니다.</p> <p>이 단계를 건너뛰면 3단계에서 선택한 그룹이 대상 그룹입니다.</p> </li> 
        <li value="2">클릭 <strong>하위 그룹 추가</strong> &gt; <strong>기존 그룹</strong>.</li> 
        <li value="3"> <p>에서 <strong>기존 그룹</strong> 상자가 나타나면 이동할 하위 그룹의 이름을 입력합니다.</p> <p>표시되는 결과에 대상 그룹 위에 그룹이 없습니다.</p> <p>마우스로 가리키고 정보 아이콘을 클릭하여 올바른 그룹을 선택할 수 있습니다 <img src="assets/info-icon.png"> 옆에 표시됩니다. 그룹 위에 있는 그룹 계층 및 해당 관리자와 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> </li> 
        <li value="4"> <p>이동할 하위 그룹의 이름을 클릭하면 목록에 표시됩니다.</p> </li> 
        <li value="5"> <p>대상 그룹으로 이동할 다른 하위 그룹에 대해 c-d 단계를 반복합니다</p> </li> 
        <li value="6"><strong>저장</strong>을 클릭합니다.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 편집</td> 
      <td> <p>편집할 하위 그룹을 선택한 다음 편집 아이콘을 클릭합니다 <img src="assets/edit-icon.png">.</p> <p>하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">그룹 만들기</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 하위 그룹 내보내기</td> 
      <td> 
       <ol> 
        <li value="1">내보낼 하위 그룹 또는 하위 그룹을 선택합니다.</li> 
        <li value="2">내보내기 아이콘을 클릭합니다 <img src="assets/export.png">를 선택한 다음 원하는 파일 형식을 선택합니다.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹을 복사하여 새 최상위 그룹을 만듭니다</td> 
      <td> <p>(Workfront 관리자만 사용할 수 있습니다.) 하위 그룹을 복사하면 상위 그룹이 됩니다. 모든 그룹 구성원 및 하위 그룹이 함께 복사됩니다. 그룹 구성원들은 원래 그룹에 있었던 모든 임무를 유지합니다.</p> <p>하위 그룹 복사에 대한 자세한 내용은 <a href="#about-copying-a-subgroup" class="MCXref xref">하위 그룹 복사 정보</a> 참조하십시오.</p> 
       <ol> 
        <li value="1">하위 그룹을 선택한 다음 복사 아이콘을 클릭합니다 <img src="assets/copy-icon.png"> 선택한 그룹을 기반으로 새 최상위 그룹을 생성하려면</li> 
        <li value="2"> <p>새 그룹의 설정을 구성합니다.</p> <p>이러한 설정에 대한 자세한 내용은 섹션의 표를 참조하십시오 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹을 만듭니다</a> 기사 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹을 만듭니다</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 삭제</td> 
      <td> <p><b>중요 사항</b>: 그룹 또는 하위 그룹을 삭제할 때는 사용자, 작업 항목 및 현재 그룹에 지정된 하위 그룹을 유지해야 합니다. 보존되도록 하려면 아래 단계에서 그룹의 객체를 다른 그룹에 재할당해야 합니다.</p> 
       <ol> 
        <li value="1">하위 그룹을 선택한 다음 삭제 아이콘을 클릭합니다 <img src="assets/delete.png">.</li> 
        <li value="2">에서 <strong>그룹 삭제</strong> 상자가 나타나고 입력을 시작한 다음 삭제할 그룹의 구성원, 작업 항목 및 하위 그룹을 이동할 그룹의 이름을 선택합니다.</li> 
        <li value="3">클릭 <strong>삭제</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>하위 그룹이 포함된 그룹을 관리하는 경우 전체 그룹 및 모든 하위 그룹에 대한 데이터를 식별하고 필터링할 수 있습니다. 보고서나 목록의 상위 ID 필드를 사용하여 이를 수행할 수 있습니다.
>
>예를 들어, 대규모 마케팅 부서를 관리하고 전체 부서가 작업하고 있는 모든 프로젝트 목록을 원하는 경우를 생각해 보십시오.
>
>Workfront에서 이 마케팅 부서는 필드 마케팅, 제품 마케팅 및 디지털 마케팅이라는 3개의 하위 그룹과 마케팅 이라는 그룹으로 표시됩니다. 전체 마케팅 부서(4개 그룹 모두)에 속하는 프로젝트를 나열하려면 다음 필터 규칙을 사용하여 프로젝트 영역에 대한 필터를 생성할 수 있습니다.
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>상위 이름 필드를 사용하여 최상위 그룹과 연관된 데이터를 식별할 수도 있지만 필터 또는 그룹화에는 표시되지 않고 보기에서만 식별할 수 있습니다.

## 상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만듭니다

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹을 만들 수 있습니다.

>[!TIP]
>
>하위 그룹 아래에 있는 그룹을 비활성화하면 해당 하위 그룹도 비활성화됩니다. 이 중 하나를 활성화하려는 경우 이 지침에 따라 상위 그룹에서 제거한 다음 다시 활성화할 수 있습니다.
>
>그룹 비활성화 및 재활성화에 대한 지침은 섹션을 참조하십시오 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) 및 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) 기사 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 최상위 그룹을 만들 그룹의 상위 그룹을 선택한 다음 편집 아이콘을 클릭합니다 ![](assets/edit-icon.png).
1. 에서 **그룹 편집** 표시되는 상자 **그룹 구성원 및 그룹 관리자**&#x200B;을 눌러 최상위 그룹을 만들 하위 그룹의 이름을 입력한 다음 해당 이름의 오른쪽에 있는 X 를 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

## 그룹의 하위 그룹 구성원 보기 및 관리

관리하는 그룹의 기본 페이지를 볼 때 그룹의 하위 그룹에서 모든 사용자를 보고 관리할 수 있습니다. 자세한 내용은 [하위 그룹 구성원 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 하위 그룹 복사 정보 {#about-copying-a-subgroup}

하위 그룹을 복사할 때에는 다음 사항을 고려하십시오.

* 복사하는 하위 그룹에 고유한 하위 그룹이 있으면 복사본은 복사본에 포함되고 이름은 다음과 같이 지정됩니다.

   ```
   Original subgroup name (Copy)
   ```

* 공개 그룹에 속하는 모든 하위 그룹도 공개되므로, 편집 사용자 액세스 권한이 있는 모든 사용자가 그룹 내외의 사용자를 하위 그룹에 추가할 수 있습니다.
