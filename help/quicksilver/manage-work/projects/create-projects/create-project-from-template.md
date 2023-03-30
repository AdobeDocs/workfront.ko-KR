---
product-area: projects;templates
navigation-topic: create-projects
title: 템플릿을 사용하여 프로젝트 만들기
description: 템플릿을 프레임워크로 사용하여 프로젝트를 만들 수 있습니다. 반복되는 프로젝트가 있는 경우 새 프로젝트의 일반 타임라인에 템플릿을 사용하면 동일한 프로젝트를 반복적으로 빌드하지 않아도 됩니다.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: e38411056b3f9be6d0241ee18e71984ef2a678a0
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 1%

---

# 템플릿을 사용하여 프로젝트 만들기

템플릿을 프레임워크로 사용하여 프로젝트를 만들 수 있습니다. 반복되는 프로젝트가 있는 경우 새 프로젝트의 일반 타임라인에 템플릿을 사용하면 동일한 프로젝트를 반복적으로 빌드하지 않아도 됩니다.

템플릿은 프로젝트와 관련된 반복 가능한 프로세스, 정보 및 설정을 캡처하는 방법을 제공합니다. 템플릿과 관련된 정보는 프로젝트로 전송됩니다. 여기에는 작업, 지정, 기간, 문서, 재무 세부 정보, 위험 및 사용자 정의 양식이 포함됩니다.

>[!TIP]
>
>Workfront은 새 프로젝트의 그룹 및 상태를 다음과 같이 정의합니다.
>
>* 템플릿에서 만든 새 프로젝트의 기본 상태는 기본 프로젝트 환경 설정 영역에서 Workfront 관리자가 정의한 상태나 그룹의 프로젝트 환경 설정 영역에서 그룹 관리자(또는 Workfront 관리자)가 정의한 상태에 해당합니다. 프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 또는 [그룹에 대한 프로젝트 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* 새 프로젝트의 그룹은 템플릿의 그룹입니다. 템플릿이 그룹과 연관되지 않으면 프로젝트의 그룹은 프로젝트를 생성하는 사용자의 홈 그룹입니다.
>
>* 새 프로젝트에 사용할 수 있는 상태는 템플릿 그룹인 프로젝트 그룹 또는 프로젝트를 만드는 사용자의 홈 그룹 상태와 일치합니다.


템플릿에서 프로젝트를 작성할 수 있는 옵션은 다음과 같습니다.

* 프로젝트 영역의 템플릿에서 프로젝트를 생성합니다
* 템플릿 수준의 템플릿에서 프로젝트 만들기
* 기존 프로젝트에 템플릿 첨부

   자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* 그룹 영역의 템플릿에서 프로젝트를 생성합니다

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 라이선스 개요*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트 및 템플릿에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿에 대한 권한 보기</p> <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받게 됩니다 </p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 영역의 템플릿에서 프로젝트를 생성합니다

프로젝트 영역의 기본 메뉴 또는 포트폴리오나 프로그램의 프로젝트 영역에서 프로젝트를 만들 수 있습니다.

1. 다음 중 하나를 수행하십시오.

   * 을(를) 클릭합니다. **기본 메뉴** ![](assets/main-menu-icon.png)를 클릭합니다. **프로젝트**&#x200B;를 확장한 다음 **새 프로젝트**.
   * 포트폴리오로 이동한 다음 확장합니다. **새 프로젝트**.

      >[!TIP]
      >
      >포트폴리오의 템플릿을 사용하여 프로젝트를 만들 경우 새 프로젝트의 Portfolio 필드가 업데이트되어 프로젝트를 만들 수 있도록 선택한 포트폴리오가 표시됩니다. 지정된 경우 템플릿의 Portfolio 필드를 덮어씁니다.

   * 프로그램으로 이동한 다음 **새 프로젝트**.

      >[!TIP]
      >
      >프로그램의 템플릿을 사용하여 프로젝트를 생성하는 경우 새 프로젝트의 프로그램 필드가 업데이트되어 프로젝트를 생성하도록 선택한 프로그램이 표시됩니다. 템플릿의 Portfolio 필드가 업데이트되어 프로젝트를 생성하도록 선택한 프로그램 포트폴리오가 표시됩니다. 지정된 경우 템플릿에 있는 프로그램 및 Portfolio 필드를 덮어씁니다.

   * 그룹 관리자인 경우 관리하는 그룹의 프로젝트 섹션에서 프로젝트를 만들 수도 있습니다. 자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >그룹의 템플릿을 사용하여 프로젝트를 만들 경우, 템플릿에서 프로젝트를 만드는 그룹은 템플릿의 그룹 필드를 지정하지 않은 경우에만 새 프로젝트의 그룹 필드에 표시됩니다. 템플릿 그룹 필드를 지정하면 새 프로젝트의 그룹 필드가 템플릿의 그룹 필드입니다.
   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 에서 템플릿 이름을 클릭합니다 **즐겨찾는 템플릿** list

   ![](assets/new-project-from-template-dropdown-with-template-favorites-nwe-350x235.png)

   또는

   다음을 수행합니다.

   1. 선택 **템플릿의 새 프로젝트**.
   1. 에서 **검색 템플릿** 필드에 템플릿 이름을 입력하고 목록에 표시되면 클릭합니다.
   1. 오른쪽에 있는 템플릿 세부 사항을 검토합니다.

      템플릿 세부 정보에는 다음이 포함됩니다.

      * 템플릿 기간
      * 템플릿 소유자
      * 상위 3개 작업의 이름이 포함된 최상위 수준의 작업 수입니다
      * 템플릿에 있는 모든 작업의 수입니다
      * 템플릿 사용자 지정 양식의 이름
   1. (선택 사항) 템플릿 이름의 위로 마우스를 가져간 후 **즐겨찾기** **아이콘** ![](assets/favorites-icon-small.png) 나중에 사용하기 위해 즐겨찾기로 표시합니다.

      또는

      를 확장합니다. **즐겨찾는 템플릿** 목록을 표시하고 드롭다운 목록에서 템플릿을 선택합니다.

      >[!TIP]
      >
      >최대 40개의 Workfront 항목을 즐겨찾기로 표시할 수 있습니다. 여기에는 템플릿 및 기타 항목이 포함됩니다.

   1. 클릭 **템플릿 사용** 템플릿을 선택한 경우.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!NOTE]
   >
   >프로젝트 목록에 이정표 보기가 적용된 경우, **템플릿 섹션에서 새로 만들기**.
   >
   >
   >![](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)   >

