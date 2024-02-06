---
title: Adobe Maestro에서의 권한 공유 개요
description: Adobe Maestro 작업 영역 또는 보기에 대한 권한을 공유하거나 제거할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Maestro에서의 권한 공유 개요

{{maestro-important-intro}}

Adobe Maestro 작업 영역 또는 보기에 대한 권한을 공유하거나 제거할 수 있습니다.

이 문서에서는 Maestro 객체의 권한 수준에 대해 설명합니다.

작업 영역 또는 보기를 공유하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [작업 공간 공유](/help/quicksilver/maestro/access/share-workspaces.md)

* [보기 공유](/help/quicksilver/maestro/access/share-views.md)

## Adobe Maestro에서 공유할 수 있는 오브젝트

Maestro에서 다음 오브젝트를 공유할 수 있습니다.

* 작업 영역

  작업 영역을 공유하면 작업 영역과 연관된 모든 레코드 유형, 레코드 및 필드도 공유됩니다. 보기는 공유되지 않습니다.

* 조회수

## Maestro에서 오브젝트 공유에 대한 고려 사항

* Adobe Workfront 라이선스 유형은 Maestro 권한과 함께 작동하여 Maestro 개체를 보거나, 기여하거나, 관리할 수 있는 액세스 권한을 부여합니다.

  라이선스 유형이 Maestro 객체의 권한 수준에 어떤 영향을 미치는지에 대한 자세한 내용은 [Adobe Maestro의 라이선스 유형 개요](/help/quicksilver/maestro/access/license-type-overview.md).
* 시스템 관리자는 다른 사용자가 만든 작업 공간을 관리하고 공유할 수 있습니다.
* 시스템 관리자가 아닌 경우 다른 사용자가 만든 작업 영역이 사용자와 공유될 경우 해당 작업 영역에 기여할 수 있습니다.
* 작업 공간은 일괄적으로 공유할 수 없습니다.
* 작업공간을 다음 엔티티와 공유할 수 있습니다.
   * 사용자
   * 그룹
* 시스템 관리자를 포함한 다른 사용자는 자신이 만들었거나 자신과 공유된 보기에만 액세스할 수 있습니다.
* 작업 영역 또는 레코드 유형 페이지의 보기에 대한 링크를 다른 사용자와 공유할 수 있습니다. 링크를 받은 사용자는 활성 사용자여야 하며 Workfront에 로그인해야 선택한 보기에 표시된 작업 영역 또는 레코드 유형 페이지에 액세스할 수 있습니다.

## Maestro 개체에 대한 권한 공유

다음 섹션의 표에서는 Maestro 작업 영역 또는 보기를 공유할 때 선택할 수 있는 권한 수준과 각 수준에서 허용하는 기능을 보여 줍니다.

>[!IMPORTANT]
>
>모든 사용자가 아래에 설명된 권한 수준을 가질 수 있는 것은 아닙니다. 사용자의 개별 라이선스는 Maestro 개체에 대해 받을 수 있는 권한 수준을 결정합니다.
>
>자세한 내용은 [Adobe Maestro의 라이선스 유형 개요](/help/quicksilver/maestro/access/license-type-overview.md).


### 작업 공간 권한

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 편집 | ✓ 덧신 |            |       |
| 공유 | ✓ 덧신 |            |       |
| 삭제 | ✓ 덧신 |            |       |
| 보기 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |

### 레코드 유형 권한

작업 영역에 권한을 부여하면 레코드 유형 권한이 상속됩니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ 덧신 |            |       |
| 삭제 | ✓ 덧신 |            |       |
| 편집 | ✓ 덧신 |            |       |
| 보기 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |

### 권한 기록

작업 영역에 권한을 부여하면 레코드 권한이 상속됩니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ 덧신 |            |       |
| 삭제 | ✓ 덧신 | ✓ 덧신 |       |
| 편집 | ✓ 덧신 | ✓ 덧신 |       |
| 보기 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |

### 필드 권한

작업 영역에 권한을 부여하면 필드 권한이 상속됩니다.
다음 권한은 필드 자체를 참조하며 각 필드와 연결된 값은 참조하지 않습니다. 필드 값을 편집하려면 레코드를 편집할 권한이 있어야 합니다.

|        | 관리 | 참여 | 보기 |
|--------|--------|------------|-------|
| 만들기 | ✓ 덧신 |            |       |
| 삭제 | ✓ 덧신 |            |       |
| 편집 | ✓ 덧신 |            |       |
| 보기 | ✓ 덧신 | ✓ 덧신 | ✓ 덧신 |


### 권한 보기

뷰를 기록하려면 별도의 권한을 부여해야 합니다. 작업 영역에 권한을 부여해도 작업 영역의 레코드 보기에 대한 권한은 부여되지 않습니다.

|        | 관리 | 보기 |
|--------|--------|-------|
| 편집 | ✓ 덧신 |       |
| 삭제 | ✓ 덧신 |       |
| 보기 | ✓ 덧신 | ✓ 덧신 |
| 적용 | ✓ 덧신 | ✓ 덧신 |






