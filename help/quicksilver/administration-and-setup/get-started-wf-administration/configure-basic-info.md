---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 시스템에 대한 기본 정보 구성
description: Adobe Workfront 시스템 구성의 일부로, 고객 정보 페이지의 기본 정보 섹션에서 조직에 대한 세부 정보를 관리할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 83d236a4d50c0eef7062f161757d2f9fe6bc4e06
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---

# 시스템 기본 정보 구성하기

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Adobe Workfront 시스템 구성의 일부로, 고객 정보 페이지의 기본 정보 섹션에서 조직에 대한 세부 정보를 관리할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 고객 정보 액세스

고객은 조직의 Workfront 인스턴스를 나타냅니다. 이 영역의 옵션은 Workfront 고객인 사용자에게 고유합니다.

고객 정보 페이지에 액세스하려면:

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **고객 정보**&#x200B;를 클릭합니다.

   구입한 Workfront 플랜에 따라 고객 정보 페이지에서 일부 섹션이 누락될 수 있습니다. 조직에서 사용하는 Workfront 플랜을 확인해야 하는 경우 계정 담당자에게 문의하십시오.

   고객 정보 영역에서 사용할 수 있는 섹션은 다음과 같습니다.

   * **기본 정보**

     Workfront에서 기본 정보를 구성하는 방법에 대한 자세한 내용은 [기본 정보 구성](#configure-basic-info)을 참조하십시오.

   * **API 키 설정**

     API 키 설정에 대한 자세한 내용은 [API 키 관리](../../administration-and-setup/manage-workfront/security/manage-api-keys.md)를 참조하십시오.

   * **IP 허용 목록**

     사용자가 Workfront허용 목록에 추가하다 에 액세스할 수 있는 IP 주소를 허용 목록에 추가하는 방법에 대한 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

   * **전자 메일 허용 목록**

     전자 메일을 허용 목록에 추가하다허용 목록에 추가하다 에 추가하는 방법에 대한 자세한 내용은 [전자 메일 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)을 참조하십시오.

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## 기본 정보 구성 {#configure-basic-info}

고객 정보 페이지의 기본 정보 영역 내에서 고객에 대한 일부 세부 정보는 Workfront으로 구성되며 읽기 전용 모드로 표시됩니다. 기타 세부 사항은 사용자가 구성할 수 있습니다. 이 영역에서 편집할 수 있는 모든 옵션은 Workfront의 모든 사용자에게 전역 영향을 줍니다.

고객 정보 영역에서 기본 정보 섹션을 구성하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **고객 정보**&#x200B;를 클릭합니다.

1. **고객 정보** 페이지 상단의 **기본 정보** 섹션에서 Workfront 인스턴스에 대한 다음 정보를 찾으십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td>회사의 이름과 일치하는 조직의 이름입니다. 이 은(는) Workfront에 의해 추가되며 편집할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">클러스터 설정 </td> 
      <td>인스턴스의 클러스터 번호입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리자 이메일</td> 
      <td> <p>Workfront 관리자의 이메일 주소입니다. Workfront 관리자 중 한 명의 이메일 주소와 일치하도록 이 필드를 편집할 수 있습니다. 이 이메일 주소와 연결된 사용자는 Workfront 시스템의 주요 Workfront 관리자로 간주됩니다. Workfront의 모든 사이트 전체 커뮤니케이션은 이 이메일 주소로 전달되므로 지속적으로 업데이트하는 것이 중요합니다.</p> <p><b>참고</b>: 관리자 전자 메일에 연결된 사용자의 액세스 수준을 비활성화, 삭제 또는 변경할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">도메인</td> 
      <td> <p>도메인은 계정이 생성될 때 Workfront에서 설정합니다.</p> <p>도메인은 Workfront에 액세스하는 데 사용하는 URL의 고유한 하위 도메인을 식별합니다.<p>예를 들어 조직에 "mycompany" 도메인이 할당된 경우 Workfront에 액세스하는 데 사용하는 URL은 <i>https://mycompany.my.workfront.com.</i>입니다.</p><p>직접 도메인을 편집할 수는 없습니다. 도메인을 변경하려면 Workfront 고객 지원 센터에 문의할 수 있습니다. Workfront 고객 지원 센터에 문의하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">고객 지원 센터에 문의</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간대</td> 
      <td> <p>Workfront 인스턴스의 기본 시간대입니다. 이 필드를 편집하여 기본 Workfront 위치의 시간대와 일치시킬 수 있습니다. 선택하는 시간대는 다음을 결정합니다. </p> 
       <ul> 
        <li>발신 이메일에 표시된 날짜 및 시간</li> 
        <li>새 사용자가 생성될 때의 기본 시간대</li> 
       </ul> <p>사용자는 프로필에서 Workfront 인스턴스의 시간대를 수정할 수 있습니다. 사용자가 시간대를 수정하면 Workfront에서 보낸 이메일의 날짜와 시간이 프로필 환경 설정과 일치합니다. 사용자 프로필 환경 설정 수정에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>을 참조하십시오. 새 일정을 만들 때 기본 시간대로 선택됩니다. 일정 만들기에 대한 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">일정 만들기</a>를 참조하세요.</p> <p>사용자가 시간대 간에 Workfront에서 공동 작업하는 데 일정을 사용하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">시간대 간 작업</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 이메일 로케일</td> 
      <td>발신 전자 메일 메시지에 사용되는 언어, 날짜 및 숫자 형식을 제어합니다. 여기에서 선택한 로케일은 새 사용자를 만들 때 기본값입니다. 사용자는 사용자 프로필에서 로케일을 수정할 수 있습니다. 사용자가 로케일을 수정하면 Workfront 이메일의 언어, 날짜 및 번호 형식이 프로필 환경 설정과 일치합니다. 프로필 환경 설정 수정에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>을 참조하세요.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">스토리지 할당량</td> 
      <td> <p>Workfront 인스턴스에서 사용할 수 있는 문서 저장 공간의 양입니다.<br>할당량에는 Workfront에 직접 업로드하는 문서가 포함되어 있습니다.<br>다음을 포함하지 않습니다.</p> 
       <ul> 
        <li>다른 서드파티 서비스 공급자(SharePoint, Google Drive, Webdam, Box, Dropbox, 기타 모든 Document Asset Management 공급자)로부터 Workfront에 연결하는 문서입니다.</li> 
        <li>Workfront 데이터(프로젝트, 작업, 문제, 사용자 등).</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
