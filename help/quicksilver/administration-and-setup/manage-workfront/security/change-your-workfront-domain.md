---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfront 도메인 변경
description: Adobe Workfront 관리자 및 인증된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하는 데 도움을 요청할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Adobe Workfront 도메인 변경

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Workfront 도메인을 변경할 수 없습니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자 및 인증된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하는 데 도움을 요청할 수 있습니다.

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

## 도메인 변경 요청

1. 다음을 클릭합니다. **지원** Workfront One 페이지에서 탭을 클릭한 다음 지원 사례를 만들기 시작합니다.
1. 다음에서 **설명** 상자에는 원하는 새 도메인과 새 도메인을 시작하려는 일정이 포함됩니다.
1. 지원 사례에 대한 상자 채우기를 완료한 다음 을(를) 클릭합니다 **제출**.

Workfront 지원 센터에 문의하여 도메인 변경에 대한 도움을 받을 수도 있습니다.

## SSO 고객인 경우 새 도메인 업데이트

회사에서 SSO를 활용하는 경우 Workfront 도메인을 변경한 후 다음 단계를 수행해야 합니다.

>[!NOTE]
>
>조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 사이드바에서 을 클릭합니다. **시스템** > **고객 정보** 고객 정보 페이지에서 도메인이 업데이트되었는지 확인하십시오.

1. 왼쪽 사이드바에서 을 클릭합니다. **시스템** > **SSO(단일 인증)**.

1. 클릭 **SAML 2.0 메타데이터 다운로드**.
1. 파일이 다운로드되면 열고 다음 사항을 확인합니다.

   1. **entityID** 은(는) 새 도메인을 가리킵니다.
   1. 내의 모든 위치 **`<md:AssertionConsumerService>`** 새 도메인을 가리킵니다.

1. 다운로드한 메타데이터 파일을 나중에 업데이트할 수 있도록 ID 공급자에게 제공합니다.
1. 조직에서 사용하는 모든 Workfront 통합에 대해 도메인이 업데이트되었는지 확인합니다.
