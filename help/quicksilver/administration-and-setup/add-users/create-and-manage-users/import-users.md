---
title: 사용자 가져오기
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: '네트워크 디렉토리 서비스(예: Active Directory 또는 다른 LDAP 디렉토리)에서 사용자를 동기화하여 Adobe Workfront 사이트로 사용자를 가져오거나 스프레드시트 가져오기 파일을 사용하여 사용자를 가져올 수 있습니다.'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# 사용자 가져오기

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>Adobe Admin Console에서 사용자 프로필 편집에 대한 지침은 문서에서 &quot;사용자 추가&quot; 섹션을 참조하십시오 [사용자 일괄 업로드](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 또는 Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

스프레드시트 가져오기 파일을 사용하여 사용자를 가져올 수 있습니다.

새 사용자를 생성하기 전에 먼저 사용자와 연결할 모든 개체를 작성했는지 확인합니다. 예를 들어, 일정을 만들지 않은 경우에는 일정을 새 사용자에게 할당할 수 없으며 일정을 새 사용자와 연결하는 데 사용하는 필드가 새 사용자 화면에 표시되지 않습니다.

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

## 스프레드시트 가져오기 파일을 사용하여 사용자를 가져옵니다

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 을(를) 클릭합니다. **새 사용자** 드롭다운 화살표를 클릭한 다음 **사용자 가져오기**.

1. 에서 **사용자 가져오기** 표시되는 상자에서 샘플 파일을 다운로드한 다음 샘플 파일을 업데이트하여 사용자의 개인 정보를 포함합니다.

   각 행에는 다음 필드가 포함되어 있습니다.

   * **이름**
   * **성**
   * **이메일 주소**

      이메일 주소는 고유해야 합니다.

   * **액세스 수준**

      액세스 레벨은 대/소문자를 구분합니다.

   * **SSO 로그인 ID**

      이 필드는 시스템에서 SSO가 활성화된 경우에만 포함됩니다. 각 사용자에 대해 이 필드에 페더레이션 ID를 추가해야 합니다. 사용자 탭에서 사용자를 만들 때 사용자가 SSO 없이 로그인할 수 있도록 하려면 사용자에 대한 암호를 설정할 수 있습니다. 그러나 가져오기 기능을 사용하면 SSO 로그인 ID를 비워 둘 수 없습니다.

   * 사용자의 이메일 주소 앞이나 뒤에 추가 공백이 없는지 확인합니다.

   행이 끝나면 다음과 같이 표시됩니다.

   ![import-new-users.png](assets/importing-new-users.png)

1. 파일을 워크스테이션의 위치에 저장합니다.
1. 클릭 **파일 선택** 에서 **사용자 가져오기** 상자.

1. 로 이동하고 저장한 파일을 선택합니다.
1. (선택 사항) **이 사용자에게 초대 전자 메일 보내기** 사용자에게 이메일 초대장을 보내고, Workfront 계정이 생성되었음을 알리고 사용자에게 암호를 설정하라는 메시지를 표시하는 옵션입니다.

   사용자의 암호를 설정하려면 이 옵션을 선택 취소합니다.

1. 클릭 **가져오기**.

   화면 상단에 사용자를 성공적으로 가져왔음을 확인하는 메시지가 표시됩니다.
