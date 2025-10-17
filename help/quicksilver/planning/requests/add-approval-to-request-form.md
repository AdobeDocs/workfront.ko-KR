---
title: Adobe Workfront Planning에서 요청 양식에 승인 추가
description: 레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Adobe Workfront Planning에서 요청 양식에 승인 추가

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.

이 문서에서는 작업 영역 관리자가 레코드 유형과 연결된 요청 양식에 승인을 추가하는 방법에 대해 설명합니다.

Workfront Planning에서 요청 양식을 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

레코드를 만들기 위해 레코드 형식에 요청을 제출하는 방법에 대한 자세한 내용은 [레코드를 만들기 위한 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 패키지 및 모든 Planning 패키지</p>
또는
<p>모든 워크플로우 패키지 및 모든 Planning 패키지</p>

<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류</a>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 양식에 승인을 추가하는 것에 대한 고려 사항

* 한 명 이상의 승인자를 요청 양식에 추가할 수 있습니다. 사용자만 승인자로 추가할 수 있습니다.
* 승인자 및 승인 일자 필드에 요청 양식을 실행하여 생성된 레코드에 승인 정보를 표시할 수 있습니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.
* 요청 양식에 여러 승인자를 추가할 때, Workfront Planning에서 레코드가 생성되기 전에 모든 승인자가 요청을 수락해야 합니다.
* 모든 승인자가 요청을 승인하면 요청 양식과 연결된 레코드 종류에 대한 레코드가 만들어집니다.
* 최소 한 명 이상의 승인자가 요청을 거부하고 다른 모든 승인자가 요청을 승인하면 Workfront의 요청 영역에 대해 요청이 만들어지지만 요청 양식과 연결된 레코드 유형에 대해서는 레코드가 만들어지지 않습니다.
* 요청 양식에 승인을 추가하는 것은 선택 사항입니다. Workfront Planning은 요청 양식이 승인과 연관되지 않은 경우 요청이 제출되면 즉시 레코드를 생성합니다.

## 요청 양식에 승인 추가

1. [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)에 설명된 대로 레코드 유형에 대한 요청 양식 만들기를 시작합니다.
1. **구성**&#x200B;을 클릭합니다.

   **구성** 영역이 표시됩니다.

   ![구성 탭](assets/configuration-tab.png)
1. **승인자** 필드에서 드롭다운 아이콘을 클릭하고 목록에서 하나 또는 여러 명의 사용자 또는 팀을 선택합니다

   또는

   승인자로 설정할 사용자 또는 팀의 이름을 입력한 다음 목록에 표시될 때 선택합니다.

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
   >
   >* 팀이 승인자로 설정된 경우 팀에서 하나의 결정만 필요합니다.


1. (선택 사항) 요청 양식을 공유한 적이 없으면 **게시**&#x200B;를 클릭합니다

   또는

   양식을 공유하려면 **공유**&#x200B;를 클릭한 다음 **링크 복사**&#x200B;를 클릭합니다.
1. (선택 사항) 사용자가 공유하는 링크를 사용하고 요청을 제출하면 Workfront Planning은 승인자에게 승인 인앱 알림과 이메일을 보냅니다.

   >[!NOTE]
   >
   >   사용자가 이메일 및 인앱 알림을 수신할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.


   요청 승인에 대한 자세한 내용은 [요청 승인](/help/quicksilver/planning/requests/approve-request.md)을 참조하세요.
