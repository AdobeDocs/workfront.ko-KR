---
title: Adobe Workfront Planning의 공유 권한 개요
description: 조직의 모든 사용자가 Adobe Workfront Planning을 사용할 수 있는 동일한 액세스 및 권한을 가지고 있는 것은 아닙니다. 이 문서에서는 Adobe Workfront Planning 작업 영역 또는 보기에 대한 권한을 공유하거나 제거하는 방법에 대한 일반적인 정보를 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 6%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Workfront Planning의 공유 권한 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>



{{planning-important-intro}}

Adobe Workfront Planning 작업 영역 또는 보기에 대한 권한을 공유하거나 제거할 수 있습니다.

이 문서에서는 Workfront Planning 객체의 권한 수준에 대해 설명합니다.

## Adobe Workfront Planning에서 공유할 수 있는 객체

다음 개체를 공유할 수 있습니다.

* 작업 영역

   * 조직 내의 다른 사용자와 작업 공간을 공유할 수 있습니다.
   * 작업 영역을 공유하면 작업 영역과 연관된 모든 레코드 유형, 레코드 및 필드도 공유됩니다.
   * 작업 영역을 공유하면 보기가 공유되지 않습니다. 뷰는 별도로 공유됩니다.

  자세한 내용은 [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)를 참조하십시오.

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a workspace with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* 보기

   * 시스템 관리자를 포함한 사용자에게 작업 공간 액세스에 대한 권한과 별도로 보기에 액세스할 수 있는 권한을 부여해야 합니다.
   * 보기를 공유할 때 필터, 그룹화, 정렬 또는 설정을 포함한 모든 보기 요소가 공유됩니다.
   * 보기를 공유할 때 보기에 표시되는 레코드는 공유되지 않습니다. 작업 영역을 공유하여 레코드를 공유해야 합니다.
   * 보기에 대한 공개 링크를 생성할 때 조직 외부의 사람들과 공개적으로 보기를 공유할 수 있습니다.공개 링크에서 레코드 페이지에 액세스하는 사람들은 연결된 레코드와 필드를 포함하여 모든 레코드와 해당 필드를 볼 수 있습니다.

  자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하세요.

내부적으로 작업 공간 또는 보기를 다음 Workfront 엔티티와 공유할 수 있습니다.

* 사용자
* 그룹

<div class="preview">

* 팀
* 회사
* 작업 역할

</div>

## Adobe Workfront Planning에서 객체 공유에 대한 고려 사항

* Adobe Workfront 라이선스 유형은 Workfront Planning 권한과 함께 작동하여 작업 공간 및 해당 개체를 보고, 기여하고, 관리할 수 있는 액세스 권한을 부여합니다.

  라이선스 유형이 Workfront Planning의 권한 수준에 영향을 주는 방법에 대한 자세한 내용은 [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)를 참조하십시오.
* 시스템 관리자는 작성하지 않은 작업 영역을 포함하여 시스템의 모든 작업 영역을 관리할 수 있습니다.
* 시스템 관리자를 포함한 다른 사용자는 자신이 만들었거나 자신과 공유된 보기에만 액세스할 수 있습니다. 시스템 관리자에게는 보기 관리에 대한 권한만 부여할 수 있습니다.
* 작업 영역 또는 보기에 대한 링크를 다른 사용자와 공유할 수 있습니다.

  다음과 같은 시나리오가 있습니다.
   * 작업 공간에 대한 링크를 받는 사용자는 활성 사용자여야 하며 작업 공간에 액세스하려면 Workfront에 로그인해야 합니다.
   * 보기에 대한 링크를 받은 사용자는 다음과 같은 방법으로 보기에 액세스할 수 있습니다.

      * 보기에 대한 링크가 내부적으로 공유된 경우 활성 사용자이고 Workfront에 로그인해야 합니다.
      * Workfront에 로그인하지 않고도 Workfront의 외부 사용자일 수 있으며 공개적으로 공유된 링크에서 보기에 액세스할 수 있습니다.

