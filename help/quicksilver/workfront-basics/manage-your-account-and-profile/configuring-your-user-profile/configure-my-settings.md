---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: 내 설정 구성
description: '사용자 [!DNL Adobe Workfront] 프로필에는 사용자 자신에 대한 정보(예: 이름, 이메일 주소, 주소, 전화번호, 제목 등)가 포함되어 있습니다. 또한 와의 상호 작용에 대한 정보도 포함되어 있습니다 [!DNL Workfront] 및 기타 사용자 를 사용할 수 있습니다.'
author: Lisa
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: 72a2927d33f40c4fe08888712bdf62e9a5db9c40
workflow-type: tm+mt
source-wordcount: '3228'
ht-degree: 1%

---

# 내 설정 구성

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

사용자 [!DNL Adobe Workfront] 프로필에는 사용자 자신에 대한 정보(예: 이름, 이메일 주소, 주소, 전화번호, 제목 등)가 포함되어 있습니다. 또한 와의 상호 작용에 대한 정보도 포함되어 있습니다 [!DNL Workfront] 및 회사의 다른 사용자(예: 알림 설정, 표시할 탭) [!DNL Workfront]또는 사용자의 역할, 관리자 및 그룹 및 팀 멤버십)

이 정보의 대부분은 이미 [!DNL Workfront] 관리자 [!DNL Workfront] 계정이 생성되었습니다.

에 있는 액세스 수준에 따라 [!DNL Workfront]를 구성 하여 이 정보 중 일부를 편집할 수 있습니다 [!UICONTROL 내 설정] 영역.

## 액세스 수준이 편집에 미치는 영향 [!UICONTROL 내 설정] 영역

보유한 액세스 수준에 따라, [!UICONTROL 내 설정] 영역.

편집 가능한 섹션에 포함된 일부 필드는 액세스 수준에서 구성할 수도 있고 구성되지 않을 수도 있는 다른 설정에 따라 편집할 수 없습니다. 찾을 필드 중 일부를 편집하는 데 필요한 추가 액세스에 대한 자세한 내용은 [!UICONTROL 내 설정]의 섹션 을 참조하십시오. [구성 [!UICONTROL 내 설정] 영역](#configuring-the-my-settings-area).

액세스 수준을 확인하려면 [!DNL Workfront] 관리자

다음 격자에는 [!UICONTROL 내 설정] 영역은 액세스 수준에 따라 표시되거나 편집할 수 있습니다.

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
   <th><strong>[!UICONTROL System Administrator]</strong> </th> 
   <th><strong>[!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Reviewer]</strong> </th> 
   <th><strong>[!UICONTROL 요청자]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Personal Info]</td> 
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
   <td rowspan="2">[!UICONTROL Preferences]</td> 
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
   <td rowspan="2">[!UICONTROL Access]</td> 
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
   <td rowspan="2">[!UICONTROL Organization]</td> 
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
   <td rowspan="2">[!UICONTROL Custom Forms]</td> 
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

## 구성 [!UICONTROL 내 설정] 영역

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]을 클릭한 다음 프로필 사진 옆에 있는 사용자 이름을 클릭합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 편집]**.

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

### [!UICONTROL 개인적인 정보]

이 섹션에는 다음 하위 섹션이 포함됩니다.

