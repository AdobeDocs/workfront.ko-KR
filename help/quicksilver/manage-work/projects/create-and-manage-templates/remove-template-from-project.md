---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트에서 템플릿 정보 제거
description: 프로젝트에서 템플릿을 제거할 수 없습니다. 템플릿이 프로젝트에 첨부된 후에만 프로젝트에 추가된 정보를 수동으로 제거할 수 있습니다. 템플릿 연결에 대한 자세한 내용은 프로젝트에 템플릿 첨부 를 참조하십시오.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 프로젝트에서 템플릿 정보 제거

프로젝트에서 템플릿을 제거할 수 없습니다. 템플릿이 프로젝트에 첨부된 후에만 프로젝트에 추가된 정보를 수동으로 제거할 수 있습니다. 템플릿 연결에 대한 자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 액세스 관리 </p> <p>프로젝트에 대한 액세스 권한 부여 이상 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트에서 템플릿 정보를 제거하는 옵션

프로젝트에 추가된 템플릿 정보를 제거하려면 다음 중 하나를 수행할 수 있습니다.

* 템플릿이 첨부된 후 프로젝트에서 정보를 수동으로 제거합니다.

   자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

* 템플릿으로 추가된 프로젝트의 작업을 삭제합니다.

   자세한 내용은 [템플릿에서 만든 작업 삭제](#delete-tasks-created-from-a-template) 섹션에 자세히 설명되어 있습니다.

* Workfront에서 템플릿을 삭제합니다. Workfront에서 템플릿을 삭제해도 프로젝트에서 템플릿에서 추가한 작업은 삭제되지 않습니다.

   자세한 내용은 [프로젝트 템플릿 삭제](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## 템플릿에서 만든 작업 삭제 {#delete-tasks-created-from-a-template}

1. 로 이동합니다. **작업** 섹션에 나열된 상태로 남아 있습니다.
1. 다음 중 하나를 수행하십시오.

   * 다음 문을 사용하여 템플릿에서 만든 작업만 표시할 작업 목록에 대한 필터를 만듭니다.

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      필터 만들기에 대한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      필터를 적용하면 템플릿 작업 ID와 연관된 작업만 목록에 표시됩니다.

   * 작업 목록에 대한 보기를 만들어 **템플릿 작업 ID** 또는 **템플릿 작업 이름** 열에 있는 필드.

      보기를 적용할 때 템플릿 작업 ID 또는 템플릿 작업 이름 열의 정보가 포함된 작업이 템플릿을 사용하여 만들어졌습니다.

      뷰 만들기에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 템플릿에서 생성된 2단계에서 식별된 모든 작업을 선택한 다음 를 클릭합니다 **삭제 아이콘****> 예, 삭제합니다**. 자세한 내용은 [작업 삭제](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
