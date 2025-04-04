---
product-area: projects;templates
navigation-topic: create-projects
title: 템플릿을 사용하여 프로젝트 만들기
description: 템플릿을 프레임워크로 사용하여 Adobe Workfront에서 프로젝트를 만들 수 있습니다. 자주 반복되는 프로젝트가 있는 경우 새 프로젝트에 템플릿을 사용하면 동일한 프로젝트를 반복적으로 작성할 필요가 없습니다.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 템플릿을 사용하여 프로젝트 만들기

<!-- Audited: 01/2024 -->

템플릿을 프레임워크로 사용하여 Adobe Workfront에서 프로젝트를 만들 수 있습니다. 자주 반복되는 프로젝트가 있는 경우 새 프로젝트의 일반 타임라인에 템플릿을 사용하면 동일한 프로젝트를 반복적으로 작성할 필요가 없습니다.

템플릿은 프로젝트와 관련된 반복 가능한 프로세스, 정보 및 설정을 캡처하는 방법을 제공합니다. 템플릿에 연결된 정보가 프로젝트로 전송됩니다. 여기에는 작업, 할당, 기간, 문서, 재무 세부 정보, 위험 및 사용자 정의 양식이 포함됩니다.

>[!TIP]
>
>Workfront은 새 프로젝트의 그룹 및 상태를 다음과 같이 정의합니다.
>
>* 템플릿에서 생성된 새 프로젝트의 기본 상태는 기본 프로젝트 환경 설정 영역에서 Workfront 관리자 또는 그룹의 프로젝트 환경 설정 영역에서 그룹 관리자(또는 Workfront 관리자)가 정의한 상태에 해당합니다. 프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)을 참조하십시오.
>
>* 새 프로젝트의 그룹은 템플릿의 그룹입니다. 템플릿이 그룹과 연결되어 있지 않으면 프로젝트의 그룹은 프로젝트를 만드는 사용자의 홈 그룹입니다.
>
>* 새 프로젝트에 사용할 수 있는 상태는 템플릿의 그룹인 프로젝트 그룹 또는 프로젝트를 만든 사용자의 홈 그룹 상태와 일치합니다.

템플릿에서 프로젝트를 만드는 다음과 같은 옵션이 있습니다.

* 프로젝트 영역의 템플릿에서 프로젝트 만들기
* 템플릿 수준의 템플릿에서 프로젝트 만들기
* 기존 프로젝트에 템플릿 첨부

  자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

* 그룹 영역의 템플릿에서 프로젝트 만들기

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p>
        <p>또는</p>
        <p>현재: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준</td> 
   <td> <p>프로젝트 및 템플릿에 대한 액세스 편집</p>

<p>사용하는 템플릿에 Portfolio 및 프로그램이 포함된 경우 포트폴리오 및 프로그램에 대한 액세스 편집</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿에 대한 권한 보기</p> 
  <p>사용하는 템플릿에 Portfolio 및 프로그램이 포함되어 있는 경우 프로젝트를 생성하려면 포트폴리오 및 프로그램에 대한 관리 권한이 있어야 합니다 </p> 
   <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받습니다.</p></td> 
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 영역의 템플릿에서 프로젝트 만들기

주 메뉴의 프로젝트 영역이나 포트폴리오 또는 프로그램의 프로젝트 영역에서 프로젝트를 만들 수 있습니다.

>[!NOTE]
>
>시스템 또는 그룹 관리자가 레이아웃 템플릿을 사용하여 인터페이스를 수정할 수 있습니다. 이 경우 다음 단계에서 참조하는 섹션 및 영역의 이름 중 일부는 Workfront 인스턴스에서 다를 수 있습니다.

1. 다음 중 하나를 수행하십시오.

   * Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭합니다. **프로젝트**&#x200B;를 클릭한 다음 **새 프로젝트**&#x200B;를 확장합니다.
   * 포트폴리오로 이동한 다음 **새 프로젝트**&#x200B;를 확장합니다.

     >[!TIP]
     >
     >포트폴리오의 템플릿을 사용하여 프로젝트를 만들면 새 프로젝트의 Portfolio 필드가 업데이트되어 프로젝트를 만들도록 선택한 포트폴리오가 표시됩니다. 지정된 경우 템플릿의 Portfolio 필드를 덮어씁니다.

   * 프로그램으로 이동한 다음 **새 프로젝트**&#x200B;를 확장합니다.

     >[!TIP]
     >
     >프로그램의 템플릿을 사용하여 프로젝트를 만들 때 새 프로젝트의 프로그램 필드가 업데이트되어 프로젝트를 만들도록 선택한 프로그램이 표시됩니다. 템플릿의 Portfolio 필드가 업데이트되어 프로젝트를 만들도록 선택한 프로그램의 포트폴리오가 표시됩니다. 지정된 경우 템플릿의 프로그램 및 Portfolio 필드를 덮어씁니다.

   * 그룹 관리자는 관리하는 그룹의 프로젝트 섹션에서 프로젝트를 만들 수도 있습니다. 자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)을 참조하세요.

     >[!TIP]
     >
     >그룹의 템플릿을 사용하여 프로젝트를 만들 때 템플릿의 그룹 필드가 지정되지 않은 경우에만 새 프로젝트의 그룹 필드에 프로젝트를 만들 그룹이 표시됩니다. 템플릿 그룹 필드를 지정하면 새 프로젝트의 그룹 필드가 템플릿의 그룹 필드가 됩니다.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![새 프로젝트 옵션](assets/new-project-dropdown.png)

