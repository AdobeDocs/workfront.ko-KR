---
product-area: projects
navigation-topic: create-projects
title: 프로젝트 만들기
description: 프로젝트는 Adobe Workfront의 대규모 작업 단위입니다. 처음부터 프로젝트를 만들거나 템플릿을 사용하거나 문제 또는 작업을 프로젝트로 전환할 수 있습니다.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 1%

---

# 프로젝트 만들기

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

프로젝트는 Adobe Workfront에서 수행해야 하는 많은 양의 작업을 나타냅니다.

## 액세스 요구 사항

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p>
        <p>또는</p>
        <p>현재: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트를 만드는 방법

다음 방법 중 하나를 사용하여 Workfront에서 프로젝트를 만들 수 있습니다.

* 템플릿을 사용하지 않고 프로젝트를 처음부터 새로 만듭니다. 이 문서에서는 처음부터 프로젝트를 만드는 방법을 설명합니다.

* 기존 프로젝트를 복사합니다.\
  프로젝트 복사에 대한 자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md)를 참조하십시오.

* 템플릿을 사용합니다.\
  템플릿을 사용하여 새 프로젝트를 만드는 방법에 대한 자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](../../../manage-work/projects/create-projects/create-project-from-template.md)를 참조하십시오.

* Microsoft 프로젝트에서 프로젝트를 가져옵니다.\
  MS 프로젝트에서 프로젝트를 가져오는 방법에 대한 자세한 내용은 [Microsoft 프로젝트에서 프로젝트 가져오기](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)를 참조하십시오.

* 킥스타트를 사용하여 프로젝트를 가져옵니다.

  Workfront 관리자는 킥스타트를 사용하여 프로젝트를 가져올 수 있습니다.

  Workfront에서 킥스타트를 사용하여 데이터를 가져오는 방법에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)를 참조하십시오.

  킥스타트를 사용하여 프로젝트를 가져오는 방법에 대한 자세한 내용은 [킥스타트 시나리오: 간단한 프로젝트 및 작업 가져오기 준비](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md)를 참조하십시오.

* Adobe Workfront 시나리오 플래너의 시나리오에서 이니셔티브를 게시합니다.

  시나리오 플래너에는 다음 중 하나가 필요합니다.

   * 현재 Workfront 라이선스 구조에 대한 추가 라이선스.
   * 새 Workfront 라이선스 구조에 대한 Ultimate 라이선스.

  Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오. 이니셔티브를 게시하여 프로젝트를 만드는 방법에 대한 자세한 내용은 [시나리오 플래너에서 이니셔티브를 게시하여 프로젝트 업데이트 또는 만들기](../../../scenario-planner/publish-scenarios-update-projects.md)를 참조하십시오.

* Workfront Planning의 레코드 유형에서 프로젝트를 연결할 때 프로젝트를 추가합니다. 프로덕션 환경에서는 Workfront Planning의 템플릿 없이 프로젝트만 만들 수 있습니다. <span class="preview">미리 보기 환경에서 템플릿을 사용하여 프로젝트를 만들 수 있습니다.</span>

  Workfront Planning에 대한 새 Workfront 라이선스와 추가 Workfront Planning 라이선스가 있어야 합니다.

  Workfront Planning에 액세스하는 방법에 대한 자세한 내용은 [액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.

  프로젝트에 레코드를 추가하여 프로젝트를 만드는 방법에 대한 자세한 내용은 문서 [Workfront Planning에서 레코드에 연결할 때 Workfront 개체 만들기](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)의 &quot;Workfront Planning의 레코드와 연결할 때 프로젝트 만들기&quot; 섹션을 참조하십시오.

## 전제 조건

시작하기 전에 다음을 확인해야 합니다.

* 시스템 또는 그룹 관리자가 설정 영역에서 &quot;사용자가 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용&quot; 기본 설정을 활성화했습니다.

  자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

## 새 프로젝트 기본 설정

프로젝트를 만들 때 Workfront에서 기본 설정 세트를 적용합니다. 예를 들어, 프로젝트를 만들 때 상태, 그룹 및 예약 모드가 미리 설정됩니다.

다음 사항을 고려하십시오.

* Workfront 관리자 또는 그룹 관리자는 전체 Workfront 인스턴스 또는 그룹에 대한 프로젝트 환경 설정을 구성할 때 새 프로젝트에 대한 기본 설정을 구성할 수 있습니다.
* Workfront은 그룹의 설정이 있는 경우 Workfront 관리자가 설정한 설정을 적용하기 전에 해당 설정을 적용합니다.
* 새 프로젝트의 기본 상태는 기본 프로젝트 환경 설정 영역에서 Workfront 관리자 또는 그룹의 프로젝트 환경 설정 영역에서 그룹 관리자(또는 Workfront 관리자)가 정의한 상태에 해당합니다.

  >[!NOTE]
  >
  >새 프로젝트의 기본 상태는 계획인 것이 좋습니다. 새 프로젝트를 변경할 때 프로젝트에 할당된 사용자에게 알림이 전송되지 않도록 합니다.
  >
  >새 프로젝트에 대한 기본 상태 및 기타 기본 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)을 참조하십시오.

