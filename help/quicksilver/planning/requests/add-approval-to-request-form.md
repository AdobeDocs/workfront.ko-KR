---
title: Adobe Workfront Planning에서 요청 양식에 승인 추가
description: 레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%

---

# Adobe Workfront Planning에서 요청 양식에 승인 추가

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.

이 문서에서는 작업 영역 관리자가 레코드 유형과 연결된 요청 양식에 승인을 추가하는 방법에 대해 설명합니다.

Workfront Planning에서 요청 양식을 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

레코드를 만들기 위해 레코드 형식에 요청을 제출하는 방법에 대한 자세한 내용은 [레코드를 만들기 위한 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

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
   <li><p> Adobe Workfront 계획<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
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
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
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
   <li><p>작업 공간 및 레코드 유형에 대한 권한 관리</p></li>
    <li><p>시스템 관리자는 자신이 만들지 않은 작업 공간을 관리할 수 있습니다. </p></li>
    </ul>
   <p>Workfront Planning 객체의 권한 공유에 대한 자세한 내용은  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning의 공유 권한 개요</a> 
  </td>
  </tr>

</tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 양식에 승인을 추가하는 것에 대한 고려 사항

* 한 명 이상의 승인자를 요청 양식에 추가할 수 있습니다. 사용자만 승인자로 추가할 수 있습니다.
* <span class="preview">승인자 및 승인 날짜 필드에 요청 양식을 제출하여 만든 레코드에 승인 정보를 표시할 수 있습니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md).</span>를 참조하세요.
* 요청 양식에 여러 승인자를 추가할 때, Workfront Planning에서 레코드가 생성되기 전에 모든 승인자가 요청을 수락해야 합니다.
* 모든 승인자가 요청을 승인하면 요청 양식과 연결된 레코드 종류에 대한 레코드가 만들어집니다.
* 최소 한 명 이상의 승인자가 요청을 거부하고 다른 모든 승인자가 요청을 승인하면 Workfront의 요청 영역에 대해 요청이 만들어지지만 요청 양식과 연결된 레코드 유형에 대해서는 레코드가 만들어지지 않습니다.
* 요청 양식에 승인을 추가하는 것은 선택 사항입니다. Workfront Planning은 요청 양식이 승인과 연관되지 않은 경우 요청이 제출되면 즉시 레코드를 생성합니다.

## 요청 양식에 승인 추가

1. [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)에 설명된 대로 레코드 유형에 대한 요청 양식 만들기를 시작합니다.
1. **구성**&#x200B;을 클릭합니다.

   **구성** 영역이 표시됩니다.

   ![구성 탭](assets/configuration-tab.png)
1. **승인자** 필드에서 드롭다운 아이콘을 클릭하고 목록에서 하나 또는 여러 이름을 선택합니다

   또는

   승인자의 이름을 입력한 다음 목록에 표시될 때 선택합니다.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* 한 명 또는 여러 명의 승인자를 요청 양식에 추가할 수 있습니다.
   >
   >* 두 명 이상의 승인자를 추가하는 경우 Workfront Planning에서 레코드를 생성하기 전에 모든 승인자가 요청을 승인해야 합니다.
   >
   >* 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다. 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 남아 있습니다.
   >
   >* 요청이 승인 또는 거부되기 전에 모든 승인자는 결정을 내려야 합니다.


1. (선택 사항) 요청 양식을 공유한 적이 없으면 **게시**&#x200B;를 클릭합니다

   또는

   양식을 공유하려면 **공유**&#x200B;를 클릭한 다음 **링크 복사**&#x200B;를 클릭합니다.
1. (선택 사항) 사용자가 공유하는 링크를 사용하고 요청을 제출하면 Workfront Planning은 승인자에게 승인 인앱 알림과 이메일을 보냅니다.

   >[!NOTE]
   >
   >   사용자가 이메일 및 인앱 알림을 수신할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.


   요청 승인에 대한 자세한 내용은 [요청 승인](/help/quicksilver/planning/requests/approve-request.md)을 참조하세요.
