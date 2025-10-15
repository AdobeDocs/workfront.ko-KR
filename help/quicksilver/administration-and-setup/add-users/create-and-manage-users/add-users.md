---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 사용자 추가
description: Workfront 관리자 또는 전체 관리 액세스 권한을 가진 사용자는 Workfront에서 사용자를 추가할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 1%

---

# 사용자 추가

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 시스템 관리자를 만들어야 합니다.**
>
>   Adobe Admin Console에서 시스템 관리자를 만드는 방법에 대한 지침은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.
>
>   Adobe Admin Console에 온보딩된 조직의 그룹 관리자는 이 절차를 사용하여 사용자를 생성하고 관리자 승인을 위해 사용자를 제출할 수 있습니다.
>
>   조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.
>
>* **조직에서 SSO(Single Sign-On)를 사용하는 경우** 사용자를 만들어 Adobe Admin Console에서 Workfront에 할당하는 것이 좋습니다. Workfront에서 이러한 사용자를 만들 수 있지만, 조직의 Admin Console이 구성되는 방식에 따라 해당 정보를 Adobe Admin Console으로 전송하는 데 문제가 있을 수 있습니다.
>  &#x200B;>   Adobe Admin Console에서 사용자를 만든 후 Workfront에서 역할, 그룹, 팀 및 액세스 수준 할당과 같은 사용자 정보를 구성할 수 있습니다.
>* **조직에서 SSO(Single Sign-On)를 사용하지 않는 경우** Workfront에서 시스템 관리자가 아닌 사용자를 직접 추가할 수 있습니다. Adobe Admin Console에서는 사용자를 추가할 수 있지만 Workfront에서 사용자를 추가하면 생성 중에 액세스 수준을 설정할 수 있으므로 시간을 절약할 수 있습니다.



처음부터 개별 사용자를 만들거나 기존 사용자를 복사하여 Adobe Workfront에서 사용자를 추가할 수 있습니다.

여러 사용자를 동시에 가져오는 방법에 대한 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)를 참조하십시오.

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <b>에서 두 개의 </b>사용자 관리<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

사용자를 추가하기 전에 아래 나열된 사용자에 대한 정보를 수집하여 해당 사용자와 연결할 정보를 결정하십시오.

* 사용자의 개인 정보는 무엇입니까? 최소한 다음이 필요합니다.

   * 전체 이름
   * 사용자 이름
   * 기본 암호
   * 이메일 주소

  >[!NOTE]
  >
  >Workfront 객체에 대한 액세스 수준을 지정할 때 사용자 보기 설정을 미세 조정하여 사용자가 다른 사용자의 연락처 정보를 볼 수 있는지 여부를 결정할 수 있습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

* 회사 내에서 새로운 사용자의 위치는 무엇입니까? 이 사람에게 부하 직원이 있습니까? 이 사람은 누구에게 보고합니까?
* 그 사람은 어떤 역할을 맡고 있나요? 이 작업 역할이 Workfront에 있습니까? 이 업무를 담당할 인원수에 제한이 있나요? 작업 역할 만들기에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.
* 사용자는 어떤 액세스 수준을 보유해야 합니까? 이미 존재합니까, 아니면 새로 만들어야 합니까? 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.
* 이 사용자는 어떤 홈 그룹에 속해야 합니까? 대상이 두 개 이상의 그룹에 있어야 합니까? 그룹에 대한 자세한 내용은 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md)를 참조하세요.
* 이 사용자는 어느 홈 팀에 속해 있어야 합니까? 대상이 두 개 이상의 팀에 속해 있어야 합니까? 팀에 대한 자세한 내용은 [팀 개요](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)를 참조하세요.
* 이 사용자와 연결하는 데 필요한 사용자 정의 정보는 무엇입니까?

  사용자에 대한 정보가 사용자가 만든 사용자 정의 필드에 캡처되어 있는 경우 사용자를 만들 때 사용자 정의 양식을 준비해야 합니다. 사용자 정의 양식에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

## 처음부터 사용자 만들기

{{step-1-to-users}}

1. 아직 Workfront에 추가되지 않은 사용자를 추가하려면 **새 사용자 > 새 사용자**&#x200B;를 클릭합니다.

   또는

   스프레드시트 가져오기 파일을 업로드하여 사용자를 추가하려면 **새 사용자 > 사용자 가져오기**&#x200B;를 클릭합니다.

   사용자를 가져오는 경우 이러한 단계를 계속할 필요가 없습니다. 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)를 참조하십시오.

1. 표시되는 **새 사용자** 상자에서 **고급 옵션 표시**&#x200B;를 클릭한 다음 사용 가능한 옵션을 구성하여 사용자 정보를 입력하십시오.

   이러한 옵션에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

