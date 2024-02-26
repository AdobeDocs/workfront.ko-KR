---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트에 다른 사용자 태그 지정
description: Adobe Workfront 개체에 업데이트 설명을 제공하면 프로젝트의 모든 사용자가 제출된 정보를 볼 수 있습니다. 그러나 프로젝트에 없는 사용자가 이 정보를 볼 때 혜택을 받을 때가 있을 수 있습니다. 프로젝트에 해당 사용자를 포함시키는 대신 업데이트에 태그를 지정하여 사용자와 공유할 수 있습니다. 태그 지정된 사용자가 이벤트 알림을 받습니다.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 56ab6fe79fe6e10be2ec61cb16ff48b30856dc0f
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 0%

---

# 업데이트에 다른 사용자 태그 지정

{{highlighted-preview}}

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

>[!IMPORTANT]
>
>현재 Adobe Workfront의 댓글 달기 환경을 다시 디자인하고 있습니다.
>
>댓글 달기 경험에 액세스하는 객체에 따라 업데이트 섹션에 다음과 같은 기능이 표시될 수 있습니다.
>* 새로운 경험
>* 기존 경험
>* 새로운 및 기존 경험
>
>새 댓글 달기 경험과 사용 가능 여부에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>새 주석 달기 경험은 Workfront 오브젝트의 업데이트 섹션에만 사용할 수 있고 다음 영역에서 오브젝트에 액세스할 때는 사용할 수 없습니다.
>
> * 홈
> * 목록의 요약 패널
> * 타임시트의 요약 패널
> * 업무 균형자의 요약 패널
>
><span class="preview">새 댓글 달기 환경은 미리 보기 환경의 목록, 타임시트 및 업무 균형자 의 요약 패널에서 사용할 수 있습니다.</span>

오브젝트를 업데이트할 때 사용자가 따르지 않을 수 있는 오브젝트에 주의를 집중시키려면 사용자를 태그 지정할 수 있습니다.

이러한 사용자를 객체에 할당하거나 구독하도록 하여 해당 사용자를 객체에 포함시키는 대신, 업데이트에서 태그를 지정하여 사용자와 공유할 수 있습니다. 태그가 지정된 사용자는 입력한 업데이트에 대한 알림을 받습니다.

## 업데이트의 사용자 태그 지정에 대한 고려 사항

* 업데이트를 태그 지정한 사용자가 이메일 알림을 받으려면 프로필에서 개인 알림을 활성화해야 합니다. 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Workfront 개체에 업데이트를 추가하는 방법에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* 문제가 프로젝트 또는 작업으로 전환되면 업데이트가 새 프로젝트 또는 작업에 복사되지만 태그가 지정된 사용자는 복사되지 않습니다. 대화를 계속하려면 참가자를 다시 태그 지정해야 합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>문제 및 문서에 대해 요청 이상, 기타 모든 오브젝트에 대해 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>문제 및 문서에 대한 요청자 이상, 기타 모든 오브젝트에 대한 검토자 이상</p> 
   <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 업데이트에 다른 사용자 태그 지정

업데이트의 다른 사람에 대한 태깅은 선택한 경험과 개체에 따라 다릅니다.

### 새로운 댓글 달기 환경의 업데이트에 다른 사람에게 태그 지정

다음과 같은 방법으로 새 댓글 달기 환경의 업데이트에 다른 사용자에게 태그를 지정할 수 있습니다.

* **자동**: 사용자가 스레드를 시작하거나, 댓글을 추가하거나, 답글을 추가하면 자동으로 태그가 지정되고 댓글 달기 상자의 사람 또는 팀 태그 영역에 추가됩니다. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >스레드가 레거시 댓글 달기 환경에서 시작되면 스레드 참여자에 자동으로 태그가 지정되지 않습니다.

* **수동**: 댓글 달기 상자의 인물 태그 영역에 사용자를 수동으로 추가하는 경우.

댓글을 편집하거나 답글을 달 때 실수로 태그가 지정된 사용자를 제거할 수도 있습니다.

