---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 만들기
description: 템플릿 영역에서 템플릿을 만들고 삭제할 수 있습니다. 새 템플릿을 작성할 때 모든 작업 및 향후 프로젝트 설정에 대한 정보를 입력할 수 있습니다. 그런 다음 이 정보는 템플릿에서 만드는 모든 프로젝트로 전송됩니다.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 6%

---

# 프로젝트 템플릿 만들기

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준 </p><p>플랜</p> <p>블루프린트에서 템플릿을 가져오려면 시스템 관리자여야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
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

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 템플릿 만들기

{{step1-to-templates}}

1. **새 템플릿**&#x200B;을 클릭합니다.

   템플릿에 제목이 없습니다.

   ![새 템플릿](assets/create-template-nwe-2022-350x102.png)

1. 템플릿 헤더에서 새 템플릿의 이름을 지정한 다음 **Enter.**&#x200B;을 누릅니다.
1. 왼쪽 패널에서 **템플릿 작업** 섹션을 클릭합니다.
1. 인라인으로 작업을 추가하려면 **템플릿 작업 추가 시작**&#x200B;을 클릭하세요.

   또는

   **새 템플릿 작업**&#x200B;을(를) 클릭하여 **새 템플릿 작업** 상자에서 템플릿에 작업을 추가합니다.

   **템플릿 작업 만들기** 상자가 새 환경에서 열립니다.

   ![새 템플릿 작업에 대한 새 경험](assets/new-template-task-box-unshimmed.png)

1. (조건부) 새 경험을 사용하여 **템플릿 작업 만들기** 상자에서 다음 영역의 정보를 업데이트합니다.

   * 템플릿 작업 이름
   * 개요
   * 할당
   * 재무
   * 사용자 정의 양식
   * 문서
   * 설정

1. **템플릿 작업 만들기** 클릭

   또는

   **템플릿 작업 만들기** 상자 아래쪽에 있는 **이전 경험으로 다시 전환**&#x200B;을 클릭합니다.

   **새 템플릿 작업**&#x200B;이 이전 환경에서 열립니다.

   ![새 템플릿 작업 상자](assets/new-template-task-box.png)

   >[!TIP]
   >
   >프로덕션에서 기본적으로 이전 경험이 열립니다.

1. **새 템플릿 작업** 상자에서 다음 영역의 정보를 업데이트합니다.

   * 개요
   * 재무
   * 설정
   * 할당
   * 사용자 정의 양식
   * 문서 첨부

     템플릿 작업에 대한 정보를 업데이트하는 것은 프로젝트의 작업을 편집하는 것과 비슷합니다. 자세한 내용은 [작업 편집](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오. <!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >템플릿에 반복 작업을 추가할 수 없습니다.

1. 다음 중 하나를 클릭합니다.

   * 현재 템플릿 작업을 저장하고 새 템플릿 작업 상자를 닫으려면 **템플릿 작업 저장**.
   * **템플릿 작업을 저장하고 다른 작업을 시작하려면** **새 템플릿 작업** 상자를 열어 다른 작업을 추가합니다.
   * 템플릿 작업을 저장하지 않고 상자를 닫으려면 **취소**.
1. (선택 사항) 템플릿 작업을 추가한 후 템플릿 작업 섹션에서 작업 목록 오른쪽 위의 **간트 차트** 아이콘을 클릭하여 템플릿의 작업 목록을 시각적으로 표시합니다.

   >[!TIP]
   >
   >이 간트 차트에서 바로 작업을 편집할 수 없습니다.

1. 새 템플릿에 정보를 추가하려면 헤더의 템플릿 이름 왼쪽에 있는 **자세히** 메뉴 ![추가 아이콘](assets/more-icon.png)을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

   >[!NOTE]
   >
   >   프로젝트 템플릿과 그룹 간의 연결(또는 그룹 부족)은 프로젝트, 작업 및 문제 환경 설정이 템플릿의 특정 설정을 결정하는 방식에 영향을 줍니다.
   >
   >자세한 내용은 [그룹의 프로젝트 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md) 문서의 &quot;템플릿 및 템플릿 작업에 환경 설정을 적용하는 방법&quot; 섹션을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 템플릿에 다음 항목을 추가합니다

   * 문서
   * 위험
   * 승인 프로세스
   * 청구 요율
   * 경비
   * 대기열 세부 정보
   * 주제 그룹 및 대기열 주제

1. (선택 사항) 템플릿의 작업에 다음 항목을 추가합니다.

   * 문서
   * 경비
   * 승인

   자세한 내용은 문서 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)의 &quot;템플릿에 항목 추가&quot; 섹션을 참조하십시오.




