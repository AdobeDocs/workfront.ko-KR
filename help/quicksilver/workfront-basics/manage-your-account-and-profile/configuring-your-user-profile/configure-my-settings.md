---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: 내 설정 구성
description: ' [!DNL Adobe Workfront] 프로필에 사용자 자신에 대한 정보(예: 이름, 전자 메일 주소, 주소, 전화 번호, 직함 등)가 포함되어 있습니다.  [!DNL Workfront]  및 회사의 다른 사용자와의 상호 작용에 대한 정보도 포함되어 있습니다.'
author: Becky
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: fb555df123701c62e9a0f2d451ad6dcd16586595
workflow-type: tm+mt
source-wordcount: '3318'
ht-degree: 1%

---

# 내 설정 구성

<!-- Audited: 01/2024 -->

<!--
<p>Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

[!DNL Adobe Workfront] 프로필에 사용자 자신에 대한 정보(예: 이름, 전자 메일 주소, 주소, 전화 번호, 직함 등)가 포함되어 있습니다. 여기에는 [!DNL Workfront] 및 회사의 다른 사용자와의 상호 작용에 대한 정보도 포함되어 있습니다(예: 알림 설정, [!DNL Workfront]에 표시할 탭 또는 작업 역할, 관리자 및 그룹 및 팀 멤버십).

이 정보 중 대부분은 [!DNL Workfront] 계정을 만들 때 [!DNL Workfront] 관리자가 이미 설정했습니다.

[!DNL Workfront]의 액세스 수준에 따라 [!UICONTROL 내 설정] 영역을 구성하여 이 정보 중 일부를 편집할 수 있습니다.

## 액세스 수준이 [!UICONTROL 내 설정] 영역 편집에 미치는 영향

사용 중인 액세스 수준에 따라 [!UICONTROL 내 설정] 영역에서 섹션을 편집할 수도 있고 편집할 수 없을 수도 있습니다.

액세스 수준에서 구성되거나 구성되지 않을 수 있는 다른 설정에 따라 편집 가능한 섹션에 포함된 일부 필드를 편집할 수 없습니다. [!UICONTROL 내 설정]에서 찾은 일부 필드를 편집하는 데 필요한 추가 액세스에 대한 자세한 내용은 [내 설정 구성[!UICONTROL 내 설정] 영역 구성](#configuring-the-my-settings-area)의 섹션을 참조하십시오.

액세스 수준을 확인하려면 [!DNL Workfront] 관리자에게 문의하십시오.

다음 표에는 액세스 수준에 따라 [!UICONTROL 내 설정] 영역에 표시되거나 편집할 수 있는 섹션이 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!UICONTROL 내 설정] 영역</strong> </th> 
   <th><strong>표시 또는 편집 가능</strong> </th> 
   <th><strong>[!UICONTROL 시스템 관리자]</strong> </th> 
   <th><strong>[!UICONTROL Standard] 또는 [!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Light] 또는 [!UICONTROL 검토자]</strong> </th> 
   <th><strong>[!UICONTROL 기여자] 또는 [!UICONTROL 요청자]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL 개인 정보]</td> 
   <td> <p>표시</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>편집 가능</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL 환경 설정]</td> 
   <td> <p>표시</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>편집 가능</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Notifications]</td> 
   <td> <p>표시</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>편집 가능</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL 액세스]</td> 
   <td>표시</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>편집 가능</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL 조직]</td> 
   <td>표시</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>편집 가능</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Resource Planning]</td> 
   <td>표시</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>편집 가능</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL 사용자 지정 Forms]</td> 
   <td>표시</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>편집 가능</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Comment]</td> 
   <td>표시</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>편집 가능</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 내 설정] 영역 구성 중

{{step1-click-profile-pic}}

1. 이름 옆에 있는 **[!UICONTROL 기타]** 메뉴를 클릭한 다음 ![기타 메뉴](assets/more-icon.png)를 클릭하고 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

