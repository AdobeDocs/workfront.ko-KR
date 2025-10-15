---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL 간트] 차트에 정보가 표시되는 방식 구성'
description: 작업 목록 간트 차트 및 프로젝트 목록 간트 차트 모두에 표시되는 정보를 구성할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# [!UICONTROL 간트 차트]에 정보가 표시되는 방식 구성

<!-- Audited: 5/2025 -->

작업 목록 간트 차트 및 프로젝트 목록 간트 차트 모두에 표시되는 정보를 구성할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> 
   <p>[!UICONTROL Light] 이상<p>
   <p>[!UICONTROL Review] 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 보기] 이상 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 보기] 이상 액세스 권한</p> </td> 
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
   <td role="rowheader"> Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Light<p>
   <p>Or</p>
   <p>Current: Review</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 디스플레이 옵션 이해

다음 표에서는 [!UICONTROL 간트 차트]의 표시 옵션에 대해 자세히 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">실제 일자</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL 실제 시작 날짜] 및 [!UICONTROL 실제 완료 날짜]는 삼각형 아이콘으로 표시됩니다. [!UICONTROL 실제 완료 일자]가 null이면 [!UICONTROL 실제 시작 일자]만 표시됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">프로젝트 개요 [!UICONTROL 실제 완료 날짜] </a> 및 <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">프로젝트 개요 [!UICONTROL 실제 시작 날짜] </a>을(를) 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>작업 할당자를 표시합니다. 임무 책임자의 이름 옆에 있는 세부 정보 링크를 마우스로 가리키면 임무에 대한 할당 비율을 포함하여 임무 책임자에 대한 자세한 정보를 볼 수 있습니다.</p> <p>[!UICONTROL 간트 차트]를 PDF으로 내보낼 때 할당자가 [!UICONTROL 간트 차트]에 표시되지 않습니다. [!UICONTROL 간트 차트]를 PDF으로 내보내면 피할당자는 작업 목록에만 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기준 요소]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>초기 프로젝트 계획에 포함된 프로젝트에 대한 주요 데이터를 나타내는 프로젝트 스냅숏입니다. 프로젝트의 타임라인 전체에서 기준선을 가져올 수 있습니다. [!UICONTROL 간트 차트]에 기준선을 표시할 수 있도록 설정하면 표시할 기준선을 선택합니다. [!UICONTROL 간트 차트]에서 한 번에 하나의 기준선만 볼 수 있으며 회색 막대 형태로 표시됩니다.</p> <p>기준선에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">프로젝트 기준선 만들기</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 커밋 일자]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>작업이 완료될 때 피할당자가 약정으로 제공하는 날짜가 [!UICONTROL 간트 차트]에 마커와 함께 표시됩니다. </p> <p>커밋 날짜에 대한 자세한 내용은 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL 커밋 날짜] 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % 완료]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  완료된 작업의 백분율이 작업 라인에 표시됩니다.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 중요 경로]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>프로젝트의 타임라인에 영향을 줄 수 있는 작업은 중요 경로의 일부로 간주되며 빨간색으로 명확하게 표시됩니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이정표] 다이아몬드</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>마일스톤과 연관된 작업 뒤에 다이아몬드 아이콘이 표시됩니다. 마일스톤 위로 마우스를 가져가면 마일스톤의 이름과 날짜를 볼 수 있습니다. [!DNL Workfront] 관리자가 각 마일스톤 다이아몬드의 색상을 결정합니다.</p> <p>마일스톤에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">마일스톤 경로 만들기</a>를 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이정표] 줄</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>마일스톤과 연결된 작업 뒤에 줄이 표시됩니다. 마일스톤 위로 마우스를 가져가면 마일스톤의 이름과 날짜를 볼 수 있습니다. [!DNL Workfront] 관리자가 각 마일스톤 줄의 색을 결정합니다.</p> <p> 이정표에 대한 자세한 내용은  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">마일스톤 경로 만들기</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 전임 작업]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="precedent_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>두 작업 간의 전임 작업 관계를 보여 주는 작업 간 행입니다. 개별 전임 작업 줄을 강조 표시하려면 해당 줄 위로 마우스를 가져갑니다. 강조 표시를 유지하려면 클릭합니다. 한 번에 하나의 전임 작업 줄만 강조 표시할 수 있습니다.</p> <p>간트 차트의 여러 페이지에 걸쳐 있는 전임 작업 또는 프로젝트 간 전임 작업이 있는 작업 옆에 [!UICONTROL 전임 작업] 아이콘이 표시됩니다.</p> <p>모든 전임 작업 및 후임 작업과 해당 세부 정보(예: 작업 이름, 전임 작업 관계 유형 및 주요 날짜)를 보려면 [!UICONTROL 전임 작업] 아이콘을 클릭합니다.</p> <p>참고: 프로젝트 목록의 [!UICONTROL 간트 차트]에는 프로젝트 간 전임 작업에 대한 정보가 표시됩니다. 다른 프로젝트 간에 전임 작업 관계를 만드는 방법에 대한 자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">프로젝트 간 전임 작업 만들기</a>를 참조하십시오.</p> <p>전임 작업에 대한 자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">전임 작업 적용</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 진행 상태]</td> 
   <td> <p>[!UICONTROL 설정 시간] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__10월_2017.png"></p> <p>[!UICONTROL Behind]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind__10월._2017.png"></p> <p>[!UICONTROL At Risk]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>지연        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>주어진 작업에 대한 현재 진행 상태입니다. </p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">작업 [!UICONTROL 진행 상태] 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">예상 일자</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>현재 완료된 작업과 남은 작업을 기준으로 예상 시작 및 완료 날짜를 표시하는 예상 예상 타임라인입니다. </p> <p>예상 완료 날짜에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">프로젝트, 작업 및 문제에 대한 예상 완료 일자 개요</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 표시 옵션 구성

1. **작업 목록 간트 차트** 또는 **프로젝트 목록 간트 차트**(으)로 이동합니다.\
   Gantt 차트의 위치에 대한 자세한 내용은 [Gantt 차트 시작[!UICONTROL 을 참조하세요.]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)

1. (선택 사항) **예상 날짜로 전환** 설정을 선택하여 예상 날짜별로 작업을 표시합니다. 기본적으로 작업은 계획된 일자에 따라 표시됩니다.
1. **옵션** 아이콘을 클릭합니다. **옵션** 대화 상자가 열립니다.\
   ![Options.png](assets/options-350x129.png)

1. [!UICONTROL 간트 차트]에 표시할 구성 옵션을 선택하십시오.

   >[!NOTE]
   >
   > 일부 구성 옵션은 프로젝트 목록 [!UICONTROL 간트 차트]에서 사용할 수 없습니다.

1. 간트 차트의 아무 곳이나 클릭하여 **옵션** 대화 상자를 닫습니다.
