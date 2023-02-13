---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 만들기
description: 템플릿 영역에서 템플릿을 생성하고 삭제할 수 있습니다. 새 템플릿을 작성할 때 모든 작업에 대한 정보와 향후 프로젝트 설정에 대한 모든 정보를 입력할 수 있습니다. 그런 다음 템플릿에서 정보를 만들면 이 정보가 프로젝트로 전송됩니다.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# 프로젝트 템플릿 만들기

템플릿 영역에서 템플릿을 생성하고 삭제할 수 있습니다. 새 템플릿을 작성할 때 모든 작업에 대한 정보와 향후 프로젝트 설정에 대한 모든 정보를 입력할 수 있습니다. 그런 다음 템플릿에서 정보를 만들면 이 정보가 프로젝트로 전송됩니다.

다음과 같은 방법으로 새 템플릿을 만들 수 있습니다.

* 이 문서에 설명된 대로 처음부터 하십시오.
* 기존 프로젝트에서 프로젝트를 템플릿으로 저장하여

   기존 프로젝트에서 템플릿을 만드는 방법에 대한 자세한 내용은 [프로젝트를 템플릿으로 저장](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* 다른 템플릿에서 복사하여

   기존 템플릿 복사에 대한 자세한 내용은 [프로젝트 템플릿 복사](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Workfront 관리자인 경우 Blueprint를 가져와서 템플릿을 만들 수 있습니다. 자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

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
   <td> <p>플랜 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Blueprint에서 템플릿을 가져오는 시스템 관리자</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>기본적으로 만든 템플릿에 대한 관리 권한이 있습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 템플릿 만들기

1. 에서 **기본 메뉴** ![](assets/main-menu-icon.png) click **템플릿**.

1. 클릭 **새 템플릿**.

   템플릿의 제목이 없습니다.

   ![새 템플릿](assets/create-template-nwe-2022-350x102.png)

1. 템플릿 헤더에 새 템플릿의 이름을 지정한 다음 키를 누릅니다 **을 입력합니다.**
1. 을(를) 클릭합니다. **템플릿 작업** 왼쪽 패널의 섹션에 있습니다.
1. 클릭&#x200B;**템플릿 작업 추가 시작**.

   또는

   클릭 **새 템플릿 작업** 을 눌러 템플릿에 작업 추가를 시작합니다.

   템플릿에 템플릿 작업을 추가하는 것은 프로젝트에 작업을 추가하는 것과 동일합니다.

   프로젝트에 작업 추가에 대한 자세한 내용은 [프로젝트에서 작업 만들기](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >템플릿에 반복 작업을 추가할 수 없습니다.

1. (선택 사항) **간트 차트** 작업 목록의 오른쪽 위 모서리에 있는 아이콘을 통해 템플릿의 작업 목록을 시각적으로 확인할 수 있습니다.

   >[!TIP]
   >
   >이 Gantt 차트에서 직접 작업을 편집할 수 없습니다.

1. 새 템플릿에 정보를 추가하려면 **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집**.

   템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 클릭 **변경 내용 저장**.
1. (선택 사항) 템플릿에 항목을 더 추가하려면 섹션을 참조하십시오 [템플릿에 추가 항목 추가](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) 기사 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 그룹 연결에 의해 결정된 템플릿 설정

프로젝트 템플릿의 그룹 연결(또는 그룹 부족)은 프로젝트, 작업 및 문제 환경 설정이 템플릿의 특정 설정을 결정하는 방식에 영향을 줍니다. 자세한 내용은 섹션을 참조하십시오 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) 기사 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
