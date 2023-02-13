---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 스푸핑 방지 및 추가 [!DNL Adobe Workfront] SPF 레코드
description: 사용자가 수신하지 않는 경우 [!DNL Adobe Workfront] 이메일 알림 을 추가하려면 [!DNL Workfront] 방화벽에 SPF 레코드를 기록합니다. SPF 레코드를 추가하려면 IT 팀과 협력해야 합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 스푸핑 방지 및 추가 [!DNL Adobe Workfront] SPF 레코드

## 문제

사용자가 수신하지 않는 경우 [!DNL Adobe Workfront] 이메일 알림 을 추가하려면 [!DNL Workfront] 방화벽에 SPF 레코드를 기록합니다. SPF 레코드를 추가하려면 IT 팀과 협력해야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

에 설명된 대로 프로덕션 환경의에 이미 IP 주소허용 목록에 추가하다를 추가한 경우 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 및 사용자는 여전히 이메일을 받지 않습니다.

1. 다음 SPF 레코드를 방화벽에 추가합니다.

   *spf.workfront.com*

   이렇게 하면 모두 자동으로 추가됩니다. [!DNL Workfront] 방화벽의에 대한 IP 주소허용 목록에 추가하다를 사용하고, SPF 레코드를 사용하는 모든 스팸 필터(SPF 레코드)를 사용하여 유효성을 검사할 수 있습니다 [!DNL Workfront] 도메인을 보낸 유효한 보낸 사람으로 서버

   >[!NOTE]
   >
   > SPF 레코드는 DNS 영역 파일의 일부인 TXT 레코드입니다. DNS 영역 파일 수정을 지원하지 않습니다.

1. 구성해야 하는 SPF 레코드 유형을 지정해야 합니다. 다음은 유효한 SPF 레코드 유형입니다.

   * 모두 (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * 존재(https://dmarcian.com/spf-syntax-table/#exists)
   * 포함(https://dmarcian.com/spf-syntax-table/#include)

   예를 들어, &quot;v=spf1 a mx에는 다음이 포함됩니다. [spf.workfront.com](http://spf.workfront.com/) -all&quot;

회사 정책으로 인해 방화벽에 SPF 레코드를 추가할 수 없는 경우, [!DNL Workfront] 지원 담당자.
