---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 최근 삭제된 항목 보기 및 관리
description: 그룹 영역에서 관리하는 그룹을 볼 때 최근에 삭제한 작업 항목, 문서 및 템플릿을 보고, 필터링하고, 복원하고, 내보낼 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# 그룹의 최근 삭제된 항목 보기 및 관리

그룹 영역에서 관리하는 그룹을 볼 때, 다음과 같은 방법으로 최근에 삭제된 프로젝트, 작업, 문제, 문서 및 템플릿을 보고 작업할 수 있습니다.

* 최근에 삭제한 항목 목록을 보고, 필터링하고, 그룹화합니다
* 선택한 최근 삭제된 항목 복원
* 최근에 삭제한 항목 목록 내보내기

그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

삭제된 항목에 대한 자세한 내용은 [삭제된 항목 관리](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>삭제된 항목은 그룹 또는 해당 하위 그룹과 연관되어야 합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹의 최근 삭제된 항목 보기 및 관리

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 그룹 이름을 클릭합니다.
1. 왼쪽 패널에서 **최근에 삭제됨**.
1. 그룹의 최근 삭제된 항목을 보고 관리할 다음 탭 중 하나를 엽니다.

   * 프로젝트
   * 작업
   * 문제
   * 문서
   * 템플릿

   각 탭에는 현재 그룹 또는 해당 하위 그룹에 속하고 지난 30일 이내에 삭제된 해당 객체 유형의 항목이 나열됩니다.

   >[!NOTE]
   >
   >프로젝트를 삭제한 경우 개별 작업, 문제 및 문서가 모두 삭제되었습니다. 작업, 문제, 문서 또는 템플릿 탭에서 개별적으로 표시되지 않습니다. 그러나 프로젝트를 복원하면 이러한 모든 하위 개체도 프로젝트에 복원됩니다.
   >
   >
   >누군가 작업, 문제, 문서 또는 템플릿을 개별적으로 삭제한 경우 해당 탭에서 이를 보고 관리할 수 있습니다.

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>개체 복원</p> </td> 
      <td> <p>최대 10개의 개체를 선택하고 <strong>복원</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>탭에서 전체 객체 목록을 내보냅니다.</p> </td> 
      <td> <p>클릭 <strong>내보내기</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>목록에서 정보 표시 변경</p> </td> 
      <td> <p>목록 위의 오른쪽 위 모서리에서 <strong>필터</strong> 을 입력하여 제공된 기준에 따라 표시되는 항목을 정의합니다. 사용 <strong>보기</strong> 로 표시되는 필드를 정의하려면 사용 <strong>그룹화</strong> 항목을 카테고리로 그룹화합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>
