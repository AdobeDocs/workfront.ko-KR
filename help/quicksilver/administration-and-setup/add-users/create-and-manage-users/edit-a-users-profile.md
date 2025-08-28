---
title: 사용자 프로필 편집
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 새 사용자를 만들고 기존 사용자의 프로필을 관리할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '3430'
ht-degree: 0%

---

# 사용자 프로필 편집

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Adobe Workfront 관리자는 사용자를 만들고 기존 사용자의 프로필을 관리할 수 있습니다. 사용자 만들기에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

사용자가 자신의 프로필을 업데이트하는 방법에 대한 자세한 내용은 [내 설정 구성](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)을 참조하십시오.

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
   <td><p>새로운 기능: 표준</p><p>또는</p><p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <b>에서 두 개의 </b>사용자 관리<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 프로필 편집

{{step-1-to-users}}

1. 사용자를 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   사용자 편집 상자가 표시됩니다.

1. **사용자 편집** 상자에서 모든 섹션의 정보를 변경한 다음 언제든지 **변경 내용 저장** <span class="preview"> 또는 **저장**</span>&#x200B;을 클릭합니다.

### 개인적인 정보

* **이름**
* **성**

  >[!NOTE]
  >
  >Workfront에서 사용자 이름을 편집해도 Adobe Admin Console에서 사용자 이름이 편집되지 않습니다.

* **전자 메일 주소**: 사용자의 전자 메일 주소도 Workfront의 사용자 이름입니다. 이 필드는 대/소문자를 구분하므로 고유해야 합니다. 사용자가 10분 내에 고유하지 않은 이메일 주소를 3번 추가하려고 하면 reCAPTCHA 응답이 나타납니다.

  계속하려면 **로봇이 아닙니다** 설정을 선택하십시오.

  허용 목록에 추가하다 전자 메일 도메인을 사용하고 목록에 없는 전자 메일 도메인을 입력하면 사용자에게 전자 메일 알림이 전송되지 않습니다. 허용 목록에 추가하다허용 목록에 추가하다 에 대한 자세한 내용은 [전자 메일 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)을 참조하십시오.

  조직이 Adobe Admin Console으로 마이그레이션된 경우 Workfront에서 사용자의 이메일 주소를 편집할 수 없습니다. 사용자의 이메일 주소는 Adobe Admin Console에서 설정됩니다.

* **암호 재설정** / <span class="preview">**암호 변경**</span>: 사용자의 암호를 재설정하려면 이 링크를 클릭하십시오. 다른 사용자의 암호를 재설정하려면 먼저 자신의 암호를 입력해야 합니다.

  다른 사용자의 암호를 재설정하려면 Workfront 관리자 또는 그룹 관리자여야 합니다.

  그룹 관리자인 경우 관리자로 지정된 그룹의 사용자에 대해서만 암호를 재설정할 수 있습니다. 또한 액세스 수준에서 사용자 관리(그룹 사용자) 권한을 활성화해야 합니다.

  ![사용자 관리자 액세스 수준 설정](assets/group-admin-user.png)

  이 설정은 기본적으로 비활성화되어 있습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

  Workfront 관리자의 암호를 재설정할 수 없습니다.

* **&lt;SSO 구성> 사용자 이름**: Workfront 관리자가 Workfront과의 SSO 통합을 사용하도록 설정한 경우 이 필드에 SSO 사용자 이름이 표시됩니다. Workfront 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다.
* **&lt;SSO 구성> 인증만 허용**: Workfront 관리자가 Workfront과의 SSO 통합을 사용하도록 설정하고 모든 사용자를 SSO로 업데이트한 경우 이 필드가 기본적으로 선택됩니다. Workfront 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다.

  이 필드를 선택하면 사용자는 SSO 자격 증명으로 Workfront에 로그인해야 합니다. 선택을 취소하면 Workfront 자격 증명으로 Workfront에 로그인할 수 있습니다.

  SSO 솔루션을 사용하여 Workfront을 구성하는 방법에 대한 자세한 내용은 [Adobe Workfront의 Single Sign-On 개요](/help/quicksilver/administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)를 참조하십시오.

  SSO용 사용자 업데이트에 대한 자세한 내용은 [SSO(Single Sign-On)용 사용자 업데이트](/help/quicksilver/administration-and-setup/add-users/single-sign-on/update-users-sso.md)를 참조하십시오.

  >[!NOTE]
  >
  >그룹 관리자인 경우 자신이 지정된 그룹의 사용자에 대해서만 &lt;SSO 구성> 필드를 편집할 수 있습니다. 또한 액세스 수준에서 사용자 관리(그룹 사용자) 권한을 활성화해야 합니다.
  >
  >그룹 관리자이고 액세스 수준에서 사용자 관리자(모든 사용자) 권한을 활성화한 경우 모든 사용자에 대한 &lt;SSO 구성> 필드를 편집할 수 있습니다.

