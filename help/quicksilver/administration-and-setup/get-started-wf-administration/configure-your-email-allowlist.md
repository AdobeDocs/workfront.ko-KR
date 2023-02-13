---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 이메일 허용 목록에 추가하다 구성
description: 조직에서 WorkfrontEnterprise 플랜을 사용하는 경우, Workfront 이메일를 만들어 Workfront에서 전자 메일을 수락할 수 있는 이메일 도메인과 사용자가 사용자 프로필에 지정한 전자 메일 주소에 포함할 수 있는 전자 메일 도메인을 제어할 수 있습니다허용 목록에 추가하다. 이 기능은 조직의 보안 정책으로 인해 사용자가 Workfront에 저장된 데이터를 외부 이메일 주소로 보내지 못하게 하는 경우에 유용합니다. 내부 회사 도메인만 포함하여 이 정책이 수행되도록 할 허용 목록에 추가하다 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 이메일 허용 목록에 추가하다 구성

조직에서 WorkfrontEnterprise 플랜을 사용하는 경우, Workfront 이메일을 만들어 다음을 제어할 수 허용 목록에 추가하다 있습니다.

* Workfront의 이메일을 수락할 수 있는 이메일 도메인입니다.
* 사용자가 사용자 프로필에 지정하는 이메일 주소에 포함될 수 있는 이메일 도메인입니다.

이 기능은 조직의 보안 정책으로 인해 사용자가 Workfront에 저장된 데이터를 외부 이메일 주소로 보내지 못하게 하는 경우에 유용합니다. 내부 회사 도메인만 포함하여 이 정책이 수행되도록 할 허용 목록에 추가하다 수 있습니다.

>[!IMPORTANT]
>
>IT 팀에서는 `notifications@my.workfront.com` 조직의 시스템에서 차단되지 않았습니다.
>
>Workfront의 모든 이메일이 해당 주소에서 전송되어 성공적인 이메일 전달을 늘리고 이메일 스푸핑을 제거합니다. 여기에는 자동화된 경고와 사용자 간 통신이 모두 포함됩니다.
>
>예를 들어, Joan Harris라는 사용자로부터 받은 Workfront 이메일의 보낸 사람 라인은 다음과 같습니다.
>
```
>Joan Harris <notifications@my.workfront.com>
>```

환경과 Adobe Workfront 서버 간의 통신을 열기 위해 조직의 방화벽을 구성하는 방법에 대한 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td> <p>Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기타 허용 목록

조직에 Enterprise 계획이 있는 경우 사용자가 지정하는 45개의 IP 주소 또는 IP 주소 범위로 Workfront에 대한 액세스를 제한하는 Adobe Workfront IP 허용 목록에 추가하다를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 대한 추가 보안 레이어가 제공됩니다. 자세한 내용은 [IP 주소별로 Adobe Workfront에 대한 액세스 제한](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

또한 방화벽이나 메일 서버가 특정 공급업체에 대해서만 액세스를 허용하도록 구성된 경우 해당에 특정 IP 주소를 추가해야 허용 목록에 추가하다 합니다. 이렇게 하면 환경과 Adobe Workfront 서버 간의 통신이 열립니다. 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 이메일 허용 목록에 추가하다 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **고객 정보**.

1. 에서 **이메일 허용 목록에 추가하다** 섹션, **도메인 허용 목록에 추가하다 활성화**&#x200B;를 클릭한 다음 **도메인 추가**.
1. 표시되는 상자에 허용할 도메인(예: )을 입력합니다 `ourcompany.com`를 클릭한 다음 **도메인 추가**.

1. 이전 단계를 반복하여 허용할 다른 도메인을 추가합니다.
1. 완료되면 를 클릭합니다 **저장**.