1. 액세스 수준에 따라 다음 섹션을 업데이트할 수 있습니다.

   * [개인적인 정보](#personal-info)
   * [환경 설정](#preferences)
   * [알림](#notifications)
   * [액세스](#access)
   * [조직](#organization)
   * [리소스 계획 수립](#resource-planning)
   * [사용자 정의 양식](#custom-form)
   * [댓글](#comment)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

### [!UICONTROL 개인 정보]

이 섹션에는 다음 하위 섹션이 포함됩니다.

* [기본 정보](#basic-info)
* [직업 정보](#job-info)
* [연락처 정보](#contact-info)

#### [!UICONTROL 기본 정보]

이 정보는 [!DNL Workfront] 관리자가 미리 구성해야 합니다. 이 하위 섹션의 모든 필드는 필수 필드입니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL First Name]</strong></td> 
   <td>이름을 업데이트합니다. 필수 필드입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 성]</strong></td> 
   <td>성을 업데이트하십시오. 필수 필드입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 이메일 주소]</strong></td> 
   <td> 이메일 주소를 업데이트합니다. 필수 필드입니다. 전자 메일 주소도 [!DNL Workfront]의 사용자 이름입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 암호 변경]</strong></td> 
   <td>이 섹션에서 암호를 재설정합니다. 암호 재설정에 대한 자세한 내용은 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">암호 재설정</a>을 참조하세요.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) &lt;SSO 구성&gt; [!UICONTROL 사용자 이름]</strong></td> 
   <td> [!DNL Workfront] 관리자가 [!DNL Workfront]과(와) SSO 통합을 사용하도록 설정한 경우 SSO 사용자 이름이 이 필드에 표시됩니다. [!DNL Workfront] 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL &lt;SSO 구성&gt; 인증만 허용]</strong></td> 
   <td> <p> [!DNL Workfront] 관리자가 [!DNL Workfront]과(와) SSO 통합을 사용하도록 설정하고 SSO를 위해 사용자를 업데이트한 경우 기본적으로 이 필드가 선택됩니다. [!DNL Workfront] 인스턴스에 대해 활성화된 SSO 구성 유형이 이 필드에 표시됩니다.</p> <p>이 필드를 선택하면 SSO 자격 증명으로 [!DNL Workfront]에 로그인해야 합니다. 선택을 취소하면 [!DNL Workfront] 자격 증명으로 [!DNL Workfront]에 로그인할 수 있습니다.</p> <p>SSO 솔루션을 사용하여 [!DNL Workfront]을(를) 구성하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">[!DNL Workfront]의 Single Sign-On: 문서 인덱스</a>을(를) 참조하십시오. SSO용 사용자 업데이트에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">SSO(Single Sign-On)용 사용자 업데이트</a>를 참조하십시오.</p> </td> 
  </tr>
 </tbody> 
</table>

#### [!UICONTROL 작업 정보]

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Title]</strong></td>
        <td>제목을 지정합니다. 이 작업은 작업 역할과 다릅니다. 제목은 리소스 예약의 일부가 아니지만 작업 역할은 입니다. 제목은 이름과 아바타가 표시되는 모든 곳에서 [!DNL Workfront] 인터페이스에 표시됩니다. 사용자 프로필을 볼 수 있는 액세스 권한이 있는 모든 사용자가 볼 수 있습니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 설명 내용]</strong></td>
        <td>이 필드에 전문적인 관심사를 지정하십시오.</td>
    </tr>
</table>

#### [!UICONTROL 연락처 정보]

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 전화 번호]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Extension]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Mobile Number]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 주소]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 상태]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 우편 번호]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 국가]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 프로필 사진]</strong></td>
        <td>프로필 사진이 아바타가 되어 이름이 표시되는 모든 곳에서 [!DNL Workfront] 시스템 전체에 표시됩니다.</td>
    </tr>
</table>

### [!UICONTROL 환경 설정]

이 섹션에서 [!DNL Workfront] 인터페이스에 표시할 내용을 지정하십시오.

