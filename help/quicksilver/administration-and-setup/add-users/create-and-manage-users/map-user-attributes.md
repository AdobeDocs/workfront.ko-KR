---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 특성 매핑 및 새 사용자 자동 프로비저닝
description: SSO(Single Sign-On)를 사용하여 ID 공급자의 Active Directory에서 Adobe Workfront 사용자에게 특성을 전달할 수 있습니다. 자동 프로비저닝 옵션(Just In Time Provisioning 또는 JIT이라고도 함)을 사용하여 Workfront에 새 사용자를 추가할 수도 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# 사용자 특성 매핑 및 새 사용자 자동 프로비저닝

SSO(Single Sign-On)를 사용하여 ID 공급자의 Active Directory에서 Adobe Workfront 사용자에게 특성을 전달할 수 있습니다. 자동 프로비저닝 옵션(Just In Time Provisioning 또는 JIT이라고도 함)을 사용하여 Workfront에 새 사용자를 추가할 수도 있습니다.

>[!NOTE]
>
>조직이 Adobe Admin Console에 온보딩된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 속성 매핑에 대한 팁

속성을 매핑할 때에는 다음 사항을 기억하십시오.

* 미리 보기 샌드박스 또는 CR(Customer Refresh) 샌드박스에서 항상 테스트합니다.
* 관리자 및 비관리자 계정으로 테스트하여 속성을 올바르게 매핑하는지 확인합니다.
* 속성은 사용자가 자동 프로비저닝 중뿐만 아니라 SSO를 통해 Workfront에 로그인할 때마다 매핑됩니다.

## 사용자 특성 매핑 및 새 사용자 자동 프로비저닝

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **단일 사인온(SSO)**.

1. 에서 **유형** 드롭다운에서 **SAML 2.0**.

1. 클릭 **사용자 특성 매핑**.

   ![](assets/map-user-attributes.png)

1. (선택 사항) Workfront에서 자동으로 Active Directory에서 새 사용자를 만들려면 **자동 프로비저닝 사용**.

   이 기능을 사용하려면 특성 매핑이 필요합니다.

1. 표시되는 옵션 행에서 Workfront 사용자에 필요한 특성을 매핑합니다.

   주소, 관리자, 작업 역할, 홈 그룹 등의 속성을 매핑할 수 있습니다.

   속성 매핑은 1:1 비율로 작동합니다. 예를 들어 사용자가 속한 모든 그룹을 설정할 수 없습니다. 사용자당 하나만 설정할 수 있습니다.

   >[!IMPORTANT]
   >
   >각 사용자에 대해 다음 속성이 필요합니다.
   >      
   >* 이름
   >* 성
   >* 이메일 주소

   >      
   >속성 매핑에서는 액세스 수준을 매핑하지 않는 것이 좋습니다. 이 경우 기본값을 설정하여 실수로 Admin Access를 제거하지 않도록 주의하십시오.

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
      <td>사용할 SSO 속성 레이블을 입력합니다./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">기본 값</td> 
      <td> <p>Workfront 사용자 속성을 선택한 후 연결 중에 값이 NULL이면 이 필드는 시스템의 해당 기본값으로 채워집니다. 속성 매핑 규칙을 적용하려는 경우에만 여기에 값을 입력합니다(7단계 참조). 기본값은 해당 규칙에 대한 예외 역할을 합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **규칙** 를 눌러 속성에 규칙을 추가합니다.

   1. 드롭다운에서 사용할 속성 수정자를 선택합니다.
   1. 오른쪽의 두 필드에 디렉토리 속성 값과 바꿀 값을 입력합니다.

      ![](assets/rule-fields.png)
   을(를) 클릭합니다 **규칙 추가** 를 눌러 속성에 규칙을 추가합니다.

1. (선택 사항) 더 많은 사용자 특성을 매핑하려면 **매핑 추가** 6-7단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.
