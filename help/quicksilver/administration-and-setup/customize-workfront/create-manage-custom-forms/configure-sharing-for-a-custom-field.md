---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 사용자 지정 필드 및 위젯에 대한 공유 구성
description: 기본적으로 사용자 지정 필드 또는 위젯을 사용자 지정 양식에 추가할 때 사용자 지정 양식에 액세스할 수 있는 시스템의 모든 사용자가 해당 항목의 레이블 및 이름과 같은 속성을 편집할 수 있습니다. 공유할 사용자를 제어하여 변경할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# 사용자 지정 필드 및 위젯에 대한 공유 구성

기본적으로 사용자 지정 필드 또는 위젯을 사용자 지정 양식에 추가할 때 사용자 지정 양식에 액세스할 수 있는 시스템의 모든 사용자가 해당 항목의 레이블 및 이름과 같은 속성을 편집할 수 있습니다. 공유할 사용자를 제어하여 변경할 수 있습니다.

사용자 지정 양식의 사용자 지정 필드 및 위젯에 대한 자세한 내용은 [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 및 [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 필드 또는 위젯에 대한 공유 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **사용자 지정 Forms**.
1. 조직의 Workfront 인스턴스에서 사용자 지정 필드 또는 위젯에 대한 공유를 구성하는 경우 다음을 수행하십시오.

   1. 을(를) 클릭합니다. **필드** 탭.
   1. 공유를 구성할 항목을 선택하고 **공유**.

   또는 기존 사용자 지정 양식에서 사용자 지정 필드 또는 위젯에 대한 공유를 구성하는 경우 다음을 수행하십시오.

   1. 사용자 지정 양식을 선택한 다음 **편집**.
   1. 오른쪽의 양식 편집 영역에서 공유를 구성할 항목을 선택합니다.
   1. 왼쪽 패널에서 **공유 필드**.


1. 에서 **사용자 지정 필드 액세스** 표시되는 상자에 항목을 공유할 사람과 공유할 방법을 지정합니다.

   1. 의 왼쪽 아래 모서리 근처에 있습니다. **사용자 지정 필드 액세스** 상자 아래의 **사용자 지정 필드에 대한 액세스 권한 부여**&#x200B;를 클릭하고 항목을 공유할 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 입력한 다음 해당 이름이 나타나면 이름을 클릭합니다.

      ![](assets/share-field-give-access-to.jpg)

   1. 항목을 공유할 방법에 대해 자세히 알아보려면 이름 오른쪽에 있는 드롭다운 목록을 클릭한 다음 다음 다음 옵션 중 하나를 사용하십시오.

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">보기</td> 
         <td> <p>을(를) 클릭합니다 <strong>고급 설정</strong> 사용자나 사용자가 액세스 권한을 사용하여 사용자 지정 양식에 항목을 추가하거나 다른 사용자와 공유할 수 있도록 할지 지정합니다.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">관리함</td> 
         <td> <p>사용자 지정 필드를 편집하고 필드 라이브러리 및 사용자 지정 양식을 작성하는 페이지에서 볼 수 있는 액세스 권한이 있습니다.</p> <p>을(를) 클릭합니다 <strong>고급 설정</strong> 사용자 또는 사용자가 액세스 권한을 사용하여 시스템에서 항목을 삭제하거나 다른 사용자와 공유할 수 있는지 지정합니다.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (선택 사항) 이전 단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) 오른쪽 상단 모서리에서 필드에 대한 시스템 전체 공유 옵션을 선택합니다.

   다음 옵션 중 일부가 이 드롭다운 메뉴에 동시에 표시되는 것은 아닙니다. 예를 들어, 두 번째 옵션은 다른 두 개 중 하나를 선택한 경우에만 표시됩니다.

   * **Workfront의 모든 사용자가 편집할 수 있도록 이 편집 가능한 시스템을 전체 시스템으로 만듭니다** (기본 옵션)

      사용자 지정 필드 또는 위젯을 추가할 때 공유 기능을 제한하지 않으면 사용자 지정 양식에 액세스할 수 있는 시스템의 모든 사용자가 사용자 지정 필드를 보고 해당 속성을 편집할 수 있습니다.

   * **시스템 전체 편집 액세스 제거**

      목록에 추가한 사람에 대해서만 액세스를 제한합니다.

   * **Workfront의 모든 사용자가 볼 수 있도록 시스템 전체에 표시**

1. 클릭 **저장** 또는 **저장 + 닫기**.

## 사용자 지정 양식을 공유할 때 사용자 지정 필드 및 위젯에 대한 액세스 권한을 상속합니다

사용자 지정 양식을 그룹, 작업 역할, 팀 또는 회사와 공유하는 경우 수신자는 양식에 있는 사용자 지정 필드 및 위젯에 대한 보기 액세스 권한을 상속합니다. 양식의 해당 항목에 대한 이 수준의 액세스 권한은 항상 유지됩니다. 따라서 양식은 작성자가 의도한 대로 수신자에 대해 작동할 수 있습니다. 이는 양식에 대한 편집 액세스 권한이 있는 수신자에게도 적용됩니다.

사용자 지정 필드 또는 위젯에 대한 액세스 권한을 상속한 사용자를 확인할 수 있으며 액세스 권한을 제거할 수 있습니다.

>[!NOTE]
>
>수신자가 공유 사용자 지정 양식의 사용자 지정 필드 또는 위젯에 대한 액세스 권한을 관리 하게 되면 해당 액세스 권한은 수신자에 대해 유지됩니다.

* [사용자 지정 필드 또는 위젯에 대한 액세스 권한을 상속받은 사용자 확인](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [공유된 사용자 지정 양식에서 사용자 지정 필드 또는 위젯에 대한 액세스 권한 제거](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 사용자 지정 필드 또는 위젯에 대한 액세스 권한을 상속받은 사용자 확인 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **사용자 지정 Forms**.
1. 을(를) 클릭합니다. **필드** 탭한 다음 필드, 이미지 또는 액세스 위젯을 선택합니다.
1. 표시되는 상자에서 **상속된 권한** 표시되는 이름을 확인합니다.
1. 클릭 **취소**.

### 공유된 사용자 지정 양식에서 사용자 지정 필드 또는 위젯에 대한 액세스 권한 제거 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

공유된 사용자 지정 양식에서 사용자 지정 필드 또는 위젯에 대한 액세스를 제거해야 하는 경우 양식 공유를 해제해야 합니다. 지침은 섹션에서 를 참조하십시오. [사용자 지정 양식에 대한 액세스 제거](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) 기사 [사용자 지정 양식 공유](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