## Adobe Workfront Planning 개체에 대한 권한 공유

다음 섹션의 표에서는 작업 영역 또는 보기를 공유할 때 선택할 수 있는 권한 수준과 각 수준에서 허용하는 기능을 보여 줍니다.

>[!IMPORTANT]
>
>모든 사용자가 아래에 설명된 권한 수준을 가질 수 있는 것은 아닙니다. 사용자의 개별 라이선스는 Workfront Planning 개체에 대해 받을 수 있는 권한 수준을 결정합니다.
>
>표준(또는 플랜) 라이선스 사용자만 작업 공간에 대한 Contribute 또는 Manage 권한을 가지며 보기에 대한 Manage 권한을 가질 수 있습니다.
> 
>다른 모든 라이선스 유형을 가진 사용자는 작업 공간 및 보기에 대한 보기 권한을 가질 수 있습니다.
>
>자세한 내용은 [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)를 참조하십시오.


### Workspace 권한

사용자가 다음 엔티티에 액세스할 수 있도록 하려면 작업 영역에 대한 권한을 사용자에게 부여해야 합니다.

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

### 레코드 유형 권한

<!--In the Production environment,--> 작업 영역에 권한을 부여할 때 레코드 유형 권한은 항상 상속됩니다.

다음은 레코드 유형에 대한 권한 수준입니다.


|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ |            |       |
| 삭제 | ✓ |            |       |
| 편집 | ✓ |            |       |
| 보기 | ✓ | ✓ | ✓ |

<!--

<div class="preview">

In the Preview environment, Record Type permissions are inherited when you grant permissions to the workspace. 

You can remove inherited permissions from the record type, but you can never grant higher permissions for the record type than users have on the workspace. 

The following scenarios exist: 

|   Workspace permissions     | Automatic inherited permissions for a Record Type |Possible Record Type permissions when Inherited permissions are turned off (granted manually)| 
|--------|--------|-------------|
| Manage |   Manage    |   Manage, No permissions           | 
| Contribute |     Contribute |  Contribute, View, No permissions        |
| View   |  View     |      View, No permissions        |     


</div>

-->

### 권한 기록

작업 영역에 권한을 부여하면 레코드 권한이 상속됩니다.

다음은 레코드에 대한 권한 수준입니다.


|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ | ✓ |       |
| 삭제 | ✓ | ✓ |       |
| 편집 | ✓ | ✓ |       |
| 보기 | ✓ | ✓ | ✓ |

### 필드 권한

작업 영역에 권한을 부여하면 필드 권한이 상속됩니다.
다음 권한은 필드 자체를 참조하며 각 필드와 연결된 값은 참조하지 않습니다. 필드 값을 편집하려면 레코드를 편집할 권한이 있어야 합니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ |            |       |
| 삭제 | ✓ |            |       |
| 편집 | ✓ |            |       |
| 보기 | ✓ | ✓ | ✓ |


### 권한 보기

뷰를 기록하려면 별도의 권한을 부여해야 합니다. 작업 영역에 권한을 부여해도 작업 영역의 레코드 보기에 대한 권한은 부여되지 않습니다.

사용자가 다음 보기 요소에 액세스할 수 있도록 하려면 사용자에게 보기에 대한 권한을 부여해야 합니다.

* 필터
* 필드 가시성
* 정렬
* 그룹화
* 행 높이
* 설정

내부적으로 또는 공개적으로 의견을 공유할 수 있습니다.

다음은 보기 및 보기 요소에 대한 권한 수준입니다.

| 내부 공유 | 관리(초대받은 사람만 액세스 가능) | 보기(초대된 사람만 액세스할 수 있음) | 작업 영역의 모든 사용자가 볼 수 있음* |
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

*이 보기 액세스 권한을 얻으려면 사용자에게 작업 영역에 대한 보기 이상의 권한이 있어야 합니다.

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