---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 중복 사용자 방지
description: 'Adobe Workfront에서 새 사용자를 만들 때 대/소문자에 따라 이메일 주소가 달라지는 경우에도 다른 사용자가 이미 사용 중인 이메일 주소를 더 이상 사용할 수 없습니다(예: JohnDoe@example.com 및 johndoe@example.com). 또한 향후 인증 개선을 준비하려면 모든 사용자에게 Workfront 인스턴스에서 고유한 이메일 주소가 있는지 확인하십시오.'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 중복 사용자 방지

Adobe Workfront에서 새 사용자를 만들 때 대/소문자에 따라 이메일 주소가 달라지는 경우에도 다른 사용자가 이미 사용 중인 이메일 주소를 더 이상 사용할 수 없습니다(예: JohnDoe@example.com 및 johndoe@example.com). 또한 향후 인증 개선을 준비하려면 모든 사용자에게 Workfront 인스턴스에서 고유한 이메일 주소가 있는지 확인하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 고유 이메일 주소로 사용자 만들기

2019.4 릴리스부터 Workfront에서 새 사용자를 만들 때 사례별로 이메일 주소가 다르더라도 더 이상 다른 사용자가 이미 사용 중인 이메일 주소를 사용할 수 없습니다. 예를 들어, 다른 사용자의 이메일 주소가 JohnDoe@example.com인 경우 이메일 주소가 johndoe@example.com인 사용자를 한 명 만들 수 없습니다.

## Workfront 인스턴스에서 기존 사용자의 이메일 주소 업데이트

Workfront 관리자는 대/소문자만 다른 이메일 주소가 일치하는 기존 사용자를 업데이트해야 합니다.
Workfront 인스턴스 내에서 중복 이메일 주소를 수정하려면 다음을 수행합니다.

1. 중복 사용자를 검사하고 더 이상 필요하지 않은 사용자를 결정합니다.

   1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **사용자**. ![](assets/users-icon-in-main-menu.png)

   1. 다음에서 **필터** 메뉴, 선택 **모두**.

   1. 다음에서 **보기** 메뉴, 선택 **사용자 로그인**.

   1. 다음에서 **그룹화** 메뉴, 선택 **없음**.

   1. 사용자 로그인 보기를 사용자 지정합니다.

      1. 클릭 **보기** > **보기 맞춤화**.

      1. 바꾸기 **ID** 열이 있는 **이메일 주소** 열.

      1. 보기 이름을 바꾸고 저장합니다.
   1. 새 그룹화를 만듭니다.

      1. 클릭 **그룹화** > **새 그룹화**.

      1. 클릭 **텍스트 모드로 전환** 페이지의 오른쪽 상단 모서리에서 을 참조하십시오.
      1. 다음 텍스트 모드 코드를 붙여넣습니다.

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 그룹화 이름을 변경하고 저장합니다.



1. 다음 중 하나를 수행합니다.

   * (기본 방법) 각 추가 계정에 대해 사용자의 이메일 주소에 + 주소를 추가합니다.

      조직의 단일 사용자가 2개 이상의 사용자 계정에 액세스해야 하는 경우 이 옵션을 선택합니다. 이메일 공급자가 + 주소 지정을 지원하지 않는 경우 각 Workfront 계정에 대해 별도의 이메일 계정을 제공해야 합니다.

      예를 들어 John Doe는 일일 사용 계정에 대한 사용자 계정 하나와 테스트 목적으로 사용할 사용자 계정 하나를 가질 수 있습니다.

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 이메일 주소에 다음 텍스트를 추가하여 가짜 도메인을 사용하도록 도메인을 변경합니다.

      `.inactive`

      예를 들어, John Doe에는 다음과 같은 도메인이 있을 수 있습니다(이러한 도메인은 고유해야 함).

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      암호 재설정에 유효한 이메일 주소가 필요하므로 더 이상 이러한 계정에 로그인할 수 없습니다. 이러한 계정은 다음으로 로그인 기능을 사용해야 액세스할 수 있습니다.

   * 필요하지 않은 사용자 삭제

      >[!IMPORTANT]
      >
      >실수로 생성된 계정 또는 테스트 계정에 대해서만 이 옵션을 선택합니다. 이 옵션은 일반적으로 0 또는 1개의 잘못된 로그인이 있는 계정에만 수행됩니다. 정기적으로 사용된 계정은 삭제해서는 안 됩니다.



Workfront 인스턴스에 대소문만 다른 이메일 주소와 일치하는 사용자가 있는 경우, Workfront에서 추가 정보와 타임라인을 업데이트해야 할 때 연락합니다.
