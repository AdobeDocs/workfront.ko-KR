---
title: 사용자 가져오기
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: '네트워크 디렉터리 서비스(예: Active Directory 또는 다른 LDAP 디렉터리)의 사용자를 동기화하여 Adobe Workfront 사이트로 사용자를 가져오거나 스프레드시트 가져오기 파일을 사용하여 사용자를 가져올 수 있습니다.'
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# 사용자 가져오기

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

스프레드시트 가져오기 파일을 사용하여 사용자를 가져올 수 있습니다.

새 사용자를 작성하기 전에 먼저 사용자와 연관시킬 모든 객체를 작성했는지 확인합니다. 예를 들어, 예약을 만들지 않은 경우 새 사용자에게 일정을 할당할 수 없으며 새 사용자와 일정을 연결하는 데 사용하는 필드가 새 사용자 화면에 나타나지 않습니다.

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

## 스프레드시트 가져오기 파일을 사용하여 사용자 가져오기

{{step-1-to-users}}

1. **새 사용자** 드롭다운 화살표를 클릭한 다음 **사용자 가져오기**&#x200B;를 클릭합니다.

1. 표시되는 **사용자 가져오기** 상자에서 샘플 파일을 다운로드한 다음 사용자의 개인 정보를 포함하도록 샘플 파일을 업데이트합니다.

   각 행에는 다음 필드가 포함되어 있습니다.

   * **이름**
   * **성**
   * **전자 메일 주소**

     이메일 주소는 고유해야 합니다.

   * **액세스 수준**

     액세스 수준은 대/소문자를 구분합니다.

   * **SSO 로그인 ID**

     이 필드는 시스템에서 SSO가 활성화되어 있을 경우에만 포함됩니다. 각 사용자에 대해 이 필드에 페더레이션 ID를 추가해야 합니다. 인물 탭에서 사용자를 만들 때 사용자가 SSO 없이 로그인할 수 있도록 하려면 사용자의 암호를 설정할 수 있습니다. 그러나 가져오기 기능을 사용하여 SSO 로그인 ID를 비워둘 수 없습니다.

   * 사용자의 이메일 주소 앞이나 뒤에 추가 공백이 없는지 확인합니다.

   행을 완료하면 다음과 같이 표시됩니다.

   ![new-users.png 가져오기](assets/importing-new-users.png)

1. 파일을 워크스테이션의 위치에 저장합니다.
1. **사용자 가져오기** 상자에서 **파일 선택**&#x200B;을 클릭합니다.

1. 저장한 파일로 이동하여 선택합니다.

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. **가져오기**&#x200B;를 클릭합니다.

   화면 맨 위에 사용자를 성공적으로 가져왔다는 확인 메시지가 표시됩니다.

>[!NOTE]
>
>사용자는 비활성화됨 및 승인 보류 중 상태로 만들어집니다.
> 
>사용자가 몇 분 내에 비활성화됨 및 승인 보류 중 상태에서 이동하지 않고 화면 새로 고침으로 승인 보류 중 배지가 제거되지 않는 경우 사용자 배치를 Adobe Admin Console에 바로 추가할 수 있습니다.
>
>지침은 [여러 사용자 관리를 참조하십시오. | Adobe 설명서의 일괄 CSV 업로드](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html).
