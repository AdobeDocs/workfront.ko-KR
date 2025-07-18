---
title: Adobe Systems Workfront Planning 사용 시 라이센스 유형 개요
description: Adobe Systems Workfront Planning에 대한 액세스 권한은 개체에 대한 사용 권한 외에도 라이센스 유형에 따라 다릅니다. 조직의 모든 사용자에게 Adobe Systems Workfront Planning을 사용할 수 있는 동일한 액세스 및 권한이 있는 것은 아닙니다. 이 문서에서는 Adobe Systems Workfront Planning에 대해 사용자가 가질 수 있는 액세스 수준에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Adobe Systems Workfront Planning을 사용하는 경우의 라이센스 유형 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Systems Workfront 라이센스 유형은 Adobe Systems Workfront Planning 권한과 함께 작동하여 다음과 같은 액세스 권한을 부여합니다.

* 작업 영역 또는 레코드 종류 보기, 참가 또는 관리
* 보기 또는 관리 보기.

Workfront Planning의 개체에 대한 사용 권한에 대한 자세한 내용은 Adobe Systems Workfront Planning[의 사용 권한 공유 개요를 참조하십시오](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Workfront Planning에 대한 액세스에 대한 자세한 내용은 Adobe Systems Planning 액세스 개요를[ 참조하십시오](/help/quicksilver/planning/access/access-overview.md).

## Workfront 라이선스 유형과 Workfront Planning 권한 간의 관계

아래 표에서는 Adobe Systems Workfront의 사용자 라이선스 유형과 해당 라이선스를 기반으로 하는 Adobe Systems Workfront Planning 개체에 부여할 수 있는 권한 수준 간의 관계를 설명합니다.

작업 영역에 사용자 권한을 부여하면 레코드 종류, 레코드 및 필드에 대한 권한도 부여됩니다.

사용자에게 작업 영역에 대한 권한 외에도 보기에 대한 별도의 권한을 부여해야 보기에 액세스하고 관리 할 수 있습니다.

레코드 종류 사용 권한을 사용할 때 다음 사항을 고려합니다.

* 사용자는 작업 영역에서 레코드 종류 권한을 자동으로 상속합니다.
* 사용자 사용자에게 작업 영역 관리 권한이 있는 경우 레코드 종류에 대한 더 낮은 액세스 권한을 가질 수 없습니다.
* 사용자는 레코드 종류가 속한 작업 영역 영역보다 레코드 종류에 대해 더 큰 권한을 가질 수 없습니다.
* 레코드 종류에 대한 사용자의 사용 권한을 제거해도 작업 영역에 대한 사용 권한은 제거되지 않으므로 작업 영역의 모든 레코드 종류에 대한 보기 액세스 권한은 제거되지 않습니다.

| Adobe Systems Workfront 라이센스 유형* | Adobe Systems Workfront Planning에서 허용되는 가장 높은 권한 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 표준 | <p>사용자는 작업 영역, 레코드 종류 및 보기를 관리 할 수 있습니다. 작업 영역, 레코드 종류, 레코드, 필드 및 보기를 만들거나, 편집하거나, 삭제할 수 있습니다.</p> <br> <p>시스템 관리자에게는 자신이 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 관리 권한이 있습니다.</p> |
| Light 또는 Contributor | <p>사용자는 공유된 작업 영역과 해당 작업 영역의 레코드 종류, 레코드 및 필드를 볼 수 있습니다.</p> <br> <p>사용자는 공유된 뷰를 볼 수 있지만 자신의 뷰를 만들 수는 없습니다. </p><br> <p>사용자는 작업 공간, 레코드 종류, 레코드 또는 필드를 생성, 편집 또는 삭제할 수 없습니다.</p> |

*Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다.
자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하세요](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


### 작업 영역 및 레코드 종류에 대한 라이센스 종류 및 사용 권한License types and permissions to workspaces and record types

Standard 라이센스가 있는 사용자만 작업 영역 및 레코드 종류에 대한 Contribute 또는 Manage 권한을 가질 수 있습니다. 작업 영역 및 레코드 종류에 대한 Contribute 및 Manage 권한도 레코드 및 필드로 이전됩니다.

다른 모든 라이선스 유형이 있는 사용자는 공유된 작업 영역 및 레코드 종류뿐만 아니라 해당 레코드 및 필드에 대한 보기 권한을 가질 수 있습니다.

시스템 관리자는 자신이 생성하지 않은 작업 공간을 포함하여 시스템의 모든 작업 공간을 볼 수 있습니다.

>[!INFO]
>
>**본보기:**
>
>기여자 또는 라이트 라이센스 사용자는 작업 영역 및 해당 개체에 기여하거나 관리 할 수 없습니다.
>
>공유 상자에는 사용자가 하위 수준 라이선스를 보유하고 있는 경우 이러한 권한 수준이 흐리게 표시되므로 작업 영역에 기여하거나 관리 권한을 부여할 수 없다는 표시가 있습니다.
>
>![작업 영역에서 기여자 사용자에 대한 권한이 회색으로 표시됨](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### 보기에 대한 라이센스 유형 및 권한

Standard 라이선스가 있는 사용자만 보기에 대한 관리 권한을 가질 수 있습니다. 다른 모든 라이센스 유형을 가진 사용자는 자신과 공유된 보기에 대한 보기 권한을 가질 수 있습니다.

>[!INFO]
>
>**본보기:**
>
>기여자 또는 라이트 라이센스 사용자는 보기를 관리 할 수 없습니다. 액세스 가능한 보기에 임시 필터, 정렬 또는 그룹화를 적용할 수 있습니다.
>
>공유 상자에는 사용자가 하위 수준 라이선스를 보유하고 있는 경우 이러한 권한 수준이 흐리게 표시되므로 보기를 관리 권한을 부여할 수 없다는 표시가 있습니다.
>
>![보기 공유의 라이트 사용자 권한이 회색으로 표시됨](assets/permissions-grayed-out-for-light-user.png)