* **프로필 사진**: **사진 업로드** / <span class="preview">**새로 업로드**</span>&#x200B;를 클릭하여 사용자의 프로필 사진을 로드합니다. JPG, GIF 또는 PNG 파일을 업로드할 수 있습니다. 파일 크기 제한은 4MB입니다.

  프로필 사진이 사용자의 아바타가 되고 사용자의 이름이 표시되는 모든 곳에서 Workfront 시스템 전체에 표시됩니다.

* **Job 정보**: 직책 등 직무에 대한 정보(**Title** 필드) 및 사용자가 담당해야 하는 전문 지식 영역(**나와 대화하기** 필드).
* **연락처 정보**: 사용자의 전화 번호(**전화 번호**, **내선)입니다.**, **휴대폰 번호** 필드) 및 주소(**주소**, **도시**, **상태**, **우편 번호** 및 **국가** 필드).

  사용자가 UUM(Unified User Management) 또는 IMS(Adobe Identity Management System)에 대해 활성화된 경우 연락처 정보 섹션의 **국가** 필드는 국가 코드 값(예: US, GB, IN)만 허용합니다.

### 환경 설정

* **시간대**: 사용자의 시간대입니다.

  사용자가 Workfront에서 시간대 간에 공동 작업하는 데 대한 자세한 내용은 [시간대 간에 작업](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)을 참조하세요.

* **전자 메일 로케일**: 사용자의 기본 전자 메일 로케일입니다. 이는 Workfront에서 이 사용자에게 제공되는 이메일의 숫자 및 날짜 형식에 영향을 줍니다.

  >[!NOTE]
  >
  >조직이 Adobe 통합 환경을 사용하는 경우 사용자의 언어 환경 설정은 Adobe 프로필에 저장되고 이메일 로케일은 사용되지 않습니다. 이러한 환경 설정에 액세스하는 방법에 대한 자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.

* **이 테스트 환경에서 전자 메일 받기**: 현재 로그인한 환경에서 전자 메일 알림을 받으려면 이 옵션을 선택하십시오.

  >[!NOTE]
  >
  >이 옵션은 미리보기 및 샌드박스 환경에서만 사용할 수 있습니다. 이메일 알림은 기본적으로 프로덕션 환경에서 활성화됩니다.

<!--* **Send work I assign to myself to my Working On tab**: This setting refers to a deprecated feature that has been removed from Workfront.-->

* **문서를 업로드할 때 자동으로 증명 생성**: 사용자가 업로드하는 문서에서 즉시 증명을 생성하려면 이 옵션을 선택하십시오.

### 알림

새 사용자에 대해 활성화해야 하는 이메일 알림을 선택합니다.

인스턴트 및 일별 다이제스트 알림을 선택할 수 있습니다.

자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

### 액세스

* **활성 상태입니다** / <span class="preview">**사용자가 활성 상태입니다**</span>: 사용자가 활성 상태임을 나타내려면 이 옵션을 활성화하십시오. 활성 사용자는 Workfront 라이선스를 사용합니다. 필드를 비활성화하면 사용자가 Workfront에 로그인할 수 없습니다.

