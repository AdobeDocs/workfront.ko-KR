---
title: 사용자 환경 설정 재설정
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다. 개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: f1fe1a2fe6e123d8a039e8d7e3547c0b0a8141df
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 3%

---

# 사용자 환경 설정 재설정

<!-- Audited: 12/2023 -->

Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다.

개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 영향을 받는 설정 정보

사용자 환경 설정을 재설정하면 일부 환경 설정은 시스템 기본값으로 되돌려지고 다른 환경 설정은 지워지거나 제거됩니다.

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

| 환경 설정 | 재설정 후 상태 |
| --- | --- |
| 보기 횟수 | 시스템 기본값으로 되돌림 <p>기존 보기는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> |
| 필터 | 시스템 기본값으로 되돌림 <p>기존 필터는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> |
| 그룹화 | 시스템 기본값으로 되돌림 <p>기존 그룹화는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> |
| 최근 항목 목록 | 지워짐 |
| 즐겨찾기 목록 | 영향을 받지 않음 |
| 사용자 환경 설정 | 시스템 기본값으로 되돌림 <p>이메일 알림은 시스템 기본값으로 되돌아갑니다. 기본 알림은 Adobe Workfront에서 사용할 수 있는 [이벤트 알림](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)에 나열됩니다.</p> |

## 사용자 환경 설정 재설정

{{step-1-to-setup}}

1. **다음으로 로그인**&#x200B;을 선택합니다.
1. 기본 설정을 재설정할 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.
1. **로그인**&#x200B;을 선택합니다.
1. 조직이 Adobe 통합 경험에 온보딩되지 않은 경우 다음 단계를 따르십시오.

   * 웹 브라우저 상단의 URL 필드에서 `/resetUser` 뒤에 `workfront.com`을(를) 추가합니다.

     >[!NOTE]
     >
     >대/소문자를 구분합니다. U는 대문자로 사용하고 나머지 문자는 소문자여야 합니다. For example:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. 조직이 Adobe 통합 경험에 온보딩된 경우 이 단계를 따르십시오.

   * 웹 브라우저 상단의 URL 필드에서 `/resetUser` 뒤에 `workfront`을(를) 추가합니다.

     >[!NOTE]
     >
     >대/소문자를 구분합니다. U는 대문자로 사용하고 나머지 문자는 소문자여야 합니다. For example:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. **Enter**&#x200B;를 누릅니다.

1. 모든 사용자 환경 설정을 다시 설정하려면 **다시 설정**&#x200B;을 클릭하세요.

   또는

   사용자의 왼쪽 탐색을 원래 레이아웃 템플릿 구성으로 재설정하려면 **왼쪽 탐색 재설정**&#x200B;을 클릭하세요.