>[!NOTE]
>
>[!UICONTROL 기여자] 또는 [!UICONTROL 요청자] 라이선스를 가진 사용자에게 [!UICONTROL 요청] 영역 외부에서 [!UICONTROL 기본 메뉴]에 추가할 수 있는 다른 왼쪽 패널 항목이 없습니다. [!DNL Workfront] 관리자는 [!UICONTROL 기여자] 또는 [!UICONTROL 요청자] 라이선스가 있는 사용자를 [!UICONTROL 기본 메뉴]의 다른 모든 영역을 포함하는 레이아웃 템플릿에 할당할 수 있습니다. 그런 다음 사용자 프로필을 편집하여 [!UICONTROL 기본 메뉴]에 표시할 영역을 선택할 수 있습니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 시간대]</strong> </td> 
   <td><p>표준 시간대를 지정합니다. 보내는 이메일 메시지에 표시되는 시간을 제어합니다.</p>
       <p>시간대는 PTO 달력 보고서에 표시되는 내용에도 영향을 줍니다.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 전자 메일 로케일]</strong> </td> 
   <td><p>여기에서 원하는 언어를 지정하십시오. 발신 전자 메일 메시지에 사용되는 언어, 날짜 및 숫자 형식을 제어합니다.</p>
   <p><strong>참고:</strong> 조직에서 Adobe 통합 환경을 사용하는 경우 언어 환경 설정은 Adobe 프로필에 저장되고 전자 메일 로케일은 사용되지 않습니다. 자세한 내용은 문서 <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md#change-the-adobe-experience-cloud-language">Adobe Experience Cloud에서 지원되는 언어</a>에서 <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md">Adobe Workfront 언어 변경</a>을 참조하십시오.</p></td> 
  </tr>
  <tr><td><strong>[!UICONTROL 작업이 자동으로 할당되면 작업 상태를 진행 중으로 자동 설정합니다.]</strong> </td>
  <td>자신에게 할당한 작업 상태를 새로 만들기 대신 진행 중으로 자동 설정하려면 이 옵션을 선택합니다.</td>
  </tr>
  <tr> 
   <td role="rowheader"><strong>(조건부) 문서 업로드 시 증명을 자동으로 생성합니다</strong></td> 
   <td>문서가 [!DNL Workfront]에 로드된 후 바로 증명 생성을 시작하려면 이 필드를 선택하십시오. 이 필드는 기본적으로 비활성화되어 있으며 Workfront 관리자만 업데이트할 수 있습니다.<br>이 필드는 회사에서 Workfront용 Workfront Proof 구성 요소를 구입한 경우와 증명 사용자로 활성화된 경우에만 사용할 수 있습니다. Workfront Proof에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Adobe Workfront에서 증명 관리</a>를 참조하십시오.
   <p><b>참고:</b> 요청에 업로드된 문서는 증명을 자동으로 생성하지 않습니다. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 알림]

