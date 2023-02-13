---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 새 사용자에게 보내는 이메일 초대 관리
description: Adobe Workfront 관리자는 이메일 초대장을 사용하여 Workfront에 사용자를 추가하고 사용자를 추가했음을 사용자에게 알릴 수 있습니다.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# 새 사용자에게 보내는 이메일 초대 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront 관리자는 이메일 초대장을 사용하여 Workfront에 사용자를 추가하고 사용자를 추가했음을 사용자에게 알릴 수 있습니다.

이메일 초대를 사용하면 새 사용자가 Workfront 계정의 암호를 선택할 수 있는 링크를 따라갈 수 있습니다. 그런 다음 계정 설정을 완료할 수 있습니다.

새 계정의 보안을 보장하기 위해 새 사용자가 자신의 암호를 선택할 수 있도록 이메일 초대를 사용하는 것이 좋습니다. 또는 계정을 만들 때 새 사용자의 암호를 선택할 수도 있습니다. Workfront에 새 사용자를 추가하는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

다음에 대한 새 사용자 이메일을 구성할 수 있습니다.

* Workfront에 추가된 새로운 사용자
* 요청자 라이센스를 사용하여 Workfront에 추가된 사용자

새 사용자는 전자 메일 초대장을 보낼 때 동일한 전자 메일을 볼 수 있습니다.

전자 메일 초대 수신에 대한 자세한 내용은 [이메일 초대 받기 및 Adobe Workfront용 암호 만들기](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

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
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

## 이메일 초대 생성 {#generate-email-invitations}

이메일 초대장은 다음 시나리오에서 생성됩니다.

* 새 사용자를 만들고 **이 사람에게 초대 전자 메일 보내기** on **새 사용자** 양식. 새 사용자 만들기에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 새 사용자를 여러 개 가져오고 **다음 사용자에게 초대 전자 메일 보내기** 선택 사항입니다. 새 사용자 가져오기에 대한 자세한 내용은 [사용자 가져오기](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* 사용자가 만들어지면 Workfront에 계정을 아직 등록하지 않았고 Workfront 암호를 설정하지 않은 사용자에 대한 초대를 수동으로 생성할 수 있습니다.\
   계정을 만들었지만 계정을 아직 등록하지 않은 사용자는 **등록되지 않음** Workfront.

   >[!NOTE]
   >
   >을 선택 취소하는 경우 **이 사람에게 전자 메일 초대 보내기** 상자를 사용하면 사용자를 만들 때 이메일 초대를 수동으로 생성할 수 없습니다. 계정을 만들 때 원래 이메일 초대를 보낸 사용자만 이메일 초대를 수동으로 다시 보낼 수 있습니다. 새 사용자 만들기에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

기존의 등록되지 않은 사용자에게 보내는 이메일 초대장을 수동으로 생성하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).
1. 을 표시하는 사용자를 선택합니다 **등록되지 않음** 레이블 지정

   ![](assets/unreg-user-qs-350x221.png)

1. 자세히 아이콘을 클릭합니다 ![](assets/more-icon.png)를 클릭한 다음 **사용자에게 등록 알림**.

   새 사용자에게 Workfront 암호를 만드는 데 사용할 수 있는 새 링크가 있는 이메일 초대장이 전송됩니다.

   >[!NOTE]
   >
   >조직에 Admin Console이 온보딩되어 있고 Workfront을 통해 사용자를 추가하는 경우 새 사용자에게 이메일 초대장을 보낼 수 없습니다.
   >
   >새 Adobe 사용자가 Admin Console에 추가되고, Admin Console이 프로세스를 완료하도록 초대하는 이메일을 보냅니다. 모든 사용자는 Adobe 시스템에 액세스하려면 등록 프로세스를 완료해야 합니다.
   >
   >기존 Adobe 사용자의 경우, 사용자는 사용 가능한 Workfront에 대한 이메일을 받을 수도 있고 받을 수도 없습니다. 이는 제품의 Adobe 관리자가 제어하는 기본 설정입니다.

## 이메일 초대 구성 {#configure-email-invitations}

Workfront 관리자는 새 사용자를 위한 이메일 초대장과 함께 포함하는 메시지를 구성할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 목록에서 **이메일** > **초대**.

1. 에서 **일반 옵션** 섹션을 수정하고 다음 사항을 수정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>다음 날 후 초대 링크를 비활성화합니다.</strong> </td> 
      <td> <p>이메일 초대를 더 이상 Workfront에 대한 유효한 링크가 포함되지 않는 시간을 선택합니다. 기본 일수는 45일입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>메시지 및/또는 서비스 기간을 포함합니다</strong> </td> 
      <td> <p>Workfront에 추가된 모든 새 사용자에 대한 이메일 초대를 수정하려면 이 옵션을 선택합니다. 요청자 라이센스가 있는 사용자는 포함되지 않습니다.</p> 
       <ul> 
        <li><strong>메시지</strong>: 모든 새 사용자에 대한 이메일 초대를 수정하도록 선택하는 경우 이메일 초대장에 포함할 텍스트를 이메일 본문으로 지정합니다.</li> 
        <li><strong>약관</strong>: 모든 새 사용자에 대한 이메일 초대를 수정하도록 선택하는 경우 이메일 초대장에 포함할 텍스트를 약관 로 지정합니다.<br></li> 
        <li><strong>헬프데스크 사용자를 위한 메시지 및/또는 서비스 기간 포함</strong>: 요청자 라이센스가 있는 Workfront에 추가된 모든 새 사용자에 대한 이메일 초대를 수정하려면 이 옵션을 선택합니다.</li> 
        <li><strong>메시지</strong>: 요청자 라이센스를 가진 모든 신규 사용자의 이메일 초대를 수정하도록 선택하는 경우 이메일 초대에 포함할 텍스트를 이메일 본문으로 지정합니다.</li> 
        <li><strong>약관</strong>: 요청자 라이센스를 가진 모든 신규 사용자의 이메일 초대를 수정하도록 선택하는 경우 이메일 초대장에 포함할 텍스트를 약관에 지정합니다.<br></li> 
        <li> <p>에서 <strong>초대 미리 보기</strong> 섹션에서 이메일 초대 미리 보기를 볼 수 있습니다. 이메일 초대를 통해 사용자 지정된 메시지를 포함하도록 선택한 경우 사용자 지정된 메시지가 이 영역에 표시됩니다.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
