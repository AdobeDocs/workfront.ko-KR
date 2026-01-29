---
title: Adobe Workfront Planning에서 요청 양식에 승인 추가
description: 레코드를 생성하기 전에 Adobe Workfront Planning 요청 양식에 승인 프로세스를 추가하여 제출된 모든 요청에 대한 승인을 시작할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
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

* 한 명 이상의 승인자를 요청 양식에 추가할 수 있습니다. 사용자만 승인자로 추가할 수 있습니다.
* 승인자 및 승인 일자 필드에 요청 양식을 실행하여 생성된 레코드에 승인 정보를 표시할 수 있습니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.
* 요청 양식에 여러 승인자를 추가할 때, Workfront Planning에서 레코드가 생성되기 전에 모든 승인자가 요청을 수락해야 합니다.
* 모든 승인자가 요청을 승인하면 요청 양식과 연결된 레코드 종류에 대한 레코드가 만들어집니다.
* 최소 한 명 이상의 승인자가 요청을 거부하고 다른 모든 승인자가 요청을 승인하면 Workfront의 요청 영역에 대해 요청이 만들어지지만 요청 양식과 연결된 레코드 유형에 대해서는 레코드가 만들어지지 않습니다.
* 요청 양식에 승인을 추가하는 것은 선택 사항입니다. Workfront Planning은 요청 양식이 승인과 연관되지 않은 경우 요청이 제출되면 즉시 레코드를 생성합니다.

## 프로덕션 환경에서 요청 양식에 승인 추가

1. [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)에 설명된 대로 레코드 유형에 대한 요청 양식 만들기를 시작합니다.
1. **구성**&#x200B;을 클릭합니다.

   **구성** 영역이 표시됩니다.

   ![구성 탭](assets/configuration-tab.png)
1. **승인자** 필드에서 승인자로 설정할 사용자 또는 팀의 이름을 입력한 다음 목록에 표시될 때 선택합니다.
1. (선택 사항 및 조건부) 두 명 이상의 승인자를 설정했으며 결정을 내리는 데 한 명의 승인자만 필요한 경우 **한 개의 결정만 필요합니다** 옵션을 활성화합니다.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* 한 명 또는 여러 명의 승인자를 요청 양식에 추가할 수 있습니다.
   >
   >* 두 명 이상의 승인자를 추가하고 [하나의 결정만 필요] 옵션을 활성화하지 않은 경우 Workfront Planning이 레코드를 생성하기 전에 모든 승인자가 요청을 승인해야 합니다.
   >
   >* 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다. 요청은 Workfront의 요청 영역에 남아 있습니다.
   >
   >* 두 명 이상의 승인자를 추가할 때 [하나의 결정만 필요] 옵션이 활성화되어 있지 않은 경우 요청이 승인 또는 거부되기 전에 모든 승인자가 결정을 내려야 합니다.
   >
   >* 팀이 승인자로 설정된 경우 팀에서 하나의 결정만 필요합니다.


1. (선택 사항) 요청 양식을 공유한 적이 없으면 **게시**&#x200B;를 클릭합니다.

   또는

   양식을 공유하려면 **공유**&#x200B;를 클릭한 다음 **링크 복사**&#x200B;를 클릭합니다.
1. (선택 사항) 사용자가 공유하는 링크를 사용하고 요청을 제출하면 Workfront Planning은 승인자에게 승인 인앱 알림과 이메일을 보냅니다.

   >[!NOTE]
   >
   >   사용자가 이메일 및 인앱 알림을 수신할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.


   요청 승인에 대한 자세한 내용은 [요청 승인](/help/quicksilver/planning/requests/approve-request.md)을 참조하세요.

<div class="preview">

## 요청 양식에 승인 규칙 추가

>[!NOTE]
>
>이 기능은 미리보기 환경에서만 사용할 수 있습니다.

승인 규칙은 제출된 요청의 필드 값에 따라 승인 프로세스를 정의합니다.

예를 들어 요청 양식에 &quot;캠페인 유형&quot; 필드가 있는 경우, 필드에 &quot;디지털&quot; 값이 있을 경우 한 사람에게, &quot;인쇄&quot; 값이 있을 경우 다른 사람에게 요청을 보내는 규칙을 만들 수 있습니다.

승인 규칙을 추가할 때 다음 사항을 고려하십시오.

* 한 명 또는 여러 명의 승인자를 승인 규칙에 추가할 수 있습니다.
* 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다. 요청은 Workfront의 요청 영역에 남아 있습니다.
* 두 명 이상의 승인자를 추가할 때 [하나의 결정만 필요] 옵션이 활성화되어 있지 않은 경우 요청이 승인 또는 거부되기 전에 모든 승인자가 결정을 내려야 합니다.
* 팀이 승인자로 설정된 경우 팀에서 하나의 결정만 필요합니다.

승인 추가에 대한 자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

요청 양식에 대한 승인 규칙을 설정하려면 다음을 수행합니다.

1. [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)에 설명된 대로 레코드 유형에 대한 요청 양식 만들기를 시작합니다.
1. **설정**&#x200B;을 클릭합니다.

   설정 탭이 표시됩니다.

1. 승인 규칙 구성을 시작하려면 왼쪽 탐색에서 승인 ![승인 아이콘](assets/approvals-icon-on-form.png)을 클릭하세요.

1. (선택 사항) 기본 승인 프로세스를 설정하려면 기본 승인 규칙 영역의 **승인자** 필드에 사용자 또는 팀을 한 명 이상 추가한 다음 기본 승인자 중 한 명이 승인한 후에 레코드를 만들려면 **한 개의 결정만 필요합니다** 확인란을 클릭합니다.

   ![기본 승인 규칙 영역](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (선택 사항) 각 추가 승인 규칙에 대해 다음을 수행합니다.

   1. **승인 규칙 추가** 클릭
   1. 자리 표시자 제목 &quot;제목 없는 승인 규칙&quot;을 클릭하고 승인 규칙의 이름을 입력합니다.
   1. **필드 선택**&#x200B;을 클릭하고 규칙을 활성화할 필드를 선택합니다.
   1. 규칙에 대한 연산자를 선택합니다. 연산자는 필드 유형에 따라 다릅니다.
   1. 선택한 연산자에 값이 필요한 경우 더하기 아이콘을 클릭하고 값을 하나 이상 추가합니다.
   1. (선택 사항) 조건 추가를 클릭하고 C-E 단계에서와 같이 추가 조건을 구성하여 AND 또는 OR를 사용하여 조건을 더 추가합니다.
   1. 승인 규칙의 작업 영역의 **승인자** 필드에서 조건이 충족될 때 승인자에서 설정할 사용자 또는 팀을 하나 이상 추가합니다.
   1. 
      1. (조건부) 승인자 중 한 명이 레코드를 승인한 후 레코드를 만들려면 **한 개의 결정만 필요합니다** 확인란을 선택합니다.

1. **저장**&#x200B;을 클릭하여 승인 규칙을 저장합니다.
1. (선택 사항) 요청 양식을 공유한 적이 없으면 **게시**&#x200B;를 클릭합니다.

</div>
