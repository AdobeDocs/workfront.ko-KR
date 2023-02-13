---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 사용자 지정 양식 삭제 또는 비활성화
description: 시스템에서 사용자 지정 양식을 삭제하거나 비활성화할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 사용자 지정 양식 삭제 또는 비활성화

시스템에서 사용자 지정 양식을 삭제하거나 비활성화할 수 있습니다.

>[!CAUTION]
>
>사용자 지정 양식을 삭제하면 양식과 연결된 개체의 사용자 지정 데이터도 모두 삭제됩니다. 삭제된 데이터는 복구할 수 없습니다. 대신 사용자 지정 양식 비활성화를 고려해 보십시오. 더 이상 사용하지 않는 사용자 지정 양식을 비활성화하면 연결된 모든 이전 데이터를 유지합니다.

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

## 사용자 지정 양식 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms.**
1. 사용자 지정 양식을 선택한 다음 **삭제**.
1. 사용자 정의 양식과 연결된 개체의 모든 데이터를 영구적으로 삭제하려면 **예, 삭제합니다.**.

## 사용자 지정 양식 비활성화

연결된 이전 데이터를 잃지 않고 더 이상 사용하지 않는 사용자 지정 양식을 비활성화할 수 있습니다. 사용자는 비활성 사용자 지정 양식을 개체에 추가할 수 없지만 이미 연결된 개체의 필드에 데이터를 보고 추가할 수 있습니다.

비활성 사용자 지정 양식의 필드도 보기에서 인라인 편집에서 계속 사용할 수 있습니다. 사용자가 인라인 편집 중에 비활성 사용자 지정 양식에서 필드를 추가하면 사용자 지정 양식이 비활성화되었더라도 양식이 개체에 자동으로 첨부됩니다.

사용자 지정 양식을 다시 활성화하면 이전에 설정한 설정이 유지되며 사용자는 비활성화되지 않은 것처럼 사용자 양식과 상호 작용할 수 있습니다.

사용자 지정 양식을 비활성화하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 비활성화할 사용자 지정 양식의 이름을 클릭합니다.
1. 을(를) 클릭합니다. **양식 설정** 탭.
1. 비활성화 **활성 상태** 선택 사항입니다.
1. 클릭 **저장 + 닫기**.