1. 다음 중 하나를 수행하십시오.

   * **이 사용자에게 초대 이메일 보내기**&#x200B;를 사용하도록 설정합니다. 이렇게 하면 사용자가 링크를 따라 Workfront에 대한 자체 암호를 만들 수 있는 이메일을 받게 됩니다. 이메일 초대를 수락하지 않고 Workfront 암호를 만드는 사용자는 Workfront에서 등록 취소됨으로 표시됩니다.
   * **이 사용자에게 초대 전자 메일 보내기**&#x200B;를 사용하지 않도록 설정한 다음 해당 사용자에 대해 **암호**&#x200B;를 입력하고 **암호 확인** 상자에서 확인합니다. 이 암호를 Workfront 외부의 사용자와 공유해야 합니다.

   >[!NOTE]
   >
   >* Workfront 관리자가 Workfront과의 SSO 통합을 활성화한 경우 이메일 초대를 비활성화하면 &lt;SSO 구성> 인증만 허용 필드가 표시되지 않습니다. 페더레이션 ID 또는 &lt;SSO 구성> 사용자 이름 필드가 계속 표시됩니다.
   >
   >* 조직이 Admin Console에 온보딩되고 Workfront을 통해 사용자를 추가하는 경우 이메일 초대를 보낼 수 있는 옵션이 없습니다.
   >
   >   기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받지 못할 수도 있습니다. 이는 제품에 대해 Adobe 관리자가 제어하는 기본 설정입니다.

1. **이 사용자 추가**&#x200B;를 클릭합니다.

   또는

   새 사용자를 저장하고 다른 사용자를 추가하려면 **사용자 추가 및 다른 사용자 시작**&#x200B;을 클릭하세요.

   >[!NOTE]
   >
   >* Adobe Admin Console에 온보딩된 조직에 사용자를 추가하는 그룹 관리자인 경우 이 단계의 옵션은 **관리자 승인을 위해 사용자 제출** 및 **승인을 위해 제출하고 다른 작업을 시작**&#x200B;입니다. 사용자는 비활성화됨 및 승인 보류 중 상태로 만들어집니다.
   > 
   >* 사용자가 몇 분 내에 비활성화됨 및 승인 보류 중 상태를 벗어나지 않고 화면 새로 고침으로 승인 보류 중 배지가 제거되지 않으면 사용자를 수동으로 승인할 수 있습니다.
   >
   >   1. 설정 > 사용자로 이동합니다.
   >   1. 사용자 목록에서 사용자를 선택합니다.
   >   1. 목록 헤더에서 점 3개 메뉴를 클릭합니다.
   >   1. **승인**&#x200B;을 선택합니다.
   >   1. 몇 분 후에 페이지를 새로 고칩니다.


## 사용자를 복사하여 새 사용자 만들기

기존 사용자를 복사하여 사용자를 생성할 수 있습니다.

>[!NOTE]
>
>이러한 방식으로 사용자를 생성하면 다음을 제외한 모든 정보가 원래 사용자의 새 생성 사용자에게 복사됩니다.
>
>* 개인 정보 섹션의 정보.
>* 로그인할 때 표시: 이 상자에서 액세스 수준에 대한 기본 랜딩 탭이 선택됩니다.
>* 부하 직원
>

기존 사용자를 복사하여 새 사용자를 생성하려면 다음을 수행합니다.

{{step-1-to-users}}

1. 복사할 사용자를 선택한 다음 복사 아이콘 ![복사 아이콘](assets/copy-icon.png)을 클릭합니다.
1. 표시되는 **사용자 복사** 상자에서 새 사용자가 사용할 수 있는 필드를 편집합니다.

   사용자와 관련된 모든 필드에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

1. **이 사용자 추가**&#x200B;를 클릭합니다.

   또는

   새 사용자를 저장하고 다른 사용자를 추가하려면 **사용자 추가 및 다른 사용자 시작**&#x200B;을 클릭하세요.

이렇게 하면 Workfront에서 사용자를 위한 새 계정이 만들어집니다.

사용자에게 초대를 보내는 옵션을 선택한 경우 링크를 따라 Workfront 암호를 만들 수 있는 이메일을 수신해야 합니다.

>[!NOTE]
>
>조직이 Admin Console에 온보딩되고 Workfront을 통해 사용자를 추가하는 경우 이메일 초대를 보낼 수 있는 옵션이 없습니다.
>
>기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받지 못할 수도 있습니다. 이는 제품에 대해 Adobe 관리자가 제어하는 기본 설정입니다.
