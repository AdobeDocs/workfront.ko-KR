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
>템플릿 및 해당 작업에는 실제 날짜가 없고, 작업이 시작될 수 있는 날짜(향후 프로젝트가 시작될 수 있는 날짜)와 작업이 완료되어야 하는 날짜가 표시됩니다. 템플릿을 사용하여 향후 프로젝트를 만들 때 프로젝트에 실제 날짜가 표시됩니다. 자세한 내용은 [프로젝트 만들기](../create-projects/create-project.md)를 참조하십시오.


다음과 같은 방법으로 새 템플릿을 만들 수 있습니다.

* 이 문서에 설명된 대로 처음부터
* 기존 프로젝트에서 프로젝트를 템플릿으로 저장

  기존 프로젝트에서 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트를 템플릿으로 저장](../../../manage-work/projects/manage-projects/save-project-as-template.md)을 참조하십시오.

* 다른 템플릿에서 복사하여

  기존 템플릿을 복사하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 복사](../../../manage-work/projects/create-and-manage-templates/copy-template.md)를 참조하십시오.

* 블루프린트를 가져왔습니다. 블루프린트를 가져오려면 Workfront 관리자여야 합니다. 자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md)을 참조하세요.

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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 템플릿 만들기

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **서식 파일**&#x200B;을 클릭합니다.

1. **새 템플릿**&#x200B;을 클릭합니다.

   템플릿에 제목이 없습니다.

   ![새 템플릿](assets/create-template-nwe-2022-350x102.png)

1. 템플릿 헤더에서 새 템플릿의 이름을 지정한 다음 **Enter.**&#x200B;을 누릅니다.
1. 왼쪽 패널에서 **템플릿 작업** 섹션을 클릭합니다.
1. **템플릿 작업 추가 시작**&#x200B;을 클릭합니다.

   또는

   템플릿에 작업을 추가하려면 **새 템플릿 작업**&#x200B;을(를) 클릭하십시오.

   템플릿에 템플릿 작업을 추가하는 것은 프로젝트에 작업을 추가하는 것과 동일합니다.

   프로젝트에 작업을 추가하는 방법에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)를 참조하십시오.

   >[!NOTE]
   >
   >템플릿에 반복 작업을 추가할 수 없습니다.

1. (선택 사항) 작업 목록의 오른쪽 상단에 있는 **간트 차트** 아이콘을 클릭하면 템플릿의 작업 목록이 시각적으로 표시됩니다.

   >[!TIP]
   >
   >이 간트 차트에서 바로 작업을 편집할 수 없습니다.

1. 새 템플릿에 정보를 추가하려면 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

1. **변경 내용 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 템플릿에 항목을 추가하려면 문서 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)에서 [템플릿에 항목 추가](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) 섹션을 참조하십시오.

## 그룹 연결에 의해 결정된 템플릿 설정

프로젝트 템플릿과 그룹 간의 연결(또는 그룹 부족)은 프로젝트, 작업 및 문제 환경 설정이 템플릿의 특정 설정을 결정하는 방식에 영향을 줍니다. 자세한 내용은 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md) 문서의 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) 섹션을 참조하십시오.
