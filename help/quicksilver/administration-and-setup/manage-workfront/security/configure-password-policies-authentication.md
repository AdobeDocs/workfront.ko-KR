---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 인증 암호 정책 구성하기
description: Adobe Workfront 관리자는 암호 정책 옵션을 구성하여 Workfront 시스템에 대한 인증 환경을 사용자 정의할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 2%

---

# 인증 암호 정책 구성하기

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 암호 정책 옵션을 구성하여 Workfront 시스템에 대한 인증 환경을 사용자 정의할 수 있습니다.

Workfront 구현 중에 인증 환경 설정을 구성하고 이후에 가끔씩만 다시 방문하는 것이 좋습니다.

암호 관리 기능이 개선되어 곧 출시될 예정입니다. 이미 조직에서 사용할 수 있습니다. 조직에서 새 인증 환경에 액세스할 수 있는지 여부에 따라 다음 섹션 중 하나를 사용합니다.

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 인증 구성(모든 고객이 사용 가능) {#configure-authentication-available-for-all-customers}

모든 고객에 대해 인증 옵션이 표시됩니다. 이 문서의 [향상된 인증 구성)](#configure-enhanced-authentication-coming-soon) 섹션에 설명된 대로 암호 관리 기능이 개선되어 곧 출시되거나 조직에서 이미 사용할 수 있습니다.

인증 기본 설정을 구성하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. **시스템** > **인증**&#x200B;을 클릭합니다.

1. 다음 필드 중 하나를 선택하여 조직에 대한 인증 설정을 설정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자가 <em>&lt;값&gt;</em>일마다 암호를 재설정하도록 강제 설정</td> 
      <td>이렇게 하면 사용자가 Workfront 암호를 재설정할 수 있는 시간대가 설정됩니다. 기본적으로 이 옵션은 비활성화되어 있습니다. 활성화하면 30일, 60일, 90일, 120일, 180일 중에서 선택할 수 있습니다. 기본값은 30일입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 이전 <em>&lt;값&gt;</em> 암호와 동일한 암호를 설정하지 못하도록 합니다.</td> 
      <td> <p>이 필드에서는 사용자가 설정된 재설정 횟수에 대해 암호를 재사용할 수 없습니다. 기본적으로 이 필드는 비활성화되어 있습니다. 이 값을 활성화하면 암호를 재사용하기 전에 이 값을 5, 10 또는 15 재설정으로 설정할 수 있습니다.</p> <p>이 옵션을 선택하면 사용자는 하루에 두 번 이상 암호를 재설정할 수 없습니다</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">잘못된 암호를 연속 5회 입력하면 <em>&lt;값&gt;</em>분 동안 계정을 잠급니다. </td> 
      <td> <p>잘못된 암호를 연속 5회 입력한 후 사용자가 Workfront에서 얼마나 오래 잠길지 선택합니다. 기본적으로 이 옵션이 활성화되어 있으며 대기 시간은 10분입니다. 계정을 10분, 30분, 1시간, 8시간 또는 24시간 동안 잠글 수 있습니다. </p> <p>사용자의 암호를 수동으로 재설정하면 이 기본 대기 값이 무시됩니다. <br>사용자가 로그인 화면을 통해 잠겨 있을 때 암호를 재설정할 수 있습니다. 암호를 잊어버린 경우 암호를 재설정하는 방법에 대한 자세한 내용은 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">암호 재설정</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">암호에는 <em>&lt;값&gt;</em>개 이상의 다른 문자 유형이 포함되어야 합니다.</td> 
      <td> <p>암호에 필요한 여러 유형의 문자 수를 선택할 수 있도록 하여 사용자 암호가 얼마나 강력해야 하는지 결정합니다.</p> <p>인식할 수 있는 사전의 단어는 암호로 사용할 수 없습니다.<br>기본적으로 Workfront의 암호에는 다음 문자 중 최소 2개가 있어야 합니다(올바른 암호를 위해 이 문자 중 3개가 있어야 할 수도 있음). </p> 
       <ul> 
        <li>대문자</li> 
        <li>소문자</li> 
        <li>숫자</li> 
        <li>기호</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

## 향상된 인증 구성{#configure-enhanced-authentication-coming-soon}

이 섹션에서는 조직에서 아직 사용할 수 없는 향상된 인증 환경에 대해 설명합니다. 조직이 새 인증 환경으로 마이그레이션되지 않은 경우 [인증 구성(모든 고객이 사용 가능)](#configure-authentication-available-for-all-customers)에 설명된 대로 인증 설정을 구성해야 합니다.

향상된 인증 기본 설정을 구성하려면 다음을 수행하십시오.

{{step-1-to-setup}}

1. **시스템** > **향상된 인증**&#x200B;을 클릭합니다.
1. **암호 길이** 상자에 올바른 암호에 필요한 최소 문자 수를 입력합니다.

   Workfront에는 최소 6자가 필요합니다.

1. (선택 사항) **암호 요구 사항** 섹션에서 사용자 암호에 필요한 문자 유형을 선택합니다.

   [암호 요구 사항] 섹션에서 일부 또는 모든 유형의 문자를 요구하여 사용자 암호의 강도를 높일 수 있습니다. 다음 옵션을 사용할 수 있습니다.

   | 소문자 | 소문자가 하나 이상 필요함 |
   |---|---|
   | 대문자 | 대문자가 하나 이상 필요합니다. |
   | 숫자 | 하나 이상의 숫자 필요 |
   | 특수 문자 | 특수 문자가 하나 이상 필요합니다. |

   {style="table-layout:auto"}

1. **저장**&#x200B;을 클릭합니다.
