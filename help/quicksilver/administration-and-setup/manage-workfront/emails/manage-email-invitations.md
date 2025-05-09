---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 새 사용자에 대한 이메일 초대 관리
description: Adobe Workfront 관리자는 전자 메일 초대를 사용하여 Workfront에 사용자를 추가하고 추가되었음을 알릴 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: dccbd5a036e1b148bc8f3e41fac3a67babe6dc9a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 새 사용자를 위한 이메일 초대 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

Adobe Workfront 관리자는 전자 메일 초대를 사용하여 Workfront에 사용자를 추가하고 추가되었음을 알릴 수 있습니다.

이메일 초대를 통해 신규 사용자는 링크를 따라 Workfront 계정의 암호를 선택할 수 있습니다. 그런 다음 계정 설정을 완료할 수 있습니다.

새 계정의 보안을 위해 새 사용자가 자신의 암호를 선택할 수 있도록 새 사용자에 대한 이메일 초대를 사용하는 것이 좋습니다. 또는 계정을 만들 때 새 사용자에 대한 암호를 선택할 수도 있습니다. Workfront에 새 사용자를 추가하는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

다음에 대한 새 사용자 이메일을 구성할 수 있습니다.

* Workfront에 추가된 모든 새 사용자
* 요청자 라이선스가 있는 Workfront에 추가된 사용자

이메일 초대를 보내면 모든 신규 사용자에게 동일한 이메일이 표시됩니다.

전자 메일 초대 수신에 대한 자세한 내용은 [전자 메일 초대 받기 및 Adobe Workfront 암호 만들기](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md)를 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 등록되지 않은 기존 사용자에게 이메일 초대 다시 보내기

전자 메일 초대는 다음 시나리오에서 생성됩니다.

* 새 사용자를 만들 때 **새 사용자** 양식에서 **이 사용자에게 초대 이메일 보내기**&#x200B;를 선택합니다. 새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.
* 새 사용자를 여러 명 가져오고 **이 사용자에게 초대 이메일 보내기** 옵션을 선택하는 경우. 여러 명의 새 사용자를 가져오는 방법에 대한 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)를 참조하십시오.
* 사용자가 생성되면 아직 Workfront에 계정을 등록하지 않았고 Workfront 암호를 설정하지 않은 사용자에게 초대를 수동으로 생성할 수 있습니다.\
  계정을 만들었지만 아직 계정을 등록하지 않은 사용자는 Workfront에서 **등록되지 않음**(으)로 표시됩니다.

  >[!NOTE]
  >
  >사용자를 만들 때 **이 사람에게 전자 메일 초대를 보내기** 상자를 선택 취소하면 전자 메일 초대를 수동으로 생성할 수 없습니다. 계정을 만들 때 원래 이메일 초대를 보낸 사용자만 이메일 초대를 수동으로 다시 보낼 수 있습니다. 새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

등록되지 않은 기존 사용자에게 이메일 초대를 수동으로 다시 보내려면

{{step-1-to-users}}

1. 이름 뒤에 **등록되지 않음** 레이블을 표시하는 사용자를 선택하십시오.

   ![등록 취소됨](assets/unreg-user-qs-350x221.png)

1. 기타 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **사용자에게 등록 알림**&#x200B;을 클릭합니다.

   새 사용자에게 Workfront 암호를 만드는 데 사용할 수 있는 새 링크로 이메일 초대가 전송됩니다.

   >[!NOTE]
   >
   >조직이 Admin Console에 온보딩되고 Workfront을 통해 사용자를 추가하는 경우 새 사용자에게 이메일 초대를 보낼 수 있는 옵션이 없습니다.
   >
   >새 Adobe 사용자가 Admin Console에 추가되고 Admin Console에서 이메일을 보내어 등록 프로세스를 완료합니다. 모든 사용자가 모든 Adobe 시스템에 액세스하려면 등록 프로세스를 완료해야 합니다.
   >
   >기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받지 못할 수도 있습니다. 이는 제품에 대해 Adobe 관리자가 제어하는 기본 설정입니다.

## 이메일 초대 구성 {#configure-email-invitations}

Workfront 관리자는 새 사용자에 대한 이메일 초대에 포함하는 메시지를 구성할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 목록에서 **전자 메일** > **초대**&#x200B;를 클릭합니다.

1. **일반 옵션** 섹션에서 다음을 수정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>다음 날짜 이후에 초대 링크 비활성화...</strong> </td> 
      <td> <p>이메일 초대에 더 이상 Workfront에 대한 유효한 링크가 포함되지 않는 시간을 선택합니다. 기본 일수는 45일입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>메시지 및/또는 서비스 기간 포함</strong> </td> 
      <td> <p>Workfront에 추가된 모든 신규 사용자에 대한 이메일 초대를 수정하려면 이 옵션을 선택합니다. 여기에는 요청자 라이선스가 있는 사용자는 포함되지 않습니다.</p> 
       <ul> 
        <li><strong>메시지</strong>: 모든 새 사용자에 대한 전자 메일 초대를 수정하도록 선택한 경우 전자 메일 초대에 포함할 텍스트를 전자 메일 본문으로 지정하십시오.</li> 
        <li><strong>약관</strong>: 모든 새 사용자에 대한 전자 메일 초대를 수정하도록 선택한 경우 전자 메일 초대에 포함할 텍스트를 약관으로 지정하십시오.<br></li> 
        <li><strong>안내 데스크 사용자를 위한 메시지 및/또는 서비스 기간을 포함하십시오</strong>: 요청자 라이선스가 있는 Workfront에 추가된 모든 새 사용자에 대한 전자 메일 초대를 수정하려면 이 옵션을 선택하십시오.</li> 
        <li><strong>메시지</strong>: 요청자 라이선스를 가진 모든 새 사용자에 대한 전자 메일 초대를 수정하도록 선택한 경우 전자 메일 초대에 포함할 텍스트를 전자 메일 본문으로 지정하십시오.</li> 
        <li><strong>약관</strong>: 요청자 라이선스를 가진 모든 새 사용자에 대한 전자 메일 초대를 수정하도록 선택한 경우 전자 메일 초대에 포함할 텍스트를 약관으로 지정하십시오.<br></li> 
        <li> <p><strong>초대 미리 보기</strong> 섹션에서 전자 메일 초대의 미리 보기를 볼 수 있습니다. 이메일 초대에 사용자 지정된 메시지를 포함하기로 선택한 경우 사용자 지정된 메시지가 이 영역에 표시됩니다.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