* [기본 정보](#basic-info)
* [작업 정보](#job-info)
* [연락처 정보](#contact-info)

#### [!UICONTROL 기본 정보]

이 정보는 이미 [!DNL Workfront] 관리자 이 하위 섹션의 모든 필드는 필수 필드입니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 이름]</strong></td> 
   <td>이름을 업데이트합니다. 필수 필드입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Last Name]</strong></td> 
   <td>성을 업데이트합니다. 필수 필드입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Address]</strong></td> 
   <td> 이메일 주소를 업데이트합니다. 필수 필드입니다. 이메일 주소도 사용자 이름이며 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 암호 재설정]</strong></td> 
   <td>이 섹션에서 암호를 재설정합니다. 암호 재설정에 대한 자세한 내용은 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">암호 재설정</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) &lt;sso configuration=""&gt; [!UICONTROL Username]</strong></td> 
   <td> 만약 [!DNL Workfront] 관리자가 [!DNL Workfront]에 로그인하면 SSO 사용자 이름이 이 필드에 표시됩니다. 에 대해 활성화된 SSO 구성 유형 [!DNL Workfront] 인스턴스가 이 필드에 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL만 허용 &lt;sso configuration=""&gt; 인증]</strong></td> 
   <td> <p> 만약 [!DNL Workfront] 관리자가 [!DNL Workfront] 및 은(는) SSO용 사용자를 업데이트했으며, 이 필드는 기본적으로 선택됩니다. 에 대해 활성화된 SSO 구성 유형 [!DNL Workfront] 인스턴스가 이 필드에 표시됩니다.</p> <p>이 필드를 선택한 경우 로그인해야 합니다 [!DNL Workfront] SSO 자격 증명으로 사용. 체크 표시를 해제하면 로그인할 수 있습니다. [!DNL Workfront] 사용 [!DNL Workfront] 자격 증명.</p> <p>구성에 대한 자세한 정보 [!DNL Workfront] SSO 솔루션 사용 시 <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">단일 사인온 [!DNL Adobe Workfront]</a>. SSO용 사용자 업데이트에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">단일 사인온용 사용자 업데이트</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 작업 정보]

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Title]</strong></td>
        <td>제목을 지정합니다. 이것은 너의 직무 역할과 같지 않다. 제목은 리소스 예약의 일부가 아니지만 작업 역할은 입니다. 제목이 [!DNL Workfront] 사용자 이름과 아바타가 표시되는 모든 곳에 인터페이스를 사용할 수 있습니다. 사용자를 볼 수 있는 액세스 권한이 있는 모든 사람이 볼 수 있습니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Talk to Me About]</strong></td>
        <td>이 필드에 전문적인 관심 사항을 지정합니다.</td>
    </tr>
</table>

#### [!UICONTROL 연락처 정보]

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Phone Number]</strong></td>
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
        <td><strong>[!UICONTROL Address]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL State]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Postal Code]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Country]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Profile Picture]</strong></td>
        <td>프로필 사진이 아바타가 되고 전체 화면에 표시됩니다 [!DNL Workfront] 시스템, 이름이 표시되는 곳</td>
    </tr>
</table>

### [!UICONTROL 환경 설정]

에 표시할 항목을 지정합니다 [!DNL Workfront] 인터페이스 섹션을 참조하십시오.

>[!NOTE]
>
>을 사용하는 사용자 [!UICONTROL 요청자] 라이센스에 추가할 수 있는 다른 왼쪽 패널 항목이 없습니다 [!UICONTROL 기본 메뉴]에 속해 있어야 합니다 [!UICONTROL 요청] 영역. 로서의 [!DNL Workfront] 관리자는 요청자 라이센스를 가진 사용자를 레이아웃 템플릿에 할당하여 [!UICONTROL 기본 메뉴]. 그런 다음 영역에 표시할 영역을 선택할 수 있습니다 [!UICONTROL 기본 메뉴] 사용자 프로필을 편집하여

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 시간대]</strong> </td> 
   <td><p>표준 시간대를 지정합니다. 보내는 이메일 메시지에 표시되는 시간을 제어합니다.</p>
       <p>시간대는 PTO 달력 보고서에 표시되는 사항에도 영향을 줍니다.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Locale]</strong> </td> 
   <td>여기에서 기본 언어를 지정합니다. 보내는 이메일 메시지에 사용되는 언어, 날짜 및 숫자 형식을 제어합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 업데이트 상태에 완료율 표시]</strong> </td> 
   <td>작업 업데이트를 입력할 때 작업 완료율을 업데이트할 수 있도록 작업의 [!UICONTROL 업데이트 상태] 필드에 백분율 표시줄을 표시하려면 이 확인란을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 내 작업 탭에 할당된 작업 보내기]</strong> </td> 
   <td>[!UICONTROL Work Requests] 탭 대신 [!UICONTROL Working On] 탭에서 직접 할당하는 작업을 표시하려면 이 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) 문서를 업로드할 때 증명을 자동으로 생성합니다</strong></td> 
   <td>이 필드를 선택하면 문서가 로드되는 즉시 증명 생성을 시작합니다 [!DNL Workfront]. 이 필드는 기본적으로 비활성화되어 있으며 Workfront 관리자만 업데이트할 수 있습니다.<br>이 필드는 회사가 Workfront용 Workfront 증명 구성 요소를 구입한 경우에만 사용할 수 있으며, 증명 사용자로 사용할 수 있습니다. Workfront 증명에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Adobe Workfront 내에서 증명 관리</a>.
   <p><b>참고:</b> 요청에 업로드된 문서는 증명을 자동으로 생성하지 않습니다. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 알림]

