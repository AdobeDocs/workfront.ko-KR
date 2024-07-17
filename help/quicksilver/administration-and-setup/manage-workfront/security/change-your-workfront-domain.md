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
source-git-commit: 22ea9b623d7bc7b216511538cf88e4d020529bd3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Adobe Workfront 도메인 변경

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Workfront 도메인을 변경할 수 없습니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 프로시저 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

Adobe Workfront 관리자 및 인증된 Workfront 지원 담당자는 Workfront 지원 팀에 조직의 Workfront 도메인을 변경하는 데 도움을 요청할 수 있습니다.

## 액세스 요구 사항

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 도메인 변경 요청

1. Experience League 시 지원 티켓 만들기를 시작합니다.
1. **설명** 상자에 원하는 새 도메인과 새 도메인을 실행하려는 기간을 포함하십시오.
1. 지원 사례에 대한 상자 작성을 완료한 다음 **제출**&#x200B;을 클릭합니다.

Workfront 지원 센터에 문의하여 도메인 변경에 대한 도움을 받을 수도 있습니다.

## SSO 고객인 경우 새 도메인 업데이트

회사에서 SSO를 활용하는 경우 Workfront 도메인을 변경한 후 다음 단계를 수행해야 합니다.

>[!NOTE]
>
>조직의 Workfront 인스턴스가 Adobe IMS를 사용하여 활성화된 경우 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 사이드바에서 **시스템** > **고객 정보**&#x200B;를 클릭하고 고객 정보 페이지에서 도메인이 업데이트되었는지 확인하십시오.

1. 왼쪽 사이드바에서 **시스템** > **SSO(Single Sign-On)**&#x200B;를 클릭합니다.

1. **SAML 2.0 메타데이터 다운로드**&#x200B;를 클릭합니다.
1. 파일이 다운로드되면 열고 다음 사항을 확인합니다.

   1. **entityID**&#x200B;이(가) 새 도메인을 가리키고 있습니다.
   1. **`<md:AssertionConsumerService>`** 내의 모든 위치가 새 도메인을 가리킵니다.

1. 다운로드한 메타데이터 파일을 나중에 업데이트할 수 있도록 ID 공급자에게 제공합니다.
1. 조직에서 사용하는 모든 Workfront 통합에 대해 도메인이 업데이트되었는지 확인합니다.
