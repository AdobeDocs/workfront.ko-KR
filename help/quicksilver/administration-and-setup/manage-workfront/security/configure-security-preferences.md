---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 시스템 환경 설정 구성
description: Adobe Workfront 관리자는 보안 환경 설정을 포함하여 Workfront 시스템에 대한 환경 설정을 구성할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 5%

---

# 시스템 환경 설정 구성

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 다음을 포함하여 Workfront 시스템에 대한 환경 설정을 구성할 수 있습니다.

* 모바일 앱 및 기타 통합 애플리케이션에서 Workfront에 액세스
* iframe에 Workfront 포함 규칙

시스템 환경 설정에서 변경한 사항은 시스템의 모든 사용자와 Workfront에서의 경험에 영향을 줍니다.

Workfront 구현 중에 시스템 환경 설정을 구성하고, 그 이후에 가끔씩만 다시 방문하는 것이 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 시스템 환경 설정 구성

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **기본 설정**&#x200B;을 클릭합니다.

1. 다음 필드 중 하나를 선택하여 조직에 대한 설정을 설정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>빠른 릴리스 프로세스 활성화</p> </td> 
      <td>분기별 릴리스 대신 조직에 대한 월별 Workfront 릴리스를 활성화할 수 있습니다.</p><p>빠른 릴리스 프로세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">조직의 빠른 릴리스 사용 또는 사용 안 함</a>을 참조하세요.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>iframe에 Workfront 포함 허용</p> </td> 
      <td>Workfront을 iframe에 포함할 수 있습니다.<p>이 옵션은 기본적으로 비활성화되어 있습니다.</p><p><b>중요</b>: iframe에 웹 기반 응용 프로그램을 표시하면 응용 프로그램이 클릭재킹 보안 취약성이 발생할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 추가 기능에서 SAML 2.0 인증 허용</td> 
      <td> <p>Workfront을 SAML 2.0 Single Sign-On 솔루션과 통합할 때 Office 365 추가 기능에 대한 iframe에서만 Workfront을 포함할 수 있습니다. </p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p><b>참고</b>: 위의 옵션 <strong>iframe에 Workfront 포함 허용</strong>을 사용하면 <strong>Office 365 추가 기능에서 SAML 2.0 인증 허용</strong> 옵션이 활성화되고 흐리게 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">외부 페이지 URL을 만들 때 세션 정보 사용을 활성화합니다.</td> 
      <td> <p>대시보드에 외부 페이지를 추가할 때 사용자가 사이트의 세션 ID 정보를 사용할 수 있도록 허용합니다.</p> <p>이 옵션은 기본적으로 안전하지 않으며 꺼져 있습니다. 통합을 위해 대신 OAuth를 사용하는 것이 좋습니다.</p> <p>대시보드에 외부 페이지를 추가하는 방법에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">외부 웹 페이지를 대시보드에 포함</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사람들이 Workfront의 모바일 애플리케이션과 Workfront Outlook 추가 기능을 사용할 수 있도록 허용</td> 
      <td> <p>사용자가 모바일 앱(iPad 및 휴대폰 앱용 Workfront 보기) 및 Workfront Outlook 앱에 액세스할 수 있습니다.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다. </p> <p>Workfront 보기에 대한 자세한 내용은 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront 보기 사용</a>을 참조하세요. 모바일 앱에 대한 자세한 내용은 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Adobe Workfront 모바일 앱 사용: 문서 색인</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 주소를 사용하여 Workfront 계정이 없는 사람들과 공동 작업</p> </td> 
      <td>Workfront 사용자는 이름 대신 이메일 주소를 포함하여 Workfront 계정이 없는 사용자와 특정 항목을 공유할 수 있습니다. 사용자는 이메일 주소를 사용하여 외부 사용자와 다음 항목을 공유할 수 있습니다.
       <ul>
        <li>문서<br></li>
        <li>문서 요청<br></li>
        <li>문서 승인</li>
        <li>캘린더</li>
       </ul><p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p><b>중요</b>: 이 옵션을 사용하지 않도록 설정한 경우 Workfront 인스턴스에서 외부 사용자 액세스 수준을 사용할 수 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">기본 제공 액세스 수준</a>을 참조하세요.</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">사용자 정의 도움말 URL</td> 
      <td>메인 메뉴 도움말 아이콘이 이동할 내부 사용자 정의 도움말 사이트를 정의할 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">사용자 지정 도움말 URL 구성</a>을 참조하십시오.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">우선 순위 작업 목록 활성화 </td> 
      <td>사용자에 대해 우선 순위 작업 목록 환경을 활성화하거나 비활성화하도록 선택할 수 있습니다. 사용자는 Workfront에 우선순위 아이콘을 계속 볼 수 있지만 기능에 액세스할 수는 없습니다. 우선 순위에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">우선 순위 시작</a>을 참조하세요.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">AI 사용</span> </td> 
      <td><span class="preview">AI Assistant를 포함하여 AI를 활성화하도록 선택할 수 있습니다. <p><b>참고</b>: 조직에서 AI를 사용하려면 특정 요구 사항을 충족해야 합니다. 요구 사항을 포함하여 AI에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI Assistant 개요</a>를 참조하십시오.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">양식 자동 완성 </span></td> 
      <td><span class="preview">이전 요청 데이터를 기반으로 요청 양식을 자동 완성하는 기능을 활성화하도록 선택할 수 있습니다. 양식 자동 완성에 대한 자세한 내용은 <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">이전 데이터의 요청 자동 채우기</a>를 참조하십시오.</span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">AI Beta 참여 </span></td> 
      <td><span class="preview">현재 Beta에 있는 AI 기능을 활성화하도록 선택할 수 있습니다. 이 옵션을 활성화하면 활성화할 AI Beta 기능을 선택할 수 있습니다. 각 AI Beta 기능에 대한 자세한 내용을 보려면 해당 기능 옆에 있는 정보 아이콘을 클릭합니다.</span></td> 
     </tr>
     <tr> 
      <td role="rowheader">테스트 환경</td> 
      <td>Workfront 테스트 환경에 액세스할 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront 미리 보기 샌드박스 환경</a>을 참조하십시오.</p></td> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

   여기에 저장한 변경 사항은 Workfront의 모든 사용자와 외부 사용자로서 시스템과 상호 작용하는 모든 사용자의 경험에 영향을 줍니다.