1. **즐겨찾는 템플릿** 목록에서 템플릿 이름을 클릭합니다.

   ![즐겨찾는 템플릿 선택](assets/new-project-from-template-dropdown-with-template-favorites.png)

   또는

   다음을 수행합니다.

   1. **템플릿의 새 프로젝트**&#x200B;를 선택하십시오.
   1. **템플릿 검색** 필드에서 템플릿 이름을 입력하고 목록에 표시될 때 클릭합니다.
   1. 오른쪽의 템플릿 세부 사항을 검토합니다.

      템플릿 세부 정보에는 다음 항목이 포함됩니다.

      * 템플릿 기간
      * 템플릿 소유자
      * 상위 3개 작업의 이름을 포함하는 최상위 작업 수
      * 템플릿의 모든 작업 수
      * 템플릿 사용자 정의 양식의 이름

   1. (선택 사항) 왼쪽 창의 템플릿 이름 위에 마우스를 놓고 **즐겨찾기** **아이콘** ![즐겨찾기 아이콘](assets/favorites-icon-small.png)을 클릭하여 나중에 사용할 수 있도록 즐겨찾기로 표시합니다.

      또는

      **즐겨찾는 템플릿** 목록을 확장하고 드롭다운 목록에서 템플릿을 선택합니다.

      >[!TIP]
      >
      >최대 40개의 Workfront 항목을 즐겨찾기로 표시할 수 있습니다. 여기에는 템플릿 및 기타 항목이 포함됩니다.

   1. 템플릿을 선택했으면 **템플릿 사용**&#x200B;을 클릭합니다.

      ![템플릿 세부 정보](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >마일스톤 보기가 프로젝트 목록에 적용된 경우 **템플릿의 새로 만들기**&#x200B;에서 템플릿 이름을 클릭합니다.
      >
      >
      >![템플릿에서 프로젝트를 만드는 마일스톤 보기](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   **새 프로젝트** 상자가 열립니다.

   ![새 프로젝트 상자](assets/new-project-from-template-box.png)

1. 템플릿에 필드가 이미 채워져 있으면 **새 프로젝트** 상자에서 필드가 미리 채워집니다. 프로젝트와 더 잘 일치하도록 미리 채워진 값을 편집할 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.
1. **프로젝트 만들기**&#x200B;를 클릭합니다.

   이전 단계에서 변경하지 않은 경우 템플릿에 정의된 모든 세부 정보가 새로 생성된 프로젝트와 자동으로 연결됩니다.

## 템플릿 영역의 템플릿에서 프로젝트 만들기

프로젝트 영역에서 시작하는 대신 템플릿으로 시작하여 템플릿에서 프로젝트를 만들 수 있습니다.

{{step1-to-templates}}

1. 사용할 템플릿의 이름을 클릭합니다.
1. **자세히** 메뉴 ![자세히 아이콘](assets/more-icon.png)을 클릭한 다음 **프로젝트 만들기**&#x200B;를 클릭합니다.

   ![템플릿에서 프로젝트 만들기](assets/project-sharing-on-template.png)

   **새 프로젝트** 상자가 열립니다.

1. 프로젝트의 이름을 입력한 다음 각 섹션을 검토하고 필요에 따라 변경합니다.

   ![새 프로젝트 상자](assets/new-project-from-template-box.png)

   템플릿에 필드가 이미 채워져 있으면 **새 프로젝트** 상자에서 필드가 미리 채워집니다. 프로젝트와 더 잘 일치하도록 미리 채워진 값을 편집할 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

1. **프로젝트 만들기**&#x200B;를 클릭합니다.

   이전 단계에서 변경하지 않은 경우 템플릿에 정의된 모든 세부 정보가 새로 생성된 프로젝트와 자동으로 연결됩니다.
