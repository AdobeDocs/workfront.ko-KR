---
title: Adobe Systems Workfront Planning에서 요청 승인
description: 사용자가 Adobe Systems Workfront Planning의 승인과 연결된 요청 양식에 요청을 제출하면 승인자는 보류 중인 승인에 대한 알림과 이메일을 받게 됩니다. Workfront Planning에서 객체를 생성하기 전에 요청 권한을 승인해야 합니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 1%

---

# Adobe Workfront Planning에서 요청 승인

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 프로덕션에 대한 월별 릴리스 후에는 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 조직에[ 대한 빠른 릴리스 활성화 또는 비활성화를 참조하세요](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

사용자가 Adobe Systems Workfront Planning의 승인과 연결된 요청 양식에 요청을 제출하면 승인자는 보류 중인 승인에 대한 알림과 이메일을 받게 됩니다. Workfront Planning에서 객체를 생성하기 전에 요청 권한을 승인해야 합니다.

이 문서에서는 작업 영역 관리자가 Workfront Planning에 제출된 요청 요청을 승인하여 레코드를 만드는 방법을 설명합니다.

다음 문서도 참조하는 것이 좋습니다.

* [Adobe Systems Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)
* [Adobe Systems Workfront Planning 요청을 제출하여 레코드 만들기](/help/quicksilver/planning/requests/submit-requests.md)
* [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## 요청 승인에 대한 고려 사항

* 제출된 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 다음 요청 상태 중 하나로 표시됩니다.

   * **검토** 보류 중: 이 상태는 승인자가 요청 개체를 열지 않은 경우에 표시됩니다.
   * **검토 중**: 하나 이상의 승인자가 요청 개체를 열면 **검토 보류 중** 상태가 **검토 중**(으)로 변경됩니다. 모든 승인자가 요청을 승인할 때까지 요청의 상태가 **검토 중** 상태로 유지됩니다.
   * **승인됨**: 승인자가 요청 개체를 승인하면 개별 상태는 **승인됨**&#x200B;이 되지만, 전체 요청 개체 상태는 모든 승인자가 결정을 내릴 때까지 **검토 중**&#x200B;으로 유지됩니다. 모든 승인자가 요청을 승인하면 요청 상태는 **승인됨**&#x200B;이 됩니다.
   * **완료**: 모든 승인자가 요청 개체를 승인하면 상태가 **완료**(으)로 변경되거나 요청에 승인이 필요하지 않은 경우.
   * **거부됨**: 승인자가 요청 개체를 거부하면 상태가 거부됨&#x200B;**이 됩니다**. 레코드가 만들어지지 않으며 레코드를 만들려면 새 요청을 제출해야 합니다.

* <span class="preview">요청 양식을 제출하여 만든 레코드에 대한 승인 정보를 승인자 및 승인 날짜 필드에 표시할 수 있습니다. 자세한 내용은 필드[ 만들기 섹션을 참조하십시오](/help/quicksilver/planning/fields/create-fields.md).</span>

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td>
   <td>
<p>어떤 </p>  
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </td>

<tr>
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>표준</p>
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <ul>
   <li><p>작업 공간 및 레코드 유형에 대한 권한 관리 </p></li>
    <li><p>시스템 관리자는 자신이 만들지 않은 작업 공간을 관리할 수 있습니다. </p></li>
    </ul>
   <p>Workfront Planning 객체의 권한 공유에 대한 자세한 내용은  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning의 공유 권한 개요</a> 
  </td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## 레코드를 만들기 위한 요청 승인

사용자가 승인과 연결된 레코드 종류 요청 양식에 요청을 추가하면 요청이 승인자에게 전송됩니다.

승인자는 승인 대기 중인 요청 중에 다음과 같은 알림을 받습니다.

* 인앱 알림
* 이메일 알림

>[!NOTE]
>
>사용자가 이메일 및 인앱 알림을 수신할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.

요청을 승인하려면:

1. 다음 중 하나를 수행하십시오.

   * Workfront Planning에 액세스하여 하나 이상의 작업 영역을 볼 수 있는 경우 화면 오른쪽 상단의 **주 메뉴** ![점 주 메뉴](assets/dots-menu.png) 또는 사용 가능한 경우 왼쪽 상단의 **주 메뉴** ![선 주 메뉴](assets/lines-menu.png)를 클릭한 다음 **요청** > **제출됨** > **계획**&#x200B;을 클릭하고 **검토 보류 중** 또는 **검토 중** 상태의 요청을 클릭합니다.

     >[!TIP]
     >
     >Workfront Planning에 액세스할 수 없거나 작업 공간을 볼 수 있는 액세스 권한이 없는 경우, 이메일 또는 인앱 알림을 사용하여 승인 요청 요청에만 액세스할 수 있습니다.

   * **화면 오른쪽 위 모서리에 있는 Unified Shell**&#x200B;의 알림![ 영역 아이콘 ](assets/notifications-area-icon-unified-shell.png)알림 영역 아이콘을 클릭하고 승인 보류 중인 요청에 대한 알림을 클릭하여 요청을 엽니다.
   * 승인 대기 중인 요청 대해 알려주는 이메일의 이메일 알림 이동한 다음 요청&#x200B;**열기를 클릭하여**&#x200B;요청 엽니다.<!--add the name of the button here, from the email-->

   요청 페이지가 읽기 전용 모드로 열립니다.

   ![검토 상태의 읽기 전용 요청 페이지](assets/read-only-reqeust-page-in-review-status.png)

1. (선택 사항) 승인자를 보려면 요청의 오른쪽 상단에 있는 **승인** 아이콘 ![승인 아이콘](assets/approvals-icon.png)을 클릭합니다.
1. 검토 및 승인을&#x200B;**클릭한**&#x200B;후 다음 중 하나를 선택합니다.

   * **승인**: 요청 승인을 합니다. 모든 승인자가 요청을 승인한 후 요청 양식과 연결된 레코드 종류에 대한 레코드가 즉시 만들어집니다.
   * **거부**: 요청, 거부하는 유일한 승인자인 경우 균일 거부합니다. 요청 양식과 연결된 레코드 종류에 대한 레코드가 만들어지지 않습니다.

   요청을 제출한 사용자는 요청이 승인되거나 거부될 때 이메일과 앱 알림을 받습니다.

   요청 상태는 승인 결정에 따라 다음과 같이 변경됩니다.

   * **완료**&#x200B;됨: 요청 승인.
   * **거부됨**: 요청 요청이 거부됩니다.

   요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 남아 있습니다.
