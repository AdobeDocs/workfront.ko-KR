---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 인증에 대한 암호 정책 구성
description: Adobe Workfront 관리자는 암호 정책 옵션을 구성하여 Workfront 시스템에 대한 인증 환경을 사용자 지정할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 2%

---

# 인증에 대한 암호 정책 구성

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 암호 정책 옵션을 구성하여 Workfront 시스템에 대한 인증 환경을 사용자 지정할 수 있습니다.

Workfront 구현 중에 인증 환경 설정을 구성하고 나중에 가끔 다시 방문하는 것이 좋습니다.

향상된 암호 관리 기능이 곧 제공될 예정이거나 이미 사용 가능할 수도 있습니다. 조직에서 새 인증 환경에 액세스할 수 있는지 여부에 따라 다음 섹션 중 하나를 사용합니다.

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

## 인증 구성(모든 고객에게 사용 가능) {#configure-authentication-available-for-all-customers}

모든 고객에 대해 인증 옵션이 표시됩니다. 섹션에 설명된 대로 향상된 암호 관리 기능이 곧 제공될 예정이거나 이미 사용 가능할 수도 있습니다. [향상된 인증 구성(준비 중)](#configure-enhanced-authentication-coming-soon) 참조하십시오.

인증 환경 설정을 구성하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **인증**.

1. 다음 필드 중 하나를 선택하여 조직의 인증 설정을 설정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자가 암호를 재설정할 때마다 강제 적용 <em>&lt;value&gt;</em> 일</td> 
      <td>이렇게 하면 사용자가 Workfront 암호를 재설정할 시간이 설정됩니다. 기본적으로 이 옵션은 비활성화됩니다. 활성화하면 30, 60, 90, 120, 180일 중에서 선택할 수 있습니다. 기본값은 30일입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 이전 암호와 동일한 암호를 설정하도록 허용하지 않음 <em>&lt;value&gt;</em> 암호</td> 
      <td> <p>이 필드에서 사용자는 설정된 수의 재설정에 대해 암호를 재사용할 수 없습니다. 기본적으로 이 필드는 비활성화됩니다. 암호를 재사용하기 전에 이 값을 5, 10 또는 15로 설정할 수 있습니다.</p> <p>이 옵션을 선택하면 지정된 날에 두 번 이상 암호를 재설정할 수 없습니다</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">잘못된 암호를 5번 연속해서 입력하면 계정을 잠급니다 <em>&lt;value&gt;</em> 분: </td> 
      <td> <p>잘못된 암호를 5번 연속해서 입력한 후 Workfront에서 사용자를 잠글 시간을 선택합니다. 기본적으로 이 옵션이 활성화되며 대기 시간은 10분입니다. 10분, 30분, 1시간, 8시간 또는 24시간 동안 계정을 잠글 수 있습니다. </p> <p>사용자에 대한 암호를 수동으로 재설정하면 이 기본 대기 값이 무시됩니다. <br>사용자는 로그인 화면을 통해 잠기면 자체 암호를 재설정할 수 있습니다. 암호를 잊어버린 경우 암호를 재설정하는 방법에 대한 자세한 내용은 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">암호 재설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">암호에 적어도 하나 이상 포함해야 합니다. <em>&lt;value&gt;</em> 다양한 문자 유형:</td> 
      <td> <p>암호에 필요한 다양한 유형의 문자를 선택할 수 있도록 하여 강력한 사용자 암호가 필요한 정도를 결정합니다.</p> <p>인식할 수 있는 사전어는 암호로 사용할 수 없습니다.<br>기본적으로 Workfront에서는 다음 중 적어도 2개가 암호에 있어야 합니다(유효한 암호를 위해 이러한 문자 중 3개가 있어야 함). </p> 
       <ul> 
        <li>대문자</li> 
        <li>소문자 문자</li> 
        <li>숫자</li> 
        <li>기호</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

## 향상된 인증 구성(준비 중) {#configure-enhanced-authentication-coming-soon}

이 섹션에서는 조직에서 아직 사용할 수 없는 향상된 인증 환경에 대해 설명합니다. 조직이 새 인증 환경으로 마이그레이션되지 않은 경우에는 다음에 설명된 대로 인증 설정을 구성해야 합니다 [인증 구성(모든 고객에게 사용 가능)](#configure-authentication-available-for-all-customers).

향상된 인증 환경 설정을 구성하려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **향상된 인증**.
1. 에서 **암호 길이** 상자에 유효한 비밀번호에 필요한 최소 문자 수를 입력합니다.

   Workfront에는 6자 이상이 필요합니다.

1. (선택 사항)에서 **암호 요구 사항** 섹션에서 사용자 암호에 필요한 문자 유형을 선택합니다.

   [암호 요구 사항] 섹션에서 모든 유형의 문자를 요구하여 사용자 암호 강도를 높일 수 있습니다. 다음 옵션을 사용할 수 있습니다.

   | 소문자 | 하나 이상의 소문자 필요 |
   |---|---|
   | 대문자 | 하나 이상의 대문자가 필요합니다. |
   | 숫자 | 숫자를 하나 이상 필요 |
   | 특수 문자 | 특수 문자가 하나 이상 필요합니다. |

   {style=&quot;table-layout:auto&quot;}

1. **저장**&#x200B;을 클릭합니다.
