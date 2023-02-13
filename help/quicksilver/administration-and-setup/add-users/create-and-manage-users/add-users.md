---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 추가
description: Workfront 관리자 또는 전체 관리자 액세스 권한이 있는 사용자는 Workfront에서 사용자를 추가할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 사용자 추가

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>Adobe Admin Console에서 사용자를 추가하는 방법에 대한 지침은
>
>* 자세한 내용은 [Adobe Admin Console을 사용하여 Workfront에서 사용자 만들기](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* 문서에서 &quot;사용자 추가&quot; 섹션을 참조하십시오 [개별 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

개별 사용자를 처음부터 만들거나 기존 사용자를 복사하여 Adobe Workfront에서 사용자를 추가할 수 있습니다.

여러 사용자를 동시에 가져오는 방법에 대한 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p><b>사용자</b> 액세스 수준에서 설정 <b>편집</b> 액세스, 사용 <b>만들기</b> 둘 중 적어도 하나 <b>사용자 관리자</b> 옵션 사용 <b>설정 세부 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>이 두 옵션 중 사용자가 <b>관리자(그룹 사용자)</b> 이 활성화되어 있으면 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> <p>에 대한 자세한 정보 <b>사용자</b> 액세스 수준에서 설정하는 방법은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

사용자를 추가하기 전에 아래에 나열된 사용자에 대한 정보를 수집하고 해당 사용자와 연결할 정보를 결정합니다.

* 사용자의 개인 정보는 무엇입니까? 최소한 다음을 수행해야 합니다.

   * 전체 이름
   * 사용자 이름
   * 기본 암호
   * 이메일 주소

   >[!NOTE]
   >
   >Workfront 객체에 대한 액세스 레벨을 지정할 때 사용자 보기 설정을 미세 조정하여 다른 사용자의 연락처 정보를 볼 수 있는지 여부를 결정할 수 있습니다. 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 회사 내에서 새 사용자의 위치는 무엇입니까? 이 사람에게 직접 보고서가 있습니까? 이 사람은 누구에게 보고합니까?
* 그 사람은 어떤 역할을 맡습니까? 이 작업 역할이 Workfront에 있습니까? 이 일을 할 수 있는 사람 수에 제한이 있나요? 작업 역할 만들기에 대한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* 사용자에게 어떤 액세스 수준이 있어야 합니까? 이미 존재합니까, 아니면 새 항목을 만들어야 합니까? 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* 이 사용자는 어떤 홈 그룹을 사용해야 합니까? 사람이 둘 이상의 그룹에 있어야 합니까? 그룹에 대한 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* 이 사용자는 어느 홈 팀에 있어야 합니까? 한 팀이 넘어야 합니까? 팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* 이 사용자와 연결해야 하는 사용자 지정 정보는 무엇입니까?

   사용자에 대한 정보가 작성한 사용자 지정 필드에 캡처되는 경우 사용자를 만들 때 사용자 지정 양식을 준비해야 합니다. 사용자 지정 양식에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 사용자를 처음부터 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 클릭 **새 사용자 > 새 사용자** 을 추가하여 아직 Workfront에 추가되지 않은 사용자를 추가합니다.

   또는

   클릭 **새 사용자 > 사용자 가져오기** 스프레드시트 가져오기 파일을 업로드하여 사용자를 추가하려면

   사용자를 가져오는 경우 이 단계를 계속할 필요가 없습니다. 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. 에서 **새 사용자** 표시되는 상자를 클릭합니다. **고급 옵션 표시**&#x200B;그런 다음 사용 가능한 옵션을 구성하여 개인 정보를 입력합니다.

   이러한 옵션에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 다음 중 하나를 수행하십시오.

   * Leave **이 사람에게 초대 전자 메일 보내기** 활성화되었습니다. 이렇게 하면 사용자가 링크를 따라 Workfront에 대한 자체 암호를 만들 수 있는 이메일을 받게 됩니다. 이메일 초대를 수락하지 않고 Workfront 암호를 만드는 사용자는 Workfront에서 등록되지 않음으로 표시됩니다.
   * 비활성화 **이 사람에게 초대 전자 메일 보내기**&#x200B;를 입력한 다음 를 입력합니다 **암호** 에 대해 을 확인하고 **암호 확인** 상자. 이 암호를 Workfront 외부의 사용자와 공유해야 합니다.

   >[!NOTE]
   >
   >Workfront 관리자가 Workfront과의 SSO 통합을 활성화한 경우 유일한 허용이 &lt;sso configuration=&quot;&quot;> 이메일 초대를 비활성화하면 인증 필드가 숨겨집니다. 페더레이션 ID 또는 &lt;sso configuration=&quot;&quot;> 사용자 이름 필드가 계속 표시됩니다.

   >[!NOTE]
   조직에 Admin Console이 온보딩되어 있고 Workfront을 통해 사용자를 추가하는 경우 이메일 초대장을 보낼 수 없습니다.
   새 Adobe 사용자가 Admin Console에 추가되고, Admin Console이 프로세스를 완료하도록 초대하는 이메일을 보냅니다. 모든 사용자는 Adobe 시스템에 액세스하려면 등록 프로세스를 완료해야 합니다.
   기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받을 수도 없습니다. 이는 제품의 Adobe 관리자가 제어하는 기본 설정입니다.

1. 클릭 **이 사용자 추가**.

   또는

   클릭 **개인 사용자 추가 및 다른 사용자 시작** 새 사용자를 저장하고 다른 사용자를 추가하려면

## 사용자를 복사하여 새 사용자를 만듭니다

기존 사용자를 복사하여 사용자를 생성할 수 있습니다.

>[!NOTE]
이러한 방식으로 사용자를 만들면 다음을 제외하고 원래 사용자의 모든 정보가 새로 생성된 사용자에게 복사됩니다.
* 개인 정보 섹션의 정보입니다.
* 로그인하면 다음을 표시합니다. 이 상자에서 액세스 수준의 기본 랜딩 탭이 선택됩니다.
* 부하 직원
>


기존 사용자를 복사하여 새 사용자를 만들려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).
1. 복사할 사용자를 선택한 다음 복사 아이콘을 클릭합니다 ![](assets/copy-icon.png).
1. 에서 **새 사용자** 표시되는 상자에서 새 사용자가 사용할 수 있는 필드를 편집합니다.

   사용자와 연결된 모든 필드에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 클릭 **이 사용자 추가**.

   또는

   클릭 **개인 사용자 추가 및 다른 사용자 시작** 새 사용자를 저장하고 다른 사용자를 추가하려면

이렇게 하면 사용자를 위한 Workfront에 새 계정이 만들어집니다.

사용자에게 초대를 보내는 옵션을 선택한 경우 사용자는 링크를 따라 Workfront 암호를 만들 수 있는 이메일을 받게 됩니다.

>[!NOTE]
조직에 Admin Console이 온보딩되어 있고 Workfront을 통해 사용자를 추가하는 경우 이메일 초대장을 보낼 수 없습니다.
새 Adobe 사용자가 Admin Console에 추가되고, Admin Console이 프로세스를 완료하도록 초대하는 이메일을 보냅니다. 모든 사용자는 Adobe 시스템에 액세스하려면 등록 프로세스를 완료해야 합니다.
기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받을 수도 없습니다. 이는 제품의 Adobe 관리자가 제어하는 기본 설정입니다.
