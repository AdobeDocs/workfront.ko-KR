---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 중복 사용자 방지
description: 'Adobe Workfront에서 새 사용자를 만들 때 이메일 주소가 경우에 따라 다르더라도(예: JohnDoe@example.com 및 johndoe@example.com) 다른 사용자가 이미 사용하고 있는 이메일 주소를 더 이상 사용할 수 없습니다. 또한 향후 인증 개선 사항을 준비하려면 모든 사용자가 Workfront 인스턴스에 고유한 이메일 주소를 가지고 있는지 확인하십시오.'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 중복 사용자 방지

Adobe Workfront에서 새 사용자를 만들 때 이메일 주소가 경우에 따라 다르더라도(예: JohnDoe@example.com 및 johndoe@example.com) 다른 사용자가 이미 사용하고 있는 이메일 주소를 더 이상 사용할 수 없습니다. 또한 향후 인증 개선 사항을 준비하려면 모든 사용자가 Workfront 인스턴스에 고유한 이메일 주소를 가지고 있는지 확인하십시오.

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

## 연습

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[이 기능에 대한 비디오 데모를 시청하십시오.](https://vimeo.com/371505632/2e6938ce06)

## 고유한 이메일 주소를 사용하여 사용자 만들기

2019.4 릴리스부터 Workfront에서 새 사용자를 만들 때 이메일 주소가 건별로 다르더라도 다른 사용자가 이미 사용하고 있는 이메일 주소를 더 이상 사용할 수 없습니다. 예를 들어, 다른 사용자에게 johndoe@example.com 이메일 주소가 있는 경우 이메일 주소가 JohnDoe@example.com인 사용자를 한 명 만들 수 없습니다.

## Workfront 인스턴스에서 기존 사용자의 이메일 주소를 업데이트합니다

Workfront 관리자는 대소문자가 다른 이메일 주소가 일치하는 기존 사용자를 업데이트해야 합니다.
Workfront 인스턴스 내에서 중복 이메일 주소를 수정하려면:

1. 중복 사용자를 살펴보고 더 이상 필요하지 않은 사용자를 결정합니다.

   1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자**. ![](assets/users-icon-in-main-menu.png)

   1. 에서 **필터** 메뉴, 선택 **모두**.

   1. 에서 **보기** 메뉴, 선택 **사용자 로그인**.

   1. 에서 **그룹화** 메뉴, 선택 **아무것도**.

   1. 사용자 로그인 보기를 사용자 지정합니다.

      1. 클릭 **보기** > **보기 사용자 지정**.

      1. 바꾸기 **ID** 열을 **이메일 주소** 열.

      1. 보기 이름을 변경하고 저장합니다.
   1. 새 그룹을 만듭니다.

      1. 클릭 **그룹화** > **새 그룹화**.

      1. 클릭 **텍스트 모드로 전환** 페이지의 오른쪽 위 모서리에서 을(를) 클릭합니다.
      1. 다음 텍스트 모드 코드를 붙여넣습니다.

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 그룹화 이름을 변경하고 저장합니다.



1. 다음 중 하나를 수행합니다.

   * (기본 설정 방법) 추가 각 계정에 대해 사용자의 이메일 주소에 + 주소를 추가합니다.

      조직의 단일 사용자가 2명 이상의 사용자 계정에 액세스해야 하는 경우 이 옵션을 선택합니다. 이메일 공급자가 더하기 주소 지정을 지원하지 않는 경우 각 Workfront 계정에 대해 별도의 이메일 계정을 제공해야 합니다.

      예를 들어, John Doe에는 일별 사용 계정에 대해 하나의 사용자 계정과 테스트 용도로 사용할 사용자 계정이 있을 수 있습니다.

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 이메일 주소에 다음 텍스트를 추가하여 가짜 도메인을 사용하도록 도메인을 변경합니다.

      `.inactive`

      예를 들어, John Doe에는 다음 도메인이 있을 수 있습니다. (고유해야 합니다.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      암호 재설정에는 유효한 전자 메일 주소가 필요하므로 더 이상 이러한 계정에 로그인할 수 없습니다. 이러한 계정은 다른 이름으로 로그인 기능을 사용해야 액세스할 수 있습니다.

   * 불필요한 사용자 삭제

      >[!IMPORTANT]
      >
      >실수 또는 테스트 계정에 대해 생성된 계정에 대해서만 이 옵션을 선택합니다. 이 옵션은 일반적으로 로그인이 영 또는 1인 계정에만 수행됩니다. 정기적으로 사용된 계정은 삭제하면 안 됩니다.



Workfront 인스턴스에 대/소문만 서로 다른 이메일 주소가 일치하는 사용자가 있는 경우, Workfront은 추가 정보 및 타임라인을 업데이트 해야 할 때 사용자에게 연락합니다.
