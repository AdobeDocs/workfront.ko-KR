---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 시스템 보안 환경 설정 구성
description: Adobe Workfront 관리자는 Workfront 시스템에 대한 보안 환경 설정을 구성할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 04cf9d37c681398f5a0e2b9d7d45c0f8b93ab44b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 5%

---

# 시스템 보안 환경 설정 구성

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Adobe Workfront 관리자는 Workfront 시스템에 대한 보안 환경 설정을 구성할 수 있습니다.

* 모바일 앱 및 기타 통합 애플리케이션에서 Workfront 액세스
* iframe에 Workfront 포함 규칙

시스템 환경 설정에서 변경한 사항은 시스템의 모든 사용자와 Workfront의 해당 경험에 영향을 줍니다.

Workfront 구현 중에 시스템 보안 환경 설정을 구성하고 가끔 해당 후 다시 방문하는 것이 좋습니다.

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

## 시스템 보안 환경 설정 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템** > **기본 설정**.

1. 에서 **보안** 섹션에서 다음 필드 중 하나를 선택하여 조직의 보안 설정을 설정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>포함 허용 <strong>Workfront</strong> iframe에서</p> </td> 
      <td>Workfront을 iframe에 포함할 수 있습니다.<p>이 옵션은 기본적으로 비활성화됩니다.</p><p><b>중요 사항</b>: 웹 기반 애플리케이션을 iframe에 표시하면 애플리케이션에서 클릭 추적 보안 취약성이 발생합니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 추가 기능에서 SAML 2.0 인증 허용</td> 
      <td> <p>Workfront이 SAML 2.0 단일 사인온 솔루션과 통합될 때 Office 365 추가 기능에 대해서만 iframe에 Workfront을 포함할 수 있습니다. </p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p><b>참고</b>: 위의 옵션을 활성화하면, <strong>iframe에 Workfront 포함 허용</strong>, 옵션 <strong>Office 365 추가 기능에서 SAML 2.0 인증 허용</strong> 이 활성화되고 흐리게 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">외부 페이지 URL을 생성할 때 세션 정보 사용을 활성화합니다</td> 
      <td> <p>외부 페이지를 대시보드에 추가할 때 사이트의 세션 ID 정보를 사용할 수 있도록 해줍니다.</p> <p>대시보드에 외부 페이지 추가에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">대시보드에 외부 웹 페이지 포함</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사람들이 Workfront의 모바일 애플리케이션 및 <strong>Workfront</strong> Outlook 추가 기능</td> 
      <td> <p>사용자가 모바일 앱(iPad 및 휴대폰 앱의 Workfront 보기) 및 Workfront Outlook 앱에 액세스할 수 있습니다.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다. </p> <p>Workfront 보기에 대한 자세한 내용은 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront 보기 사용</a>. 모바일 앱에 대한 자세한 내용은 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Adobe Workfront 모바일 앱 사용</a>.</p> <p>Outlook 플러그인에 대한 자세한 내용은 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Outlook용 Adobe Workfront 설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 주소를 사용하여 Workfront 계정이 없는 사람과 공동 작업</p> </td> 
      <td>Workfront 사용자가 이름 대신 이메일 주소를 포함하여 Workfront 계정이 없는 사람과 특정 항목을 공유할 수 있습니다. 사용자는 전자 메일 주소를 사용하여 외부 사용자와 다음 항목을 공유할 수 있습니다.
       <ul>
        <li>문서<br></li>
        <li>문서 요청<br></li>
        <li>문서 승인</li>
        <li>캘린더</li>
       </ul><p>이 옵션은 기본적으로 활성화되어 있습니다.</p> <p><b>중요 사항</b>: 이 옵션을 비활성화하면 Workfront 인스턴스에서 외부 사용자 액세스 수준을 사용할 수 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfront의 내장된 액세스 수준</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">외부 사용자는 암호를 사용해 등록해야 합니다</td> 
      <td> <p>Workfront에서 항목을 보기 전에 외부 사용자가 등록해야 합니다. 기본적으로 이 옵션은 비활성화됩니다. 이 옵션을 활성화하면 이메일 주소로 특정 업데이트에 포함된 Workfront 계정이 없는 사람에게 계정을 만들라는 메시지가 표시되면 포함된 항목을 볼 수 있습니다. 그러면 외부 사용자 계정이 만들어집니다.</p> <p>이 옵션은 기본적으로 비활성화됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음 시간 후 자동으로 사용자 로그아웃</td> 
      <td> 비활성 기간 후, 사용자가 Workfront에서 로그아웃되는 시기를 지정할 수 있습니다. 기본적으로 사용자는 8시간 동안 활동이 없으면 로그아웃됩니다. <p>이 옵션은 단일 사인온 솔루션을 사용하는 Workfront 고객에게도 영향을 줍니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음 시간 후 자동으로 모바일 사용자 로그아웃 </td> 
      <td>사용자가 비활성 기간 후 Workfront 애플리케이션에서 로그아웃되는 시기를 지정할 수 있습니다. 기본적으로 사용자는 7일 동안 활동이 없으면 로그아웃됩니다. <p>이 옵션은 단일 사인온 솔루션을 사용하는 Workfront 고객에게도 영향을 줍니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

   여기서 저장한 변경 내용은 Workfront의 모든 사용자 및 외부 사용자로 상호 작용하는 모든 사용자의 경험에 영향을 줍니다.