* **액세스 수준**: 이 사용자에게 할당할 액세스 수준을 선택하십시오.

  사용자에게 액세스 수준을 할당할 때 자신의 액세스 수준과 같거나 낮은 수준을 할당할 수 있습니다. (예를 들어 액세스 수준이 표준인 경우 관리자 액세스 수준을 할당할 수 없습니다.)

  하지만 Workfront 관리자가 자신의 액세스 수준에서도 활성화되지 않은 액세스 수준에 대해 기본이 아닌 권한을 활성화한 경우에는 기본적으로 자신의 액세스 수준보다 낮은 액세스 수준을 할당할 수 없습니다.

  예를 들어 작업을 삭제할 수 있는 액세스 권한이 없는 Standard 라이센스가 있는 경우 Light 라이센스가 Standard 라이센스보다 낮지만 작업을 삭제할 수 있는 액세스 권한이 있는 Light 라이센스를 다른 사용자에게 할당할 수 없습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

  액세스 수준에 대한 자세한 내용은 [Adobe Workfront 액세스 구성](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md)을 참조하십시오.

  >[!NOTE]
  >
  >조직에서 새 액세스 모델(표준/라이트/기여자)을 사용하는 경우 해당 사용자가 해당 월에 대한 결정 한도에 이미 도달한 경우 표준 또는 라이트 사용자를 기여자 액세스 수준에 재할당할 수 없습니다.
  >
  >새 액세스 모델에 대한 자세한 내용은 [새 액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)를 참조하십시오.
  >
  >결정 한도에 대한 자세한 내용은 [비유료 사용자에 대한 제한된 문서 및 증명 결정 개요](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)를 참조하십시오.

* **레이아웃 템플릿**: 사용자에 대한 레이아웃 템플릿을 선택합니다. 이 레이아웃 템플릿은 사용자의 홈 그룹, 홈 팀 또는 기본 역할에 할당된 모든 레이아웃 템플릿보다 우선합니다. 레이아웃 템플릿의 할당 우선 순위에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

  다음 목록은 이 필드에서 사용할 수 있는 템플릿 목록이 액세스 권한에 따라 어떻게 달라지는지 설명합니다.

   * Workfront 관리자는 모든 시스템 수준 및 그룹 수준 레이아웃 템플릿을 볼 수 있습니다.
   * 그룹 관리자는 시스템 수준 레이아웃 템플릿과 관리하는 그룹과 관련된 템플릿을 볼 수 있습니다.
   * Standard 또는 Plan 라이선스가 있고 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준 레이아웃 템플릿만 볼 수 있습니다.

     그룹 수준 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

### 조직