1. 다음 **새 프로젝트** 상자가 열립니다.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

1. 템플릿에 필드가 이미 채워져 있는 경우 해당 필드는에서 미리 채워집니다. **새 프로젝트** 상자. 미리 채워진 값을 편집하여 프로젝트와 더 잘 일치시킬 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).
1. 클릭 **프로젝트 만들기**.

   템플릿에 정의된 모든 세부 사항은 이전 단계에서 변경하지 않은 경우 새로 생성된 프로젝트와 자동으로 연결됩니다.

## 템플릿 영역의 템플릿에서 프로젝트를 생성합니다

프로젝트 영역에서 시작하는 대신 템플릿으로 시작하여 템플릿으로 프로젝트를 생성할 수 있습니다.

 

1. 에서 **기본 메뉴**&#x200B;를 클릭합니다. **템플릿**.

1. 사용할 템플릿의 이름을 클릭합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **프로젝트를 만듭니다.**

   ![템플릿에서 프로젝트 만들기](assets/project-sharing-on-template-nwe-2022-350x172.png)

   다음 **새 프로젝트** 상자가 열립니다.

1. 프로젝트 이름을 지정한 다음 각 섹션을 검토하고 필요에 맞게 변경합니다.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

   템플릿에 필드가 이미 채워져 있는 경우 해당 필드는에서 미리 채워집니다. **새 프로젝트** 상자. 미리 채워진 값을 편집하여 프로젝트와 더 잘 일치시킬 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 클릭 **프로젝트를 만듭니다.**

   템플릿에 정의된 모든 세부 사항은 이전 단계에서 변경하지 않은 경우 새로 생성된 프로젝트와 자동으로 연결됩니다.