[!DNL Workfront]에서 받을 알림을 지정하십시오. 알림 구성에 대한 자세한 내용은 [전자 메일 알림 수정](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

### [!UICONTROL 액세스]

계정이 설정되면 [!DNL Workfront] 관리자가 액세스 및 해당 계정과 연결된 다른 구성 요소를 구성했습니다.

[!DNL Workfront] 관리자만 이 섹션의 모든 필드를 보고 편집할 수 있습니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL이 활성 상태입니다]</strong> </td> 
   <td>이 필드는 [!DNL Workfront] 관리자이기도 한 사용자만 볼 수 있으며 기본적으로 활성화되어 있어야 합니다. 사용자가 활성 상태로에 로그인할 수 있음을 의미합니다. [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 액세스 수준]</strong> </td> 
   <td>이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL Workfront 관리자] 액세스 수준이 있는 사용자에게 표시되며 [!DNL Workfront] 관리자만 편집할 수 있습니다. [!DNL Workfront] 관리자인 경우 이 필드를 수정할 때 액세스 수준을 더 낮은 수준으로 변경하지 않도록 주의하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 레이아웃 템플릿]</strong> </td> 
   <td>이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL [!DNL Workfront] 관리자] 액세스 수준이 있는 사용자에게 표시되며, 관리자 액세스 권한도 있는 [!UICONTROL [!DNL Workfront] 관리자] 또는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스를 가진 사용자만 편집할 수 있습니다. 여기에서 레이아웃 템플릿을 선택하여 Workfront 인터페이스의 룩과 필드를 업데이트합니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">사용자 액세스 권한 부여</a>에서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자 액세스 수준을 사용하여 사용자를 편집하도록 사용자 액세스 권한 구성</a>을 참조하십시오.<br>레이아웃 템플릿 및 이러한 템플릿이 인터페이스에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>를 참조하십시오.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 사용자가 증명을 생성할 수 있음(... 증명 라이선스 중... 남아 있음)]</strong></td> 
   <td>이 필드는 회사에서 레거시 [!DNL Workfront] 패키지를 사용하고 [!DNL Workfront Proof] 구성 요소를 구입한 경우에만 사용할 수 있습니다. 이 옵션을 선택하면 증명 사용자로 활성화됩니다. 구매한 총 증명 라이선스 수 중 시스템에 사용된 증명 라이선스 수도 표시됩니다. 이 필드는 [!DNL Workfront]명의 관리자이기도 한 사용자만 볼 수 있고 편집할 수 있습니다. [!DNL Workfront]에서 증명을 위한 플랜 옵션에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">증명 기능에 대한 액세스([!DNL Workfront]</a>)를 참조하십시오.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 권한 프로필]</strong></td> 
   <td> <p>이 필드에는 [!DNL Workfront Proof]의 액세스 수준이 표시됩니다. 다음 경우에만 사용할 수 있습니다.</p> 
    <ul> 
     <li>회사에서 레거시 [!DNL Workfront] 패키지를 사용하고 [!DNL Workfront Proof] 구성 요소를 구매했거나 최신 [!DNL Workfront] 패키지에 [!UICONTROL Standard], [!UICONTROL Work] 또는 [!UICONTROL Plan] 라이센스가 있습니다.</li> 
     <li>증명 사용자로 활성화되었습니다.</li> 
    </ul> <p>[!DNL Workfront] 관리자는 자신을 제외한 모든 사용자에 대한 필드를 편집할 수 있으므로 모든 사용자는 자신의 프로필에서 필드를 보기 전용으로 볼 수 있습니다. 권한 프로필에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">증명 권한 프로필 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 조직]

