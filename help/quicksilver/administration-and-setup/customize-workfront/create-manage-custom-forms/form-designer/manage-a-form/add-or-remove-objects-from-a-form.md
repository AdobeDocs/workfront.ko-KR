---
title: 양식 디자이너를 사용하여 기존 사용자 지정 양식에서 개체 유형을 추가하거나 삭제합니다
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 양식 디자이너를 사용하여 사용자 지정 양식에서 개체 유형을 추가하거나 제거할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# 양식 디자이너를 사용하여 기존 사용자 지정 양식에서 개체 유형을 추가하거나 삭제합니다

양식 디자이너를 사용하여 기존 사용자 지정 양식에서 개체 유형을 추가하거나 삭제할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>
   <p>현재 계획: 표준</p>
   <p>또는</p>
   <p>기존 계획: 계획</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td><p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 기존 사용자 지정 양식에 개체 유형 추가

양식에 객체 유형을 추가하여 여러 객체에 첨부할 수 있습니다.

>[!NOTE]
>
>섹션 브레이크 권한은 개체 유형의 영향을 받을 수 있습니다. 사용자 지정 양식 섹션에 대한 제한된 편집 권한은 프로젝트, 작업, 문제 및 사용자 개체 유형에만 사용할 수 있습니다.
>
>자세한 내용은 [여러 객체 유형이 섹션 브레이크 권한에 영향을 주는 방식](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms** 왼쪽 패널에 표시됩니다.

   표시되는 보기에서 조직을 위해 만들어진 모든 사용자 지정 양식을 검토할 수 있습니다. 또한 각 양식을 만든 사용자, 양식 사용 중인 객체 유형 및 양식 활성 여부를 확인할 수 있습니다.

1. 개체 유형을 추가할 사용자 지정 양식을 선택한 다음 **편집**.

1. 양식 맨 위에서 더하기 기호 + 를 클릭합니다 **개체 유형**&#x200B;를 클릭한 다음 표시되는 메뉴에서 원하는 유형을 선택합니다. 이 과정을 반복하여 개체 유형을 원하는 만큼 추가할 수 있습니다.

   ![](assets/add-new-object.png)

1. 클릭 **저장 후 닫기**.

   >[!TIP]
   >
   >을(를) 클릭합니다 **적용** 언제든지 사용자 지정 양식을 만들어 변경 사항을 저장하고 양식을 열어 둡니다.

## 사용자 지정 양식에서 개체 유형 삭제

기존 사용자 지정 양식에서 객체 유형을 삭제할 수 있습니다. 사용자 지정 양식에는 하나 이상의 개체 유형이 있어야 합니다.

>[!CAUTION]
>
>사용자가 삭제하려는 유형의 개체에 사용자 지정 양식을 이미 첨부하고 해당 데이터에 데이터를 추가한 경우 해당 데이터는 양식에서 해당 개체 유형을 삭제할 때 영구적으로 삭제됩니다. 사용자에게 나중에 필요한 이전 정보가 포함될 수 있습니다.
>
>일반적으로 이미 사용 중인 사용자 지정 양식을 편집하는 횟수를 최소화하는 것이 좋습니다. 사용자 지정 양식을 사용하는 사용자에게 변경 사항에 대해 알리는 알림 시스템이 없습니다.

객체 유형을 삭제하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms** 왼쪽 패널에 표시됩니다.
1. 편집할 사용자 지정 양식을 선택한 다음 **편집**.
1. 다음 중 하나에서 X 를 클릭합니다. **개체 유형** 양식에서 삭제하려는 **삭제** 경고 메시지에 표시되지 않습니다.

   ![](assets/delete-object-types.png)

1. (선택 사항) 양식에서 제거할 다른 개체 유형에 대해 이전 단계를 반복합니다.
1. 클릭 **완료**&#x200B;를 클릭한 다음 **닫기 및 저장**.
