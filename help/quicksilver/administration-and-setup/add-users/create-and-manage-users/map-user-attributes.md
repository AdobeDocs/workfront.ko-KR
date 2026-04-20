---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 속성 매핑
description: SSO(Single Sign-On)를 사용하여 ID 공급자의 Active Directory에서 Adobe Workfront 사용자에게 속성을 전달할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: d8ccdeac9a658ca7a2862781e98c2c3c6fa0e8a0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 3%

---

# 사용자 속성 매핑

<!--Audited 2/2024-->

SSO(Single Sign-On)를 사용하여 ID 공급자의 Active Directory에서 Adobe Workfront 사용자에게 속성을 전달할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>Workfront 관리자여야 합니다.</p></td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 속성 매핑 팁

속성을 매핑할 때는 다음 사항에 유의하십시오.

* 항상 미리보기 샌드박스 또는 CR(고객 새로 고침) 샌드박스에서 테스트하십시오.
* 관리자 및 비관리자 계정으로 테스트하여 속성을 올바로 매핑하고 있는지 확인합니다.
* 매핑된 속성은 사용자가 단일 사인온을 통해 로그인할 때마다 적용됩니다.

  예: &quot;last name&quot;을 매핑하고 ID 공급자의 값을 업데이트하지 않고 Workfront에서 이름을 업데이트하는 경우, 다음에 사용자가 로그인할 때 ID 공급자의 값에 맞게 성을 덮어씁니다.

## 조직의 사용자 속성 매핑

1. Adobe Workfront 왼쪽 상단의 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-left.png)을 클릭한 다음 **설정** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.

1. **Adobe** 탭을 선택합니다.

1. (선택 사항 및 조건부) 조직에서 특성 매핑을 클래식 경험에 구성한 경우 해당 특성 매핑을 Adobe 통합 경험에 복사하려면 **매핑 마이그레이션**&#x200B;을 클릭합니다. 그런 다음 이러한 매핑을 삭제, 삭제 또는 편집할 수 있습니다.

   >[!NOTE]
   >
   >Adobe 통합 경험에서 매핑을 처음 구성할 때 매핑을 마이그레이션하는 것이 좋습니다. 나중에 다시 마이그레이션하는 데 아무런 해가 없지만, 두 번 이상 마이그레이션하는 것은 불필요합니다.

1. 새 특성 매핑을 만들려면 **매핑 추가**&#x200B;를 클릭하십시오.

1. Workfront 필드 이름 옆에 있는 화살표를 클릭하고 매핑할 [!DNL Workfront] 필드를 선택합니다.

1. (선택 사항) 지정된 필드에 대해 두 개 이상의 규칙을 만들려면 **항상** 옆에 있는 화살표를 클릭하고 규칙을 사용할 연산자를 선택합니다.

1. (조건부) Always 외에 연산자를 선택한 경우 연산자가 적용되는 Workfront 필드 및 값을 선택합니다.

   >[!NOTE]
   >
   >연산자 `Is Truthy` 및 `Is Falsy`에는 값이 필요하지 않습니다.

1. ID 관리자의 속성 값을 Workfront 필드에 적용할지 또는 특정 상수 값을 적용할지 여부를 선택합니다.

1. 적용할 ID 관리자 필드의 이름을 입력하거나 적용할 상수 값의 텍스트를 입력합니다.

1. (선택 사항) 동일한 Workfront 필드에 대한 규칙을 더 추가하려면 **새 규칙 추가**&#x200B;를 클릭하고 4-9단계를 수행합니다.

   >[!IMPORTANT]
   >
   > * Always 규칙 아래의 모든 규칙은 무시됩니다. Always 규칙이 있는 경우 규칙 목록의 맨 아래로 이동해야 합니다. 규칙 오른쪽에 있는 세 점 메뉴를 클릭하여 목록에서 규칙을 이동하고 규칙을 위나 아래로 이동할 수 있습니다.
   > * 목록 중간에 규칙을 만들려면 새 규칙의 위나 아래에 적용할 규칙 옆에 있는 점 3개를 클릭하고 **위에 규칙 추가** 또는 **아래에 규칙 추가**&#x200B;를 선택합니다.

1. 규칙을 삭제하려면 삭제할 규칙 옆에 있는 세 점 메뉴를 클릭하고 **삭제**&#x200B;를 선택합니다.
1. 매핑을 삭제하려면 해당 매핑 카드에 있는 **삭제** 아이콘을 클릭합니다.

1. 저장하려면 페이지 맨 위로 스크롤하여 **저장**&#x200B;을 클릭합니다.