받을 알림을 지정합니다 [!DNL Workfront]. 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL 액세스]

액세스 및 이와 관련된 기타 구성 요소는 [!DNL Workfront] 관리자, 계정이 설정되면

전용 [!DNL Workfront] 관리자는 이 섹션의 모든 필드를 보고 편집할 수 있습니다.

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL이 활성화되어 있음]</strong> </td> 
   <td>이 필드는 또한 [!DNL Workfront] 관리자는 기본적으로 선택되어 있어야 합니다. 즉, 사용자가 활성 상태이며 로그인할 수 있습니다 [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Access Level]</strong> </td> 
   <td>이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL Workfront 관리자] 액세스 수준을 가진 사용자에게만 표시되며, [!DNL Workfront] 관리자 만약 [!DNL Workfront] 관리자는 이 필드를 수정할 때 액세스 수준을 더 낮은 수준으로 변경하지 않도록 주의하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 레이아웃 템플릿]</strong> </td> 
   <td>이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL]을 사용하는 사용자에게 표시됩니다 [!DNL Workfront] administrator] 액세스 수준이며 [!UICONTROL에서만 편집할 수 있습니다. [!DNL Workfront] 관리자] 또는 관리자 액세스 권한이 있는 [!UICONTROL Plan] 라이센스가 있는 사용자 Workfront 인터페이스의 모양 및 필드를 업데이트하려면 레이아웃 템플릿을 여기에서 선택합니다. 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자 편집을 위한 사용자 액세스 권한 구성</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.<br>레이아웃 템플릿 및 레이아웃이 인터페이스에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a></td> 
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
   <td role="rowheader"><strong>(조건부) [!UICONTROL 사용자는 증명을 생성할 수 있습니다(... 사용 중인 증명 라이센스 왼쪽).]</strong></td> 
   <td>이 필드는 회사가 기존 [!DNL Workfront] 계획 및 구매 [!DNL Workfront Proof] 구성 요소. 이 옵션을 선택하면 교정 사용자로 활성화됩니다. 또한 구매한 전체 증명 라이센스 수 중 시스템에 사용된 증명 라이센스 수도 표시합니다. 이 필드는 또한 사용자가 볼 수 있고 편집할 수 있습니다 [!DNL Workfront] 관리자 제품 교정을 위한 계획 옵션에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">에서 언어 교정 기능에 액세스 [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 권한 프로필]</strong></td> 
   <td> <p>이 필드에는 사용자가 액세스할 수 있는 수준이 표시됩니다 [!DNL Workfront Proof]. 다음 경우에만 사용할 수 있습니다.</p> 
    <ul> 
     <li>회사에서 기존 을 사용합니다 [!DNL Workfront] 계획 및 구매 [!DNL Workfront Proof] 구성 요소나 새 구성 요소에 [!UICONTROL Work] 또는 [!UICONTROL Plan] 라이센스가 있는 경우 [!DNL Workfront] 계획.</li> 
     <li>증명 사용자로 활성화됩니다.</li> 
    </ul> <p>[!DNL Workfront] 관리자는 자신을 제외한 모든 사용자의 필드를 편집할 수 있으므로 모든 사용자는 자신의 프로필에 대해 필드를 보기 전용으로 볼 수 있습니다. 권한 프로필에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">증명 권한 프로필 개요</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 조직]