이 정보는 일반적으로 [!DNL Workfront] 관리자가 [!DNL Workfront] 계정을 만들 때 구성합니다. 이 섹션에서 조직 또는 조직 구조에 대한 정보를 업데이트할 수도 있습니다. [!UICONTROL 표준], [!UICONTROL 계획] 또는 [!UICONTROL 시스템 관리자] 액세스 수준이 있는 사용자만 이 섹션을 편집할 수 있습니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>드롭다운 목록에서 귀하가 속한 회사의 이름을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 보고 대상]</strong></td> 
   <td>프로필에 대해 <strong>[!UICONTROL Company]</strong>을(를) 선택한 후 이 필드에 관리자 이름을 지정할 수도 있습니다. 여기에서는 이름을 하나만 지정할 수 있으며, 직접 관리자의 이름을 지정하는 것이 좋습니다. 이름을 입력하고 목록에 표시될 때 클릭하여 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 부하 직원]</strong></td> 
   <td>프로필에 대해 <strong>[!UICONTROL Company]</strong>을(를) 선택한 후 이 필드에 부하 직원의 이름을 지정할 수도 있습니다. 여기에서 필요한 수만큼 직접 보고서를 지정할 수 있습니다. 이름을 입력하고 목록에 표시될 때 클릭하여 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 홈 팀]</strong> </td> 
   <td> <p>드롭다운 메뉴에서 <strong>[!UICONTROL 홈 팀]</strong>을(를) 선택합니다. 이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 액세스 수준이 있는 사용자에게 표시되며, 관리자 액세스 권한도 있는 [!DNL Workfront]명의 관리자 또는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스를 가진 사용자만 편집할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">사용자 액세스 권한 부여</a>에서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자 액세스 수준을 사용하여 사용자를 편집하도록 사용자 액세스 권한 구성</a>을 참조하십시오.<br></p> <p>레이아웃 템플릿이 팀과 연결되어 있는 경우 <strong>홈 팀</strong>이(가) [!DNL Workfront] 인터페이스의 모양과 느낌에 영향을 줄 수 있습니다. </p> <p>팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>를 참조하세요.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기타 팀]</strong> </td> 
   <td> <p>두 개 이상의 팀에 속할 수 있습니다. 팀 이름을 입력하여 이 필드에 속한 추가 팀을 지정한 다음, 목록에 표시될 때 클릭하여 선택합니다. 너무 많은 팀에 속해 있으면 팀에 할당된 작업에 대해 혼란이 발생할 수 있습니다. 팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>를 참조하세요.</p> <p>이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 라이선스가 있는 사용자에게 표시되며, [!DNL Workfront]명의 관리자 또는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스가 있고 관리 사용자 액세스 권한도 있는 사용자만 편집할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">사용자 액세스 권한 부여</a>에서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자 액세스 수준을 사용하여 사용자를 편집하도록 사용자 액세스 권한 구성</a>을 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 홈 그룹]</strong> </td> 
   <td> <p>드롭다운 메뉴에서 <strong>[!UICONTROL 홈 그룹]</strong>을(를) 선택합니다.</p> <p>참고: 필수 필드입니다. 그룹에 연결되지 않은 사용자를 가질 수 없습니다.<br></p> <p>이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 수준이 있는 사용자에게 표시됩니다. <strong>[!UICONTROL 홈 그룹]</strong> 필드를 편집할 수 있는 사용자에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">사용자 프로필 편집</a>을 참조하십시오. <strong>[!UICONTROL 홈 그룹]</strong>은(는) 모든 프로젝트의 기본 그룹이며, 새로 만드는 모든 사용자의 기본 <strong>[!UICONTROL 홈 그룹]</strong>입니다. 만든 모든 사용자 정의 양식은 기본적으로 <strong>[!UICONTROL 홈 그룹]</strong>과(와) 공유됩니다.</p> <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>를 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기타 그룹]</strong> </td> 
   <td> <p>여러 그룹에 속할 수 있습니다. 그룹 이름을 입력하여 이 필드에 속해 있는 추가 그룹을 지정합니다. 목록에 표시될 때 클릭하여 선택합니다. 이 필드는 [!UICONTROL Standard], [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 액세스 수준이 있는 사용자에게 표시됩니다. <strong>[!UICONTROL 기타 그룹]</strong> 필드를 편집할 수 있는 사용자에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">사용자 프로필 편집</a>을 참조하십시오.</p> <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>를 참조하세요.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 리소스 계획]

리소스 계획 정보는 작업 할당의 타임라인, 현재 진행 중인 프로젝트의 로그 시간, 비용 및 매출에 영향을 줍니다. 일반적으로 이 영역은 [!DNL Workfront] 관리자, 프로젝트 또는 리소스 관리자 또는 직접 관리자가 업데이트합니다.

이 섹션에서 다음 중 하나를 사용하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 비활성화 날짜 설정]</strong></td>
   <td><p>일정 시간이 지나면 계정을 비활성화하도록 예약하려면 이 단추를 클릭합니다. 표시되는 <strong>[!UICONTROL 예약된 비활성화 날짜]</strong>에서 계정이 비활성화되는 다음 날짜를 지정합니다. 사용자 비활성화에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>에서 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">비활성화 예약</a>을 참조하세요. </p><p>[!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스가 있거나 [!DNL Workfront] 관리자인 경우 계정의 비활성화 필드를 편집할 수 있습니다. </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기본 역할]</strong></td> 
   <td> <p>Workfront에서 수행할 수 있는 기본 작업 역할입니다. 할당된 모든 작업 및 문제도 기본적으로 이 작업 역할에 할당됩니다. 작업 역할은 리소스 관리에서 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>를 참조하십시오.</p> <p>관리자 액세스 권한이 있는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스가 있거나 [!DNL Workfront] 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">사용자 액세스 권한 부여</a>에서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자 액세스 수준을 사용하여 사용자를 편집하도록 사용자 액세스 권한 구성</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 기본 역할]을 선택한 경우 [!UICONTROL FTE 가용성 백분율] 필드가 표시됩니다.</strong></td> 
   <td>이 작업 역할에 할당된 예약 시간의 백분율을 지정합니다. 기본 역할에 대한 [!UICONTROL PERCENTAGE OF FTE Availability]의 기본값은 100%입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기타 역할]</strong> </td> 
   <td> <p>[!DNL Workfront]에서 여러 작업 역할을 가질 수 있습니다. 작업 역할은 리소스 관리에서 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>를 참조하십시오.</p> <p>관리자 액세스 권한이 있는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스가 있거나 [!DNL Workfront] 관리자인 경우에만 이 필드를 업데이트할 수 있습니다. 관리자 액세스 권한을 가진 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 액세스 권한 부여</a>에서 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자 액세스 수준을 사용하여 사용자를 편집하도록 사용자 액세스 권한 구성</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) 다른 역할을 하나 또는 여러 개 선택한 경우 각 역할에 대해 [!UICONTROL PERCENTAGE OF FTE Availability] 필드가 표시됩니다.</strong></td> 
   <td> <p>각 작업 역할에 할당되는 예약 시간의 백분율을 지정합니다. [!UICONTROL Other Roles]에 대한 [!UICONTROL PERCENTAGE OF FTE Availability]의 기본값은 0%입니다.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>참고:  
     <ul> 
      <li>[!UICONTROL 기타 역할]에 0% FTE 가용성이 있는 경우, 사용자가 이러한 역할의 작업에 할당되지 않으면 [!UICONTROL 리소스 플래너]에 표시되지 않습니다.</li> 
      <li> <p>모든 역할에 대한 모든 <strong>[!UICONTROL Percentage of FTE Availability]</strong>의 합은 100%여야 합니다. 각 [!UICONTROL PERCENTAGE OF FTE Availability]는 [!UICONTROL Resource Planner]의 사용자당 각 역할에 대해 [!UICONTROL Available Hours]를 계산합니다. </p> <p>사용자당 각 역할에 대한 [!UICONTROL 사용 가능한 시간]은 사용자의 사용 가능한 시간에 따라 다릅니다. [!DNL Workfront] 관리자가 [!UICONTROL 리소스 관리 환경 설정]에서 FTE를 계산하기 위해 선택한 메서드에 따라 [!DNL Workfront]에서 사용자의 사용 가능한 시간을 계산합니다. 사용자 가용성의 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>를 참조하십시오. 리소스 관리 환경 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>을 참조하십시오.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>예약</strong></td> 
   <td> <p>타임시트와 시간에 대한 관리 액세스 권한도 있는 [!DNL Workfront]명의 관리자 또는 [!UICONTROL Standard] 또는 [!UICONTROL Plan] 라이선스를 가진 사용자만 이 필드를 업데이트할 수 있습니다. 타임시트 및 시간 관리 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 사용자 관리 액세스 권한 부여</a>의 "타임시트 및 시간" 섹션을 참조하십시오.</p> <p>드롭다운 메뉴에서 올바른 타임시트를 선택합니다. 이렇게 하면 [!DNL Workfront] 관리자가 설정한 사양에 따라 타임시트가 자동으로 생성됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기본 시간 유형]</strong> </td> 
   <td>기본 시간 유형을 선택합니다. Workfront에 시간을 기록할 때마다 시스템에서 기본적으로 사용하는 시간 유형입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 사용 가능한 시간 유형]</strong> </td> 
   <td>시간을 기록할 때 선택할 수 있는 시간 유형을 선택합니다. [!DNL Workfront] 관리자가 이 드롭다운 메뉴의 시간 유형을 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 리소스 풀]</strong> </td> 
   <td>속해 있는 리소스 풀을 선택하십시오. 이 필드는 보고 및 정보 제공용으로만 사용됩니다. Tt는 자원 스케줄링 또는 계획에 영향을 주지 않습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>여기서 지정한 숫자는 시스템 수준의 [!UICONTROL 리소스 관리 환경 설정]이 <strong>[!UICONTROL 기본 일정]</strong>(으)로 설정된 경우에만 기본 일정에 따라 가용성을 계산하기 위해 고려됩니다.</p> <p>예를 들어 FTE 값이 0.5이고 [!UICONTROL 기본 일정]이 40시간이면 일주일에 20시간 동안 작업할 수 있습니다.</p> <p>시스템 수준의 [!UICONTROL 리소스 관리 환경 설정]이 <strong>[!UICONTROL The User's Schedule]</strong>(으)로 설정된 경우 여기서 지정한 값이 무시되며 일정에 지정된 내용에 따라 작업할 수 있습니다. 이 경우 [!UICONTROL Resource Planner]에 대한 FTE는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>사용자 FTE 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 플래너에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>를 참조하십시오.</p> <p>[!DNL Workfront]에서 일정을 만드는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">일정 만들기</a>를 참조하십시오.</p> <p>리소스 관리 환경 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 시간당 비용]</strong> </td> 
   <td>사용자의 시간당 비용 금액을 지정합니다. [!DNL Workfront]의 비용 추적에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>을 참조하세요. 액세스 수준에서 재무 데이터에 액세스할 수 있는 권한이 없거나 [!DNL Workfront] 관리자인 경우 이 정보를 업데이트할 수 없습니다. 재무 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 시간당 청구]</strong> </td> 
   <td>사용자의 시간당 청구 금액을 지정합니다. 청구 및 수익 추적에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>를 참조하십시오. 액세스 수준에서 재무 데이터에 액세스할 권한이 없거나 [!DNL Workfront] 관리자인 경우 이 정보를 업데이트할 수 없습니다. 재무 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>를 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 정의 양식]

