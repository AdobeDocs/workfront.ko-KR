---
title: Adobe 마에스트로에 대한 액세스 권한 부여
description: Adobe Maestro에서 액세스 권한을 부여하고 정보를 공유하는 방법을 알아봅니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Adobe 마에스트로에 대한 액세스 권한 부여

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro에 액세스하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

다음 전제 조건이 충족되는 경우 조직의 모든 사용자가 Maestro에 액세스할 수 있습니다.

<!--the first requisite will be removed when we go to GA-->

* 조직이 Adobe Maestro 비공개 베타 프로그램에 등록되었습니다.
* 시스템 관리자는 레이아웃 템플릿을 사용하여 Main Menu에 Maestro 영역을 추가해야 합니다.

  시스템 관리자를 포함한 모든 사용자에 대해 기본적으로 Maestro가 Main Menu에 표시되지 않습니다.

  자세한 내용은 [레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>사용자 또는 Maestro의 정보와 관련된 액세스 수준 또는 권한이 없습니다. 해당 환경에서 Maestro가 활성화된 모든 사용자는 다른 사용자가 Maestro에 추가하는 모든 정보를 보고, 편집하고, 삭제할 수 있습니다.

## 다른 사용자와 메인 메뉴의 마에스트로 영역 공유

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

조직이 Maestro Beta 프로그램에 등록되면 레이아웃 템플릿을 사용하여 모든 사용자의 메인 메뉴에 Maestro 영역을 추가할 수 있습니다.

1. 에 로그인 **Workfront** Workfront 관리자입니다.

1. 추가 **마에스트로** 아이콘 ![](assets/maestro-icon.png) (으)로 **메인 메뉴** 사용 **레이아웃 템플릿**.

   자세한 내용은 [레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Maestro에 액세스하려는 사용자에게 레이아웃 템플릿을 할당합니다.

   자세한 내용은 [레이아웃 템플릿에 사용자 할당](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   템플릿에 할당된 모든 사용자는 이제 메인 메뉴에서 Maestro에 액세스할 수 있습니다.

   사용자는 작업 공간, 레코드 유형, 레코드 및 필드를 만들 수 있습니다.

<!--

## Share permissions to a workspace

Only system administrators can access all workspaces in Maestro. As a system administrator, you must share a workspace with other users for them to view, manage, or contribute to it. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->