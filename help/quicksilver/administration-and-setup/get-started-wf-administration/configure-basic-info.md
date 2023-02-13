---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 시스템에 대한 기본 정보 구성
description: Adobe Workfront 시스템 구성의 일부로, 고객 정보 페이지의 기본 정보 섹션에서 조직에 대한 세부 사항을 관리할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# 시스템에 대한 기본 정보 구성

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Adobe Workfront 시스템 구성의 일부로, 고객 정보 페이지의 기본 정보 섹션에서 조직에 대한 세부 사항을 관리할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> <col> 
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
   <td> <p>Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 고객 정보 액세스

고객은 조직의 Workfront 인스턴스를 나타냅니다. 이 영역의 옵션은 Workfront의 고객으로서 사용자에게 고유합니다.

고객 정보 페이지에 액세스하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템** > **고객 정보**.

   구매한 Workfront 계획에 따라 고객 정보 페이지에서 일부 섹션이 누락될 수 있습니다. 조직에서 사용하는 Workfront 계획을 찾아야 하는 경우에는 계정 담당자에게 문의하십시오.

   고객 정보 영역에서 사용할 수 있는 섹션은 다음과 같습니다.

   * **기본 정보**

      Workfront에서 기본 정보 구성에 대한 자세한 내용은 [기본 정보 구성](#configure-basic-info).

   * **API 키 설정**

      API 키 설정에 대한 자세한 내용은 [API 키 관리](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP 허용 목록**

      사용자가 Workfront에 액세스할 수 있는에 IP 주소허용 목록에 추가하다를 추가하는 방법에 대한 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **라이선스**

      라이센스에 대한 자세한 내용은 [시스템에서 사용 가능한 라이센스 관리](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## 기본 정보 구성 {#configure-basic-info}

고객 정보 페이지의 기본 정보 영역 내에서 고객에 대한 일부 세부 사항은 Workfront에서 구성하며 읽기 전용 모드로 표시됩니다. 기타 세부 사항은 사용자가 구성할 수 있습니다. 이 영역에서 편집할 수 있는 모든 옵션은 Workfront의 모든 사용자에게 전역 영향을 줍니다.

고객 정보 영역에서 기본 정보 섹션을 구성하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **시스템** > **고객 정보**.

1. 에서 **기본 정보** 섹션 맨 위에 있는 **고객 정보** 페이지에서 Workfront을 사용하여 인스턴스에 대한 다음 정보를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td>회사 이름과 일치하는 조직의 이름입니다. 이 항목은 Workfront에 의해 추가되며 편집할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">클러스터 설정 </td> 
      <td>인스턴스에 대한 클러스터 번호입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리자 이메일</td> 
      <td> <p>Workfront 관리자의 이메일 주소입니다. Workfront 관리자 중 한 명의 이메일 주소와 일치하도록 이 필드를 편집할 수 있습니다. 이 이메일 주소와 연결된 사용자는 Workfront 시스템의 기본 Workfront 관리자로 간주됩니다. Workfront에서 제공하는 모든 사이트 전체 통신은 이 이메일 주소로 전송되므로 이를 계속 업데이트해야 합니다.</p> <p><b>참고</b>: 관리자 이메일에 연결된 사용자의 액세스 수준을 활성화, 삭제 또는 변경할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">도메인</td> 
      <td> <p>도메인은 계정이 만들어지면 Workfront에서 설정합니다.</p> <p>도메인은 Workfront에 액세스하는 데 사용하는 URL의 고유한 하위 도메인을 식별합니다.<p>예를 들어 조직에 "mycompany" 도메인이 할당된 경우 Workfront에 액세스하는 데 사용하는 URL은 <i>https://mycompany.my.workfront.com</i></p><p>도메인을 직접 편집할 수는 없습니다. 도메인을 변경하려면 Workfront 고객 지원 센터에 문의하십시오. Workfront 고객 지원 센터에 문의하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">고객 지원에 문의</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간대</td> 
      <td> <p>Workfront 인스턴스의 기본 시간대입니다. 기본 Workfront 위치의 시간대와 일치하도록 이 필드를 편집할 수 있습니다. 선택하는 시간대에는 다음 내용이 결정됩니다. </p> 
       <ul> 
        <li>보내는 전자 메일에 표시된 날짜 및 시간</li> 
        <li>새 사용자를 만들 때 기본 시간대입니다</li> 
       </ul> <p>사용자는 프로필 아래에서 Workfront 인스턴스에 대한 시간대를 수정할 수 있습니다. 사용자가 시간대를 수정하면 Workfront에서 이메일의 날짜 및 시간이 프로필 환경 설정과 일치합니다. 사용자 프로필 기본 설정 수정에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>. 새 일정을 만들 때 기본 시간대로 선택됩니다. 예약 작성에 대한 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">예약 만들기</a>.</p> <p>시간대에서 Workfront에서 사용자가 공동 작업하는 데 도움이 되는 예약을 사용하는 방법에 대한 자세한 내용은 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">시간대 작업</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">로케일</td> 
      <td>보내는 전자 메일 메시지에 사용되는 언어, 날짜 및 숫자 형식을 제어합니다. 새 사용자가 생성될 때 기본적으로 여기서 선택한 로케일이 사용됩니다. 사용자는 사용자 프로필에서 로케일을 수정할 수 있습니다. 사용자가 로케일을 수정하면 Workfront에서 이메일의 언어, 날짜 및 숫자 형식이 프로필 환경 설정과 일치합니다. 프로필 환경 설정 수정에 대한 자세한 내용은 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">내 설정 구성</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">스토리지 할당량</td> 
      <td> <p>Workfront 인스턴스에서 사용할 수 있는 문서 저장 공간의 크기입니다.<br>할당량에 Workfront에 직접 업로드하는 문서가 포함되어 있습니다.<br>포함되지 않습니다.</p> 
       <ul> 
        <li>다른 타사 서비스 공급자(SharePoint, Google Drive, Webdam, Box, Dropbox, 기타 Document Asset Management 공급자)에서 Workfront에 연결하는 문서입니다.</li> 
        <li>Workfront 데이터(프로젝트, 작업, 문제, 사용자 등)입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제품 버전</td> 
      <td>사용자에게 할당된 Workfront 인스턴스의 유형입니다. 대부분의 Workfront 고객을 위한 제품 버전은 다음과 같습니다 <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
