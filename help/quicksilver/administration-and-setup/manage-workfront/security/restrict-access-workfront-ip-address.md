---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: IP 주소별로 Adobe Workfront에 대한 액세스 제한
description: Workfront에 대한 액세스를 지정한 IP 주소 또는 IP 주소 범위로 제한하는 Adobe Workfront IP 허용 목록에 추가하다를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 대한 추가 보안 레이어가 제공됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# IP 주소별로 Adobe Workfront에 대한 액세스 제한

Workfront에 대한 액세스를 지정한 IP 주소 또는 IP 주소 범위로 제한하는 Adobe Workfront IP 허용 목록에 추가하다를 구성할 수 있습니다. 이렇게 하면 Workfront 애플리케이션에 대한 추가 보안 레이어가 제공됩니다.

이러한 IP 주소 또는 IP 주소 범위는 네트워크 관리자가 제공해야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기타 허용 목록

방화벽이나 메일 서버가 특정 공급업체에만 액세스할 수 있도록 구성된 경우 해당에 특정 IP 주소를 추가해야 허용 목록에 추가하다 합니다. 이렇게 하면 환경과 Adobe Workfront 서버 간의 통신이 열립니다. 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

또한, 조직에서 Enterprise 플랜을 사용하는 경우, Workfront에서 전자 메일을 수락할 수 있는 이메일 도메인과 사용자가 Workfront 사용자 프로필에 지정한 전자 메일 주소에 포함할 수 있는 전자 메일 도메인을 제어하도록 Workfront 전자 메일을 구성할 수 있습니다허용 목록에 추가하다. 자세한 내용은 [이메일 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## 에 IP 주소 허용 목록에 추가하다 추가

Workfront에 IP 주소를 허용 목록에 추가하다 추가한 후에는 해당 IP 주소만 Workfront에 액세스하는 데 사용할 수 있습니다. 다른 IP 주소에서 Workfront에 액세스하려고 하는 사용자에게는 해당 IP 주소가 차단되었음을 나타내는 오류 메시지가 표시됩니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **고객 정보.**

1. 에서 **IP 허용 목록에 추가하다** 섹션, **IP를 허용 목록에 추가하다 활성화합니다.**

   이 옵션은 기본적으로 비활성화됩니다.

1. Workfront 시스템에 액세스하는 데 현재 사용하는 IP 주소를 지정합니다.

   또는

   현재 Workfront 시스템에 액세스하는 데 사용하는 IP 주소 범위를 지정하십시오.

   Workfront에 액세스하는 데 사용하는 IP 주소허용 목록에 추가하다를 사용하도록 설정하려면 먼저 허용 목록에 추가하다에 추가해야 합니다.

1. 클릭 **IP 범위 추가,** 그런 다음 Workfront에 액세스할 수 있는 IP 주소 또는 IP 주소 범위를 지정합니다.
1. (선택 사항) 이전 단계를 반복하여 IP 주소 또는 IP 주소 범위를 더 추가합니다.

   최대 45개의 주소 또는 범위를 추가할 수 있습니다.

1. 클릭 **저장.**