이 정보는 일반적으로 [!DNL Workfront] 관리자가 [!DNL Workfront] 계정이 필요합니다. 이 섹션에서 조직 또는 조직 구조에 대한 정보를 업데이트할 수도 있습니다. 다음을 가진 사용자만 [!UICONTROL 계획] 또는 [!UICONTROL 시스템 관리자] 액세스 수준에서 이 섹션을 편집할 수 있습니다. 

이 하위 섹션에서 다음 중 하나를 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>드롭다운 목록에서 자신이 속한 회사의 이름을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL Reports To]</strong></td> 
   <td>을(를) 선택한 후 <strong>[!UICONTROL Company]</strong> 프로필의 경우 이 필드에 관리자의 이름을 지정할 수도 있습니다. 여기에서 이름을 하나만 지정할 수 있으며 바로 아래 관리자의 이름을 지정하는 것이 좋습니다. 이름을 입력하고 목록에 표시될 때 클릭하여 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL Direct Reports]</strong></td> 
   <td>을(를) 선택한 후 <strong>[!UICONTROL Company]</strong> 프로필에 대해 이 필드에 직접 보고서의 이름을 지정할 수도 있습니다. 여기에서 필요한 만큼 직접 보고서를 지정할 수 있습니다. 이름을 입력하고 목록에 표시될 때 클릭하여 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Team]</strong> </td> 
   <td> <p>선택 <strong>[!UICONTROL Home Team]</strong> 를 클릭합니다. 이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 액세스 수준이 있는 사용자에게만 표시되며, [!DNL Workfront] 관리자 또는 관리자 액세스 권한도 있는 [!UICONTROL Plan] 라이센스가 있는 사용자 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자 편집을 위한 사용자 액세스 권한 구성</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.<br></p> <p>사용자 <strong>홈 팀</strong> 사용자의 모양과 느낌에 영향을 줄 수 있습니다 [!DNL Workfront] 인터페이스로, 레이아웃 템플릿이 팀과 연결된 경우 </p> <p> <br>팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Teams]</strong> </td> 
   <td> <p>둘 이상의 팀에 속할 수 있습니다. 팀 이름을 입력하기 시작하여 이 필드에 속한 추가 팀을 지정한 다음, 목록에 표시될 때 클릭하여 선택합니다. 너무 많은 팀에 속하면 팀에 할당된 작업에 대해 혼동을 일으킬 수 있습니다. 팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>.</p> <p>이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 라이센스가 있는 사용자에게만 표시되며, [!DNL Workfront] 관리자 또는 관리자 액세스 권한도 있는 [!UICONTROL Plan] 라이센스가 있는 사용자 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자 편집을 위한 사용자 액세스 권한 구성</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Group]</strong> </td> 
   <td> <p>선택 <strong>[!UICONTROL Home Group]</strong> 를 클릭합니다.</p> <p>참고: 필수 필드입니다. 사용자와 그룹이 연결되어 있지 않은 사용자는 가질 수 없습니다.<br></p> <p>이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 수준을 가진 사용자에게 표시됩니다. 을 편집할 수 있는 사용자에 대한 자세한 정보 <strong>[!UICONTROL Home Group]</strong> 필드, 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md#prerequisites" class="MCXref xref">사용자 추가</a> 섹션 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">사용자 추가</a>.Your <strong>[!UICONTROL Home Group]</strong> 는 모든 프로젝트에 대한 기본 그룹 및 기본값입니다 <strong>[!UICONTROL Home Group]</strong> 새 사용자를 위해 만들 수 있습니다. 사용자가 만드는 모든 사용자 지정 양식은 사용자와 공유됩니다 <strong>[!UICONTROL Home Group]</strong> 기본적으로 제공됩니다.</p> <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기타 그룹]</strong> </td> 
   <td> <p>여러 그룹에 속할 수 있습니다. 을 입력하여 이 필드에 속한 추가 그룹을 지정합니다. 목록에 표시될 때 클릭하여 선택합니다. 이 필드는 [!UICONTROL Plan] 또는 [!UICONTROL System Administrator] 액세스 수준을 가진 사용자에게 표시됩니다. 을 편집할 수 있는 사용자에 대한 자세한 정보 <strong>[!UICONTROL 기타 그룹]</strong> 필드에서 "기타 그룹" 섹션을 참조하십시오. <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">사용자 추가</a>.</p> <p>그룹에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 리소스 계획 수립]

