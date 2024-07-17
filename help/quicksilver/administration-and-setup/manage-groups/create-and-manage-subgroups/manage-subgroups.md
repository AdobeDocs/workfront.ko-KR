---
user-type: administrator
product-area: system-administration;user-management
keywords: 관리,하위 그룹,편집
navigation-topic: create-and-manage-subgroups
title: 하위 그룹 관리
description: 하위 그룹의 그룹 관리자는 하위 그룹을 생성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다. 상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수도 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 1%

---

# 하위 그룹 관리

하위 그룹의 그룹 관리자는 하위 그룹을 생성, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 및 삭제할 수 있습니다.

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수도 있습니다.

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

하위 그룹에 대한 자세한 내용은 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)를 참조하세요.

## 액세스 요구 사항

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

## 하위 그룹 만들기, 이동, 보기, 편집, 복사, 이름 변경, 내보내기 또는 삭제

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

   표시되는 목록에서 관리하는 그룹과 포함된 하위 그룹을 볼 수 있습니다. Adobe Workfront 관리자는 모든 그룹을 볼 수 있습니다.

1. 작업할 하위 그룹을 포함하는 그룹의 이름을 클릭합니다.

   또는

   하나 이상의 하위 그룹을 이동할 경우 대상 그룹의 이름을 누릅니다. 이후 단계에서 이동할 하위 그룹을 지정합니다.

1. 왼쪽 메뉴에서 **하위 그룹**&#x200B;을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">새 하위 그룹 만들기</td> 
      <td> <p>보고 있는 그룹에서 한 수준 아래로 새 하위 그룹을 만들려면 <strong>하위 그룹 추가</strong>를 클릭합니다.</p> <p>또는 목록의 다른 하위 그룹 아래에 새 하위 그룹을 만들려면 해당 하위 그룹을 선택한 다음 <strong>s</strong><strong>하위 그룹</strong>을 클릭합니다.</p> <p>하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">하위 그룹 만들기</a>의 표를 참조하십시오.</p> <p>그룹 계층은 15개 수준을 초과할 수 없지만, 단일 수준에는 병렬 그룹의 수가 무제한으로 포함될 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 이동 </td> 
      <td> <p>기존 하위 그룹을 관리하는 다른 그룹으로 이동할 수 있습니다.</p> <p>그룹 계층은 15개 수준을 초과할 수 없지만, 단일 수준에는 병렬 그룹의 수가 무제한으로 포함될 수 있습니다.</p> 
       <ol> 
        <li value="1"> <p>(선택 사항) 하위 그룹을 선택하여 대상 그룹으로 지정합니다.</p> <p>이 단계를 건너뛸 경우 3단계에서 선택한 그룹이 대상 그룹입니다.</p> </li> 
        <li value="2"><strong>하위 그룹 추가</strong> &gt; <strong>기존 그룹</strong>을 클릭합니다.</li> 
        <li value="3"> <p>표시되는 <strong>기존 그룹</strong> 상자에서 이동할 하위 그룹의 이름을 입력하세요.</p> <p>표시되는 결과에 대상 그룹 위의 그룹이 포함되지 않습니다.</p> <p>마우스로 가리키고 그 옆에 표시되는 정보 아이콘 <img src="assets/info-icon.png">을(를) 클릭하여 올바른 그룹을 선택하고 있는지 확인할 수 있습니다. 그룹 및 해당 관리자의 상위 그룹 계층과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> </li> 
        <li value="4"> <p>목록에 표시할 때 이동할 하위 그룹의 이름을 클릭합니다.</p> </li> 
        <li value="5"> <p>대상 그룹으로 이동할 다른 모든 하위 그룹에 대해 c-d 단계를 반복합니다</p> </li> 
        <li value="6"><strong>저장</strong>을 클릭합니다.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 편집</td> 
      <td> <p>편집할 하위 그룹을 선택한 다음 편집 아이콘 <img src="assets/edit-icon.png">을(를) 클릭합니다.</p> <p>하위 그룹을 구성하는 데 사용할 수 있는 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">그룹 만들기</a>의 표를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 하위 그룹 내보내기</td> 
      <td> 
       <ol> 
        <li value="1">내보낼 하위 그룹 또는 하위 그룹을 선택합니다.</li> 
        <li value="2">내보내기 아이콘 <img src="assets/export.png">을(를) 클릭한 다음 원하는 파일 형식을 선택합니다.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹을 복사하여 새 최상위 그룹을 생성합니다.</td> 
      <td> <p>(Workfront 관리자만 사용 가능) 하위 그룹을 복사하면 상위 그룹이 됩니다. 모든 그룹 멤버와 하위 그룹이 함께 복사됩니다. 그룹 구성원은 원래 그룹에 있던 모든 임무를 유지합니다.</p> <p>하위 그룹을 복사하는 방법에 대한 자세한 내용은 이 문서에서 <a href="#about-copying-a-subgroup" class="MCXref xref">하위 그룹 복사 정보</a>를 참조하십시오.</p> 
       <ol> 
        <li value="1">하위 그룹을 선택한 다음 복사 아이콘 <img src="assets/copy-icon.png">을(를) 클릭하여 선택한 그룹을 기반으로 새 최상위 그룹을 만듭니다.</li> 
        <li value="2"> <p>새 그룹의 설정을 구성합니다.</p> <p>이러한 설정에 대한 도움말을 보려면 문서 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹 만들기</a>에서 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">기존 그룹 또는 하위 그룹을 복사하여 최상위 그룹 만들기</a> 섹션의 표를 참조하십시오.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하위 그룹 삭제</td> 
      <td> <p><b>중요</b>: 그룹 또는 하위 그룹을 삭제할 때 현재 할당된 사용자, 작업 항목 및 모든 하위 그룹을 유지해야 합니다. 그룹의 객체를 아래 단계에서 다른 그룹에 재할당하라는 메시지가 표시되면 보존을 확인하는 데 도움이 됩니다.</p> 
       <ol> 
        <li value="1">하위 그룹을 선택한 다음 삭제 아이콘 <img src="assets/delete.png">을(를) 클릭합니다.</li> 
        <li value="2">표시되는 <strong>그룹 삭제</strong> 상자에서 입력을 시작한 다음 삭제할 그룹의 구성원, 작업 항목 및 하위 그룹을 이동할 그룹 이름을 선택합니다.</li> 
        <li value="3"><strong>삭제</strong>를 클릭합니다.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>하위 그룹을 포함하는 그룹을 관리할 때 전체 그룹과 모든 하위 그룹에 대한 데이터를 식별하고 필터링할 수 있는 것이 유용합니다. 이 작업은 보고서나 목록의 최상위 ID 필드를 사용하여 수행할 수 있습니다.
