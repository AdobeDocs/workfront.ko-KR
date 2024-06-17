---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 만들기
description: 템플릿 영역에서 템플릿을 만들고 삭제할 수 있습니다. 새 템플릿을 작성할 때 모든 작업 및 향후 프로젝트 설정에 대한 정보를 입력할 수 있습니다. 그런 다음 이 정보는 템플릿에서 만드는 모든 프로젝트로 전송됩니다.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 2%

---

# 프로젝트 템플릿 만들기

<!-- Audited: 1/2024 -->

템플릿 영역에서 템플릿을 만들고 삭제할 수 있습니다. 새 템플릿을 작성할 때 모든 작업 및 향후 프로젝트 설정에 대한 정보를 입력할 수 있습니다. 그런 다음 이 정보는 템플릿에서 만드는 모든 프로젝트로 전송됩니다.

>[!NOTE]
>
>템플릿 및 해당 작업에는 실제 날짜가 없고, 작업이 시작될 수 있는 날짜(향후 프로젝트가 시작될 수 있는 날짜)와 작업이 완료되어야 하는 날짜가 표시됩니다. 템플릿을 사용하여 향후 프로젝트를 만들 때 프로젝트에 실제 날짜가 표시됩니다. 자세한 내용은 [프로젝트 만들기](../create-projects/create-project.md).


다음과 같은 방법으로 새 템플릿을 만들 수 있습니다.

* 이 문서에 설명된 대로 처음부터
* 기존 프로젝트에서 프로젝트를 템플릿으로 저장

  기존 프로젝트에서 템플릿 만들기에 대한 자세한 내용은 [프로젝트를 템플릿으로 저장](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* 다른 템플릿에서 복사하여

  기존 템플릿 복사에 대한 자세한 내용은 [프로젝트 템플릿 복사](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 블루프린트를 가져왔습니다. 블루프린트를 가져오려면 Workfront 관리자여야 합니다. 자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준 </p><p>또는 </p><p>현재: 플랜 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">블루프린트에서 템플릿을 가져오려면 시스템 관리자여야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>기본적으로 사용자가 만드는 템플릿에 대한 관리 권한이 있습니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 템플릿 만들기

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **템플릿**.

1. 클릭 **새 템플릿**.

   템플릿에 제목이 없습니다.

   ![새 템플릿](assets/create-template-nwe-2022-350x102.png)

1. 템플릿 헤더에서 새 템플릿의 이름을 지정한 다음 키를 누릅니다 **들어갑니다.**
1. 다음을 클릭합니다. **템플릿 작업** 왼쪽 패널의 섹션입니다.
1. 클릭 **템플릿 작업 추가 시작**.

   또는

   클릭 **새 템플릿 작업** 을(를) 클릭하여 템플릿에 작업을 추가합니다.

   템플릿에 템플릿 작업을 추가하는 것은 프로젝트에 작업을 추가하는 것과 동일합니다.

   프로젝트에 작업을 추가하는 방법에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >템플릿에 반복 작업을 추가할 수 없습니다.

1. (선택 사항) **간트 차트** ( 작업 목록 오른쪽 위 모서리에 있음)으로 이동하여 템플릿의 작업 목록을 시각적으로 표시합니다.

   >[!TIP]
   >
   >이 간트 차트에서 바로 작업을 편집할 수 없습니다.

1. 새 템플릿에 정보를 추가하려면 **자세히** 메뉴 ![](assets/more-icon.png)을 클릭한 다음 을 클릭합니다 **편집**.

   템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. **변경 내용 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 템플릿에 항목을 추가하려면 섹션을 참조하십시오 [템플릿에 추가 항목 추가](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) 이 문서에서 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 그룹 연결에 의해 결정된 템플릿 설정

프로젝트 템플릿과 그룹 간의 연결(또는 그룹 부족)은 프로젝트, 작업 및 문제 환경 설정이 템플릿의 특정 설정을 결정하는 방식에 영향을 줍니다. 자세한 내용은 섹션을 참조하십시오 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) 이 문서에서 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