자원 계획 정보는 작업 지정 시간, 로그 시간, 비용 및 현재 프로젝트 수익에 영향을 줍니다. 일반적으로 이 영역은 [!DNL Workfront] 관리자, 프로젝트 또는 리소스 관리자 또는 직접 관리자

이 섹션에서 다음 중 하나를 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Schedule Deactivation]</strong></td> 
   <td>일정 기간 후에 계정을 비활성화하도록 예약하려면 이 확인란을 선택합니다. 에서 <p><strong>[!UICONTROL 예약 비활성화 날짜]</strong> 그러면 계정이 비활성화된 이후의 날짜를 지정합니다. 사용자 비활성화에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">사용자 비활성화 예약</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>. </p><p>계획 라이센스가 있거나 [!DNL Workfront] 관리자 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기본 역할]</strong></td> 
   <td> <p>Workfront에서 수행할 수 있는 기본 작업 역할입니다. 할당되는 모든 작업 및 문제도 기본적으로 이 작업 역할에 할당됩니다. 자원 관리에는 직무 역할이 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> <p>관리자 액세스 권한이 있는 [!UICONTROL Plan] 라이센스가 있거나 [!DNL Workfront] 관리자 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자 편집을 위한 사용자 액세스 권한 구성</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) [!UICONTROL 기본 역할]을 선택한 경우 [!UICONTROL FTE 가용성의 백분율] 필드가 표시됩니다.</strong></td> 
   <td>이 작업 역할에 할당된 예약된 시간의 백분율을 지정합니다. 기본 역할에 대한 [!UICONTROL FTE 가용성 백분율]의 기본값은 100%입니다</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기타 역할]</strong> </td> 
   <td> <p>에 여러 작업 역할이 있을 수 있습니다 [!DNL Workfront]. 자원 관리에는 직무 역할이 필수적입니다. 작업 역할에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> <p>관리자 액세스 권한이 있는 [!UICONTROL Plan] 라이센스가 있거나 [!DNL Workfront] 관리자 관리자 액세스 권한이 있는 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">사용자 지정 액세스 수준을 사용하여 사용자 편집을 위한 사용자 액세스 권한 구성</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(조건부) 하나 이상의 기타 역할을 선택한 경우, 각 역할에 대해 [!UICONTROL FTE 가용성의 백분율] 필드가 표시됩니다.</strong></td> 
   <td> <p>각 작업 역할에 할당된 예약된 시간의 백분율을 지정합니다. [!UICONTROL Other Roles]에 대한 [!UICONTROL Percentage of FTE Availability] 기본값은 0%입니다.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>참고:  
     <ul> 
      <li>[!UICONTROL 기타 역할]에 0%의 FTE 가용성이 있는 경우, 사용자가 이러한 역할의 작업에 할당되지 않는 한 [!UICONTROL Resource Planner]에는 표시되지 않습니다.</li> 
      <li> <p>모두 <strong>[!UICONTROL FTE 가용성의 백분율]</strong> 모든 역할에 대해 100%가 같아야 합니다. 각 [!UICONTROL FTE 가용성의 백분율]은 [!UICONTROL Resource Planner]에서 사용자당 각 역할에 대해 [!UICONTROL 사용 가능한 시간]을 계산합니다. </p> <p>사용자당 각 역할에 대한 [!UICONTROL 사용 가능한 시간]은 사용자의 사용 가능한 시간에 따라 다릅니다. 사용자의 사용 가능한 시간은 [!DNL Workfront] 에서 선택한 메서드에 따라 [!DNL Workfront] 관리자는 [!UICONTROL Resource Management Preferences]에서 FTE를 계산합니다. 사용자의 가용성 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>. 리소스 관리 환경 설정 구성에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>일정</strong></td> 
   <td> <p>전용 [!DNL Workfront] 작업표 및 시간에 대한 관리자 액세스 권한이 있는 [!UICONTROL Plan] 라이센스가 있는 관리자 또는 사용자는 이 필드를 업데이트할 수 있습니다. 작업표 및 시간에 대한 관리 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p>드롭다운 메뉴에서 올바른 작업표를 선택합니다. 이렇게 하면 사용자가 설정한 사양에 따라 작업표가 자동으로 생성됩니다 [!DNL Workfront] 관리자 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 기본 시간 유형]</strong> </td> 
   <td>기본 시간 유형을 선택합니다. Workfront에 로그인할 때마다 기본적으로 시스템에서 사용하는 시간 유형입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 사용 가능한 시간 유형]</strong> </td> 
   <td>시간을 기록할 때 선택할 수 있는 시간 유형을 선택합니다. 이 드롭다운 메뉴의 시간 유형은 [!DNL Workfront] 관리자</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 리소스 풀]</strong> </td> 
   <td>속해 있는 리소스 풀을 선택합니다. 이 필드는 보고 및 정보용으로만 사용되며 리소스 예약이나 계획에 영향을 주지 않습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>여기에서 지정하는 숫자는 시스템 수준의 [!UICONTROL Resource Management Preferences]가 로 설정된 경우에만 기본 일정을 기반으로 가용성을 계산하도록 고려됩니다 <strong>[!UICONTROL 기본 일정]</strong>.</p> <p>예를 들어 FTE 값이 0.5이고 [!UICONTROL 기본 일정]이 40시간인 경우 일주일에 20시간 동안 작업할 수 있습니다.</p> <p>시스템 수준의 [!UICONTROL Resource Management Preferences]가 <strong>[!UICONTROL 사용자의 일정]</strong>로 지정하는 값은 무시되며, 일정에 지정된 대로 작업할 수 있습니다. 이 경우 [!UICONTROL Resource Planner]에 대한 FTE는 다음 공식으로 계산됩니다. </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>사용자 FTE 계산에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">리소스 계획자에서 사용자 및 역할에 대한 시간 및 FTE 계산 개요</a>.</p> <p>예약 작성에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p>리소스 관리 기본 설정 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">리소스 관리 환경 설정 구성</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL 시간당 비용]</strong> </td> 
   <td>사용자의 시간당 비용 크기를 지정합니다. 의 비용 추적에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>. 액세스 수준에서 재무 데이터에 액세스할 수 없거나 사용자가 [!DNL Workfront] 관리자 재무 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Billing per Hour]</strong> </td> 
   <td>사용자에 대한 시간당 청구 금액을 지정합니다. 청구 및 수익 추적에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>. 액세스 수준에서 재무 데이터에 액세스할 수 없거나 사용자가 [!DNL Workfront] 관리자 재무 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 정의 양식]

