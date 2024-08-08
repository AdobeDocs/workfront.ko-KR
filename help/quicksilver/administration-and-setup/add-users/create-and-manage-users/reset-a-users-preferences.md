---
title: 사용자 환경 설정 재설정
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다. 개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 2%

---

# 사용자 환경 설정 재설정

<!-- Audited: 12/2023 -->

Adobe Workfront 관리자는 Workfront 시스템의 모든 사용자에 대한 사용자 환경 설정을 재설정하거나 제거할 수 있습니다.

개별 사용자는 자신의 사용자 환경 설정을 재설정할 수도 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 영향을 받는 설정 정보

사용자 환경 설정을 재설정하면 일부 환경 설정은 시스템 기본값으로 되돌려지고 다른 환경 설정은 지워지거나 제거됩니다.

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
   <td>보기</td> 
   <td> <p> 시스템 기본값으로 되돌림</p> <p>기존 보기는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>필터</td> 
   <td> <p>시스템 기본값으로 되돌림</p> <p>기존 필터는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>그룹화</td> 
   <td> <p>시스템 기본값으로 되돌림</p> <p>기존 그룹화는 삭제되지 않습니다. 다시 선택할 수 있습니다.</p> </td> 
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
   <td> <p>시스템 기본값으로 되돌림</p> <p>이메일 알림은 시스템 기본값으로 되돌아갑니다. 기본 알림은 Adobe Workfront에서 사용할 수 있는 <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">이벤트 알림</a>에 나열됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>사용자 정의 탭</td> 
   <td>제거됨</td> 
  </tr> 
  <tr> 
   <td>사용자 정의 전역 탐색 옵션</td> 
   <td>레이아웃 템플릿 정의 또는 레이아웃 템플릿이 할당되지 않은 경우 시스템 기본값으로 다시 설정합니다.</td> 
  </tr> 
 </tbody> 
</table>

## 사용자 환경 설정 재설정

{{step-1-to-setup}}

1. **다음으로 로그인**&#x200B;을 선택합니다.
1. 기본 설정을 재설정할 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.
1. **로그인**&#x200B;을 선택합니다.
1. 웹 브라우저 상단의 URL 필드에서 `workfront.com` 뒤에 `/resetUser`을(를) 추가합니다.

   >[!NOTE]
   >
   >대/소문자를 구분합니다. U는 대문자로 사용하고 나머지 문자는 소문자여야 합니다. For example:
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. **Enter**&#x200B;를 누릅니다.
1. 모든 사용자 환경 설정을 재설정하려면 **재설정**&#x200B;을 선택하세요.

   또는

   사용자 지정 탭만 재설정하려면 **탭 재설정**&#x200B;을 선택하세요.
