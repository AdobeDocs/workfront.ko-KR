---
product-area: projects
navigation-topic: manage-tasks
title: 작업 편집
description: 작업 편집
author: Alina
feature: Work Management
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 9c7af82b02649f33728d05126587fb5035e9e110
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 4%

---

# 작업 편집

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


만든 작업 또는 Contribute 또는 관리 권한이 있는 작업에 대한 정보를 편집할 수 있습니다.

## 액세스 요구 사항

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
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <ul> 
     <li> <p>작업에 권한을 부여하여 [작업 세부 사항] 영역에서 편집할 수 있습니다 </p> </li> 
     <li> <p>작업 편집 상자에서 작업을 편집할 수 있는 권한 관리</p> </li> 
    </ul> 
    <ul> 
     <li> <p>프로젝트에 대한 권한 부여 이상</p> </li> 
    </ul> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 편집 제한 사항

작업을 편집할 수 없는 몇 가지 제한 사항이 있습니다.

작업을 편집할 때는 다음 사항을 고려하십시오.

* 작업을 업데이트하면 현재 상태인 프로젝트의 알림이 트리거됩니다. 작업에 할당된 사용자에 대한 혼동을 방지하려면 프로젝트가 현재 상태에 있을 때 편집 작업을 가능한 한 제한합니다.
* 승인 프로세스에 있는 작업은 편집할 수 없습니다. 승인 프로세스에서 작업에 대한 상태를 기록하거나 업데이트할 수만 있습니다.

   ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Workfront 관리자 또는 그룹 관리자가 [프로젝트 환경 설정] 영역에서 이 기능을 활성화한 경우에만 완료, 사용 중지 또는 승인 보류 중인 프로젝트의 작업에 문서를 편집하고 추가할 수 있습니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 프로젝트가 완료, 완료 또는 승인 프로세스에 있는 경우 항상 작업에 대해 다음 정보를 편집할 수 있습니다.

   * 로그 시간
   * 기존 비용 편집
   * 사용자 지정 양식 첨부

## 목록에서 작업 편집

목록 보기에 표시된 인라인 편집 필드를 통해 작업 목록에서 작업 정보를 편집할 수 있습니다.

목록의 작업 편집에 대한 자세한 내용은 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## 요약을 사용하여 목록의 작업 편집

[요약] 패널을 사용하여 목록에서 작업을 편집할 수 있습니다. [요약] 패널에서 작업 편집에 대한 자세한 내용은 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) 문서.

## 작업 편집 상자에서 작업 편집