사용자 정의 양식을 사용자 프로필과 연결할 수 있습니다. 이렇게 하면 위에서 설명한 [!DNL Workfront] 네이티브 필드에 저장할 수 없는 추가 사용자 정보를 저장할 수 있습니다.

사용자 정의 양식을 사용자 프로필에 첨부하려면 다음 액세스 권한 또는 권한 중 하나가 있어야 합니다.

* [!DNL Workfront] 관리자입니다.
* [!UICONTROL 표준] 또는 [!UICONTROL 플랜] 라이선스 사용자이며 사용자 정의 양식이 그룹 중 하나와 공유됩니다.

모든 사용자는 프로필과 연결된 사용자 정의 양식을 볼 수 있습니다.

사용자 프로필에 사용자 정의 양식을 첨부하려면 [!DNL Workfront] 관리자가 사용자 개체에 대한 사용자 정의 양식을 구성해야 합니다. 사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### [!UICONTROL 댓글]

프로필의 [!UICONTROL 업데이트] 탭에 저장된 사용자 프로필에 댓글을 기록할 수 있습니다.

[!UICONTROL 사람] 아이콘을 클릭하여 업데이트에 다른 사용자를 포함할 수 있습니다.

[!UICONTROL 잠금] 아이콘을 클릭하여 이 업데이트를 사용자와 같은 회사에 있는 사용자에게 비공개로 설정할 수 있습니다.
