---
title: 사용자의 환경 설정 재설정
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다. 개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# 사용자의 환경 설정 재설정

Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다.

개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.

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

## 영향을 받는 설정 정보

사용자 기본 설정을 재설정하면 일부 기본 설정이 시스템 기본값으로 복원되고 다른 기본 설정은 지워지거나 제거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>환경 설정</strong> </th> 
   <th><strong>재설정 후 상태</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>조회수</td> 
   <td> <p> 시스템 기본값으로 되돌립니다.</p> <p>기존 보기는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>필터</td> 
   <td> <p>시스템 기본값으로 되돌립니다.</p> <p>기존 필터는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>그룹화</td> 
   <td> <p>시스템 기본값으로 되돌립니다.</p> <p>기존 그룹화는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>최근 항목 목록</td> 
   <td>지워짐</td> 
  </tr> 
  <tr> 
   <td>즐겨찾기 목록</td> 
   <td>영향을 받지 않음</td> 
  </tr> 
  <tr> 
   <td>사용자 환경 설정</td> 
   <td> <p>시스템 기본값으로 되돌립니다.</p> <p>전자 메일 알림이 시스템 기본값으로 되돌립니다</p> </td> 
  </tr> 
  <tr> 
   <td>사용자 정의 사용자 정의 탭</td> 
   <td>제거됨</td> 
  </tr> 
  <tr> 
   <td>사용자 정의 전역 탐색 옵션</td> 
   <td>레이아웃 템플릿이 할당되지 않은 경우 레이아웃 템플릿 정의나 시스템 기본값으로 다시 설정합니다.</td> 
  </tr> 
 </tbody> 
</table>

## 사용자 환경 설정 재설정

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 선택 **다른 이름으로 로그인**.
1. 재설정하려는 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.
1. 선택  **로그인**.
1. 웹 브라우저 상단에 있는 URL 필드에서 을 추가합니다 `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >대/소문자를 구분합니다. U는 대문자로 사용하고 나머지 문자는 소문자로 입력해야 합니다. For example:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. 누르기 **Enter 키**.
1. 모든 사용자 환경 설정을 재설정하려면 **재설정**.

   또는

   사용자 지정 탭만 재설정하려면 **탭 재설정**.
