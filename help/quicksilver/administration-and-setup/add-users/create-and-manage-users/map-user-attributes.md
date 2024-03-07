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
source-git-commit: 20f9e9468c85235c0afadfee4d925a796ff89c54
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 1%

---

# 사용자 속성 매핑

<!--Audited 2/2024-->

SSO(Single Sign-On)를 사용하여 ID 공급자의 Active Directory에서 Adobe Workfront 사용자에게 속성을 전달할 수 있습니다.

## 액세스 요구 사항

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
   <td><p>새로운 기능: 표준</p><p>또는</p><p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 속성 매핑 팁

속성을 매핑할 때는 다음 사항에 유의하십시오.

* 항상 미리보기 샌드박스 또는 CR(고객 새로 고침) 샌드박스에서 테스트하십시오.
* 관리자 및 비관리자 계정으로 테스트하여 속성을 올바로 매핑하고 있는지 확인합니다.
* 매핑된 속성은 사용자가 단일 사인온을 통해 로그인할 때마다 적용됩니다.

  예: &quot;last name&quot;을 매핑하고 ID 공급자의 값을 업데이트하지 않고 Workfront에서 이름을 업데이트하는 경우, 다음에 사용자가 로그인할 때 ID 공급자의 값에 맞게 성을 덮어씁니다.

## 조직의 사용자 속성 매핑

속성 매핑 절차는 조직이 Adobe 통합 경험을 사용하는지 여부에 따라 다릅니다.

조직이 Adobe 통합 환경에 있는지 확인하려면 Workfront에 액세스하는 데 사용하는 URL을 검사하십시오.

| URL | Adobe 경험 |
|---|---|
| (CompanyName).my.workfront.com | 클래식 경험 |
| experience.adobe.com | 통합 경험 Adobe |

* [클래식 경험에서 사용자 속성 매핑](#map-user-attributes-in-the-classic-experience)
* [Adobe 통합 경험의 사용자 속성 매핑](#map-user-attributes-in-the-adobe-unified-experience)

### 클래식 경험에서 사용자 속성 매핑

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **SSO(단일 인증)**.

1. 다음에서 **유형** 드롭다운, 클릭 **SAML 2.0**.

1. 클릭 **사용자 속성 매핑**.

   ![](assets/map-user-attributes.png)

1. 표시되는 옵션 행에서 Workfront 사용자에게 필요한 속성을 매핑합니다.

   주소, 관리자, 작업 역할, 홈 그룹 등의 속성을 매핑할 수 있습니다.

   속성 매핑은 1:1 비율로 작동합니다. 예를 들어 사용자가 속한 모든 그룹을 설정할 수 없으며 사용자당 하나만 설정할 수 있습니다.

   >[!IMPORTANT]
   >
   >속성 매핑에서는 액세스 수준을 매핑하지 않는 것이 좋습니다. 기본값 설정 시 관리자 액세스를 실수로 제거하지 않도록 주의하십시오.

   다음 표에서는 속성을 매핑하는 데 사용할 수 있는 필드에 대해 설명합니다.

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront 사용자 속성</td> 
      <td>매핑할 속성의 이름을 선택합니다</td> 
     </tr> 
     <tr> 
      <td role="rowheader">디렉터리 속성</td> 
      <td>사용할 SSO 속성 레이블을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 값</td> 
      <td> <p>Workfront 사용자 속성을 선택한 후 연결 중에 값이 NULL이면, 이 필드는 시스템에서 해당 기본값으로 채워집니다. 속성 매핑 규칙을 적용할 경우에만 여기에 값을 입력합니다(7단계 참조). 기본값은 이러한 규칙에 대한 예외로 작동합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **규칙** 을 눌러 속성에 규칙을 추가합니다.

   1. 드롭다운에서 사용할 속성 수정자를 선택합니다.
   1. 오른쪽의 2개 필드에 디렉토리 속성 값과 대체할 값을 입력합니다.

      ![](assets/rule-fields.png)

   다음을 클릭할 수 있습니다. **규칙 추가** 를 클릭하여 속성에 규칙을 더 추가합니다.

1. (선택 사항) 더 많은 사용자 속성을 매핑하려면 **매핑 추가** 6~7단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.

### Adobe 통합 경험의 사용자 속성 매핑

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-left.png) Adobe Workfront의 왼쪽 상단 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **SSO(단일 인증)**.

1. 다음 항목 선택 **Adobe** 탭.

1. (선택 사항 및 조건부) 조직에서 속성 매핑을 클래식 경험에 구성한 경우 해당 속성 매핑을 Adobe 통합 경험에 복사하려면 다음을 클릭하십시오. **매핑 마이그레이션**. 그런 다음 이러한 매핑을 삭제, 삭제 또는 편집할 수 있습니다.

   >[!NOTE]
   >
   >Adobe 통합 경험에서 매핑을 처음 구성할 때 매핑을 마이그레이션하는 것이 좋습니다. 나중에 다시 마이그레이션하는 데 아무런 해가 없지만, 두 번 이상 마이그레이션하는 것은 불필요합니다.

1. 새 속성 매핑을 만들려면 다음을 클릭하십시오. **매핑 추가**.

1. Workfront 필드 이름 옆에 있는 화살표를 클릭하고 [!DNL Workfront] 매핑할 필드입니다.

1. (선택 사항) 주어진 필드에 대해 두 개 이상의 규칙을 만들려면 옆에 있는 화살표를 클릭합니다 **항상** 규칙을 사용할 연산자를 선택합니다.

1. (조건부) Always 외에 연산자를 선택한 경우 연산자가 적용되는 Workfront 필드 및 값을 선택합니다.

   >[!NOTE]
   >
   >연산자 `Is Truthy` 및 `Is Falsy` 값은 필요하지 않습니다.

1. ID 관리자의 속성 값을 Workfront 필드에 적용할지 또는 특정 상수 값을 적용할지 여부를 선택합니다.

1. 적용할 ID 관리자 필드의 이름을 입력하거나 적용할 상수 값의 텍스트를 입력합니다.

1. (선택 사항) 동일한 Workfront 필드에 대한 규칙을 더 추가하려면 **새 규칙 추가**&#x200B;을 누르고 4-9단계를 수행합니다.

   >[!IMPORTANT]
   >
   > * Always 규칙 아래의 모든 규칙은 무시됩니다. Always 규칙이 있는 경우 규칙 목록의 맨 아래로 이동해야 합니다. 규칙 오른쪽에 있는 세 점 메뉴를 클릭하여 목록에서 규칙을 이동하고 규칙을 위나 아래로 이동할 수 있습니다.
   > * 목록 중간에 규칙을 만들려면 새 규칙의 위나 아래에 놓을 규칙 옆에 있는 세 점 메뉴를 클릭하고 을 선택합니다 **위에 규칙 추가** 또는 **아래에 규칙 추가**.

1. 규칙을 삭제하려면 삭제할 규칙 옆에 있는 세 점 메뉴를 클릭하고 을 선택합니다 **삭제**.
1. 매핑을 삭제하려면 **삭제** 아이콘은 카드에 있습니다.

1. 저장하려면 페이지 상단으로 스크롤하여 을 클릭합니다. **저장**.