사용자 지정 양식을 사용자 프로필과 연결할 수 있습니다. 이렇게 하면 사용자의 추가 정보를 저장할 수 있습니다. 그렇지 않으면 [!DNL Workfront] 위에 설명된 기본 필드.\
사용자에게 사용자 지정 양식을 첨부하려면 다음 액세스 권한 또는 사용 권한이 있어야 합니다.

* 당신은 [!DNL Workfront] 관리자
* 당신은 [!UICONTROL 계획] 라이선스 사용자 및 사용자 지정 양식이 그룹 중 하나와 공유됩니다.

모든 사용자는 사용자와 연결된 사용자 지정 양식을 볼 수 있습니다.

사용자 [!DNL Workfront] 사용자 프로필에 사용자 정의 양식을 첨부할 수 있도록 관리자는 사용자 개체에 대한 사용자 정의 양식을 구성해야 합니다. 사용자 지정 양식 만들기에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### [!UICONTROL 댓글]

사용자 프로필에 대한 설명을 기록하고 [!UICONTROL 업데이트] 사용자의 탭입니다.

을(를) 클릭합니다. [!UICONTROL 사람] 아이콘을 사용하여 업데이트에 다른 사용자를 포함할 수 있습니다.

을(를) 클릭합니다. [!UICONTROL 잠금] 사용자와 동일한 회사에 있는 사용자에게 이 업데이트를 비공개 상태로 만들 수 있습니다.