>
>예를 들어 대규모 마케팅 부서를 관리하고 전체 부서가 작업 중인 모든 프로젝트 목록을 원한다고 가정해 보겠습니다.
>
>Workfront에서 이 마케팅 부서는 Marketing이라는 그룹으로 표시되며, 3개의 하위 그룹인 Field Marketing, Product Marketing 및 Digital Marketing을 포함합니다. 전체 마케팅 부서(4개 그룹 모두)에 속하는 프로젝트를 나열하려면 다음 필터 규칙으로 프로젝트 영역에 대한 필터를 만들 수 있습니다.
>
>```
>Group: Top Parent ID > Equal > Marketing
>```
>
>최상위 이름 필드를 사용하여 최상위 그룹과 연관된 데이터를 식별할 수도 있지만 필터나 그룹화가 아닌 보기에서만 가능합니다.

## 상위 그룹에서 하위 그룹을 제거하고 최상위 그룹으로 만들기

상위 그룹에서 하위 그룹을 제거하여 최상위 그룹으로 만들 수 있습니다.

>[!TIP]
>
>하위 그룹이 있는 그룹을 비활성화하면 해당 하위 그룹도 비활성화됩니다. 이들 중 하나를 활성화하려면 다음 지침을 사용하여 상위 그룹에서 제거한 다음 다시 활성화할 수 있습니다.
>
>그룹 비활성화 및 다시 활성화에 대한 지침은 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md) 문서의 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) 및 [그룹 세부 정보 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) 섹션을 참조하십시오.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png)을(를) 클릭합니다.

1. 최상위 그룹을 만들 그룹의 상위 그룹을 선택한 다음 [편집] 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.
1. **그룹 구성원 및 그룹 관리자** 아래에 나타나는 **그룹 편집** 상자에서 최상위 그룹을 만들 하위 그룹의 이름을 입력한 다음 표시될 때 이름 오른쪽에 있는 X를 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

## 그룹의 하위 그룹 구성원 보기 및 관리

관리하는 그룹의 기본 페이지를 볼 때 그룹의 하위 그룹에 있는 모든 사용자를 보고 관리할 수 있습니다. 지침은 [하위 그룹 구성원 보기 및 관리](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)를 참조하세요.

## 하위 그룹 복사 정보 {#about-copying-a-subgroup}

하위 그룹을 복사할 때에는 다음 사항을 고려하십시오.

* 복사하는 하위 그룹에 고유한 하위 그룹이 있는 경우 해당 하위 그룹이 복사본에 포함되며 해당 이름의 형식은 다음과 같습니다.

  ```
  Original subgroup name (Copy)
  ```

* 공개 그룹에 속한 모든 하위 그룹도 공개이므로 그룹 내외에서 사용자 편집 액세스 권한이 있는 모든 사용자는 하위 그룹에 사용자를 추가할 수 있습니다.
