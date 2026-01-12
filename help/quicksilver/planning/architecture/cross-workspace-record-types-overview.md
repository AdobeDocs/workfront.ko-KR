---
title: Cross-workspace 레코드 유형 개요
description: 레코드 종류를 전역 또는 연결할 수 있도록 설정할 수 있습니다. 글로벌 레코드 유형은 Adobe Workfront Planning의 중앙 또는 기본 작업 영역에서 여러 작업 영역에 추가할 수 있지만 연결 가능한 레코드 유형은 자체 작업 영역이 아닌 다른 작업 영역에서 연결할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 895fcc9e8bfc6ef21e82ae6dab4c370b0e267cad
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 0%

---


# 작업 영역 간 레코드 유형 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드 유형에 대해 작업 영역 간 기능을 활성화할 수 있습니다. 작업 영역 간 레코드 유형은 두 개 이상의 작업 영역에서 참조하거나 액세스할 수 있습니다.

>[!IMPORTANT]
>
>기록 유형에 대해 교차 작업 영역 기능을 활성화하려면 조직에서 다음 패키지를 구매해야 합니다.
>
>연결 가능한 레코드 유형을 구성하려면:
>
>
>* 모든 Workfront 패키지 및 모든 Planning 패키지
>
>   또는
>
>* 모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지
>
><span class="preview">전역 레코드 종류를 구성하려면:</span>
>
>* <span class="preview">모든 Workfront 패키지 및 Planning Plus 패키지</span>
>     
>   또는
>
>* <span class="preview">모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</span>
>
>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오.
>자세한 내용은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.


다음은 레코드 유형의 작업 영역 간 기능입니다.

* <span class="preview">**글로벌 레코드 종류**: 사용자가 관리하는 다른 작업 영역에 글로벌 레코드 종류를 추가할 수 있습니다.</span>

* **연결 가능한 레코드 종류**: 사용자는 다른 작업 영역에서 이 레코드 종류에 연결할 수 있습니다.

