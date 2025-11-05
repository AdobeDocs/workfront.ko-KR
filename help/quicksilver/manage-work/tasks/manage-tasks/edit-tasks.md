---
product-area: projects
navigation-topic: manage-tasks
title: 작업 편집
description: 직접 만들었거나 Contribute 또는 Manage 권한이 있는 작업에 대한 정보를 편집할 수 있습니다. 이 문서에서는 작업을 검색하고, 찾고, 편집할 수 있는 권한이 있는 경우 해당 작업을 편집하는 방법에 대해 설명합니다.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '3828'
ht-degree: 4%

---

# 작업 편집

<!--Audited: 10/2025-->

<!--take out prod and preview references at release, or new and old experience-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->


직접 만들었거나 Contribute 또는 Manage 권한이 있는 작업에 대한 정보를 편집할 수 있습니다.

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
   <td> <p>표준</p>
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <ul> 
     <li> <p>작업에 대한 기여 권한을 사용하여 작업 세부 정보 영역에서 다음 정보를 편집할 수 있습니다. </p>
     <ul>
     <li>설명</li>
     <li>상태</li>
     </ul>  
      </li> 
     <li> <p>세부 정보 영역 및 작업 편집 상자의 모든 정보를 편집하려면 작업에 대한 권한 관리</p> </li> 
    </ul> 
    <ul> 
     <li> <p>프로젝트에 대한 상위 권한 기여</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a task to edit the following information in the Task Details area: </p>
     <ul>
     <li>Description</li>
     <li>Status</li>
     </ul>  
      </li> 
     <li> <p>Manage permissions to a task to edit all the information in the Details area and the Edit Task box</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute or higher permissions to the project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## 작업 편집 제한 사항

일부 제한 사항으로 인해 작업을 편집할 수 없습니다.

작업을 편집할 때 다음 사항을 고려하십시오.

* 작업을 업데이트하면 현재 상태인 프로젝트에 대한 알림이 트리거됩니다. 작업에 할당된 사용자의 혼동을 방지하기 위해 프로젝트가 현재 상태일 때 편집 작업을 가능한 한 제한하십시오.
* 승인 진행 중인 작업은 편집할 수 없습니다. 승인 프로세스에서 작업에 대한 시간을 기록하거나 상태를 업데이트할 수만 있습니다.

  ![승인 프로세스를 사용하여 작업 편집](assets/edit-task-in-approval-process-nwe-350x148.png)

* Workfront 관리자 또는 그룹 관리자가 프로젝트 환경 설정 영역에서 이 기능을 활성화한 경우에만 상태가 완료, 중단 또는 승인 보류 인 프로젝트의 작업을 편집하고 문서를 추가할 수 있습니다. 프로젝트 환경 설정 지정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

* 프로젝트가 완료, 정지됨으로 표시되었거나 승인 프로세스에 있는 경우 언제든지 작업에 대한 다음 정보를 편집할 수 있습니다.

   * 로그 시간
   * 기존 경비 편집
   * 사용자 정의 양식 첨부

* 다른 사용자는 작업에 대한 업데이트를 보려면 페이지를 새로 고쳐야 합니다.

## 목록에서 작업 편집

목록 보기에 표시된 필드를 인라인 편집하여 작업 목록에서 작업 정보를 편집할 수 있습니다.

목록에서 작업을 편집하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)을 참조하십시오.

## 요약을 사용하여 목록에서 작업 편집

요약 패널을 사용하여 목록에서 작업을 편집할 수 있습니다. 요약 패널에서 작업을 편집하는 방법에 대한 자세한 내용은 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) 문서의 &quot;요약에서 작업 편집&quot; 섹션을 참조하십시오.

## 작업 편집 상자에서 작업 편집

작업 편집 또는 작업 세부 정보 영역을 사용하여 작업을 편집할 수 있습니다. 다음 단계에서는 작업 편집 상자에서 작업을 편집하는 방법에 대해 설명합니다.

{{step1-click-main-menu}}