작업 편집 또는 작업 세부 정보 영역을 사용하여 작업을 편집할 수 있습니다. 다음 단계에서는 작업 편집 상자에서 작업 편집을 설명합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **프로젝트**&#x200B;를 클릭한 다음 프로젝트 이름을 클릭하여 엽니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 편집할 작업을 클릭합니다.
1. (선택 사항) 작업에 대한 제한된 정보를 편집하려면 **작업 세부 사항** 왼쪽 패널에 표시됩니다.

   ![](assets/nwe-task-details-expanded-350x273.png)

   작업 세부 사항 섹션의 다음 영역에서 정보를 편집하는 것이 좋습니다.

   * **개요**

      이 영역은 기본적으로 확장됩니다.

   * **사용자 정의 양식**

      객체에 첨부된 사용자 정의 양식이 있는 경우에만 세관 양식 이름이 표시됩니다.

   * **재무**
   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 수정한 방법에 따라 작업 세부 사항 영역의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   작업 세부 사항 섹션에 표시되는 필드에 대한 자세한 내용은

   아래 설명된 대로 작업 편집 상자에서 작업을 계속 편집합니다.

   세부 정보 섹션에서 정보를 편집하려면 다음을 수행합니다.

   1. (선택 사항) **모두 축소** 아이콘 ![](assets/collapse-all-icon.png) 오른쪽 위 모서리에서 모든 영역을 축소합니다.
   1. (선택 사항 및 조건부) 영역이 축소되면 **오른쪽 화살표** ![](assets/right-pointing-arrow.png) 각 영역 옆에 있으면 편집할 영역을 확장합니다.
   1. [작업 세부 정보] 탭의 정보 편집에 대한 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 세부 정보 개요 영역의 작업 정보 관리](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [작업 세부 정보 섹션의 작업 재무 관리](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
   1. (선택 사항) 작업에 첨부된 사용자 지정 양식이 없는 경우 **사용자 지정 양식 추가** 필드를 선택한 다음 목록에 표시될 때 선택한 다음 **변경 내용 저장**.
   1. (선택 사항) **내보내기** 아이콘 ![](assets/export.png) 개요 및 사용자 지정 양식 정보를 PDF 파일로 내보내려면 **내보내기**. 다음 중에서 선택합니다.

      * 모두 선택(하나 이상의 사용자 지정 양식이 첨부된 경우에만 표시)
      * 개요
      * 하나 이상의 사용자 지정 양식의 이름

      PDF 파일이 컴퓨터에 다운로드됩니다.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      자세한 내용은 [사용자 지정 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).




1. 작업에 대한 모든 정보를 편집하려면 **자세히** 메뉴 ![](assets/more-icon.png) 작업 이름 옆에 있는 **편집**.

   또는

   작업 목록에서 작업을 선택한 다음 **편집** 아이콘 ![](assets/edit-icon.png) 를 클릭합니다.

   작업 편집 상자가 열립니다.

   >[!IMPORTANT]
   >
   >편집 옵션을 보려면 작업에 대한 관리 권한이 있어야 합니다.

   모든 작업 필드는 [작업 편집] 상자에서 사용할 수 있으며 왼쪽 패널에 나열된 영역별로 그룹화됩니다.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 수정한 방법에 따라 작업 세부 사항 영역의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   다음 섹션에서 정보를 지정하는 것이 좋습니다.

   * [작업 이름](#task-name)
   * [개요](#overview)
   * [할당](#assignments)
   * [사용자 정의 양식](#Custom%C2%A0F)
   * [재무](#finance)
   * [설정](#settings)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 작업 편집 상자의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 작업 이름 {#task-name}

1. 위에 설명된 대로 작업 편집을 시작합니다.
1. 클릭 **작업 이름** 왼쪽 패널에 표시됩니다.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. 작업 이름을 업데이트합니다.

1. 클릭 **저장** 또는 다음 섹션으로 계속 진행합니다.

### 개요 {#overview}

1. 위에 설명된 대로 작업 편집을 시작합니다.
1. 클릭 **개요** 왼쪽 패널에 표시됩니다.

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
      <td> <p>작업이 속한 개발 단계를 나타내는 작업의 상태를 선택합니다.</p> <p><b>팁</b>

   작업 헤더에서 작업 상태 를 업데이트할 수 있습니다. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">우선 순위</td> 
      <td> <p>작업의 우선 순위를 지정할 수 있는 시각적 플래그입니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p> 없음</p> </li> 
      <li> <p> 낮음 </p> </li> 
      <li> <p>기본 </p> </li> 
      <li> <p>높음 </p> </li> 
      <li> <p> 긴급 </p> </li> 
       </ul> <p>Workfront 관리자가 선택한 프로젝트 환경 설정에 따라 우선순위 이름이 다를 수 있습니다. 작업 우선순위에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">작업 우선 순위 업데이트</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">작업 날짜 및 제한 섹션</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 제한 사항</td> 
      <td> <p>작업 제약 조건을 지정하여 작업을 완료해야 하는 시기를 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p><span>고정 일자</span> </p> <p>을(를) 지정합니다 <strong>계획된 시작</strong> 그리고 <strong>계획 완료 일자</strong>. </p> </li> 
      <li> <p><span>일자에 시작</span> </p> <p>을(를) 지정합니다 <strong>계획 시작 날짜</strong>. </p> </li> 
      <li> <p><span>다음까지 완료:</span> </p> <p>을(를) 지정합니다 <strong>계획 완료 일자</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>가능한 한 빨리</span></p> </li> 
      <li> <p><span>가능한 늦게</span></p> </li> 
      <li> <p><span>가장 빠른 가용 시간</span></p> </li> 
      <li> <p> <span>최근 사용 가능한 시간</span></p> </li> 
      <li> <p><span>다음 이전에 시작</span> </p> </li> 
      <li> <p>계획 시작 일자 지정</p> </li> 
      <li> <p><span>다음 이후에 시작:</span> </p> <p>을(를) 지정합니다 <strong>계획 시작 날짜</strong>. </p> </li> 
      <li> <p> 완료 <span>늦어도</span></p> <p>을(를) 지정합니다 <strong>계획 완료 일자</strong>. </p> </li> 
      <li> <p> 완료 <span>보다 이른 항목 없음</span></p> <p>을(를) 지정합니다 <strong>계획 완료 일자</strong></p> </li> 
       </ul> <p>작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">커밋 날짜 및 시간</td> 
      <td> <p>작업에 할당된 사용자가 작업을 완료하는 날짜입니다. 계획 완료 일자와 다를 수 있습니다. 할당된 사람만 이 필드를 편집할 수 있습니다. Workfront의 커밋 날짜에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">커밋 날짜 개요</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획 시작 날짜 및 시간</td> 
      <td> <p>작업을 시작할 계획입니다. 작업의 계획 시작 날짜가 설정되고 다음과 같은 여러 요인에 의해 영향을 받습니다.</p> 
       <ul> 
      <li>작업 계획 시작 날짜에 대한 시스템 전체 기본 설정에 따라 프로젝트에 대한 새 작업의 시작 날짜는 기본적으로 오늘 또는 프로젝트 시작 날짜일 수 있습니다. <span>프로젝트와 연결된 그룹의 그룹 관리자도 그룹에 대해 이 기본 설정을 설정할 수 있습니다.</span> 시스템 수준 또는 그룹 수준 작업 환경 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">시스템 전체 작업 및 문제 환경 설정 구성</a>.</li> 
      <li>작업의 전임자에 따라, 계획 시작 날짜는 이전 관계의 전임자에 따라, 작업이 끝난 후 또는 시작 날짜에 다음 사용 가능한 날짜가 되도록 Workfront이 선택합니다. 이전 관계에 대한 자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">작업 선행 작업 개요</a>.</li> 
      <li>프로젝트 관리자 또는 작업 소유자는 작업 제약 조건이 고정 날짜 또는 시작 날짜여야 할 때 계획 시작 날짜를 수동으로 설정할 수 있습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획 완료 날짜 및 시간</td> 
      <td> <p>작업이 계획될 때의 예상 완료 날짜입니다. 계획 완료 일자는 다음과 같은 여러 요인에 의해 설정할 수 있습니다.</p> 
       <ul> 
      <li>계획 완료 일자는 작업 기간을 계획 시작 일자에 추가하여 계획 시작 일자에서 계산됩니다. 프로젝트 관리자 또는 Workfront이 작업 기간을 지정하면 계획된 완료 날짜로 업데이트가 트리거됩니다. 계획 일자가 변경되면 기간 이 업데이트되었기 때문에 종종 해당됩니다.</li> 
      <li>프로젝트 관리자 또는 작업 소유자는 작업 제약 조건이 고정 날짜 또는 종료해야 하는 경우 계획 완료 날짜를 수동으로 설정할 수 있습니다. 작업 제한에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">작업 제한 개요</a>.</li> 
      <li>작업의 기간 유형이 변경되고 작업의 자원 수가 동시에 변경되면 계획 완료 날짜도 변경됩니다. 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 시작 날짜 및 시간</td> 
      <td> <p>작업의 실제 시작 날짜를 지정합니다. 일반적으로 작업의 상태를 진행 중으로 변경하면 기본값이 자동으로 채워집니다. 실제 시작 날짜는 프로젝트 관리자 또는 작업 소유자가 수동으로 수정할 수도 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 완료 날짜 및 시간</td> 
      <td> <p>작업이 완료되는 실제 날짜와 시간을 지정합니다. 작업이 완료되는 기본 날짜 및 시간은 항상 상태가 완료됨이 되는 실제 시간과 일치합니다. 실제 완료 날짜는 프로젝트 관리자 또는 작업 소유자가 수동으로 수정할 수도 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>작업 시간 섹션</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 노력 </td> 
      <td>

   <p>작업을 완료하는 데 필요한 작업량입니다. 프로젝트 관리자는 계획 시간 대신 이 필드를 사용하여 작업을 완료하는 데 필요한 노력을 예상할 수 있습니다. 이 필드는 다음 조건을 충족할 때만 표시됩니다.</p> 
      <ul> 
      <li> <p>작업에 단순 기간 유형이 있습니다. </p> <p><b>팁</b>

   작업 기간 유형을 변경하면 이 필드가 흐리게 표시됩니다. </p> </li>
   <li>프로젝트 관리자가 작업 노력을 사용하여 프로젝트의 작업 계획 시간 필드를 자동으로 계산합니다. </li> 
      </ul> 
      <p>다음 옵션 중에서 선택합니다.</p> 
      <ul> 
      <li>소형</li> 
      <li>Medium <span style="font-weight: normal;">(새 작업의 기본값입니다.)</span></li> 
      <li>대형</li> 
      </ul> 
      <p><b>메모</b>

   작업량을 업데이트하면 작업 계획 시간 이 업데이트될 수 있습니다. 프로젝트 업데이트 유형이 자동인 경우 즉시 업데이트가 수행됩니다. 프로젝트 업데이트 유형이 수동인 경우 갱신된 계획 시간을 보려면 타임라인을 재계산해야 합니다. </p>

   <p>계획 시간 대신 작업 노력을 사용하여 작업 노력을 추정하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **저장** 또는 다음 섹션으로 계속 진행합니다.

### 할당 {#assignments}

1. 위에 설명된 대로 작업 편집을 시작합니다.
1. 클릭 **지정** 왼쪽 패널에 표시됩니다.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. 클릭 **사람, 역할 및 팀 검색** 작업을 지정할 사용자, 역할 또는 팀의 이름을 입력하고 작업을 클릭하거나 목록에 표시되면 Enter 키를 누릅니다.

   >[!NOTE]
   >
   >사용자 이름에 특수 문자가 포함되어 있으면 검색 필드에 특수 문자를 포함해야 합니다.

   >[!TIP]
   >
   >여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >사용자, 작업 역할 또는 팀이 비활성화되기 전에 할당된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
   >
   >* 작업 항목을 활성 자원에 재지정합니다.
   >* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


1. (선택 사항) 을 선택하여 할당자가 작업의 기본 할당자인지 여부를 나타냅니다 **소유자** 이름 옆에 있는 라디오 단추입니다. 팀은 작업의 기본 할당자가 될 수 없습니다.
1. (조건부 및 선택 사항) 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">기간 유형</td> 
      <td> <p>이는 다음 간 관계를 식별합니다. </p> 
       <ul> 
      <li> <p>작업에 할당된 리소스 수 </p> </li> 
      <li> <p>작업을 완료하는 데 필요한 총 작업 수 </p> </li> 
      <li> <p> 작업의 총 기간입니다. </p> </li> 
       </ul> <p>Workfront 관리자 <span> 또는 그룹 관리자</span> 시스템 또는 그룹의 작업에 대한 기본 기간 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>. </p> <p>기간 유형을 사용하면 작업의 필요에 따라 일관된 자원 지정을 설정할 수 있습니다. 작업의 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p>계산된 할당 </p> </li> 
      <li> <p> 계산된 작업 </p> </li> 
      <li> <p>작업량 고정 </p> </li> 
      <li> <p>단순</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">발생 횟수 당 기간</td> 
      <td> <p>이 항목은 반복 작업의 상위 작업에만 표시됩니다. 각 반복 작업의 기간을 표시합니다. 반복 작업 만들기에 대한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>. </p> <p> <b>메모</b>

   개별 반복 작업에서 수정된 기간은 이 필드에 표시된 값을 표시하지 않습니다. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">기간</td> 
      <td> 
      <div> 
      <div> 
      <p>작업이 완료되기 전에 작업을 열어 둘 수 있도록 허용하는 시간입니다. </p> 
      <p><b>중요 사항</b>

   작업 기간은 일반적으로 계획 시작 및 계획 완료 일자 사이의 시간이므로 프로젝트 타임라인에 영향을 줍니다.</p>

   <p>작업의 기간과 시간 단위를 나타내려면 다음을 수행합니다.</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">시간 길이를 입력하고 드롭다운 메뉴에서 사용 가능한 시간 단위 중에서 선택합니다.</p> <p><b>팁</b></p>
      작업 목록에서 작업 기간 을 업데이트하면 시간 단위의 약어를 사용할 수 있습니다. </p> </li> 
      </ul> 
      <p> 다음 테이블의 정규 시간 또는 경과 시간 옵션 중에서 선택할 수 있습니다. </p> 
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
      <td>일. 기본값입니다. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>주</td> 
      <td>W</td> 
      </tr> 
      <tr> 
      <td>개월</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>경과 시간 (분)</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>경과 시간</td> 
      <td>에</td> 
      </tr> 
      <tr> 
      <td>경과 일수</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>경과 주 수</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>경과 기간 (월)</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>메모</b>

   <p>경과 시간은 작업의 지속 시간에 대한 시간 단위입니다. 휴일, 주말 및 휴일이 포함된 작업의 계획 시작 일자와 계획 완료 일자 사이의 시간입니다. 즉, 경과 시간은 달력 일수의 경과입니다.

   일반 시간은 휴일, 주말 및 휴가를 고려하여 작업 지속 시간에서 제외합니다. 작업 기간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">계획된 시간</td> 
   <td> <p>작업에 대한 계획 시간(시간)을 지정합니다. 이 시간은 작업을 완료하는 데 작업의 할당자가 걸리는 실제 시간입니다. 기간 유형이 계산된 지정으로 설정된 경우 작업에 대한 계획 시간 금액만 지정할 수 있습니다. 기간 유형에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 기간 및 기간 유형 개요</a>.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">할당</td> 
   <td> <p>작업 제약 조건이 계산된 작업 또는 작업 제어인 경우 <strong>할당 %</strong> (할당 백분율). 할당자가 이 작업에 사용할 수 있는 일정 시간입니다. 할당자에 대한 할당 비율을 변경하면 작업의 계획 시간이 변경됩니다. </p> <p>작업 제약 조건이 간단하면 다음을 지정할 수 있습니다.</p> 
      <ul> 
      <li> <p>각 할당자의 할당 시간</p> </li> 
      <li> <p>작업 예정 시간</p> </li> 
      <li> <p>작업 기간</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">할당자의 역할</td> 
   <td> <p>에서 역할 선택 <strong>할당자의 역할</strong> 담당자를 할당자로 선택한 경우 드롭다운 메뉴. 할당자가 이 작업에서 수행할 수 있는 역할입니다. </p> <p><b>팁</b>

   프로필의 각 할당자와 연관된 작업 역할만 드롭다운 메뉴에 나타납니다.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. 클릭 **저장** 또는 다음 섹션으로 계속 진행합니다.

### 사용자 정의 양식

작업을 프로젝트에 추가할 때 작업에 자동으로 첨부할 기본 사용자 지정 양식을 정의할 수 있습니다. 모든 새 작업에 대한 기본 작업 사용자 지정 양식을 포함하도록 프로젝트를 설정하는 방법에 대한 자세한 내용은 문서의 &quot;작업&quot; 섹션을 참조하십시오 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 위에 설명된 대로 작업 편집을 시작합니다.
1. 클릭 **사용자 지정 Forms** 왼쪽 패널에서 또는 사용자 지정 양식이 이미 연결되어 있는 경우 사용자 지정 양식의 이름을 클릭합니다.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 클릭 **사용자 지정 양식 추가** 작업과 연결할 사용자 지정 양식 또는 양식을 선택합니다. 이 필드에서 사용자 지정 양식을 선택하려면 먼저 사용자 지정 양식을 작성해야 합니다. 활성 사용자 지정 양식만 목록에 표시됩니다.

   사용자 지정 양식 작성에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).작업에 최대 10개의 사용자 지정 양식을 추가할 수 있습니다.

1. (조건부) 사용자 지정 양식을 작업에 첨부한 경우 양식의 필드를 편집합니다. 작업을 저장하려면 먼저 모든 필수 필드를 지정해야 합니다.

   >[!NOTE]
   >
   >Workfront 관리자가 사용자 지정 양식의 섹션에 대한 권한을 설정하는 방법에 따라 모든 사람이 주어진 사용자 지정 양식에서 동일한 필드를 보거나 편집할 수 있는 것은 아닙니다. 사용자 지정 양식의 섹션 내에서 필드를 편집할 수 있는 권한은 작업 자체에 대한 사용 권한에 따라 다릅니다. 작업 권한 설정에 대한 자세한 내용은 [작업 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. 클릭 **저장** 또는 다음 섹션으로 계속 진행합니다.

### 재무 {#finance}

1. 다음에 설명된 대로 작업 편집을 시작합니다. [작업 편집](#Edit2) 섹션에 자세히 설명되어 있습니다.
1. 클릭 **재무** 왼쪽 패널에 표시됩니다.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">비용 유형</td> 
      <td> <p>작업에 대한 원가 유형을 지정합니다. 이렇게 하면 작업의 시간 수를 기준으로 작업 비용이 계산되는 방식을 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
        <li> <p>비용 없음</p> </li> 
        <li> <p>고정 시간별 </p> </li> 
        <li> <p> 시간별 사용자 </p> </li> 
        <li> <p> 시간별 역할</p> </li> 
       </ul> <p>추적 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a> . Workfront 관리자 또는 그룹 관리자가 시스템 또는 그룹의 작업에 대한 기본 비용 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수익 유형</td> 
      <td> <p>작업에 대한 매출 유형을 지정합니다. 이렇게 하면 작업의 시간 수를 기반으로 작업에 대한 매출이 계산되는 방식을 결정합니다. </p> <p>다음 옵션 중에서 선택합니다. </p> 
       <ul> 
      <li> <p> 청구 불가 </p> </li> 
      <li> <p>시간별 사용자 </p> </li> 
      <li> <p>시간별 역할 </p> </li> 
      <li> <p>고정 시간별 </p> </li> 
      <li> <p>시간별 사용자(상한 포함) </p> </li> 
      <li> <p>시간별 역할(수용작업량 포함) </p> </li> 
      <li> <p>시간별 + 고정 사용자 </p> </li> 
      <li> <p>시간별 + 고정 역할 </p> </li> 
      <li> <p>고정 수입 </p> </li> 
       </ul> <p>매출 추적에 대한 자세한 내용은<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a> . </p> <p>Workfront 관리자 또는 그룹 관리자는 시스템 또는 그룹의 작업에 대한 기본 매출 유형 설정을 선택합니다. 프로젝트 기본값 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">시스템 전체 프로젝트 환경 설정 구성</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **저장** 또는 다음 섹션을 계속 진행합니다.

### 설정 {#settings}

1. 다음에 설명된 대로 작업 편집을 시작합니다. [작업 편집](#Edit2) 섹션에 자세히 설명되어 있습니다.
1. 클릭 **설정** 왼쪽 패널에 표시됩니다.

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
      <li> <p>정시에 가정함 </p> </li> 
      <li> <p>지연 경고 무시</p> </li> 
      <li> <p> Autocomplete </p> </li> 
      <li> <p>전임 작업 </p> </li> 
       </ul> <p>작업의 추적 모드에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">작업 추적 모드 개요</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">리소스 레벨링</td> 
      <td> <p>을(를) 선택합니다 <strong>자원 평준화에서 제외</strong> 작업에 할당된 자원을 평준화에서 제외하려면 필드를 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">레벨링 지연</td> 
      <td> <p>평준화 지연 을 시간 단위로 지정합니다. </p> <p> 평준화에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">작업 평준화 지연 업데이트</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 진행</td> 
      <td> <p>작업과 연결할 승인 프로세스를 선택합니다. 작업에 연결하려면 먼저 Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. 승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자도 그룹별 승인 프로세스를 만들 수 있습니다. </p> <p>승인 프로세스 생성에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">작업 항목에 대한 승인 프로세스 생성</a>. 승인 프로세스를 추가할 때 다음 사항을 고려하십시오. </p> 
       <ul>

   <li> <p>활성 승인 프로세스만 목록에 표시됩니다. </p> </li>

   <li> <p>시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 이외의 그룹과 연관된 승인 프로세스가 목록에 표시되지 않습니다. </p>

   <p><b>중요 사항</b>

   프로젝트 그룹이 변경되면 이전에 첨부된 그룹별 승인 프로세스가 단일 사용 승인 프로세스가 됩니다. 프로젝트 그룹의 변경 사항이나 승인 프로세스의 변경 사항이 승인 설정에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">그룹 및 승인 프로세스 변경이 지정된 승인 프로세스에 미치는 영향</a>. </p>

   </li>

   <li> <p>작업이 프로젝트에 추가될 때 작업에 자동으로 첨부할 기본 승인 프로세스를 정의할 수 있습니다. 기본 작업 승인 프로세스를 포함하도록 프로젝트를 설정하는 방법에 대한 자세한 내용은 문서의 "작업" 섹션을 참조하십시오 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a>. </p> </li>

   <li> <p>일괄 편집 작업은 다음과 같은 시나리오가 있습니다. </p> 
      <ul> 
      <li> <p>동일한 그룹에서 여러 태스크를 선택하면 시스템 레벨과 그룹 레벨 승인 프로세스가 모두 이 필드에 표시됩니다. </p> </li> 
      <li> <p>여러 그룹에서 여러 작업을 선택하면 시스템 수준 승인 프로세스만 이 필드에 표시됩니다. </p> </li> 
      <li> <p>작업에 단일 사용 승인 프로세스가 첨부된 경우 선택한 시스템 레벨 또는 그룹 레벨 승인 프로세스로 대체됩니다. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. **저장**&#x200B;을 클릭합니다.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## 작업 헤더에서 작업 편집(제한)

작업 헤더에서 제한된 양의 정보를 편집할 수 있습니다.

시스템 또는 그룹 관리자는 작업 헤더에 표시되는 필드를 사용자 지정할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

다음 필드는 기본적으로 프로젝트 헤더에 포함됩니다.

* 작업 이름
* 완료율
* 할당
* 계획 완료 날짜 및 시간

   >[!CAUTION]
   >
   >일부 작업 제약 조건 및 기타 종속성으로 인해 이 필드를 편집할 수 없습니다. 작업 제한에 대한 자세한 내용은 [작업 제한 개요](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 상태
* 현재 승인 프로세스에서 승인자로 설정된 경우 승인 결정을 수행합니다

## 일괄 작업 편집

목록에서 작업에 적용할 변경 사항을 자동으로 저장하도록 선택하면 작업을 일괄적으로 편집하고 모든 정보를 동시에 업데이트할 수 있습니다.

일괄 작업 저장에 대한 자세한 내용은 문서의 &quot;일괄 작업 편집&quot; 섹션을 참조하십시오 [목록의 작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
