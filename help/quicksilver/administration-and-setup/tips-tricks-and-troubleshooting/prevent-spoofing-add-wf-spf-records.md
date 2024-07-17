---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 스푸핑 방지 및  [!DNL Adobe Workfront] SPF 레코드 추가
description: 사용자가  [!DNL Adobe Workfront] 전자 메일 알림을 받지 못한 경우 방화벽에  [!DNL Workfront] SPF 레코드를 추가해야 합니다. SPF 레코드를 추가하려면 IT 팀과 협력해야 합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 스푸핑 방지 및 [!DNL Adobe Workfront]개의 SPF 레코드 추가

## 문제

사용자가 [!DNL Adobe Workfront]개의 전자 메일 알림을 받지 못하는 경우 [!DNL Workfront]개의 SPF 레코드를 방화벽에 추가해야 합니다. SPF 레코드를 추가하려면 IT 팀과 협력해야 합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

[방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)에 설명된 대로 프로덕션 환경에 맞게 IP 주소를 이미 허용 목록에 추가하다허용 목록에 추가하다 에 추가했으며 사용자가 여전히 이메일을 받지 못하는 경우:

1. 다음 SPF 레코드를 방화벽에 추가합니다.

   *spf.workfront.com*

   이렇게 하면 방화벽의 모든 [!DNL Workfront] IP 주소가 자동으로 방화벽에 있는 허용 목록에 추가하다에 추가되고 모든 스팸 필터(SPF 레코드 사용)가 [!DNL Workfront] 서버를 도메인에 대해 유효한 발신자로 확인할 수 있습니다.

   >[!NOTE]
   >
   > SPF 레코드는 DNS 영역 파일의 일부인 TXT 레코드입니다. DNS 영역 파일 수정을 지원하지 않습니다.

1. 구성해야 하는 SPF 레코드 유형을 지정해야 합니다. 다음은 유효한 SPF 레코드 유형입니다.

   * 모두(https://dmarcian.com/spf-syntax-table/#all)
   * ip4(https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6(https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx(https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * 존재함(https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   예를 들어 &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

회사 정책으로 인해 방화벽에 SPF 레코드를 추가할 수 없는 경우 [!DNL Workfront] 지원 담당자에게 문의하십시오.
