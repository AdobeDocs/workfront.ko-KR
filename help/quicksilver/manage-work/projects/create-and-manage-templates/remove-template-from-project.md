---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에서 템플릿 정보 제거
description: 프로젝트에서 템플릿을 제거할 수 없습니다. 템플릿이 프로젝트에 첨부된 후 프로젝트에 추가된 정보는 수동으로만 제거할 수 있습니다. 템플릿 첨부에 대한 자세한 내용은 프로젝트에 템플릿 첨부를 참조하십시오.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# 프로젝트에서 템플릿 정보 제거

프로젝트에서 템플릿을 제거할 수 없습니다. 템플릿이 프로젝트에 첨부된 후 프로젝트에 추가된 정보는 수동으로만 제거할 수 있습니다. 템플릿을 첨부하는 방법에 대한 자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

## 액세스 요구 사항

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
   <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업에 대한 액세스 편집</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 액세스 관리 </p> <p>프로젝트에 대한 Contribute 이상 액세스 </p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트에서 템플릿 정보를 제거하는 옵션

프로젝트에 추가된 템플릿 정보를 제거하려면 다음 중 하나를 수행할 수 있습니다.

* 템플릿을 첨부한 후 프로젝트에서 정보를 수동으로 제거합니다.

  자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

* 템플릿과 함께 추가된 프로젝트의 작업을 삭제합니다.

  자세한 내용은 이 문서의 [템플릿에서 만든 작업 삭제](#delete-tasks-created-from-a-template) 섹션을 참조하십시오.

* Workfront에서 템플릿을 삭제합니다. Workfront에서 템플릿을 삭제해도 프로젝트에서 템플릿에서 추가된 작업은 삭제되지 않습니다.

  자세한 내용은 [프로젝트 템플릿 삭제](../../../manage-work/projects/create-and-manage-templates/delete-templates.md)를 참조하십시오.

## 템플릿에서 생성된 작업 삭제 {#delete-tasks-created-from-a-template}

1. 프로젝트의 **작업** 섹션으로 이동합니다.
1. 다음 중 하나를 수행하십시오.

   * 다음 문을 사용하여 템플릿에서 생성된 작업만 표시하도록 작업 목록에 대한 필터를 만듭니다.

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     필터 만들기에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

     필터를 적용하면 템플릿 작업 ID와 연결된 작업만 목록에 표시됩니다.

   * 작업 목록에 대한 보기를 만들어 열에 **템플릿 작업 ID** 또는 **템플릿 작업 이름** 필드를 표시합니다.

     보기를 적용하면 템플릿 작업 ID 또는 템플릿 작업 이름 열에 정보가 포함된 작업이 템플릿을 사용하여 생성되었습니다.

     보기 만들기에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

1. 2단계에서 템플릿에서 만든 작업을 모두 선택한 다음 **삭제 아이콘****> 예, 삭제**를 클릭합니다. 자세한 내용은 [작업 삭제](../../../manage-work/tasks/manage-tasks/delete-tasks.md)를 참조하십시오.
