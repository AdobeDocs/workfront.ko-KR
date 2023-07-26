---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 사용자 정의 양식의 오브젝트 유형 삭제
description: 기존 사용자 정의 양식에서 해당 양식과 연결된 오브젝트 유형을 삭제할 수 있습니다. 이 작업을 수행하면 사용자는 더 이상 해당 유형의 오브젝트에 양식을 첨부할 수 없습니다.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 사용자 정의 양식의 오브젝트 유형 삭제

기존 사용자 정의 양식에서 해당 양식과 연결된 오브젝트 유형을 삭제할 수 있습니다. 이 작업을 수행하면 사용자는 더 이상 해당 유형의 오브젝트에 양식을 첨부할 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 정의 양식의 오브젝트 유형 삭제

기존 사용자 정의 양식에서 오브젝트 유형을 삭제할 수 있습니다.

사용자 정의 양식에는 하나 이상의 오브젝트 유형이 있어야 합니다.

>[!CAUTION]
>
>사용자가 삭제하려는 유형의 객체에 사용자 정의 양식을 이미 첨부하고 해당 객체에 데이터를 추가한 경우, 양식에서 해당 객체 유형을 삭제하면 해당 데이터가 영구적으로 삭제됩니다. 여기에는 사용자가 나중에 필요로 하는 이전 정보가 포함될 수 있습니다.
>
>일반적으로 이미 사용 중인 사용자 정의 양식을 편집하는 횟수를 최소화하는 것이 좋습니다. 사용자 정의 양식을 사용하는 사람에게 변경 사항을 알리는 알림 시스템이 없습니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms** 왼쪽 패널에서
1. 편집할 사용자 정의 양식을 선택한 다음 **편집**.
1. 다음 중 하나에서 X를 클릭합니다. **오브젝트 유형** 양식에서 삭제할 항목을 클릭한 다음 **삭제** 경고 메시지가 표시됩니다.

   ![](assets/click-x-object-types.jpg)

1. (선택 사항) 양식에서 제거할 다른 객체 유형에 대해 이전 단계를 반복합니다.
1. 클릭 **완료**&#x200B;을 클릭한 다음 을 클릭합니다 **닫기 및 저장**.