* Workfront에서 새 프로젝트의 그룹 및 상태를 정의하는 방법에 대한 시나리오는 다음과 같습니다.

   * 처음부터 프로젝트를 만드는 경우 프로젝트의 그룹은 홈 그룹입니다.

     프로젝트 상태 는 홈 그룹(있는 경우) 또는 Workfront 인스턴스의 프로젝트 환경 설정에 있는 기본 상태입니다. 프로젝트를 만들 때 기본 상태를 프로젝트 그룹에 사용할 수 있는 상태로 변경할 수 있습니다.

   * 템플릿을 사용하여 프로젝트를 만드는 경우 템플릿의 설정이 Workfront 또는 그룹 관리자가 설정한 설정보다 우선합니다.

     새 프로젝트의 그룹은 템플릿의 그룹입니다. 템플릿이 그룹과 연결되어 있지 않으면 프로젝트의 그룹은 프로젝트를 만드는 사용자의 홈 그룹입니다.

     템플릿에서 생성된 새 프로젝트의 기본 상태는 기본 프로젝트 환경 설정 영역에서 Workfront 관리자 또는 그룹의 프로젝트 환경 설정 영역에서 그룹 관리자(또는 Workfront 관리자)가 정의한 상태에 해당합니다. 템플릿에서 프로젝트를 생성할 때 기본 상태를 템플릿의 그룹인 프로젝트 그룹 또는 프로젝트를 생성한 사용자의 홈 그룹 상태 중 하나로 변경할 수 있습니다.

   * 문제를 전환하여 프로젝트를 만드는 경우 새 프로젝트 그룹은 문제의 기존 프로젝트 그룹입니다. 문제를 전환하는 사용자에게 문제의 프로젝트에 대한 액세스 권한이 없거나 문제의 프로젝트에 그룹이 없는 경우 새 프로젝트의 그룹은 문제를 전환하는 사용자의 홈 그룹입니다.

     새 프로젝트의 상태는 프로젝트와 연관된 그룹의 그룹 상태(원래 프로젝트의 그룹 또는 문제를 전환하는 사용자의 홈 그룹)와 일치합니다.

     문제를 전환하여 프로젝트를 만들 때 템플릿을 사용하는 경우 위의 두 번째 시나리오를 참조하여 어떤 그룹 및 Workfront이 새 프로젝트에 적용되는지 파악하십시오.

## 처음부터 프로젝트 만들기

>[!NOTE]
>
>템플릿을 사용하여 프로젝트를 만드는 경우 [템플릿을 사용하여 프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) 문서도 보는 것이 좋습니다.


1. 다음 중 하나를 수행하십시오.

   * Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭합니다. **프로젝트**&#x200B;를 클릭한 다음 **새 프로젝트**&#x200B;를 확장합니다.
   * 포트폴리오로 이동한 다음 **새 프로젝트**&#x200B;를 확장합니다.
   * 프로그램으로 이동한 다음 **새 프로젝트**&#x200B;를 확장합니다.
   * 그룹 관리자는 관리하는 그룹의 프로젝트 섹션에서 프로젝트를 만들 수도 있습니다. 자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)을 참조하세요.

   ![새 프로젝트 메뉴](assets/new-project-dropdown-nwe-350x358.png)

1. 처음부터 프로젝트를 만들려면 메뉴에서 **새 프로젝트**&#x200B;를 클릭하십시오.
1. 프로젝트의 이름을 입력합니다. Enter 키를 눌러 이름을 저장합니다.

   ![프로젝트 이름 입력](assets/rename-untitled-project.png)

   프로젝트 페이지의 머리글에는 프로젝트의 현재 상태 및 진행 상황에 대한 간략한 개요가 표시됩니다. 프로젝트 정보가 업데이트되면 프로젝트 헤더의 정보가 변경됩니다.

1. **작업 추가 시작**&#x200B;을 클릭합니다.

   또는

   프로젝트에 작업을 추가하고 리소스를 할당하려면 **새 작업**&#x200B;을(를) 클릭하십시오.

   프로젝트에 작업을 추가하는 방법에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)를 참조하십시오.

1. 프로젝트 이름 옆에 있는 **자세히** 메뉴를 클릭한 다음 **편집** ![편집 아이콘](assets/qs-edit-icon.png)을 클릭하여 프로젝트 세부 정보를 편집합니다.

   **프로젝트 편집** 대화 상자가 열립니다.

   프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

1. (선택 사항) 프로젝트 설정을 구성하고 작업을 추가한 후 프로젝트의 상태를 **현재**(으)로 변경할 수 있습니다.

   이는 이제 프로젝트를 시작할 준비가 되었으며 작업에 할당된 사용자가 이제 해당 작업을 시작할 수 있음을 나타냅니다.

   프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 목록에 액세스](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)를 참조하십시오.
