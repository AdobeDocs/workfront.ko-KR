---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 허용 목록에 추가하다 이메일 구성
description: 조직에서 WorkfrontEnterprise 플랜을 사용하는 경우 Workfront 허용 목록에 추가하다 이메일 도메인을 만들어 Workfront에서 보낸 이메일을 수락할 수 있는 이메일 도메인과 사용자가 사용자 프로필에 지정한 이메일 주소에 있을 수 있는 이메일 도메인을 제어할 수 있습니다. 이 기능은 조직의 보안 정책이 사용자가 Workfront에 저장된 데이터를 외부 이메일 주소로 보내지 못하도록 제한하는 경우 유용합니다. 이 정책이 적용되도록 하려면 허용 목록에 추가하다에 내부 회사 도메인만 포함할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 허용 목록에 추가하다 이메일 구성

조직에서 Workfront 엔터프라이즈 플랜을 사용하는 경우 Workfront 이메일 허용 목록을 만들어 다음을 제어할 수 있습니다.

* Workfront에서 보낸 이메일을 수락할 수 있는 이메일 도메인.
* 사용자가 사용자 프로필에 지정하는 이메일 주소에 포함될 수 있는 이메일 도메인.

이 기능은 조직의 보안 정책이 사용자가 Workfront에 저장된 데이터를 외부 이메일 주소로 보내지 못하도록 제한하는 경우 유용합니다. 이 정책이 적용되도록 하려면 허용 목록에 추가하다에 내부 회사 도메인만 포함할 수 있습니다.

>[!IMPORTANT]
>
>IT 팀은 `notifications@my.workfront.com`에서 들어오는 전자 메일이 조직의 시스템에서 차단되지 않았는지 확인해야 합니다.
>
>성공적인 이메일 전달을 높이고 이메일 스푸핑을 방지하기 위해 Workfront의 모든 이메일이 해당 주소에서 전송됩니다. 여기에는 자동화된 경고와 사용자 간 통신이 모두 포함됩니다.
>
>예를 들어 Joan Harris라는 사용자로부터 받은 Workfront 이메일의 보낸 사람 라인은 다음과 같습니다.
>`Joan Harris <notifications@my.workfront.com>`

사용자 환경과 Adobe Workfront 허용 목록에 추가하다 서버 간 통신을 열 수 있도록 조직의 방화벽을 구성하는 방법에 대한 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

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
   <td> <p>Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 기타 허용 목록

조직에서 엔터프라이즈 계획을 수립하는 경우, Workfront 액세스를 지정한 75개의 IP 주소 또는 IP 주소 범위로 제한하는 Adobe Workfront IP 허용 목록에 추가하다를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 추가 보안 계층을 제공할 수 있습니다. 자세한 내용은 [IP 주소로 Adobe Workfront에 대한 액세스 제한](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)을 참조하십시오.

허용 목록에 추가하다 또한 방화벽 또는 메일 서버가 특정 공급업체에만 액세스할 수 있도록 구성된 경우 특정 IP 주소를 해당 공급업체에 추가해야 합니다. 그러면 환경과 Adobe Workfront 서버 간에 통신이 열립니다. 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하세요.

## 허용 목록에 추가하다 이메일 구성

{{step-1-to-setup}}

1. **시스템** > **고객 정보**&#x200B;를 클릭합니다.
1. **전자 메일 허용 목록 허용 목록에 추가하다** 섹션에서 **도메인 활성화**&#x200B;를 선택한 다음 **도메인 추가**&#x200B;를 클릭합니다.
1. 표시되는 상자에서 `ourcompany.com`과(와) 같이 허용할 도메인을 입력한 다음 **도메인 추가**&#x200B;를 클릭합니다.
1. 이전 단계를 반복하여 허용하려는 다른 도메인을 추가합니다.
1. 완료되면 **저장**&#x200B;을 클릭하세요.