* **회사**: 사용자의 회사입니다. 사용자는 한 회사에만 연결할 수 있습니다. 회사를 사용자와 연결하려면 먼저 회사를 만들어야 합니다. 활성 회사만 목록에 표시됩니다. 회사 만들기에 대한 자세한 내용은 [회사 만들기 및 편집](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.
* **보고 대상**: 사용자를 위해 회사를 지정한 경우 이 필드에 사용자의 직접 관리자를 지정할 수도 있습니다. 사용자에게는 한 명의 관리자만 있을 수 있습니다. 사용자가 회사와 먼저 연결되어 있지 않으면 이 필드가 표시되지 않습니다.
* **부하 직원**: 사용자를 위해 회사를 지정한 경우 사용자의 부하 직원도 지정할 수 있습니다. 사용자는 여러 부하 직원을 보유할 수 있습니다. 사용자가 회사와 먼저 연결되어 있지 않으면 이 필드가 표시되지 않습니다.
* **홈 팀**: 사용자의 홈 팀을 지정합니다. 사용자는 홈 팀을 하나만 보유할 수 있습니다. 홈 팀은 레이아웃 템플릿을 할당할 때 또는 사용자에게 할당된 작업 및 문제에 대한 처리 중 단추를 정의할 때 중요합니다.
* **다른 팀**: 사용자가 여러 팀에 속할 수 있습니다. 사용자는 홈 영역에서 팀에 할당된 작업 항목을 볼 수 있습니다.
* **홈 그룹** / <span class="preview">**현재 홈 그룹**</span>: 사용자를 할당할 적절한 그룹을 선택하십시오. 이를 통해 사용자는 그룹과 공유되는 객체에 액세스할 수 있습니다. 사용자의 홈 그룹과 레이아웃 템플릿을 공유할 수도 있습니다.

  필수 필드입니다. 모든 사용자는 홈 그룹과 연결되어 있어야 합니다. 홈 그룹을 선택하지 않으면 홈 그룹이 새 사용자의 홈 그룹으로 할당됩니다.

  다음 중 하나가 참인 경우에만 사용자에게 그룹을 할당할 수 있습니다.

   * Workfront 관리자입니다
   * 그룹의 관리자입니다.
   * 그룹이 공개 그룹임

* **기타 그룹**: 사용자가 여러 그룹에 속할 수 있습니다. Workfront 관리자이거나 그룹의 관리자이거나 그룹이 공개인 경우에만 그룹을 사용자에게 할당할 수 있습니다.

  >[!IMPORTANT]
  >
  >100개가 넘는 그룹에 사용자를 추가하면 그룹 목록을 로드하는 Workfront 영역에서 성능 문제가 발생할 수 있습니다.

  공용 그룹에 대한 자세한 내용은 [그룹 만들기](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)를 참조하십시오.

  그룹에 대한 자세한 내용은 [그룹 개요](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md)를 참조하세요.

### 리소스 계획 수립

* **작업 시간**: 사용자가 오버헤드를 포함하지 않고 실제 작업에 사용할 수 있는 FTE(Full Time Equivalent) 시간의 백분율을 나타냅니다. 작업 시간은 최대 1의 10진수여야 하며 0일 수 없습니다. 예를 들어, 실제 작업에 대한 20% 가용성은 0.2입니다.

  필드의 기본값은 1이며, 사용자가 전체 FTE를 실제 프로젝트 관련 작업에 사용함을 나타냅니다.

  시스템은 이 숫자를 사용하여 실제 프로젝트 관련 작업에 대한 사용자의 가용성을 계산합니다.

  Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

  일정 예외 및 휴무는 사용자의 용량에 영향을 줄 수도 있습니다.

  Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다. 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

  >[!TIP]
  >
  >작업 시간 값을 1로 설정하면 사용자가 프로젝트 관련 작업에 전체 시간에 해당하는 전체 시간을 사용할 수 있음을 나타냅니다.

* **비활성화 예약** / <span class="preview">**비활성화 날짜 설정**</span>: 이 사용자를 특정 날짜 및 특정 시간에 비활성화하도록 예약하려면 이 확인란을 선택 / <span class="preview">이 단추를 클릭</span>하십시오.
* **예약된 비활성화 날짜** / <span class="preview">**비활성화 날짜**</span>: 사용자가 비활성화되는 날짜 및 시간입니다. 비활성화에 대한 사용자 예약에 대한 자세한 내용은 [사용자 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)에서 [비활성화에 대한 사용자 예약](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)을 참조하십시오.
* **기본 역할**: 사용자가 Workfront에서 수행할 수 있는 기본 작업 역할입니다. 사용자가 할당된 모든 작업 및 문제도 이 작업 역할에 할당됩니다. 작업 역할은 리소스 관리에서 필수적입니다. 관리자 액세스 권한이 있는 Standard 또는 Plan 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

  활성 작업 역할만 목록에 표시됩니다.

* (조건부) **기본 역할**&#x200B;을(를) 선택한 경우 **FTE 가용성의 백분율** 필드가 표시됩니다. 사용자의 일정 중 이 작업 역할에 할당되는 시간의 백분율을 지정합니다. 기본 역할에 대한 FTE 가용성 백분율의 기본값은 100%입니다.
* **다른 역할**: 사용자는 Workfront에서 여러 작업 역할을 가질 수 있습니다. 작업 역할은 리소스 관리에서 필수적입니다. 사용자가 이행할 수 있는 작업 역할 수에는 제한이 없습니다. 그러나 너무 많은 수의 작업 역할에 한 명의 사용자를 할당하지 않는 것이 좋습니다. 리소스 관리가 너무 복잡해질 수 있기 때문입니다.

  활성 작업 역할만 목록에 표시됩니다. 작업 역할에 대한 자세한 내용은 [작업 역할 만들기 및 관리](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

  관리자 액세스 권한이 있는 Standard 또는 Plan 라이선스가 있거나 Workfront 관리자인 경우에만 이 필드를 업데이트할 수 있습니다.

  관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

* (조건부) 하나 이상의 **다른 역할**&#x200B;을(를) 선택한 경우 각 역할에 대해 **FTE 가용성의 백분율** 필드가 표시됩니다. 사용자 일정이 각 작업 역할에 할당되는 시간의 백분율을 지정합니다. 다른 역할에 대한 FTE 가용성 백분율의 기본값은 0%입니다.

  다른 역할에 0% FTE 가용성이 있는 경우 사용자가 이러한 역할의 작업에 할당되지 않는 한 리소스 플래너에 표시되지 않습니다.

  미리 보기의 <span class="preview">다음 중:</span>
  ![사용자 역할 및 FTE](assets/user-roles-fte-2025.png)

  프로덕션:
  ![사용자 역할 및 FTE](assets/user-settings-roles-and-dte-boxes-rp-story.png)

  모든 역할에 대한 모든 **FTE 가용성의 백분율**&#x200B;의 합은 100%여야 합니다. FTE 가용성의 각 비율은 리소스 플래너의 사용자당 각 역할에 대한 가용 시간을 계산합니다. 사용자당 각 역할에 대한 사용 가능한 시간은 사용자의 사용 가능한 시간에 따라 다릅니다.

  Workfront 관리자가 리소스 관리 환경 설정에서 FTE를 계산하기 위해 선택한 방법에 따라 사용자의 사용 가능한 시간이 Workfront에서 계산됩니다.

  사용자 가용성의 계산에 대한 자세한 내용은 [리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)를 참조하십시오.

  리소스 관리 환경 설정 구성에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

  <span class="preview">(선택 사항) 프로젝트 중에 사용자의 작업 역할이 변경된 경우 재무 계산에 유효 날짜 작업 역할 할당이 사용됩니다.</span>

  <span class="preview">**날짜별로 역할 정의**&#x200B;를 클릭하고 **기본 역할** 및 **다른 역할**&#x200B;을 선택한 다음 각 역할에 대한 할당 비율을 입력합니다. 역할은 기존 역할(다른 백분율 사용)과 동일하거나 새 역할일 수 있습니다. 이러한 역할이 활성화된 시작 날짜를 선택합니다. 미래의 날짜가 될 수 있습니다. 최신 역할이 활성화되면 **이전 역할 표시**&#x200B;를 클릭하여 이전의 비활성 역할을 볼 수 있습니다.</span>

* **일정**: 일정을 사용자와 연결합니다. 사용자의 일정은 사용자가 할당된 작업의 타임라인을 계산합니다.

  일정을 사용자와 연결하려면 먼저 일정을 만들어야 합니다. 일정 만들기에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하세요.

  >[!NOTE]
  >
  >사용자와 연결하는 일정이 사용자의 시간대와 일치하는 것이 좋습니다.

  >[!IMPORTANT]
  >
  >Workfront은 **리소스 가용성 계산** 설정이 **사용자의 일정**(으)로 설정된 경우에만 사용자의 일정을 사용합니다. 이 설정이 리소스 관리에 사용되는 일정에 영향을 주는 방법에 대한 자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

* **타임시트 프로필**: 타임시트가 자동으로 생성되도록 타임시트 프로필을 사용자와 연결합니다.

  이 필드에서 사용할 수 있는 프로필 목록은 액세스 권한에 따라 다릅니다.

   * Workfront 관리자는 모든 시스템 수준 및 모든 그룹 수준의 타임시트 프로필을 볼 수 있습니다.
   * 그룹 관리자는 시스템 수준의 타임시트 프로필과 관리하는 그룹과 관련된 프로필을 볼 수 있습니다.
   * 표준 또는 플랜 라이선스가 있고 사용자 편집 액세스 권한이 있는 사용자는 시스템 수준의 타임시트 프로필만 볼 수 있습니다. 그룹 수준 타임시트 프로필에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

* **기본 시간 유형**: 사용자의 기본 시간 유형을 선택합니다. 사용자가 시간을 기록할 때 기본적으로 사용되는 시간 유형입니다.
* **사용 가능한 시간 유형**: 사용자가 사용할 수 있는 시간 유형을 선택합니다. 이러한 시간 유형은 사용자가 시간을 기록할 수 있는 Workfront의 모든 곳에서 볼 수 있습니다. 사용자는 프로젝트 수준과 사용자 수준에서 활성화된 시간 유형만 볼 수 있습니다. 사용자가 사용할 수 있는 시간 유형에 대한 자세한 내용은 [시간 유형 및 가용성 정의](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)를 참조하십시오.
* **시간 기록**: 사용자가 작업 항목에 시간을 몇 시간 또는 며칠 내에 기록할지 여부를 선택합니다. 자세한 내용은 [시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성](/help/quicksilver/timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)을 참조하십시오.
* **FTE**: 사용자의 FULL TIME입니다. Workfront은 시스템 수준의 리소스 관리 기본 설정이 기본 일정으로 설정된 경우에만 이 숫자를 사용하여 기본 일정을 기준으로 사용자의 가용성을 계산합니다.

  FTE는 사용자가 직장에서 보낼 수 있는 시간을 나타냅니다. 여기에는 간접비와 프로젝트 작업에 소비된 시간이 포함됩니다. 예를 들어, 회의나 교육에서 보내는 시간도 FTE에 포함됩니다.

  FTE는 최대 1까지의 십진수여야 하며 0일 수 없습니다. 예를 들어 FTE 값이 0.5이고 Workfront의 기본 일정이 40시간인 경우 사용자는 일주일에 20시간 동안 사용할 수 있습니다.

  필드의 기본값은 1입니다.

  일정 예외, 휴무 및 작업 시간 값은 사용자의 가용성에 영향을 줄 수 있습니다.

  Workfront은 설정 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다.

  시스템 수준의 리소스 관리 기본 설정이 사용자 일정으로 설정된 경우 여기에서 지정한 값이 무시되며 사용자는 일정에 지정된 내용에 따라 사용할 수 있는 것으로 간주됩니다.

  자세한 내용은 [리소스 관리 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하십시오.

  Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 [일정 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오.

* **리소스 풀**: 사용자를 리소스 풀과 연결합니다. 자세한 내용은 [사용자와 리소스 풀 연결](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)을 참조하세요.
* **비용 비율**: 사용자의 시간당 비용입니다.

  날짜 유효 비용 요율을 보려면 **요율 추가**&#x200B;를 클릭하십시오. 기간에 대한 원가율 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 원가율 1에는 시작 일자가 없고 최종 원가율에는 종료 일자가 없습니다.

  일부 날짜는 자동으로 추가됩니다. 예를 들어, 원가 환율 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 원가 환율 2를 추가하면, 종료 일자가 2023년 4월 30일로 원가 환율 1에 추가되므로 간격이 없습니다.

* **청구 요금**: 사용자의 시간당 청구 금액입니다.

  날짜 유효 청구 요금을 보려면 **요금 추가**&#x200B;를 클릭하십시오. 기간에 대한 청구 요금의 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 청구 요금 1에는 시작 일자가 없으며 마지막 청구 요금에 종료 일자가 없습니다.

  일부 날짜는 자동으로 추가됩니다. 예를 들어 청구 요금 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 초를 추가하는 경우, 2023년 4월 30일인 종료 일자가 청구 요금 1에 추가되므로 간격이 없습니다.

  미리 보기의 <span class="preview">다음 중:</span>
  ![사용자 비용 및 청구 요금](assets/user-cost-billing-rates-2025.png)

  프로덕션:
  ![사용자 비용 및 청구 요금](assets/edit-user-cost-billing-rate-2.png)

### 사용자 정의 양식

기존 사용자 정의 양식을 이 사용자와 연결합니다. 사용자 정의 양식을 사용자와 연결하려면 먼저 사용자 정의 양식을 만들어야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다. 편집 액세스 권한이 없는 필드는 개별 사용자 정의 양식에 표시되지 않습니다.

>[!NOTE]
>
>외부 조회 필드 및 Workfront 기본 필드와 같은 고급 사용자 정의 양식 기능은 사용자 편집 대화 상자가 아닌 세부 정보 페이지에서 사용자 레코드를 열 때만 사용할 수 있습니다. (사용자 목록에서 사용자 이름을 클릭하여 세부 정보를 엽니다.)

사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### 댓글

사용자 및 해당 사용자 프로필의 업데이트 영역에 보낼 설명을 입력합니다.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personal Info </td> 
      <td> 
       <ul> 
        <li><p><b>First Name</b></p></li>
        <li><p><b>Last Name</b></p><p><b>NOTE:</b></p><p>Editing a user's name in Workfront does not edit the user's name in the Adobe Admin Console.</p></li> 
        <li> <p><b>Email Address:</b> The email address for a user is also their username in Workfront. This field is case-sensitive and must be unique. If any user attempts to add a non-unique email address 3 times within a 10-minute window, a reCAPTCHA response appears.</p> <p> Select the <b>I am not a robot</b> setting before you can proceed.</p><p>If you use the email allowlist and enter an email domain not on the list, the user will not receive email notifications. For more information about the allowlist, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configure your email allowlist</a>.</p><p>If your organization has been migrated to the Adobe Admin Console, you cannot edit a user's email address in Workfront. The user's email address is set in the Adobe Admin Console. </li> 
        <li> <p><b>Reset Password</b>: Click this link to reset the user's password. You must enter your own password before you can reset another user's password.</p> <p>To reset another user's password, you must be a Workfront administrator, or a group administrator.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>If you are a group administrator, you can reset passwords only for users in the groups where you are designated as an administrator. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
           <li> <p>You cannot reset the password of a Workfront administrator.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Username</b>: If your Workfront administrator enabled an SSO integration with Workfront, the SSO Username displays in this field. The type of SSO configuration enabled for your Workfront instance is visible in this field. </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt; Authentication</b>: If your Workfront administrator enabled an SSO integration with Workfront and has updated all users for SSO, this field is selected by default. The type of SSO configuration enabled for your Workfront instance is visible in this field.</p> <p>When this field is selected, the user is required to log into Workfront with their SSO credentials. Unchecking it will allow them to log in to Workfront with their Workfront credentials.</p> <p>For more information about configuring Workfront with an SSO solution, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> If you are a group administrator, you can edit the &lt;SSO Configuration&gt; fields only for users in the groups where you are designated as such. Also, the User Admin (Group Users) permission must be enabled in your access level.
        <p>If you are a group administrator and you have the User Admin (All Users) permission enabled in your access level, you can edit the &lt;SSO Configuration&gt; fields for all users.</p> </li> 
        <li><b>Job Info:</b> Information about the job, like the job title (in the <b>Title</b> field), and what area of expertise the user is responsible for (in the <b>Talk to Me About</b> field).</li> 
        <li><p><b>Contact Info</b>: The user's phone number (in the <b>Phone number, Ext.</b>, and <b>Mobile number</b> fields) and address (in the <b>Address, City, State, Postal Code, Country</b> fields ).</p>
        <p>If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the <b>Country</b> field in the Contact Info section only accepts country code values (for example, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferences </td> 
      <td> 
       <ul> 
      <li> <p><b>Time Zone:</b> The user's time zone.</p> <p>For information about helping users collaborate in Workfront across time zones, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </li>

      <li><p><b>Email Locale</b>: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.</p>
      <p><b>NOTE:</b> When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li> 
      
      <li><b>Receive emails from this test environment</b>: Check this option if you want to receive email notifications from the environment that you are currently logged in.
      <p><b>NOTE</b></p>
      <p>This option is available only in the Preview and Sandbox environments. Email notifications are enabled in the Production environment by default. </p>
      </li> 
      
      </li> 
       <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       <li><b>Automatically generate proofs when uploading documents</b>: Check this option if you want the documents that the user uploads to immediately generate a proof. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Select the email notifications which should be enabled for the new user.</p> <p>You can select instant as well as daily digest notifications.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
      <li><b>Is Active:</b> Select this box to indicate that the user is active. Active users use a Workfront license. Clearing the box deactivates the user and prevents them from logging in to Workfront.</li> 
       <li> <p><b>Access Level:</b> Select the access level to assign to this user.</p> 
       <p>When you assign an access level to a user, you can assign a level equal to or lower than your own access level.</p>
       <p>For example, if your access level is Plan, you cannot assign the Administrator access level. However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level. </p>
       <p>For example, if you have a Plan license with no access to delete tasks, you cannot assign someone a Work license with access to delete tasks, although the Work license is lower than the Plan license. For more information, see  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> 
       <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month. </p><p>For more information on the new access model, see <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a>. </p><p>For information on decision limits, see <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Limited document and proof decision for non-paid users overview</a>.</p></li> 
       <li> <p><b>Layout Template</b>: Choose a Layout Template for the user. This Layout Template takes precedence over any Layout Template assigned to the user's Home Group, Home Team or Primary Role. For more information about the assignment priority of Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> <p><b>NOTE</b>:  <p>The following list describes how the list of templates you have available in this field depends on your access:</p> 
       <ul> 
       <li>As a Workfront administrator, you can see all system-level and group-level Layout Templates.</li> 
       <li>As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.</li> 
       <li>As a user with a Plan license and access to edit users, you can see only system-level Layout Templates.</li> 
       </ul> <p>For more information about group-level Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization </td> 
      <td> 
       <ul> 
      <li><b>Company</b>: The company of the user. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</li> 
      <li><b>Reports to:</b> If you specified a company for the user, you can also specify the direct manager of the user in this field. A user can have only one manager. This field does not display if the user is not associated with a company first. </li> 
      <li><b>Direct Reports:</b> If you specified a company for the user, you can also specify the direct reports of the user. A user can have multiple direct reports. This field does not display if the user is not associated with a company first.</li> 
      <li><b>Home Team</b>: Specify the home team for the user. Users can only have one home team. The Home Team is important when assigning a layout template or when defining the Work On It button for the tasks and issues assigned to the user. </li> 
      <li><b>Other Teams</b>: Users can belong to multiple teams. A user can view work items assigned to any of their teams in their Home area. </li> 
      <li> <p><b>Home Group:</b> Select an appropriate group to assign the user. This gives the user the ability to access objects that are shared with the group. You can also share layout templates with the user's Home Group.</p> <p>This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the new user's Home Group.</p> <p><b>NOTE</b>:</p> 
      <p> You can assign a group to a user only if one of the following is true:</p>
      <ul><li>you are a Workfront administrator</li>
      <li>you are the administrator of the group</li>
      <li>the group is public.</li></ul> 
      <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.</p> <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning </td> 
      <td> 
       <ul>
       <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.  

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user's capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 
      <li> <b>Schedule Deactivation</b>: Check this box if you want to schedule this user to be deactivated on a certain date and at a certain time. </li> 
       <li><b>Scheduled Deactivation Date</b>: The date and time on which the user becomes deactivated. For information about scheduling users for deactivation, see the <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that the user can fulfill in Workfront. Every task and issue that the user is assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Only active job roles display in the list. </p> </li> 
       <li>If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the user's schedule is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%. </li> 
       <li> <p><b>Other Roles</b>: A user can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.<p>Only active job roles display in the list. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. <br>For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the user's schedule is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>The sum of all <b>Percentages of FTE Availability</b> for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </p>
       <span class="preview"><p>(Optional) Date effective job role assignments are used in financial calculations if the user's job role changes during a project.</p><p>Click <b>Define roles by date</b>, select the <b>Primary Role</b> and <b>Other Roles</b>, and enter the allocation percentage for each role. The roles could be the same as the existing roles (using different percentages), or new roles. Select the <b>Start date</b> when these roles become active. This can be a future date. When the newest roles become active, you can click <b>Show previous roles</b> to see the previous, inactive roles.</p> </li></span>
       <li> <p><b>Schedule</b>: Associate a schedule with the user. The schedule of the user calculates the timeline of the tasks the user is assigned to.</p> <p>You must create a schedule before you can associate it with a user. For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>NOTE</b>: We recommend that the schedule you associate with the user matches the user's Time Zone.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the user to ensure that timesheets generate automatically for the user.</p> <p><b>NOTE</b>:  The list of profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.</li>
       <li>As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.</li>
       <li>As a user with a Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Create, edit, and assign timesheet profiles</a>.</li>
      </ul></p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the user. This is the hour type that is used by default when the user logs time.</li> 
       <li><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the user can log time. A user can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</li> 
       <li><b>Log Time in:</b> Select whether the user should log time on work items in hours or days. For more information, see <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure whether time is logged in hours or days</a>.</li>
       
      <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
      
      <li><b>Resource Pools</b>: Associate the user with Resource Pools. For more information, see <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</li> 
      
      <li><b>Cost Rate</b>: The amount of cost per hour for the user.
      <p>For date effective cost rates, click <strong>Add Rate</strong>. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.</p><p>Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.</p></li> 
      
      <li><b>Billing Rate</b>: The amount of billing per hour for the user.
      <p>For date effective billing rates, click <strong>Add Rate</strong>. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.</p><p> <img alt="User cost and billing rates" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td><p>Associate an existing user custom form with this user. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)</p> <p>For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Create a custom form</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comment</td> 
      <td>Type the comment you want to send to the users and to the Updates area of their user profiles.</td> 
     </tr> 
    </tbody> 
   </table>
-->