1. 에 설명된 대로 작업 항목 업데이트를 시작합니다. [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 댓글 소유자는 자동으로 태그를 지정하고 댓글 달기 상자의 사람 또는 팀 태그 영역에 추가됩니다.

   >[!TIP]
   >
   >댓글 소유자는 댓글 상자의 태그 사용자 또는 팀 영역에서 자신의 이름을 볼 수 없습니다.

1. 다음에서 **사람 또는 팀에 태그 지정** 필드에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   또는

   다음에 @ 기호를 입력합니다. **댓글 작성** 영역에 업데이트에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   >[!TIP]
   > 
   >이름이 유사하거나 동일한 사용자가 있을 때 올바른 사용자를 식별하려면 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인합니다.
   > 
   >업데이트에서 태그 지정할 때 사용자를 보려면 최소 하나 이상의 작업 역할과 연결되어 있어야 합니다.
   > 
   >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   <div class="preview">

   미리보기 환경의 태그 지정 예:
   ![사용자 태그 지정](assets/tag-others-unified-commenting-with-all-tab.png)

   </div>

   프로덕션 환경의 태그 지정 예:
   ![](assets/tag-others-unified-commenting.png)

1. (선택 사항) 업데이트를 비공개로 설정하려면 을 활성화합니다 **내 회사에 비공개** 업데이트 상자의 오른쪽 아래 모서리에 있습니다. 이렇게 하면 회사의 사용자에게만 업데이트가 표시됩니다. 다음 **내 회사에 비공개** 옵션은 회사가 Workfront 프로필에 지정된 경우에만 사용할 수 있습니다.

   >[!NOTE]
   >
   >* 이 옵션은 사용자가 회사와 연결되어 있을 때만 표시됩니다.
   >* 회사 외부의 태그 지정된 사용자는 업데이트 탭에 개인 댓글이 표시되지 않더라도 인앱 알림이나 이메일을 계속 받을 수 있습니다. 외부 사용자와 정보를 공유하지 않으려면 업데이트에 외부 사용자에게 태그를 지정하지 않는 것이 좋습니다.

1. (선택 사항) 여러 사용자와 팀을 추가하려면 2단계를 반복합니다. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >&quot;직원 또는 팀 태그&quot; 필드에 나열된 모든 사용자 및 팀 구성원은 업데이트에 대한 인앱 알림을 받으며 이메일 알림 설정의 구성에 따라 이메일을 받을 수 있습니다. 댓글 또는 회신에 태그를 지정한 사용자는 해당 댓글 또는 회신에 대한 알림을 받고, 나머지 스레드 동안 스레드 멤버로 이름이 나열된 상태로 볼 수 있지만 자신을 다시 태그 지정하지 않는 한 다른 알림을 받지 않습니다. 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 및 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 클릭 **제출**.\
   업데이트에 포함된 사용자에게는 객체에 대한 보기 권한이 자동으로 부여되고 객체에 대한 업데이트를 보고 응답할 수 있습니다.

   태그가 지정된 엔티티의 이름이 해당 아바타 옆에 최대 2개의 엔티티로 표시됩니다. 두 개 이상의 엔티티에 태그가 지정되어 있으면 태그가 지정된 추가 엔티티 수와 함께 첫 번째 엔티티의 이름이 표시됩니다.

   ![](assets/members-icons-expanded-unshimmed.png)

   작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (선택 사항) **자세히** 메뉴 ![](assets/more-menu.png) 주석의 오른쪽 상단 모서리에서 을(를) 클릭한 다음 을(를) 클릭합니다 **편집**. 태그된 사용자를 제거한 다음 **제출**. 댓글을 입력한 후 15분 이내에만 편집할 수 있습니다. 추가한 의견만 편집할 수 있습니다.

   >[!TIP]
   >
   >기존 댓글 달기 경험을 사용하여 댓글과 댓글을 추가할 때 새로운 댓글 달기 경험을 사용하는 사람은 특별히 태그가 지정되지 않은 댓글 소유자를 수동으로 제거할 수 없습니다.


### 기존 업데이트 섹션의 업데이트에 대해 다른 사람에게 태그 지정

기존 업데이트 섹션에서 사용자에 수동으로 태그를 지정할 수 있습니다.

1. 에 설명된 대로 작업 항목 업데이트를 시작합니다. [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 다음에서 **알림** 필드에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   또는

   다음에 @ 기호를 입력합니다. **새 업데이트 시작** 영역에 업데이트에 포함할 사용자 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   >[!TIP]
   >
   >이름이 유사하거나 동일한 사용자가 있을 때 올바른 사용자를 식별하려면 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인합니다.
   >
   >업데이트에서 태그 지정할 때 사용자를 보려면 최소 하나 이상의 작업 역할과 연결되어 있어야 합니다.
   >
   >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (선택 사항) 업데이트를 비공개로 설정하려면 을 활성화합니다 **내 회사에 비공개** 업데이트 상자의 오른쪽 아래 모서리에 있습니다. 이렇게 하면 회사의 사용자에게만 업데이트가 표시됩니다. 다음 **내 회사에 비공개** 옵션은 회사가 Workfront 프로필에 지정된 경우에만 사용할 수 있습니다.

   >[!NOTE]
   >
   >회사 외부의 태그 지정된 사용자는 업데이트 탭에 개인 댓글이 표시되지 않더라도 인앱 알림이나 이메일을 계속 받을 수 있습니다. 외부 사용자와 정보를 공유하지 않으려면 업데이트에 외부 사용자에게 태그를 지정하지 않는 것이 좋습니다.

1. (선택 사항) 여러 사용자와 팀을 추가하려면 2단계를 반복합니다.

   >[!NOTE]
   >
   >알림 필드에 나열된 모든 사용자 및 팀원은 업데이트에 대한 인앱 알림을 받으며 이메일 알림 설정의 구성에 따라 이메일을 받을 수 있습니다. 댓글 또는 회신에 태그를 지정한 사용자는 해당 댓글 또는 회신에 대한 알림을 받으며 스레드의 나머지 부분에 대해 알림 필드에서 자신의 이름을 볼 수 있지만 다시 태그 지정하지 않는 한 다른 알림을 받지 않습니다. 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 및 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 클릭 **업데이트**.\
   업데이트에 포함된 사용자에게는 객체에 대한 보기 권한이 자동으로 부여되고 객체에 대한 업데이트를 보고 응답할 수 있습니다.

   업데이트 스레드의 맨 위에서 각 회신에서 누가 태그 지정되었는지 확인할 수 있습니다. 이러한 사용자는 오브젝트에 가입된 사용자와 함께 오브젝트에 대한 업데이트 또는 회신이 이루어질 때마다 알림을 받습니다.

   ![](assets/tagging-transparency-350x192.png)

   작업 항목을 업데이트할 때 사용할 수 있는 추가 기능에 대한 자세한 내용은 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



