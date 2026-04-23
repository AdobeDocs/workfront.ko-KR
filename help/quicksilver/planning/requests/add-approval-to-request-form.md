---
title: Adobe Workfront Planning에서 요청 양식에 승인 추가
description: 레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 1%

---

# Adobe Workfront Planning에서 요청 양식에 승인 추가

<!--update the metadata with real information when making this available in TOC and in the left nav-->

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

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

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

* 한 명 이상의 승인자를 요청 양식에 추가할 수 있습니다. 사용자와 팀을 승인자로 추가할 수 있습니다.
* 승인자 및 승인 일자 필드에 요청 양식을 실행하여 생성된 레코드에 승인 정보를 표시할 수 있습니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.
* 요청 양식에 여러 승인자를 추가할 때, Workfront Planning에서 레코드가 생성되기 전에 모든 승인자가 요청을 수락해야 합니다.
* 모든 승인자가 요청을 승인하면 요청 양식과 연결된 레코드 종류에 대한 레코드가 만들어집니다.
* 최소 한 명 이상의 승인자가 요청을 거부하고 다른 모든 승인자가 요청을 승인하면 Workfront의 요청 영역에 대해 요청이 만들어지지만 요청 양식과 연결된 레코드 유형에 대해서는 레코드가 만들어지지 않습니다.
* 요청 양식에 승인을 추가하는 것은 선택 사항입니다. Workfront Planning은 요청 양식이 승인과 연관되지 않은 경우 요청이 제출되면 즉시 레코드를 생성합니다.

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## 요청 양식에 승인 규칙 추가

승인 규칙은 제출된 요청의 필드 값을 기준으로 승인 프로세스를 정의합니다.

예를 들어 요청 양식에 &quot;캠페인 유형&quot; 필드가 있는 경우, 필드에 &quot;디지털&quot; 값이 있을 경우 한 사람에게, &quot;인쇄&quot; 값이 있을 경우 다른 사람에게 요청을 보내는 규칙을 만들 수 있습니다.

승인 규칙을 추가할 때 다음 사항을 고려하십시오.

* 한 명 또는 여러 명의 승인자를 승인 규칙에 추가할 수 있습니다.
* 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다. 요청은 Workfront의 요청 영역에 남아 있습니다.
* 두 명 이상의 승인자를 추가할 때 [하나의 결정만 필요] 옵션이 활성화되어 있지 않은 경우 요청이 승인 또는 거부되기 전에 모든 승인자가 결정을 내려야 합니다.
* 팀이 승인자로 설정된 경우 팀의 한 멤버로부터 하나의 결정만 필요합니다.

요청 양식에 대한 승인 규칙을 설정하려면 다음을 수행합니다.

1. [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md) 문서에 설명된 대로 레코드 유형에 대한 요청 양식 만들기를 시작합니다.
1. 요청 양식이 열리면 **설정**&#x200B;을 클릭합니다.

   **설정** 탭이 열립니다.

1. 승인 규칙 구성을 시작하려면 왼쪽 패널에서 **승인** ![승인 아이콘](assets/approvals-icon-on-form.png)을 클릭하세요.

1. (선택 사항) 기본 승인 프로세스를 설정하려면 **기본 승인 규칙** 영역의 **승인자** 필드에 하나 이상의 사용자 또는 팀을 추가한 다음 기본 승인자 중 하나가 승인했을 때 레코드를 만들려면 **한 개의 결정만 필요합니다** 확인란을 클릭합니다.

   ![기본 승인 규칙 영역](assets/default-approvers.png)

1. (선택 사항) 승인 규칙 추가를 시작합니다. 각 사용자 지정 승인 규칙에 대해 다음 작업을 수행합니다.

   1. **승인 규칙 추가** 클릭
   1. 자리 표시자 제목 **제목 없는 승인 규칙**&#x200B;을 클릭하고 승인 규칙의 이름을 입력합니다.
   1. **필드 선택**&#x200B;을 클릭하고 규칙을 활성화할 필드를 선택합니다.
   1. 규칙에 대한 연산자를 선택합니다. 연산자는 필드 유형에 따라 다릅니다.
   1. 선택한 연산자에 값이 필요한 경우 더하기 아이콘을 클릭하고 값을 하나 이상 추가합니다.
   1. (선택 사항) 조건을 더 추가하려면 **조건 추가**&#x200B;를 클릭하고 C-E단계와 같이 추가 조건을 구성하여 **And** 또는 **Or** 문을 통해 연결합니다.
   1. 승인 규칙의 **작업** 영역의 **승인자** 필드에 조건이 충족될 때 승인자에서 설정할 사용자 또는 팀을 하나 이상 추가하십시오.
   1. (조건부 및 선택 사항) 승인자 중 한 명이 레코드를 승인한 후 레코드를 만들려면 **한 개의 결정만 필요합니다** 확인란을 선택하십시오. 그렇지 않으면 모든 승인자는 요청이 승인되거나 거부되기 전에 승인을 결정해야 합니다.

   >[!NOTE]
   >
   >   승인 규칙을 추가할 때 다음 사항을 고려하십시오.
   >
   >   * 기본 규칙만 설정된 경우, 제출된 모든 요청에 적용됩니다.
   >   * 사용자 지정 규칙이 충족되면 기본값이 요청 승인 워크플로에 적용되지 않습니다. 일치하는 사용자 지정 규칙만 승인에 적용되고 기본 규칙은 무시됩니다.
   >   * 여러 사용자 지정 규칙이 충족되면 해당 순서의 첫 번째 규칙이 적용됩니다. 이 경우 기본 승인이 있는 경우 적용되지 않습니다.

1. **저장**&#x200B;을 클릭하여 승인 규칙을 저장합니다.
1. (선택 사항) 요청 양식을 공유한 적이 없으면 **게시**&#x200B;를 클릭합니다.
