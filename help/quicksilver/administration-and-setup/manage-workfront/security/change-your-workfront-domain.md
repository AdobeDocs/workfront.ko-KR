---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfront 도메인 변경
description: Adobe Workfront 관리자 및 승인된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하도록 지원을 요청할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Adobe Workfront 도메인 변경

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>조직이 Adobe Admin Console에 온보딩된 경우 Adobe Workfront 도메인을 변경하려면 다음을 참조하십시오 [도메인 설정](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자 및 승인된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하도록 지원을 요청할 수 있습니다.

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

## 도메인 변경 요청

1. 을(를) 클릭합니다. **지원** Workfront 한 페이지에서 탭을 클릭한 다음 지원 사례 만들기를 시작합니다.
1. 에서 **설명** 상자에 원하는 새 도메인과 새 도메인을 라이브로 전환할 기간을 포함하십시오.
1. 지원 사례에 대한 상자 작성을 완료한 다음 을 클릭합니다 **제출**.

Workfront 지원 센터에 문의하여 도메인 변경에 대한 도움을 받을 수도 있습니다.

## SSO 고객인 경우 새 도메인 업데이트

회사에서 SSO를 사용하는 경우 Workfront 도메인을 변경한 후 다음 단계를 수행해야 합니다.

>[!NOTE]
>
>Adobe IMS에서 조직의 Workfront 인스턴스가 활성화된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 사이드바에서 **시스템** > **고객 정보** 고객 정보 페이지에서 도메인이 업데이트되었는지 확인합니다.

1. 왼쪽 사이드바에서 **시스템** > **단일 사인온(SSO)**.

1. 클릭 **SAML 2.0 메타데이터 다운로드**.
1. 파일이 다운로드되면 파일을 열고 다음을 확인합니다.

   1. **entityID** 은(는) 새 도메인을 가리킵니다.
   1. 내의 모든 위치 **`<md:AssertionConsumerService>`** 새 도메인을 가리킵니다.

1. 다운로드한 메타데이터 파일을 ID 공급자에 제공하여 ID 공급자가 끝날 때 업데이트할 수 있도록 합니다.
1. 조직이 사용하는 모든 Workfront 통합에 대해 도메인이 업데이트되었는지 확인합니다.
