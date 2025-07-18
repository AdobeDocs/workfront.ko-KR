---
title: Adobe Workfront Planning의 공유 권한 개요
description: 조직의 모든 사용자에게 Adobe Systems Workfront Planning을 사용할 수 있는 동일한 액세스 및 권한이 있는 것은 아닙니다. 이 문서에서는 Adobe Workfront Planning 작업 영역 또는 보기에 대한 권한을 공유하거나 제거하는 방법에 대한 일반적인 정보를 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Adobe Systems Workfront Planning의 공유 권한 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Adobe Systems Workfront Planning 작업 영역, 레코드 유형 또는 보기에 대한 권한을 공유하거나 제거할 수 있습니다.

Planning 요청 양식을 공유할 수도 있습니다. 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

이 문서에서는 Workfront Planning 작업 공간, 레코드 유형, 레코드, 필드 및 보기에 대한 권한 수준에 대해 설명합니다.

## Adobe Workfront Planning에서 공유할 수 있는 객체

일부 Workfront Planning 객체는 수동으로 공유할 수 있지만 다른 객체는 다른 객체에서 이러한 권한을 상속합니다.

Workfront Planning에서 다음 객체를 수동으로 공유할 수 있습니다.

* 작업 영역

   * 조직 내부 사용자와 작업 공간을 공유할 수 있습니다.
   * 작업 영역 영역을 공유하면 작업 영역과 연결된 모든 레코드 종류, 레코드 및 필드도 공유됩니다.
   * 작업 영역 공유 시 보기는 공유되지 않습니다. 보기는 별도로 공유됩니다.

  자세한 내용은 작업 영역 공유를 참조하세요 [&#128279;](/help/quicksilver/planning/access/share-workspaces.md)

* 레코드 유형

   * 조직 내부의 사용자와 레코드 종류를 공유할 수 있습니다.
   * 작업 영역 영역에 부여된 사용 권한 수준은 레코드 종류에 대해 상속된 사용 권한으로 표시됩니다.
   * 사용자가 작업 영역에 대해 가지고 있는 것보다 더 높은 권한 수준으로 레코드 종류를 공유할 수 없습니다.

  자세한 내용은 레코드 종류[ 공유를 참조하십시오](/help/quicksilver/planning/access/share-record-types.md).


* 보기

   * 시스템 관리자를 포함한 사용자에게 작업 공간 액세스에 대한 권한과 별도로 보기에 액세스할 수 있는 권한을 부여해야 합니다.
   * 보기를 공유할 때 필터, 그룹화, 정렬 또는 설정을 포함한 모든 보기 요소가 공유됩니다.
   * 보기를 공유할 때 보기에 표시되는 레코드는 공유되지 않습니다. 레코드는 작업 영역을 공유하여 공유해야 합니다.
   * 보기에 대한 공개 링크 링크를 생성할 때 조직 외부 사용자와 공개적으로 보기를 공유할 수 있습니다. 공개 링크에서 레코드 페이지에 액세스하는 사용자는 연결된 레코드 및 필드를 포함하여 모든 레코드와 해당 필드를 볼 수 있습니다.

  자세한 내용은 보기[ 공유를 참조하십시오](/help/quicksilver/planning/access/share-views.md).

내부적으로 작업 공간, 보기 또는 레코드 유형을 다음 Workfront 엔티티와 공유할 수 있습니다.

* 사용자
* 그룹
* 팀
* 회사
* 작업 역할

작업 영역 및 레코드 종류를 다른 사용자와 공유하면 레코드 종류의 권한 수준이 연결된 레코드 및 필드로 자동으로 상속됩니다.

>[!IMPORTANT]
>
>조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩된 경우 Planning 개체를 공유하려는 사용자를 Adobe Admin Console에 추가해야 합니다. Planning 개체는 Adobe Admin Console 에 추가되지 않은 Workfront 사용자와 공유할 수 없습니다.


## Adobe Systems Workfront Planning의 개체 공유에 대한 고려 사항

* Adobe Systems Workfront 라이선스 유형은 Workfront Planning 권한과 함께 작동하여 작업 공간 및 해당 개체를 보고, 기여하고, 관리할 수 있는 액세스 권한을 부여합니다.

  라이선스 유형이 Workfront Planning의 권한 수준에 미치는 영향에 대한 자세한 내용은 Adobe Systems Workfront Planning[ 사용 시 라이선스 유형 개요를 참조하십시오](/help/quicksilver/planning/access/license-type-overview.md).
* 시스템 관리자는 자신이 생성하지 않은 작업 영역을 포함하여 시스템의 모든 작업 공간을 관리 할 수 있습니다.
* 시스템 관리자를 포함한 다른 사용자는 자신이 만들었거나 공유한 뷰에만 액세스할 수 있습니다. 시스템 관리자에게는 보기 관리 권한만 부여할 수 있습니다.
* 작업 영역 또는 뷰에 대한 링크 링크를 다른 사용자와 공유할 수 있습니다.

  다음과 같은 시나리오가 있습니다.
   * 작업 공간에 대한 링크를 받는 사용자는 활성 사용자여야 하며 작업 공간에 액세스하려면 Workfront에 로그인해야 합니다.
   * 보기에 대한 링크 링크를 받는 사용자는 다음과 같은 방법으로 보기에 액세스할 수 있습니다.

      * 뷰에 대한 링크 가 내부적으로 공유된 경우 활성 사용자이고 Workfront에 로그인해야 합니다.
      * Workfront의 외부 사용자일 수 있으며 Workfront에 로깅 하지 않고 공개적으로 공유된 링크 링크에서 뷰에 액세스할 수 있습니다.

## Adobe Systems Workfront Planning 개체에 대한 공유 권한

다음 섹션의 표에서는 작업 영역 또는 뷰를 공유할 때 선택할 수 있는 사용 권한 수준과 각 수준에서 허용하는 기능을 보여 줍니다.

>[!IMPORTANT]
>
>모든 사용자가 아래에 설명된 권한 수준을 가질 수 있는 것은 아닙니다. 사용자의 개별 라이선스에 따라 Workfront Planning 개체에 대해 받을 수 있는 권한 수준이 결정됩니다.
>
>표준(또는 플랜) 라이선스 사용자만 작업 영역에 대한 Contribute 또는 관리 권한과 보기에 대한 관리 권한을 가질 수 있습니다.
> 
>다른 모든 라이센스 유형이 있는 사용자는 작업 영역 및 보기에 대한 보기 권한을 가질 수 있습니다.
>
>자세한 내용은 Adobe Systems Workfront Planning[을 사용할 때의 라이센스 유형 개요를 참조하십시오](/help/quicksilver/planning/access/license-type-overview.md).


### 작업 영역에 대한 사용 권한

사용자에게 작업 영역에 대한 권한 부여하여 다음 엔터티에 액세스할 수 있도록 해야 합니다.

* 작업 영역
* 레코드 유형
* 레코드
* 필드

작업 공간에 대한 권한 수준은 다음과 같습니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 편집 | ✓ |            |       |
| 공유 | ✓ |            |       |
| 삭제 | ✓ |            |       |
| 보기 | ✓ | ✓ | ✓ |

### 레코드 유형에 대한 권한

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

작업 영역에 권한을 부여할 때 레코드 유형 권한은 항상 상속됩니다.

작업 영역에서 받은 레코드 유형의 상속된 권한을 제거할 수 있습니다.

사용자에게 작업 영역 권한보다 레코드 종류에 대한 낮은 권한을 부여할 수 있습니다.

그러나 다음을 수행할 수 없습니다.

* 레코드 종류에 대해 사용자가 작업 영역 영역에 대해 가지고 있는 것보다 더 높은 권한을 부여합니다.
* 작업 영역 관리자에게 레코드 종류에 대한 낮은 권한을 부여합니다.
* 레코드 종류 권한에서 사용자를 제거하여 레코드 종류 또는 작업 영역에 대한 보기 권한을 제거합니다.

다음과 같은 시나리오가 있습니다.

| 작업 영역 권한 | 레코드 종류에 대해 자동으로 상속된 권한 | 상속된 사용 권한이 꺼져 있을 때 가능한 레코드 종류 사용 권한(수동으로 부여됨) |
|--------|--------|-------------|
| 관리 | 관리 | 관리, 권한 제거* |
| 참여 | 참여 | Contribute, 보기 제거 권한* |
| 보기 | 보기 | 보기, 권한 제거* |

>[!NOTE]
>
>*레코드 유형에서 권한을 제거하면 작업 영역에서 해당 권한을 제거하지 않는 한 작업 영역과 모든 레코드 유형에 대한 보기 권한이 계속 유지됩니다.

### 레코드에 대한 권한

작업 영역 및 레코드 유형에 대한 권한을 부여하면 레코드 유형에서 레코드 권한이 상속됩니다.

다음은 레코드에 대한 권한 수준입니다.


|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ | ✓ |       |
| 삭제 | ✓ | ✓ |       |
| 편집 | ✓ | ✓ |       |
| 보기 | ✓ | ✓ | ✓ |

### 필드를 기록할 수 있는 권한

필드 사용 권한은 작업 영역 및 레코드 종류에 사용 권한을 부여할 때 레코드 종류에서 상속됩니다.

다음 권한은 각 필드와 연결된 값이 아니라 필드 자체를 참조합니다. 필드 값을 편집하려면 레코드를 편집할 수 있는 권한이 있어야 합니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ |            |       |
| 삭제 | ✓ |            |       |
| 편집 | ✓ |            |       |
| 보기 | ✓ | ✓ | ✓ |


### 보기에 대한 권한

레코드 뷰에 별도의 권한을 부여해야 합니다. 작업 영역에 사용 권한을 부여해도 작업 영역의 레코드 뷰에 대한 사용 권한은 부여되지 않습니다.

사용자가 다음 보기 요소에 액세스할 수 있도록 보기에 대한 권한 부여해야 합니다.

* 필터
* 필드 가시성
* 정렬
* 그룹화
* 행 높이
* 설정

내부 또는 공개적으로 보기를 공유할 수 있습니다.

다음은 보기 및 보기 요소에 대한 권한 수준입니다.

| 내부 공유 | 관리(초대받은 사람만 액세스할 수 있음) | 보기(초대받은 사람만 접근 가능) | 작업 영역 내의 모든 사용자가 볼 수 있음* |
|--------|--------|-------|------------------------------|
| 편집 | ✓ |       |                            |
| 삭제 | ✓ |       |                            |
| 공유 | ✓ |       |                           |
| 보기 | ✓ | ✓ | ✓ |
| 적용 | ✓ | ✓ | ✓ |

| 공개 공유 | 보기 |
|--------|-------|
| 보기 | ✓ |
| 적용 | ✓ |

*사용자는 이 보기 액세스 권한을 얻기 위해 작업 영역에 대한 보기 이상의 권한이 있어야 합니다.

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->
