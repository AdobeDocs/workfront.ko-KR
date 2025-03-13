---
title: Adobe Workfront Planning 사용 시 라이선스 유형 개요
description: Adobe Workfront Planning에 대한 액세스 권한은 객체에 대한 권한 외에 라이선스 유형에 따라 다릅니다. 조직의 모든 사용자가 Adobe Workfront Planning을 사용할 수 있는 동일한 액세스 및 권한을 가지고 있는 것은 아닙니다. 이 문서에서는 사용자가 Adobe Workfront Planning에 보유할 수 있는 액세스 수준에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# Adobe Workfront Planning 사용 시 라이선스 유형 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront 라이선스 유형은 Adobe Workfront Planning 권한과 함께 작동하여 다음 액세스 권한을 부여합니다.

* 작업 영역 <!--<span class="preview">or record types</span>--> 보기, 참여 또는 관리
* 보기를 보거나 관리합니다.

Workfront Planning의 개체에 대한 사용 권한에 대한 자세한 내용은 [Adobe Workfront Planning의 사용 권한 공유 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

Workfront Planning에 액세스하는 방법에 대한 자세한 내용은 [Adobe Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.

## Workfront 라이선스 유형과 Workfront Planning 권한 간의 관계

아래 표에서는 Adobe Workfront에 있는 사용자의 라이선스 유형과 해당 라이선스를 기반으로 Adobe Workfront Planning 개체에 부여할 수 있는 권한 수준 간의 관계를 설명합니다.

작업 영역에 대한 사용자 권한을 부여하면 레코드 유형, 레코드 및 필드에 대한 권한도 부여됩니다.

보기에 액세스하고 관리할 수 있도록 작업 공간에 대해 보유하고 있는 권한 외에 보기에 대한 별도의 권한을 사용자에게 부여해야 합니다.

<!--

<div class="preview">

Consider the following when working with record type permissions: 

* Users automatically inherit record type permissions from workspaces. 
* When a user has Manage permissions to a workspace, they cannot have a lesser access to record type. 
* Users cannot have greater permissions to a record type than they have for the workspace the record type belongs to.

</div>
-->

| Adobe Workfront 라이선스 유형* | Adobe Workfront Planning에서 허용되는 가장 높은 권한 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 표준 | <p>사용자는 작업 영역 <!--<span class="preview">, record types, </span> --> 및 보기를 관리할 수 있습니다. 작업 공간, 레코드 유형, 레코드, 필드 및 보기를 생성, 편집 또는 삭제할 수 있습니다.</p> <br> <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 관리 권한을 가집니다.</p> |
| 라이트 또는 기여자 | <p>사용자는 공유된 작업 공간과 해당 작업 공간의 레코드 유형, 레코드 및 필드를 볼 수 있습니다.</p> <br> <p>사용자는 공유된 보기를 볼 수 있지만 자신의 보기를 만들 수는 없습니다. </p><br> <p>사용자는 작업 공간, 레코드 유형, 레코드 또는 필드를 작성, 편집 또는 삭제할 수 없습니다.</p> |

*Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다.
자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.


### 작업 공간에 대한 라이선스 유형 및 권한

<!--should we add "record types" in the title above and to this section?-->

표준 라이선스가 있는 사용자만 작업 영역 <!--<span class="preview">and record types</span>-->에 대한 Contribute 또는 Manage 권한을 가질 수 있습니다. 작업 영역 <!--<span class="preview">and record types</span>-->에 대한 Contribute 및 Manage 권한도 레코드 종류, 레코드 및 필드로 전송됩니다.

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

다른 모든 라이선스 유형을 가진 사용자는 레코드 유형, 레코드 및 필드뿐만 아니라 공유된 작업 공간 <!--<span class="preview"> and record types </span> -->에 대한 보기 권한을 가질 수 있습니다.

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

시스템 관리자는 작성하지 않은 작업 영역을 포함하여 시스템의 모든 작업 영역을 볼 수 있습니다.

<!--does the shot below need to be replaced for record types??-->

>[!INFO]
>
>**예:**
>
>기여자 또는 라이트 라이선스 사용자는 작업 공간 및 해당 개체에 기여하거나 관리할 수 없습니다.
>
>하위 수준 라이선스를 보유하고 있는 경우 이러한 권한 수준이 흐리게 표시되므로 사용자에게 작업 영역에 기여하거나 관리할 수 있는 권한을 부여할 수 없다는 표시가 공유 상자에 표시됩니다.
>
>![작업 영역의 기여자 사용자에 대한 권한이 회색으로 표시됨](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### 라이선스 유형 및 보기에 대한 권한

Standard 라이선스를 가진 사용자만 보기에 대한 관리 권한을 가질 수 있습니다. 다른 모든 라이선스 유형을 가진 사용자는 공유된 보기에 대한 보기 권한을 가질 수 있습니다.

>[!INFO]
>
>**예:**
>
>기여자 또는 라이트 라이선스 사용자는 보기를 관리할 수 없습니다. 액세스 가능한 보기에 임시 필터, 정렬 또는 그룹화를 적용할 수 있습니다.
>
>하위 수준 라이선스를 보유하고 있는 경우 이러한 권한 수준이 흐리게 표시되므로 사용자에게 보기 관리에 대한 권한을 부여할 수 없다는 표시가 공유 상자에 있습니다.
>
>![보기 공유에서 라이트 사용자에 대한 사용 권한이 회색으로 표시됨](assets/permissions-grayed-out-for-light-user.png)