이 문서에서는 작업 영역 간 레코드 유형에 대한 개요를 제공합니다. 레코드 종류의 작업 영역 간 기능을 정의하는 방법에 대한 자세한 내용은 [레코드 종류에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.

<div class="preview">

## 글로벌 레코드 유형 개요

글로벌 레코드 유형은 Workfront Planning의 중앙 또는 기본 작업 영역에서 여러 작업 영역에 추가할 수 있습니다.

일반적인 워크플로우를 사용하여 여러 팀 조직을 위한 Workfront Planning을 구현할 때 각 팀의 작업 영역에 추가하여 작업을 캡처 및 관리할 수 있는 주요 레코드 유형(예: 캠페인 또는 결과물)에 대한 일관된 구조와 메타데이터를 정의해야 할 수 있습니다.

중앙 수준으로 롤업하려면 각 팀의 작업이 필요할 수도 있습니다.

이러한 워크플로우에서는 한 작업 공간에 모든 것을 추가하거나 모든 작업 공간에 조직의 모든 사람을 추가할 필요 없이 팀 간 가시성을 잠금 해제하면서 팀이 작업을 일관되게 캡처하도록 할 수 있습니다. 글로벌 레코드 유형을 사용하여 이를 수행할 수 있습니다.

글로벌 레코드 유형을 사용하려면 다음을 수행하십시오.

1. 관리하는 작업 영역에서 레코드 유형을 전역으로 구성합니다.

   작업 영역 관리자는 표준 라이선스를 가진 사용자, 팀, 그룹, 역할 및 회사에 권한을 부여하여 선택한 레코드 유형을 자신이 관리하는 작업 영역에 추가할 수 있습니다.

   원래 레코드 유형은 원래 작업 영역에 존재하지만 다른 작업 영역에서 볼 수 있게 됩니다.

   자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.
1. 글로벌 레코드 유형으로 구성된 기존 작업 영역에서 보조 작업 영역에 레코드 유형을 추가합니다.

   기록 유형은 다음 작업 공간에 존재합니다.

   * 글로벌 레코드 유형으로 지정된 원래 작업 영역입니다.
   * 보조 작업 영역.

   자세한 내용은 [다른 작업 영역에서 기존 레코드 형식 추가](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)를 참조하십시오.

   다음 섹션에서는 글로벌 레코드 유형과 원래 또는 보조 작업 공간에서 글로벌 레코드 유형이 작동하는 방식에 대한 고려 사항을 설명합니다.

### 원래 작업 영역의 글로벌 레코드 유형에 대한 고려 사항

글로벌로 구성된 레코드 종류에는 다음 속성이 있습니다.

* 모든 정보(모양, 원본 필드)는 원본 작업공간에서만 편집할 수 있습니다.

* 원래 작업공간의 글로벌 레코드 유형에 대해 다음 작업을 수행할 수 있습니다.

   * 편집

     글로벌 레코드 유형 편집에는 해당 모양, 작업 영역 간 기능 및 원본 작업 영역에서 만들어진 모든 필드 편집이 포함됩니다.
   * 공유

     레코드 유형을 공유하면 작업 공간에 사용자가 추가되고 해당 사용자와 레코드가 공유됩니다.
   * 삭제

     글로벌 레코드 유형이 추가된 모든 보조 작업 영역에서 if의 모든 인스턴스를 삭제한 후에만 원래 작업 영역에서 글로벌 레코드 유형을 삭제할 수 있습니다.

     자세한 내용은 [레코드 종류 삭제](/help/quicksilver/planning/architecture/delete-record-types.md)를 참조하세요.
   * 다른 작업 영역에서 연결 가능하도록 설정
   * 요청 양식 만들기 및 관리
   * 자동화 제작 및 관리

* 글로벌 레코드 유형에 추가하는 레코드는 추가된 작업 영역에 대한 보기 권한이 있는 사용자만 볼 수 있습니다. <!-- this needs to be more specific: what does "o the workspace where they were added" mean? - added in which kind of workspaces? secondary or primary; asking Lilit-->
* 보조 작업공간에서 추가하는 레코드는 원래 작업공간에서 롤업되고 표시됩니다. 원래 작업 영역의 모든 멤버에게 보기 권한이 부여됩니다.
* 원래 글로벌 레코드 유형을 여러 보조 작업 공간에 추가하면 다음과 같은 시나리오가 있습니다.

   * 원래 작업 영역의 구성원은 해당 작업 영역의 구성원이 아니더라도 작업 영역에서 추가된 모든 레코드에 대한 보기 권한을 자동으로 부여받습니다.
   * 보조 작업 영역 구성원은 자신이 구성원으로 있는 작업 영역의 레코드만 볼 수 있습니다. <!--change this to: Secondary workspace members can view only records from the workspace the records were added and where they have at least permissions to view the record workspace and the record type.-->

* 글로벌 레코드 유형에 연결된 레코드 유형은 이 레코드 유형이 추가된 작업 영역에서 연결에 사용할 수 있습니다.

  예를 들어, 지역 레코드 유형과 연결된 캠페인 글로벌 레코드 유형이 있고 캠페인 레코드 유형을 보조 작업 공간에 추가한 경우, 지역은 보조 작업 공간에서 서로 연결할 수 있게 됩니다. 이제 보조 작업 영역 구성원은 캠페인을 만들고 지역에 연결할 수 있습니다.

* 원래 작업 영역에서 글로벌 레코드 유형에 대해 생성된 필드는 레코드 유형이 추가된 모든 작업 영역에서 볼 수 있습니다.

  원래 작업 영역에서만 필드 설정을 편집할 수 있습니다.

  원래 작업 영역에서 생성된 필드의 설정은 보조 작업 영역에 대한 권한에 관계없이 모든 구성원의 보조 작업 영역에서 읽기 전용입니다.

  보조 작업 영역 관리자는 원래 작업 영역에 구성된 필드의 필드 설정을 수정할 수 없습니다. 원래 작업 영역의 작업 영역 관리자만 원래 작업 영역에서 필드 설정을 수정할 수 있습니다.

### 보조 작업 영역의 글로벌 레코드 유형에 대한 고려 사항

* 보조 작업 영역 기여자는 팀 작업 영역에서 글로벌 레코드 유형에 대한 기여 권한을 받습니다. 보조 작업 영역에서 레코드를 추가하고 관리할 수 있습니다.

* 보조 작업 영역 뷰어는 팀 작업 영역에서 글로벌 레코드 유형에 대한 보기 권한을 받습니다. 레코드를 추가하고 관리할 수 없습니다.

* 보조 작업 영역 관리자는 보조 작업 영역의 글로벌 레코드 유형에서 추가된 레코드 유형에 대해 다음과 같은 추가 작업을 수행할 수 있습니다.

   * 삭제하십시오.

     보조 작업 영역에서 레코드 유형을 삭제하면 보조 작업 영역에서만 레코드 유형이 제거됩니다. 보조 작업 영역에서 추가된 레코드 및 필드도 삭제됩니다. 레코드 유형은 원래 작업 공간이나 추가된 다른 보조 작업 공간에서 삭제되지 않습니다.

     자세한 내용은 [레코드 종류 삭제](/help/quicksilver/planning/architecture/delete-record-types.md)를 참조하세요.
   * 레코드 유형의 보기를 공유합니다.

     보조 작업 영역의 글로벌 레코드 유형에서는 보기를 공개적으로 공유할 수 없습니다. 보조 작업 영역 내부에서만 보기를 공유할 수 있습니다. 원래 작업 영역에서 글로벌 레코드 유형에 대한 보기를 내부적으로 공개적으로 공유할 수 있습니다.

     자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.

<!--Uncomment this at prod on Jan 15: * Share it-->

<!--You can share a global record type added to a secondary workspace from the secondary space. By sharing a global record type in a secondary workspace, the following also occur:

    * Users are added to the workspace with View permissions.
    * Users receive the same permissions to all the records of the global record type in the secondary workspace.-->

<!--when they will be able to add fields to the secondary space, this bullet will need this extra information: 
    After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.-->

<!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it-->

* 보조 작업 영역의 글로벌 레코드 유형에 대해 다음 작업을 수행할 수 있는 사용자는 없습니다.

   * 편집

     모양, 작업 영역 간 기능 또는 원본 작업 영역에서 추가된 필드는 편집할 수 없습니다.
   * &#x200B;<!-- remove this at Prod on Jan 15--> 공유
   * 요청 양식 만들기 및 관리
   * 자동화 제작 및 관리

* 보조 작업 영역에 추가된 레코드는 이러한 작업 영역에 대한 보기 이상의 권한이 있는 경우에만 다음 작업 영역에서 볼 수 있습니다.

   * 보조 작업 공간이 추가됩니다.
   * 글로벌 레코드 유형의 원래 작업 영역입니다.
   * 전역 작업 영역이 추가되는 모든 기타 작업 영역

  <!--replace he above bullet with this: 
        * Records added in a secondary workspace are visible from the following workspaces, only if you have View or higher permissions to these workspaces:
        * The secondary place where they were added
        * The global record type's original workspace
    -->

* 보조 작업 공간에서 생성된 레코드에 대한 시나리오는 다음과 같습니다.

   * 원래 작업 영역에 대한 관리 권한이 있고 보조 작업 영역에 대한 권한이 없는 경우 원래 작업 영역의 보조 작업 영역에서 추가된 레코드를 볼 수 있지만, 원래 작업 영역에서 관리할 수는 없습니다.
   * 보조 작업 영역에 대한 관리 권한이 있는 경우 글로벌 레코드 유형의 원래 작업 영역과 해당 레코드가 추가된 보조 작업 영역 모두에서 레코드를 관리할 수 있습니다.
   * 해당 작업 영역에 대한 보기 권한이 있는 경우에만 글로벌 레코드 유형이 추가된 추가 보조 작업 영역에서 레코드를 볼 수 있습니다. <!-- take this bullet out when we change this functionality on Jan 15-->

### 글로벌 레코드 유형의 연결에 대한 액세스 권한

원본 작업공간의 글로벌 레코드 유형에 연결된 레코드 유형은 글로벌 레코드 유형이 추가된 다른 작업공간에서 볼 수 있으며 글로벌 레코드 유형이 추가된 보조 작업공간에서 연결에 사용할 수 있습니다.

### 글로벌 레코드 유형의 API 액세스

Workfront Planning API를 사용하여 보조 작업 공간에서 글로벌 레코드 유형에 레코드를 추가할 때 시스템은 사용자가 글로벌 레코드 유형의 원래 작업 공간에서 레코드를 만들 수 있는 액세스 권한이 있는지 확인합니다.

다음과 같은 경우:

* 사용자에게 액세스 권한이 있는 경우 글로벌 레코드 유형의 원래 작업 영역에 레코드가 생성됩니다.

* 사용자에게 액세스 권한이 없는 경우 글로벌 레코드 유형의 원래 작업 영역에 액세스할 수 없고 레코드를 만들 수 있는 작업 영역 ID를 제공해야 한다는 오류가 표시됩니다.

</div>

## 연결 가능한 레코드 유형 개요

관리하는 모든 작업 영역에서 연결 가능한 것으로 정의된 레코드 유형에 연결할 수 있습니다.

팀에는 다른 작업 영역의 레코드 유형에 연결된 레코드가 필요하거나 다른 작업 영역의 레코드에 속한 레코드에서 캡처된 정보를 보아야 할 수 있습니다. 레코드 종류를 연결 가능한 것으로 지정하여 이 구성을 수행할 수 있습니다.

연결 가능한 레코드 유형을 사용하려면 다음을 수행하십시오.

1. 특정 작업 영역에서 연결할 수 있도록 레코드 종류를 구성하십시오.

   작업 영역 관리자는 연결할 수 있는 지정된 레코드 유형의 작업 영역을 선택할 수 있습니다.

   원본 레코드 유형은 원본 작업 공간에 존재하며 다른 작업 공간에서 로 연결할 수 있습니다.

   자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.
1. 관리하는 다른 작업 영역에서 연결 가능한 것으로 지정된 레코드 유형에 연결합니다.

   자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