1. **프로젝트**&#x200B;를 클릭한 다음 프로젝트 이름을 클릭하여 엽니다.
1. 왼쪽 패널에서 **작업**&#x200B;을 클릭합니다.
1. 편집할 작업을 클릭합니다.
1. (조건부) 작업에 대한 제한된 정보를 편집하려면 왼쪽 패널에서 **작업 세부 정보**&#x200B;를 클릭하십시오.

   ![](assets/nwe-task-details-expanded-350x273.png)

   작업 세부 정보 섹션의 다음 영역에서 정보를 편집하는 것이 좋습니다.

   * **개요**

     이 영역은 기본적으로 확장되어 있습니다.

   * **사용자 정의 양식**

     세관 양식의 이름은 객체에 첨부된 사용자 정의 양식이 있는 경우에만 표시됩니다.

   * **재무**

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 수정한 방법에 따라 작업 세부 정보 영역의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

   작업 세부 정보 섹션에 표시되는 필드에 대한 자세한 내용은 아래 설명된 대로 작업 편집 상자에서 작업을 계속 편집합니다.

   세부 정보 섹션에서 정보를 편집하려면 다음 작업을 수행하십시오.

   1. (선택 사항) 모든 영역을 축소하려면 오른쪽 상단의 **모두 축소** 아이콘 ![](assets/collapse-all-icon.png)을(를) 클릭합니다.
   1. (선택 사항 및 조건부) 영역이 축소되면 각 영역 옆에 있는 **오른쪽 방향 화살표** ![](assets/right-pointing-arrow.png)를 클릭하여 편집할 영역을 확장합니다.
   1. 작업 세부 정보 탭의 정보 편집에 대한 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 세부 정보 개요 영역에서 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [작업 세부 정보 섹션에서 작업 재무 관리](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (선택 사항) 작업에 첨부된 사용자 정의 양식이 없는 경우 **사용자 정의 양식 추가** 필드에 양식 이름을 입력한 다음 목록에 표시될 때 선택하고 **변경 내용 저장**&#x200B;을 클릭합니다.
   1. (선택 사항) **내보내기** 아이콘 ![](assets/export.png)을(를) 클릭하여 개요 및 사용자 정의 양식 정보를 PDF 파일로 내보낸 다음 **내보내기**&#x200B;를 클릭합니다. 다음 중에서 선택합니다.

      * 모두 선택(사용자 정의 양식이 하나 이상 첨부된 경우에만 표시됨)
      * 개요
      * 하나 이상의 사용자 정의 양식 이름

      PDF 파일이 컴퓨터로 다운로드됩니다.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      자세한 내용은 [사용자 정의 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)를 참조하십시오.

1. (조건부) 작업에 대한 모든 정보를 편집하려면 작업에 대한 관리 권한이 있는 사용자는 작업 이름 옆에 있는 **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.

   또는

   작업 목록에서 작업을 선택한 다음 목록 맨 위에 있는 **편집** 아이콘 ![](assets/edit-icon.png)을(를) 클릭합니다.

   작업 편집 상자가 열립니다.

   >[!IMPORTANT]
   >
   >편집 옵션을 보려면 작업에 대한 관리 권한이 있어야 합니다.

   모든 작업 필드는 작업 편집 상자에서 사용할 수 있으며 왼쪽 패널에 나열된 영역별로 그룹화됩니다.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 수정한 방법에 따라 작업 세부 정보 영역의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

   다음 섹션 중 하나에서 정보를 지정하는 것이 좋습니다.

   * [작업 이름](#task-name)
   * [개요](#overview)
   * [할당](#assignments)
   * [사용자 정의 양식](#Custom%C2%A0F)
   * [재무](#finance)
   * [설정](#settings)
   * [댓글](#comment)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 작업 편집 상자의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

### 작업 이름 {#task-name}

1. 위에서 설명한 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **작업 이름**&#x200B;을 클릭합니다.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. 작업 이름을 업데이트합니다.

1. **저장**&#x200B;을 클릭하거나 다음 섹션을 계속합니다.

### 개요 {#overview}

1. 위에서 설명한 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **개요**&#x200B;를 클릭합니다.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. 작업에 대한 다음 정보를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>작업에 대한 추가 정보를 추가합니다. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">기본 정보 섹션</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td> <p>작업이 속한 개발 단계를 나타내는 작업 상태를 선택합니다.</p> <p><b>팁</b>

   작업 헤더에서 작업 상태를 업데이트할 수 있습니다. </p>

   <p>Workfront 또는 그룹 관리자는 작업 상태의 이름을 사용자 지정할 수 있습니다. 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md">상태 만들기 또는 편집</a>을 참조하세요. 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">우선순위</td> 
      <td> <p>작업의 우선 순위를 지정할 수 있는 시각적 플래그입니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p> 없음</p> </li> 
      <li> <p> 낮음 </p> </li> 
      <li> <p>일반 </p> </li> 
      <li> <p>높음 </p> </li> 
      <li> <p> 긴급 </p> </li> 
       </ul> <p>Workfront 관리자가 선택한 프로젝트 환경 설정에 따라 우선순위 이름이 다를 수 있습니다. 작업 우선 순위에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">작업 우선 순위 업데이트</a>를 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">작업 날짜 및 제한 섹션</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 제한 사항</td> 
      <td> <p>작업 제한 사항을 지정하여 작업을 완료해야 하는 시기를 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p><span>고정 날짜</span> </p> <p><strong>계획된 시작</strong> 및 <strong>계획된 완료 일자</strong>를 지정하십시오. </p> </li> 
      <li> <p><span>다음 일자에 시작해야 함</span> </p> <p><strong>계획된 시작 일자</strong>를 지정하십시오. </p> </li> 
      <li> <p><span>다음 일자에 완료해야 함</span> </p> <p><strong>계획된 완료 일자</strong>를 지정하십시오. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>빠른 시일 내에</span></p> </li> 
      <li> <p><span>가능한 한 늦게</span></p> </li> 
      <li> <p><span>가장 빠른 가용 시간</span></p> </li> 
      <li> <p> <span>최근 사용 가능한 시간</span></p> </li> 
      <li> <p><span>다음 이후에 시작</span> </p> </li> 
      <li> <p>계획된 시작 일자 지정</p> </li> 
      <li> <p><span>다음 이후에 시작</span> </p> <p><strong>계획된 시작 일자</strong>를 지정하십시오. </p> </li> 
      <li> <p> <span>다음 이후에 완료</span></p> <p><strong>계획된 완료 일자</strong>를 지정하십시오. </p> </li> 
      <li> <p> <span>다음 이후에 완료</span></p> <p><strong>계획된 완료 일자</strong> 지정</p> </li> 
       </ul> <p>작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">커밋 일자 및 시간</td> 
      <td> <p>작업에 할당된 사용자가 작업을 완료하기로 약정하는 날짜입니다. 계획된 완료 일자와 다를 수 있습니다. 할당자만 이 필드를 편집할 수 있습니다. Workfront의 커밋 날짜에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">커밋 날짜 개요</a>를 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 시작 일자 및 시간</td> 
      <td> <p>작업이 시작될 예정인 시간. 작업의 계획된 시작 일자가 설정되며 여러 요인에 의해 영향을 받습니다.</p> 
       <ul> 
      <li>작업 계획 시작 날짜에 대한 시스템 전체 기본 설정에 따라 프로젝트의 새 작업 시작 날짜는 기본적으로 오늘 또는 프로젝트 시작 날짜일 수 있습니다. <span>프로젝트와 연결된 그룹의 그룹 관리자가 그룹에 대한 이 환경 설정을 지정할 수도 있습니다.</span> 시스템 수준 또는 그룹 수준 작업 환경 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">시스템 전체 작업 및 문제 환경 설정 구성</a>을 참조하십시오.</li> 
      <li>작업의 전임 작업에 따라, Workfront에서 전임 작업이 완료된 후 사용 가능한 다음 날짜로 계획된 시작 날짜를 선택하거나 전임 작업 관계에 따라 시작 날짜를 선택합니다. 전임 작업 관계에 대한 자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">작업 전임 작업 개요</a>를 참조하십시오.</li> 
      <li>작업 제한 사항이 고정 일자 또는 필수 시작 일자인 경우 프로젝트 관리자 또는 작업 소유자는 계획된 시작 일자를 수동으로 설정할 수 있습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>를 참조하십시오.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 완료 일자 및 시간</td> 
      <td> <p>작업이 계획될 때 표시되는 예상 완료 일자입니다. Workfront은 다음 요소 중 일부를 사용하여 계획된 완료 일자를 설정합니다.</p> 
       <ul> 
      <li>작업의 기간을 계획된 시작 일자에 추가하여 계획된 시작 일자부터 계획된 완료 일자가 계산됩니다. 프로젝트 관리자 또는 Workfront이 작업의 기간을 지정하면 계획된 완료 일자로 업데이트가 트리거됩니다. 계획된 일자가 변경되면 작업 기간이 업데이트되었기 때문인 경우가 많습니다.</li> 
      <li>작업 제한 사항이 고정 일자 또는 완료 일이어야 하는 경우 프로젝트 관리자 또는 작업 소유자는 계획된 완료 일자를 수동으로 설정할 수 있습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>를 참조하십시오.</li> 
      <li>작업의 기간 유형이 변경되고 작업의 리소스 수가 동시에 변경되면 계획된 완료 일자도 변경됩니다. 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>를 참조하십시오.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 시작 일자 및 시간</td> 
      <td> <p>작업의 실제 시작 일자를 지정합니다. 일반적으로 작업 상태를 진행 중으로 변경하면 기본값이 자동으로 채워집니다. 실제 시작 일자는 프로젝트 관리자 또는 작업 소유자가 수동으로 수정할 수도 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 완료 일자 및 시간</td> 
      <td> <p>작업이 완료되는 실제 날짜와 시간을 지정합니다. 작업이 완료되는 기본 날짜 및 시간은 상태가 완료됨이 되는 실제 시간과 항상 일치합니다. 실제 완료 일자는 프로젝트 관리자 또는 작업 소유자가 수동으로 수정할 수도 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>작업 시간 섹션</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 노력 </td> 
      <td>

   <p>작업을 완료하는 데 필요한 작업량입니다. 프로젝트 관리자는 계획된 시간 대신 이 필드를 사용하여 작업을 완료하는 데 필요한 노력을 예상할 수 있습니다. 이 필드는 다음 조건이 충족될 때만 표시됩니다.</p> 
      <ul> 
      <li> <p>작업에 간단한 기간 유형이 있습니다. </p> <p><b>팁</b>

   작업 기간 유형을 변경하면 이 필드가 흐리게 표시됩니다. </p> </li>
   <li>프로젝트 관리자가 [작업 노력 사용]을 활성화하여 프로젝트의 작업 계획 시간 필드를 자동으로 계산합니다. </li> 
      </ul> 
      <p>다음 옵션 중에서 선택합니다.</p> 
      <ul> 
      <li>소형</li> 
      <li>Medium <span style="font-weight: normal;">(새 작업의 기본값)</span></li> 
      <li>대형</li> 
      </ul> 
      <p><b>메모</b>

   작업량을 업데이트하면 작업 계획 시간이 업데이트될 수 있습니다. 프로젝트 업데이트 유형이 자동인 경우 즉시 업데이트됩니다. 프로젝트 업데이트 유형이 수동인 경우 업데이트된 계획된 시간을 보려면 타임라인을 다시 계산해야 합니다. </p>

   <p>계획된 시간 대신 작업 노력을 사용하여 작업 노력을 예측하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 노력 개요</a>를 참조하십시오. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭하거나 다음 섹션을 계속합니다.

### 할당 {#assignments}

1. 위에서 설명한 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **할당**&#x200B;을 클릭합니다.

   <!--<span class="preview">The Assignments area opens in the new experience.</span>-->

   <!--indent the bullets below to show new experience functionality:
      1. (Conditional) Using the new experience, do the following:-->

   <!--Indent this according to what you did above: 

      1. <span class="preview">Start typing the name of a user, job role, or team in the **Search people, role or team** field, then select them when they display in the list</span>

      Or

      <span class="preview">Click **Assign to me** to assign the task to yourself. </span>

      1. Update the following information:


      1. (Conditional and optional) Update the following fields: 

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader">Duration Type</td> 
      <td> <p>This identifies the relationship between the following: </p> 
      <ul> 
      <li> <p>The number of resources assigned to a task </p> </li> 
      <li> <p>The total effort required to complete the task </p> </li> 
      <li> <p> The total duration of the task. </p> </li> 
      </ul> <p>Your Workfront administrator or a group administrator selects the default Duration Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> <p>Select from the following options: </p> 
      <ul> 
      <li> <p>Calculated Assignment </p> </li> 
      <li> <p> Calculated Work </p> </li> 
      <li> <p>Effort Driven </p> </li> 
      <li> <p>Simple</p> </li> 
      </ul> </td> 
      </tr> 
      <td role="rowheader">Duration per Occurrence</td> 
      <td> <p>This displays only on the parent of recurring tasks. It displays the duration of each recurring task, as defined when the task was created. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <b>NOTE</b>          
      Durations modified in individual recurring tasks do not display the value indicated in this field. </p> </td> 
      </tr>
      <tr> 
      <td role="rowheader">Duration</td> 
      <td> 
      <div> 
      <div> 
      <p>This is the amount of time that you allow a task to remain open before it is completed. </p> 
      <p><b>IMPORTANT</b>
   
      Because the task duration is typically the amount of time between the Planned Start and the Planned Completion Dates, it affects the timeline of the project.</p> 
   
      <p>To indicate the Duration of the task and the unit of time do the following:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Type the length of time and select from the units of time available in the drop-down menu.</p> <p><b>TIP</b></p>
      When you update the Duration of tasks in a task list, you can use the abbreviation for the unit of time. </p> </li> 
      </ul> 
      <p> You can choose from the regular time or elapsed time options in the following table: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Unit of Time</td> 
      <td>Abbreviation</td> 
      </tr> 
      <tr> 
      <td>Minutes</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Hours</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Days. This is the default. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Weeks</td> 
      <td>W</td> 
      </tr> 
      <tr> 
      <td>Months</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>Elapsed Minutes</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Elapsed Hours</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Elapsed Days</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Elapsed Weeks</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Elapsed Months</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
      </table> 

      <p><b>NOTE</b>
      
      <p>Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. 

      Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. For more information about task duration, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p>
      </td> 
      </tr> 
      <tr> 
      <td role="rowheader">Planned Hours</td> 
      <td> <p>Specify the number of Planned Hours for the task, in hours. This is the amount of actual time that it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the Duration Type is set to Calculated Assignment. For more information about duration types, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> 
      <b>NOTE</b>
      <p>
      When creating recurring tasks, the Planned Hours are those of each occurrence. The Planned Hours of the parent tasks are the total of all Planned Hours from all the occurrences. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.
      </p>
      
      </td> 
      </tr> 
      </tbody> 
      </table>

      (**********<tr> 
      <td role="rowheader">Allocation</td> 
      <td> <p>If your Task Constraint is Calculated Work or Effort Driven, specify the <strong>Allocation %</strong> (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. </p> <p>When the Task Constraint is Simple, you can specify the following:</p> 
         <ul> 
         <li> <p>Allocation Hours of each assignee.</p> </li> 
         <li> <p>Planned Hours of the task</p> </li> 
         <li> <p>Duration of the task</p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
      <td role="rowheader">Assignee's Role</td> 
      <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this task. </p> <p><b>TIP</b>
         Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
         </tr>
         </tbody> 
         </table>************)-->
   <!--1. <span class="preview">(Optional) Click Switch to old experience at the bottom of the **Edit Task** box. </span>
      <span class="preview">The Assignments area opens in the old experience. </span>
      ![](assets/nwe-assignments-section-edit-task-box-350x217.png)-->

1. **사람, 역할 또는 팀 검색**&#x200B;을 클릭하고 작업에 할당할 사용자, 역할 또는 팀의 이름을 입력한 다음 해당 작업을 클릭하거나 목록에 표시될 때 Enter 키를 누릅니다.

   >[!NOTE]
   >
   >사용자 이름에 특수 문자가 포함되어 있으면 검색 필드에 특수 문자를 포함해야 합니다.

   >[!TIP]
   >
   >여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
   >
   >* 작업 항목을 활성 리소스에 재할당합니다.
   >* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.

1. (선택 사항) 피할당자의 이름 옆에 있는 **소유자** 라디오 단추를 선택하여 피할당자가 작업의 기본 피할당자인지 여부를 나타냅니다. 팀은 작업의 기본 피할당자가 될 수 없습니다.
1. (선택 사항) 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">기간 유형</td> 
      <td> <p>이는 다음 간의 관계를 식별합니다. </p> 
       <ul> 
      <li> <p>작업에 할당된 리소스 수 </p> </li> 
      <li> <p>작업을 완료하는 데 필요한 총 작업입니다. </p> </li> 
      <li> <p> 작업의 총 기간입니다. </p> </li> 
       </ul> <p>Workfront 관리자 또는 그룹 관리자는 시스템 또는 그룹의 작업에 대해 기본 기간 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">시스템 전체 작업 및 문제 환경 설정 구성</a>을 참조하십시오. </p> <p>기간 유형을 사용하면 작업의 요구 사항에 따라 일관된 자원 할당을 설정할 수 있습니다. 작업의 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>를 참조하십시오. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p>계산된 할당 </p> </li> 
      <li> <p> 계산된 작업 </p> </li> 
      <li> <p>작업량 고정 </p> </li> 
      <li> <p>단순</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">발생 횟수 당 기간</td> 
      <td> <p>자동연장 작업의 상위 항목에만 표시됩니다. 작업을 만들 때 정의된 대로 각 반복 작업의 기간이 표시됩니다. 반복 작업 만들기에 대한 자세한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>를 참조하십시오. </p> <p> <b>참고</b>

   개별 반복 작업에서 수정된 기간은 이 필드에 표시된 값을 표시하지 않습니다. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td> 
      <div> 
      <div> 
      <p>작업이 완료되기 전에 작업을 열어 두도록 허용하는 시간입니다. </p> 
      <p><b>중요 사항</b>

   작업 기간은 일반적으로 계획된 시작 일자와 계획된 완료 일자 사이의 시간이기 때문에 프로젝트의 타임라인에 영향을 줍니다.</p>

   <p>작업 기간 및 시간 단위를 표시하려면 다음을 수행합니다.</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">시간 길이를 입력하고 드롭다운 메뉴에서 사용 가능한 시간 단위 중에서 선택합니다.</p> <p><b>팁</b></p>
      작업 목록에서 작업 기간을 업데이트할 때 시간 단위의 약어를 사용할 수 있습니다. </p> </li> 
      </ul> 
      <p> 다음 표의 정규 시간 또는 경과 시간 옵션 중에서 선택할 수 있습니다. </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>시간 단위</td> 
      <td>약어</td> 
      </tr> 
      <tr> 
      <td>분</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>시간</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>일. 이것이 기본값입니다. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>주</td> 
      <td>주</td> 
      </tr> 
      <tr> 
      <td>개월</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>경과 시간(분)</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>경과 시간</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>경과 일수</td> 
      <td>에드</td> 
      </tr> 
      <tr> 
      <td>경과 주수</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>경과 기간(월)</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>메모</b>

   <p>경과 시간은 작업 기간에 대한 시간 단위입니다. 휴일, 주말 및 휴무를 포함하는 작업의 계획된 시작 일자와 계획된 완료 일자 사이의 시간입니다. 즉, 경과 시간은 역일이 경과된 때이다.

   정규 시간은 공휴일, 주말 및 휴무를 고려하여 작업 기간에서 제외합니다. 작업 기간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>를 참조하십시오. </p>
   </div> 
      </div> </td> 
      </tr> 
      <tr> 
      <td role="rowheader">계획된 시간</td> 
      <td> <p>작업에 대한 계획된 시간(시간)을 지정합니다. 작업 할당자가 완료하는 데 걸리는 실제 시간입니다. [기간 유형]이 [계산된 할당]으로 설정된 경우 작업의 계획된 시간 수만 지정할 수 있습니다. 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>를 참조하십시오.</p> 
      <b>참고</b>
      <p>
      반복 작업을 만들 때 계획된 시간은 각 발생에 해당하는 시간입니다. 상위 작업의 계획된 시간은 모든 발생 항목에서 모든 계획된 시간의 합계입니다. 반복 작업 만들기에 대한 자세한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>를 참조하십시오.
      </p>

   </td> 
      </tr> 
      <tr> 
      <td role="rowheader">할당</td> 
      <td> <p>작업 제한 사항이 계산된 작업량 또는 작업량 기준인 경우 각 할당자에 대해 <strong>할당 %</strong>(할당 백분율)을 지정하십시오. 피할당자의 일정에서 이 작업에 소비할 수 있는 시간입니다. 피할당자에 대한 할당 백분율을 변경하면 작업의 계획된 시간이 변경됩니다. </p> <p>작업 제한 사항이 단순하면 다음을 지정할 수 있습니다.</p> 
         <ul> 
         <li> <p>각 할당자의 할당 시간.</p> </li> 
         <li> <p>작업의 계획된 시간</p> </li> 
         <li> <p>작업 기간</p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
      <td role="rowheader">할당자의 역할</td> 
      <td> <p>사용자를 피할당자로 선택한 경우 <strong>피할당자의 역할</strong> 드롭다운 메뉴에서 역할을 선택합니다. 피할당자가 이 작업에서 수행할 수 있는 역할입니다. </p> <p><b>팁</b>

   프로필의 각 피할당자와 연결된 작업 역할만 드롭다운 메뉴에 나타납니다.</p> </td>
   </tr>
   </tbody>
   </table>

1. **변경 내용 저장** <!--<span class="preview"> or **Save** </span> -->을 클릭하거나 다음 섹션을 계속합니다.

### 사용자 정의 양식

작업이 프로젝트에 추가될 때 작업에 자동으로 첨부될 기본 사용자 정의 양식을 정의할 수 있습니다. 모든 새 작업에 대한 기본 작업 사용자 정의 양식을 포함하도록 프로젝트를 설정하는 방법에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md) 문서의 &quot;작업&quot; 섹션을 참조하십시오.

1. 위에서 설명한 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭하거나 사용자 지정 양식이 이미 첨부되어 있는 경우 해당 양식 이름을 클릭합니다.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. **사용자 정의 양식 추가**&#x200B;를 클릭하고 작업에 연결할 사용자 정의 양식을 선택합니다. 이 필드에서 사용자 정의 양식을 선택하려면 먼저 사용자 정의 양식을 작성해야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다.

   사용자 정의 양식 작성에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오. 작업에 최대 10개의 사용자 정의 양식을 추가할 수 있습니다

1. (조건부) 사용자 정의 양식을 작업에 첨부한 경우 양식의 모든 필드를 편집합니다. 작업을 저장하려면 먼저 모든 필수 필드를 지정해야 합니다.

   >[!NOTE]
   >
   >Workfront 관리자가 사용자 정의 양식의 섹션에 대한 권한을 설정하는 방법에 따라 모든 사용자가 지정된 사용자 정의 양식에서 동일한 필드를 보거나 편집할 수 있는 것은 아닙니다. 사용자 정의 양식의 섹션 내에서 필드를 편집할 수 있는 권한은 작업 자체에 대한 권한에 따라 다릅니다. 작업 권한 설정에 대한 자세한 내용은 [작업 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)를 참조하십시오.

1. **저장**&#x200B;을 클릭하거나 다음 섹션을 계속합니다.

### 재무 {#finance}

1. 이 문서의 [작업 편집](#Edit2) 섹션에 설명된 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **재무**&#x200B;을 클릭합니다.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">비용 유형</td> 
      <td> <p>작업에 대한 비용 유형을 지정합니다. 작업의 시간 수를 기반으로 작업의 비용 계산 방법을 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
        <li> <p>비용 없음</p> </li> 
        <li> <p>고정 시간별 </p> </li> 
        <li> <p> 시간별 사용자 </p> </li> 
        <li> <p> 시간별 역할</p> </li> 
       </ul> <p>비용 추적에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a> 을 참조하십시오. Workfront 관리자 또는 그룹 관리자는 시스템 또는 그룹의 작업에 대해 기본 비용 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 차원의 프로젝트 환경 설정 구성</a> 을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수익 유형</td> 
      <td> <p>작업에 대한 수익 유형을 지정합니다. 작업의 시간 수를 기반으로 작업의 매출 계산 방법을 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p> 과금 불가 </p> </li> 
      <li> <p>시간별 사용자 </p> </li> 
      <li> <p>시간별 역할 </p> </li> 
      <li> <p>고정 시간별 </p> </li> 
      <li> <p>시간별 사용자(상한 포함) </p> </li> 
      <li> <p>시간별 역할(수용작업량 포함) </p> </li> 
      <li> <p>시간별 + 고정 사용자 </p> </li> 
      <li> <p>시간별 + 고정 역할 </p> </li> 
      <li> <p>고정 수입 </p> </li> 
       </ul> <p>수익 추적에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a> 를 참조하십시오. </p> <p>Workfront 관리자 또는 그룹 관리자는 시스템 또는 그룹의 작업에 대한 기본 수익 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 차원의 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭하거나 다음 섹션을 계속합니다.

### 설정 {#settings}

1. 이 문서의 [작업 편집](#Edit2) 섹션에 설명된 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **설정**&#x200B;을 클릭합니다.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">추적 모드</td> 
      <td> <p>작업의 진행 상태를 추적하는 방법을 지정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p> 사용자는 업데이트해야 합니다. </p> </li> 
      <li> <p>정시 추정 </p> </li> 
      <li> <p>지연 경고 무시</p> </li> 
      <li> <p> 자동 완성 </p> </li> 
      <li> <p>전임 작업 </p> </li> 
       </ul> <p>작업의 추적 모드에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">작업 추적 모드 개요</a>를 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 레벨링</td> 
      <td> <p>작업에 할당된 리소스를 레벨링에서 제외하려면 <strong>리소스 레벨링에서 제외</strong> 필드를 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">레벨링 지연</td> 
      <td> <p>레벨링 지연 시간(시간)을 지정합니다. </p> <p> 레벨링 지연에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">작업 레벨링 지연 업데이트</a>를 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 진행</td> 
      <td> <p>태스크와 연관시킬 승인 프로세스를 선택합니다. 작업과 연결하려면 Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. 승인 프로세스에 대한 관리 액세스 권한이 있는 사용자는 그룹별 승인 프로세스를 만들 수도 있습니다. </p> <p>승인 프로세스 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">작업 항목에 대한 승인 프로세스 만들기</a>를 참조하십시오. 승인 프로세스를 추가할 때는 다음 사항을 고려하십시오. </p> 
       <ul>

   <li> <p>활성 승인 프로세스만 목록에 표시됩니다. </p> </li>

   <li> <p>시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 그룹 이외의 그룹과 연결된 승인 프로세스가 목록에 표시되지 않습니다. </p>

   <p><b>중요 사항</b>

   프로젝트의 그룹이 변경되면 이전에 첨부된 그룹별 승인 프로세스가 일회성 승인 프로세스가 됩니다. 프로젝트 그룹 변경 또는 승인 프로세스 변경 내용이 승인 설정에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">그룹 및 승인 프로세스 변경 내용이 할당된 승인 프로세스에 미치는 영향</a>을 참조하십시오. </p>

   </li>

   <li> <p>작업이 프로젝트에 추가될 때 작업에 자동으로 첨부되도록 기본 승인 프로세스를 정의할 수 있습니다. 기본 작업 승인 프로세스를 포함하도록 프로젝트를 설정하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a> 문서의 "작업" 섹션을 참조하십시오. </p> </li>

   <li> <p>작업을 일괄 편집할 때 다음과 같은 시나리오가 있습니다. </p> 
      <ul> 
      <li> <p>동일한 그룹에서 여러 작업을 선택하면 시스템 레벨 및 그룹 레벨 승인 프로세스가 모두 이 필드에 표시됩니다. </p> </li> 
      <li> <p>다른 그룹에서 여러 작업을 선택하면 이 필드에는 시스템 수준 승인 프로세스만 표시됩니다. </p> </li> 
      <li> <p>작업에 일회용 승인 프로세스가 첨부되어 있으면 선택한 시스템 수준 또는 그룹 수준 승인 프로세스로 바뀝니다. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. **저장**&#x200B;을 클릭하거나 다음 섹션을 계속합니다.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

### 댓글

1. 이 문서의 [작업 편집](#Edit2) 섹션에 설명된 대로 작업 편집을 시작합니다.
1. 왼쪽 패널에서 **댓글**&#x200B;을 클릭합니다.

   작업 상자 편집에 대한 ![댓글 섹션](assets/comment-section-on-edit-task-box.png)

1. 제공된 공간에 업데이트를 추가합니다.
1. (선택 사항) 다음 중 하나를 업데이트에 추가합니다.

   * **인물 태그** 영역에서 업데이트에 사용자 또는 팀을 추가하거나 @을 사용하여 업데이트에 포함하십시오.
   * 회사 내 사용자에 대한 업데이트를 비공개로 유지하려면 **내 회사에 비공개** 확인란을 선택하십시오.

   >[!TIP]
   >
   >**회사에 비공개** 설정은 Workfront 프로필이 회사와 연결되어 있을 때만 사용할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

## 작업 헤더에서 작업 편집(제한적)

작업 헤더에서 제한된 양의 정보를 편집할 수 있습니다.

시스템 또는 그룹 관리자는 작업 헤더에 표시되는 필드를 사용자 정의할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)을 참조하십시오.


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

작업 헤더에는 기본적으로 다음 필드가 포함됩니다.

* 작업 이름
* 완료율

  자세한 내용은 [작업에 대한 완료율 보기 및 업데이트](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md)를 참조하십시오.
* 할당
* 계획된 완료 일자 기준

  >[!CAUTION]
  >
  >일부 작업 제한 사항 및 기타 종속성으로 인해 작업의 계획된 완료 일자를 편집할 수 없습니다. 작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)를 참조하십시오.

* 상태
* 현재 승인 프로세스에서 승인자로 설정된 경우 승인 결정을 내립니다

## 일괄 작업 편집

목록에서 작업을 일괄적으로 편집하고, 변경 사항을 목록에 자동으로 저장하도록 선택하면 모든 정보를 동시에 업데이트할 수 있습니다.

작업을 일괄 저장하는 방법에 대한 자세한 내용은 문서 [목록에서 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)의 &quot;일괄 작업 편집&quot; 섹션을 참조하십시오.
