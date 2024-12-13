---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: IP 주소로 Adobe Workfront 액세스 제한
description: Adobe Workfront IP 주소 75로 Workfront 액세스를 제한하거나 지정한 IP 주소 범위로 액세스를 제한하는 허용 목록에 추가하다 IP 를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 추가 보안 계층을 제공할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# IP 주소로 Adobe Workfront에 대한 액세스 제한

Adobe Workfront IP 주소 75로 Workfront 액세스를 제한하거나 지정한 IP 주소 범위로 액세스를 제한하는 허용 목록에 추가하다 IP 를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 추가 보안 계층을 제공할 수 있습니다.

이러한 IP 주소 또는 IP 주소 범위는 네트워크 관리자가 제공해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>기업</p> </td> 
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

## 기타 허용 목록

허용 목록에 추가하다 방화벽 또는 메일 서버가 특정 공급업체에 대해서만 액세스를 허용하도록 구성된 경우 특정 IP 주소를 해당 공급업체에 추가해야 합니다. 그러면 환경과 Adobe Workfront 서버 간에 통신이 열립니다. 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하세요.

또한, 조직에서 Enterprise 플랜을 사용하는 경우, Workfront의 이메일을 수락할 수 있는 이메일 도메인과 사용자가 Workfront 사용자 프로필에 지정한 이메일 주소에 있을 수 있는 이메일 도메인을 제어하도록 Workfront 이메일 허용 목록을 구성할 수 있습니다. 허용 목록에 추가하다 자세한 내용은 [전자 메일 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)을 참조하십시오.

## 허용 목록에 추가하다에 IP 주소 추가

Workfront허용 목록에 추가하다 에 IP 주소를 추가한 후에는 해당 IP 주소만 Workfront에 액세스하는 데 사용할 수 있습니다. 다른 IP 주소에서 Workfront에 액세스하려고 하는 사용자에게는 IP 주소가 차단되었음을 나타내는 오류 메시지가 표시됩니다.

{{step-1-to-setup}}

1. **시스템** > **고객 정보**&#x200B;를 클릭합니다.

1. **IP 허용 목록허용 목록에 추가하다 을 사용**&#x200B;하는 IP **섹션에서 IP**&#x200B;활성화를 선택합니다.

   이 옵션은 기본적으로 비활성화되어 있습니다.

1. 현재 Workfront 시스템에 액세스하는 데 사용 중인 IP 주소를 지정합니다.

   또는

   현재 Workfront 시스템에 액세스하는 데 사용 중인 IP 주소 범위를 포함하는 IP 주소 범위를 지정합니다.

   Workfront이 활성화되기 전에 허용 목록에 추가하다에 액세스하기 위해 사용하는 IP 주소를 허용 목록에 추가하다에 추가해야 합니다.

1. **IP 범위 추가,**&#x200B;를 클릭한 다음 Workfront에 액세스할 수 있는 IP 주소 또는 IP 주소 범위를 지정합니다.
1. (선택 사항) 이전 단계를 반복하여 IP 주소 또는 IP 주소 범위를 추가합니다.

   최대 75개의 주소 또는 범위를 추가할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.
