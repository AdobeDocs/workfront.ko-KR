---
content-type: reference
navigation-topic: workfront-navigation
title: 용어집 [!DNL Adobe Workfront] 용어
description: 다음 [!DNL Adobe Workfront] 용어집 목록은에서 일반적으로 사용되는 용어 목록입니다. [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] 인터페이스, 보고서 또는 의 의미를 이해하려고 합니다. [!DNL Workfront] 에 정의된 개념 [!DNL Workfront] 설명서를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: b57f5038746094dde4b98bd28361e730c28ba412
workflow-type: tm+mt
source-wordcount: '20060'
ht-degree: 0%

---


# 용어집 [!DNL Adobe Workfront] 용어

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>이 문서는 다음에 접할 수 있는 용어를 이해하기 위한 참조로 사용해야 합니다. [!DNL Adobe Workfront] 응용 프로그램, [!DNL Workfront] 설명서 또는 일반적으로 작업 계획 및 관리에 대해 언급할 때. 현재 이 정보를 업데이트하고 있으므로 이 테이블이 완료되지 않을 수 있습니다. 본 정보가 완벽하다고 간주할 때 본 면책조항을 삭제하겠습니다.

다음 표는 Adobe Workfront에서 일반적으로 사용되는 용어 목록입니다.

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>오브젝트 이름</strong></th> 
   <th><strong>설명</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 액세스 수준]</td> 
   <td>사용자가 Workfront 내의 다양한 오브젝트 및 도구와 상호 작용하는 방법을 결정하는 사용자 프로필입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 활성 작업]</td> 
   <td>현재 프로젝트에서 전임 작업 이(가) 수행할 수 없으며 향후 계획된 시작 일자가 있는 작업 제한이 없는 미완료 작업입니다. 즉, 오늘날에도 작업이 가능합니다.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>위치 [!DNL Workfront Goals], 활동은 목표에 대한 진행 표시기입니다. 수동으로 업데이트하는 진행률 표시줄이거나 목표와 연결된 프로젝트일 수 있습니다. 보고서에 활동을 표시할 수 없으며 [!DNL Workfront] API. 활동에 대한 자세한 내용은 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront 목표에서 결과 및 활동 시작</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 비용]</td> 
   <td> <p>작업 및 문제의 경우 작업 또는 문제에 할당된 리소스의 시간당 비용 요율과 관련하여 기록된 실제 시간과 관련된 비용입니다. 프로젝트의 경우 프로젝트의 작업 및 문제의 총 [!UICONTROL 실제 비용]입니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 지출 비용]</td> 
   <td> <p>프로젝트 또는 작업에 대해 기록된 모든 비용에 대한 [!UICONTROL 실제 금액]의 합계입니다.</p> <b>예 </b>
   <p>작업 1에 대한 경비를 만들고 [!UICONTROL 실제 비용] 필드에 $600.00을 입력하면 이 작업에 대한 [!UICONTROL 실제 비용]은 $600.00입니다. </p> 
   <p>프로젝트의 경우 [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 비용]을 계산합니다.</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 실제 근로시간]</td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 [!UICONTROL 실제 시간]은 프로젝트, 작업 또는 문제에 기록된 모든 시간의 합계입니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span> 작업 1에 대한 [!UICONTROL 업데이트] 탭에서 '로그 시간'을 클릭하고 25시간을 입력하면 작업 1의 실제 시간 = 25시간이 됩니다. </p> <p>[!DNL Workfront] 다음 공식을 사용하여 상위 작업 또는 프로젝트에 대한 [!UICONTROL 실제 시간]을 계산합니다.</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 인건비]</td> 
   <td> <p>작업 또는 프로젝트에 투자된 노동력과 연관된 [!UICONTROL 실제 비용]입니다. </p> <p>작업의 경우, [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 인건비]를 계산합니다.</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>작업에 [!UICONTROL User Hourly]의 [!UICONTROL 비용 유형]이 있는 경우 [!DNL Workfront] 사용자 비율을 사용합니다. 작업에 [!UICONTROL Role Hourly]의 [!UICONTROL 비용 유형]이 있는 경우, [!DNL Workfront] 작업 역할 비율을 사용하여 [!UICONTROL 실제 인건비]를 계산합니다. </p> <p>프로젝트의 경우 [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 인건비]를 계산합니다.</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>예를 들어 사용자가 [!UICONTROL User Hourly] [!UICONTROL Cost Type]을 사용하여 작업에 5시간을 기록하고 시간당 요금이 $100인 경우 [!UICONTROL Actual Labor Cost]는 $500입니다.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 수익] </td> 
   <td> <p>프로젝트 또는 작업의 [!UICONTROL 실제 수익]은 프로젝트 또는 작업의 [!UICONTROL 실제 시간]과(와) 연결된 금액입니다. </p> <p>의 수익 추적에 대한 정보 [!DNL Workfront], 참조 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 실제 시작]</td> 
   <td>사용자가 할당된 작업에서 진행 중인 오브젝트를 변경할 때의 타임스탬프.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL 애자일] 방식</td> 
   <td>다양한 분야의 사람들이 함께 일하는 팀과의 요구 사항 및 솔루션의 공동 진화를 기반으로 한 방법론의 일종입니다. 고정된 타임라인을 기반으로 유연성과 변화를 유도한다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 애자일 팀]</td> 
   <td>장래의 작업을 백로그에서 가져와서 [!UICONTROL Iteration]이라고 하는 지정된 기간 내에 작업하기 때문에 기존 팀과 다릅니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 모든 내 팀]</td> 
   <td> <p>이 항목이 [!UICONTROL filters]에서 참조되면 이 필드에는 로그인한 사용자가 속한 팀 중 하나에 속한 사용자나 로그인한 사용자가 속한 팀에 할당된 작업 항목이 표시됩니다. </p> <p>다른 사용자와 공유할 때 보고서를 더 일반적으로 만들려면 필터에서 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 항상 정보가 사용자 지정되므로 로그인하는 사용자에 따라 서로 다른 정보를 표시하는 보고서만 만들 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당 날짜]</td> 
   <td> <p>이 필드는 다음 유형의 보고서에서 찾을 수 있습니다.</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project](재무 데이터)</li> 
     <li>[!UICONTROL 예산 시간]</li> 
    </ul> <p>의 경우<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL 프로젝트(재무 데이터)] 보고서: </p> 
    <ul> 
     <li>다음을 이해하려고 할 때 이 보고서 작성 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 리소스에 할당된 [!UICONTROL 계획된 시간]의 양입니다.</li> 
     <li> <p>[!UICONTROL 할당 날짜]는 작업에 [!UICONTROL 작업 역할] 할당이 시작되는 주의 첫째 날(일요일)입니다. 리소스([!UICONTROL 작업 역할])는 할당된 작업의 [!UICONTROL Duration] 동안 주에 있는 수만큼 [!UICONTROL 할당 날짜]를 가질 수 있습니다. 작업이 여러 달에 걸쳐 있는 경우 해당 월의 첫 번째 날이 작업의 [!UICONTROL Duration] 내에 있으면 [!UICONTROL 할당 날짜]가 될 수도 있습니다.</p> <p>예를 들어, 3주 이상이고 [!UICONTROL 계획된 시간]이 90개인 작업에 [!UICONTROL 작업 역할]을 할당할 수 있습니다. 이러한 시간은 작업 기간 동안 균등하게 분배되므로 매일 작업 역할에 6 [!UICONTROL 계획된 시간]을 할당합니다.</p> <p><em> 작업의 [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ [!UICONTROL Duration] 동안 [!UICONTROL Work Days]의 수입니다. </em> </p> <p>그 결과 세 개의 [!UICONTROL 할당 날짜]가 있으며, 작업의 [!UICONTROL 기간] 동안 매주 일요일마다 하나씩 특정 수의 [!UICONTROL 계획된 시간]과 연결되어 있습니다.<br>작업이 한 달의 마지막 주 중간에 시작하여 새 달의 시작 후 2주 후에 끝나는 경우 작업에는 4개의 [!UICONTROL 할당 날짜]가 있습니다. 하나는 작업의 [!UICONTROL 기간] 동안 매주 일요일에, 하나는 새 달의 첫째 날에 할당됩니다.</p> <p>이 정보를 최대한 활용하려면 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 프로젝트(재무 데이터) 보고서를 작성하고 [!UICONTROL 할당 날짜]에 대한 매트릭스 그룹화를 추가한 다음 가장 정확한 데이터에 대해 주별, 월별, 분기별 또는 연도별 결과를 그룹화합니다.<br>매트릭스 그룹 빌드에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">매트릭스 보고서 만들기</a>.</p> </li> 
    </ul> <p>재무 정보는 [!UICONTROL 프로젝트(재무 데이터)] 보고서와 관련된 데이터가 5년 미만인 경우에만 표시됩니다. 예를 들어 작업 역할이 2015년 1월에 작업에 할당되었고 오늘이 2021년 9월인 경우 작업 역할에 대한 [!UICONTROL 할당 날짜]와 같은 재무 필드가 [!UICONTROL 프로젝트(재무 데이터)] 보고서에 채워지지 않습니다. </p> 
    <div> 
     <p>[!UICONTROL 예산 시간] 보고서의 경우:</p> 
     <ul> 
      <li>리소스 또는 리소스 플래너의 프로젝트에 할당된 [!UICONTROL 예산 시간]의 양을 이해하려고 할 때 이 보고서를 작성하십시오.</li> 
      <li> <p>[!UICONTROL 할당 날짜]는 [!UICONTROL 리소스 플래너]에서 시간을 예산 설정한 주의 첫째 날(일요일)입니다. </p> <p><b>팁</b></p> <p>한 주가 2개월 동안 지속되는 경우 보고서에는 두 개의 행이 생성됩니다. 하나는 첫 번째 요일(첫 번째 달 중 첫 번째 주의 일요일)에 해당하고 두 번째 행은 두 번째 달의 첫 번째 요일을 표시합니다. </p> <p>예를 들어 6월 30일(일요일) - 7월 6일(토요일) 주에 대해 사용자에 대해 8시간을 예산하는 경우 두 행은 6월 30일과 7월 1일의 [!UICONTROL 할당 일자]를 표시합니다. </p> </p> <p>리소스 예산 편성에 대한 자세한 내용은 [!DNL Resource Planner], 문서 참조 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">의 예산 리소스 [!DNL Resource Planner] [!UICONTROL Project] 및 [!UICONTROL Role] 뷰 사용</a>.</p> <p>[!UICONTROL 예산 시간] 보고서 작성에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">보고서: 예산 시간</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 알림]</td> 
   <td> <p>시스템 내의 사용자에게 정보를 전달하는 방법입니다. 이 정보는 종종 다음 위치에서 제공됩니다. [!DNL Workfront] 을 관리자와 연결하거나 관리자에서 사용자로 연결합니다. </p> <p>자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">공지 보내기</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 앱 통합]</td> 
   <td>앱은 소프트웨어 응용 프로그램에 대한 커넥터를 가장 일반적으로 나타내지만 데이터를 조작하는 특수 기능을 나타낼 수도 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자 결정]</td> 
   <td> <p>[!UICONTROL Proof Approval] 보고서에서 이 필드는 더 이상 활성화되지 않은 증명에 대한 증명 승인 결정을 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자 단계]</td> 
   <td>[!UICONTROL 증명 승인 보고서]에서 이 필드는 증명 현재 단계에 대한 정보를 표시합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>작업, 문서 또는 타임시트와 같은 특정 작업 항목에서는 감독자 또는 다른 사용자가 해당 작업 항목을 승인해야 할 수 있습니다. 이러한 승인 프로세스를 승인이라고 합니다. </p> <p>자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인 날짜]</td> 
   <td>[!UICONTROL Proof Approval] 보고서에서 이 필드에는 증명이 승인된 날짜가 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자]</td> 
   <td>주어진 작업 항목에서 승인해야 하는 사용자 또는 작업 역할 또는 타임시트의 시간 항목을 승인하는 사용자입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>[!UICONTROL 작업 또는 문제] 보고서에서 이 필드에는 작업 또는 문제의 소유자 또는 [!UICONTROL 기본 피할당자]가 표시됩니다. 이 필드를 기준으로 필터링하거나 그룹화할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>문제 또는 작업에 할당된 사용자, 작업 역할 또는 팀입니다. 프로젝트, 포트폴리오 또는 프로그램에는 할당이 있을 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 할당된 모든 엔터티(사용자, 작업 역할, 팀)의 목록이 표시됩니다. [!UICONTROL Assignment Users] 및 [!UICONTROL Assignment Roles] 필드를 사용하여 이 필드별로 필터링할 수 있습니다. 팀 필드를 사용하여 작업 또는 문제에 할당된 팀별로 필터링할 수 있습니다. 이 필드로 보고서를 그룹화할 수 없습니다.</p> <p>[!UICONTROL 휴지통]에 배치된 작업 항목은 다음을 포함하는 [!UICONTROL Assignment] 개체를 참조하는 일부 보고서에 계속 표시됩니다. [!DNL OR] 필터 수정자가 사용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 할당된 작업 역할에 대한 정보가 표시됩니다. 이 필드에는 [!UICONTROL 기본 소유자]와 작업 또는 문제에 할당된 기타 작업 역할이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당 상태]</td> 
   <td> <p>할당, 작업 또는 문제 보고서에서 [!UICONTROL 할당 상태]는 작업 항목에 할당된 사용자가 작업을 수락하거나 완료하기 위해 [!UICONTROL 작업 완료] 단추 또는 [!UICONTROL 완료] 단추를 클릭했는지 여부를 표시합니다. 다음 [!UICONTROL Assignment States]이(가) 있습니다.</p> 
    <ul> 
     <li><b>[!UICONTROL 요청됨]</b>: 사용자가 작업 또는 문제에 할당되었지만 아직 작업을 시작하기 위해 [!UICONTROL Work On It] 버튼을 클릭하지 않았습니다.</li> 
     <li><b>[!UICONTROL 작동 중]</b>: 사용자가 [!UICONTROL Work On It] 버튼을 클릭했으며 현재 항목에서 작업 중입니다. </li> 
     <li><b>[!UICONTROL 완료]</b>: 사용자가 [!UICONTROL Done] 단추를 클릭하여 항목에 대한 작업을 완료했습니다. </li> 
    </ul> <p>자세한 내용은 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL 처리 중] 및 [!UICONTROL 완료] 단추 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당 팀]</td> 
   <td>
   <p>[!UICONTROL task] 또는 [!UICONTROL issue] 보고서에서 이 필드에는 작업 또는 문제에 할당된 팀에 대한 정보가 표시됩니다. 필드에는 [!UICONTROL 기본 소유자]와 작업 또는 문제에 할당된 다른 팀이 표시됩니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 할당된 사용자에 대한 정보가 표시됩니다. 이 필드에는 [!UICONTROL 기본 소유자]와 작업 또는 문제에 할당된 다른 사용자가 표시됩니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 속성]</td> 
   <td>속성은 다음과 같은 트레이트입니다. [!DNL Workfront] 개체.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감사 영역]</td> 
   <td> <p>감사는 Workfront에서 발생한 작업을 기록하는 시스템 메시지입니다. 다음 감사 유형이 기록됩니다.</p> 
    <ul> 
     <li>[!UICONTROL 범위 변경]</li> 
     <li>[!UICONTROL 첨부 파일 작업]</li> 
     <li>[!UICONTROL 일반 편집]</li> 
     <li>[!UICONTROL 상태 변경]</li> 
     <li>[!UICONTROL 참고]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL 오류 항목]</li> 
     <li>[!UICONTROL 상태 변경]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>기록된 변경 사항([!UICONTROL 감사 영역])을 통해 추적되는 이벤트에 의해 자동으로 생성된 메모의 컬렉션입니다. 각 메모에는 작업을 수행한 사용자, 수행한 작업 및 수행한 시간이 기록됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 자동 및 변경 시]</td> 
   <td> <p>[!UICONTROL 프로젝트 업데이트] 유형 중 하나입니다. 이렇게 하면 야간 다시 계산 프로세스가 실행되고 프로젝트 또는 프로젝트 내의 작업이 업데이트될 때 프로젝트의 예상 및 계획된 타임라인이 다시 계산됩니다. </p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형 선택 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>가용성</p></td> 
   <td> <p>이 용어는 "사용자 가용성" 또는 "리소스 가용성"과 관련하여 사용되며 리소스(사용자 또는 작업 역할)가 작업할 수 있는 시간을 보여 줍니다. </p> 
   <p>Workfront은 여러 필드를 사용하고 시스템에 있는 리소스 관리 기본 설정의 설정에 따라 사용자 가용성을 계산합니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>. </p>
   <p>리소스 가용성에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">리소스 관리 시작</a></p>
   또는 "용량"은 리소스 가용성을 나타내는 데에도 사용됩니다. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL 자동 전용]</td> 
   <td> <p>[!UICONTROL 프로젝트 업데이트] 유형 중 하나입니다. 이렇게 하면 야간 다시 계산 프로세스가 실행될 때 예상 및 계획 타임라인이 다시 계산됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형 선택</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>일상적인 기본 비즈니스 목표를 실행하는 데 기여하는 "일상적인 비즈니스" 작업.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 백로그]</td> 
   <td>새로운 문제를 처리할 준비가 될 때까지 문제가 유지되는 애자일 환경의 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 기준 요소]</td> 
   <td>애자일 환경에서 반복을 측정할 데이터 소스입니다.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL 청구 가능 경비]</td> 
   <td> <p>고객에게 청구 가능으로 표시된 비용. 이는 계획된 비용이거나 실제 비용일 수 있습니다.</p> <p>뷰 및 보고서에 추가할 수 있는 계획된 청구 가능 경비 및 실제 청구 가능 경비 필드를 사용할 수 있습니다. 프로젝트 또는 작업 세부 정보 페이지에는 표시되지 않습니다.</p>
   <p>다음 유형의 보고서에서 이러한 필드를 찾을 수 있습니다.</p>
   <ul>
   <li>기준선</li>
   <li>템플릿</li>
   <li>프로젝트(재무 데이터)</li>
   </ul>
   <p>경비를 청구 가능 경비로 표시하는 방법에 대한 자세한 내용은 다음을 참조하십시오. <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">프로젝트 경비 관리</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL 청구 기록]</td> 
   <td> <p>청구할 수 있는 수익, 시간 또는 비용을 기록합니다. 이 정보는 외부 회계 시스템에서 송장을 생성하는 데 사용할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">청구 기록 만들기</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>청구 기록 상태</td> 
   <td> <p>청구 기록 또는 시간 보고서에서 청구 기록 상태는 청구 기록이 청구되었는지 또는 청구되지 않았는지 여부를 나타냅니다. 청구된 청구 기록과 연결된 시간을 편집하거나 프로젝트를 삭제할 수 없습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >청구 기록 만들기</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL 브랜딩]</td> 
   <td><p>맞춤화 프로세스 [!DNL Workfront] 색상 및 로고를 사용하여 회사를 미러링하는 모양을 인터페이스에 제공합니다.</p><p><strong>참고</strong><br>조직이 로 온보딩된 경우 [!DNL Adobe Experience Cloud], 브랜딩을 사용할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 탐색 표시]</td> 
   <td> <p>페이지 맨 위에 있는 영역으로, 사용자가 애플리케이션에서 있는 위치의 계층적 위치를 보여 줍니다.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">자세한 내용은 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">탐색 표시 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산 상태]</td> 
   <td> <p>사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이(가) 제거되어 필드를 업데이트할 수 없습니다. </p> <p>이 필드에는 프로젝트가 [!UICONTROL Capacity Planner]에 추가되었는지 여부와 예산 계산이 완료되었는지 여부가 표시됩니다. [!UICONTROL Capacity Planner]가에서 제거되었습니다. [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산 완료 일자]</td> 
   <td> <p>사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이(가) 을(를) 제거했습니다. 이 필드는 업데이트할 수 없습니다. </p>
   <p> 이 필드는 [!UICONTROL project] 및 [!UICONTROL tasks] 보고서와 목록에 계속 표시됩니다.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산 비용]</td>

<td> <p>프로젝트의 리소스 예산 책정과 관련된 비용입니다. </p>
   <p>필드는 의 다음 영역에 표시됩니다. [!DNL Workfront] 다음 이름:</p>
   <ul>
   <li><strong>[!UICONTROL 예산 비용]</strong>: [!UICONTROL 비즈니스 사례 요약] 패널에서</li>
   <li><strong>[!UICONTROL 비용]</strong>: [!UICONTROL Cost]로 정보를 볼 때 [!UICONTROL Utilization] 영역에서 다음을 수행합니다</li>
   <li><strong>[!UICONTROL 프로젝트 예산 비용]</strong>: 목록 및 보고서에서</li>
   </ul>   
    <p>프로젝트에 대한 [!UICONTROL 예산 비용]은 다음 공식을 사용하여 계산됩니다.</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>[!UICONTROL 예산 비용] 계산에 대한 자세한 내용과 의 이 개념에 대한 다양한 이름을 알아보려면 [!DNL Workfront], 참조 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">프로젝트 예산 비용 계산</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 예산 시간]</td> 
   <td> <p>프로젝트에서 완료하는 데 필요한 작업에 대한 리소스 예산 시간. 이 필드는 프로젝트 또는 프로젝트 리소스에 대해 [!UICONTROL 비즈니스 사례]([!UICONTROL 리소스 플래너])의 [!UICONTROL 리소스 예산 책정] 영역에서 예산이 책정된 시간을 나타냅니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 [!UICONTROL 예산 인건비] 및 [!UICONTROL 예산 시간] 이해</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 의 사용자 예산 편성에 대한 자세한 내용 [!DNL Resource Planner], 문서 참조 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">의 예산 리소스 [!DNL Resource Planner] [!UICONTROL Project] 및 [!UICONTROL Role] 뷰 사용</a>. </p> 
    <p>[!UICONTROL 비즈니스 사례] 또는 [!UICONTROL Resource Planner]의 [!UICONTROL Resource Budgeting] 영역에서 예산이 책정된 시간은 다음 영역에 표시됩니다. [!DNL Workfront] 및 을 사용하여 메시지를 보낼 수 있습니다.</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL 예산 시간] 표시 이름</strong></td> 
        <td><strong>영역 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 시간]</td> 
        <td>[!UICONTROL 비즈니스 사례]의 [!UICONTROL Resource Budgeting] 영역</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Hours]에서 본 [!UICONTROL Resource Planner]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 예산 시간]</td> 
        <td> <p>사용률 보고서 [!UICONTROL 시간] 보기</p> <p>[!UICONTROL 사용률] 보고서에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL Resource Utilization] 보고서 개요</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 버드. Hours]</td> 
        <td> <p>[!UICONTROL 예산 시간] 보고서</p><p>예산 시간 보고서의 [!UICONTROL 예산 시간] 개체는 더 이상 사용되지 않는 리소스 관리 도구와 관련된 정보를 참조합니다. "[!UICONTROL 버드만. 이 보고서의 "시간" 필드는 프로젝트 [!UICONTROL 비즈니스 사례]의 [!UICONTROL 리소스 플래너] 또는 [!UICONTROL 리소스 예산 책정] 영역에서 예산 책정된 시간을 나타냅니다. </p> <p>보고서 만들기에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 리소스 플래너 예산 시간] </td> 
        <td> <p>다음 보고서에 있습니다.</p>
        <ul>
        <li>[!UICONTROL 프로젝트] 보고서
        <li>[!UICONTROL 프로젝트(재무 데이터)] 보고서
        <li>[!UICONTROL Task] 보고서
        <li>[!UICONTROL Issue] 보고서
        <li>[!UICONTROL 예산 시간] 보고서</li>
        </ul>
         <p>보고서 만들기에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>에 [!UICONTROL 예산 시간]에 대한 다른 언급 [!DNL Adobe Workfront] 는 Workfront에서 제거된, 더 이상 사용되지 않는 기능을 사용하여 예산 책정된 시간을 나타냅니다. 이는 보기 전용 필드이며 현재 리소스 예산 책정 도구를 사용할 때 현재 정보로 업데이트되지 않습니다. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산 인건비]</td> 
   <td> <p>리소스 관리자로서 사용자가 프로젝트에서 완료하는 데 필요한 작업에 대한 작업 역할에 예산을 책정하는 시간과 관련된 비용입니다. </p> <p>프로젝트 보고서의 [!UICONTROL 예산 인건비]는 다음 공식을 사용하여 계산됩니다.</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>이 필드는 다음을 의미할 수 있습니다.</p> 
    <ul> 
     <li> <p>프로젝트의 작업 역할 비용과 관련된 [!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역이나 [!UICONTROL Resource Planner]에 표시되는 인건비입니다. [!UICONTROL 예산 인건비] 계산에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 [!UICONTROL 예산 인건비] 및 [!UICONTROL 예산 시간] 이해</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>프로젝트에서 프로젝트에 연결된 이니셔티브에서 추정된 [!UICONTROL People Costs]를 반영하는 [!UICONTROL 비즈니스 사례]의 [!UICONTROL Resource Budgeting] 영역에 표시되는 인건비 [!DNL Scenario Planner] 시나리오 플래너를 사용하여 프로젝트 리소스의 예산을 책정하는 경우. 이니셔티브에 대한 자세한 내용은 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">시나리오 플래너의 이니셔티브 개요</a>. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> </li> 
     <p>이 아이콘은 의 다음 영역에 다음 이름으로 표시됩니다.</p>
   <ul>
   <li><strong>[!UICONTROL 예산 인건비]</strong>: [!UICONTROL 비즈니스 사례]의 [!UICONTROL 리소스 예산 책정] 영역에서.
   <li><strong>[!UICONTROL 예산 비용]</strong>: [!UICONTROL 사용률] 보고서 [!UICONTROL 비용] 보기에서
   <p>자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 가동률 정보 보기 </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: [!DNL Resource Planner] 프로젝트 또는 [!DNL Role] 보기, 비용별로 볼 때
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: 다음 보고서에서: 
   <ul>
    <li>[!UICONTROL 프로젝트] 보고서</li>
    <li>[!UICONTROL 프로젝트(재무 데이터)] 보고서</li>
    <li>[!UICONTROL Task] 보고서</li>
    <li>[!UICONTROL Issue] 보고서</li>
    <li>[!UICONTROL 예산 시간] 보고서</li> 
    </ul>
    <p>보고서 만들기에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL 예산 시작 일자]</td> 
  <td> <p>사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이(가) 을(를) 제거했습니다. 이 필드는 업데이트할 수 없습니다.</p>
  <p>이 영역은에서 제거되었습니다. [!DNL Workfront]. </p> 
  <p>필드는 여전히 [!UICONTROL project] 및 [!UICONTROL task] 보고서와 목록에 표시됩니다.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 번다운 차트]</td> 
   <td>완료된 작업과 남은 작업을 시각적으로 표시하는 라인 차트입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 비즈니스 사례]</td> 
   <td> <p>프로젝트를 [!UICONTROL Idea] 상태에서 [!UICONTROL Planning] 상태로 앞으로 이동해야 하는지 여부를 평가하는 데 사용되는 도구입니다. 즉, [!UICONTROL 비즈니스 사례]는 특히 포트폴리오의 다른 프로젝트와 비교할 때 프로젝트를 시작하고 완료하는 것이 가치가 있는지 여부를 조직에서 결정하는 데 도움이 됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">프로젝트에 대한 [!UICONTROL 비즈니스 사례] 만들기 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 비즈니스 사례 예산 시간]</td> 
   <td> <p>사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이(가) 을(를) 제거했습니다. 이 필드는 업데이트할 수 없습니다.</p> <p>이 필드는 프로젝트 및 [!UICONTROL 작업] 목록과 보고서에 계속 표시됩니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>작업 [!UICONTROL 기간 유형] 중 하나입니다. 작업의 [!UICONTROL Duration] 및 [!UICONTROL Work Required]를 기반으로 작업에 할당된 사용자가 작업에 할당되는 8시간 근무일의 백분율을 계산합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL Duration] 및 [!UICONTROL Duration Type] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계산된 작업]</td> 
   <td> <p>[!UICONTROL 기간 유형] 작업 중 하나입니다. 그러면 [!UICONTROL Duration] 및 사용자 [!UICONTROL Assignment] 백분율(8시간 근무일을 기반으로 함)이 지정된 작업에 대한 [!UICONTROL 작업 필요]가 계산됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL Duration] 및 [!UICONTROL Duration Type] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>에는 두 가지 유형의 캘린더가 있습니다 [!DNL Workfront]: [!UICONTROL 홈 캘린더] 및 캘린더 보고서.</p> <p>[!UICONTROL 홈 캘린더]는 사용자가 의 사용 가능한 시간에 대한 워크로드를 관리할 수 있는 개인 캘린더입니다. [!DNL Workfront]. 사용자는 또한 [!UICONTROL 홈 캘린더]를 [!DNL Outlook] ([!DNL Google] 및 [!DNL Microsoft] 통합 예정). </p> <p>[!UICONTROL 홈 캘린더]에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL 홈 캘린더] 보기</a>.</p> <p>달력 보고서는 사용자가 기한과 작업 상태, 이벤트를 할당할 사용자 등 이벤트의 날짜 및 기타 중요한 세부 정보를 볼 수 있는 동적 보고서입니다.</p> <p> 달력 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">달력 보고서 개요</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL 시작 가능]</td> 
   <td> <p>이 필드는 작업이 작업을 시작할 준비가 되었는지 여부를 나타냅니다. 시작할 준비가 되면 작업의 [!UICONTROL 시작 가능] 필드를 [!UICONTROL True]로 설정합니다. </p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">작업에 대한 "[!UICONTROL 시작 가능]" 개요</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>용량</p> </td> 
   <td> <p>작업에 할당할 수 있는 리소스 사용 가능 시간. "가용성"을 참조하십시오. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL 범주]</p> </td> 
   <td> <p>범주는 사용자 정의 양식입니다. 이 개체에 대한 보고서를 작성하고 다른 개체 보고서에도 표시할 수 있습니다. 일부 객체에는 사용자 정의 양식 또는 범주가 있을 수 없습니다. 다음 객체에는 사용자 정의 양식이 있을 수 있습니다. <br></p> 
    <ul> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 문서]</li> 
     <li>[!UICONTROL 비용]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL 반복]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범주 이름]</td> 
   <td> <p>다음 개체의 보기에 열로 추가되면 해당 개체와 연결된 모든 사용자 정의 양식의 목록이 표시됩니다.</p> 
    <ul> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 작업]<br></li> 
     <li>[!UICONTROL 문제]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL 문서]<br></li> 
     <li>[!UICONTROL 비용]<br></li> 
     <li>[!UICONTROL 프로그램]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL 반복]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 변경 관리]</td> 
   <td>범위, 일정, 비용 및 리소스 요인의 변경 사항에 대한 계획된 작업을 정의, 이해 및 조정하는 데 중점을 둔 실습 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 변경 순서]</td> 
   <td>합의된 범위에 대한 요청된 변경 사항을 요약하는 프로젝트에 대해 제기된 문제 유형입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변경 전용]</td> 
   <td>프로젝트 [!UICONTROL 업데이트 유형] 중 하나입니다. 프로젝트에 대해 작업을 업데이트하거나 작업을 편집할 때 [!UICONTROL Project Projected] 및 [!UICONTROL Planned] 타임라인만 업데이트됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변경 순서]</td> 
   <td> <p>일반적으로 프로젝트를 완료하기 전에 계획되지 않은 양의 작업을 수행해야 함을 나타내는 [!UICONTROL Issue] 유형 중 하나입니다.</p> <p>[!UICONTROL Issue] 유형에 대한 자세한 내용은 문서의 "기본 문제 유형" 섹션을 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">기본 문제 유형 사용자 지정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 하위 작업]</td> 
   <td>[!UICONTROL 상위 작업]([!UICONTROL 요약 작업])의 [!UICONTROL 하위 작업]인 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 하위]</td> 
   <td>[!UICONTROL 상위 작업]([!UICONTROL 요약 작업])에 대한 [!UICONTROL 하위 작업]의 컬렉션입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] 및 [!UICONTROL Training]</td> 
   <td>학습 모듈, 인증, 표준 또는 실무 커뮤니티입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>사용자가 작업 결과물에 대한 기대를 설정할 수 있는 커뮤니케이션 도구입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 커밋 일자]</td> 
   <td>사용자가 작업 결과물에 대한 기대치를 설정할 수 있는 커뮤니케이션 도구입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] 및 [!UICONTROL Reporting]</td> 
   <td>프로젝트, 프로그램 또는 포트폴리오의 예외 및 상태를 검토하는 표준</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>[!UICONTROL Company]는 의 조직 단위입니다. [!DNL Workfront]. </p> 
   <p> 사용자 또는 프로젝트를 하나의 회사와 연결할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">회사 만들기 및 편집</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료 날짜]</td> 
   <td> <p>프로젝트, 작업 또는 문제가 완료되도록 설정된 날짜입니다. 에는 몇 가지 유형의 [!UICONTROL 완료 날짜]가 있습니다. [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL 실제 완료 날짜]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">프로젝트 [!UICONTROL 실제 완료 일자] 개요 </a>.</li> 
     <li>[!UICONTROL 계획된 완료 일자]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">프로젝트 [!UICONTROL 계획된 완료 일자] 설정</a> 및 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">[!UICONTROL 계획된 완료 일자] 작업의 개요</a>.</li> 
     <li>[!UICONTROL 예상 완료 일자]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">프로젝트, 작업 및 문제에 대한 [!UICONTROL 예상 완료 일자] 개요</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료 일자]</td> 
   <td>[!UICONTROL Template]의 시작과 관련하여 [!UICONTROL Template Task] 또는 [!UICONTROL Template]이 완료되어야 하는 날짜입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료 모드]</td> 
   <td> <p>프로젝트가 [!UICONTROL Complete]로 표시되는 방식을 나타냅니다. 다음 두 가지 값을 가질 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Manual]: 사용자는 프로젝트 상태를 [!UICONTROL Complete](으)로 변경해야 합니다.</li> 
     <li>[!UICONTROL 자동]: 프로젝트의 모든 작업이 100% 완료되고 모든 문제가 종료되면 프로젝트 상태가 [!UICONTROL 완료]로 자동 변경됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>작업, 문제 또는 프로젝트의 진행 상황을 시각적으로 보여줍니다.</p> <p>프로젝트의 경우 조건은 프로젝트 소유자가 수동으로 설정하거나 사용자가 자동으로 설정할 수 있습니다. [!DNL Workfront], 프로젝트의 진행 상태를 기반으로 합니다. </p> <p>프로젝트 조건에 사용할 수 있는 값은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL 문제 발생]</li> 
    </ul> <p>프로젝트 조건에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL 프로젝트 상태] 및 [!UICONTROL 상태 유형] 개요</a>.</p>
     <p>작업 및 문제 조건을 보고서에 표시할 수 있는 숫자와 연결할 수 있습니다. 아래 목록에는 작업 및 문제 조건에 대한 기본 이름과 번호가 표시됩니다. 시스템 관리자는 조건 이름을 업데이트할 수 있으며 다른 번호로 새 조건을 추가할 수 있습니다. 숫자가 조건과 연결된 후에는 편집할 수 없습니다.  </p> 
     <p>작업의 경우 작업 소유자가 조건을 수동으로 설정합니다. 작업 조건에 사용할 수 있는 값은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL 원활하게 진행 중] (0)<br></li> 
     <li> [!UICONTROL 몇 가지 문제] (1)<br></li> 
     <li>[!UICONTROL 주요 장애물] (2)</li> 
    </ul> <p>작업 조건에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">작업 및 문제에 대한 [!UICONTROL Condition] 업데이트</a>.</p> <p>문제의 경우 문제 소유자가 조건을 수동으로 설정합니다. 문제 조건에 사용할 수 있는 값은 다음과 같습니다.<br></p> 
    <ul> 
     <li>[!UICONTROL 원활하게 진행 중] (0)<br></li> 
     <li>[!UICONTROL 몇 가지 문제] (1)<br></li> 
     <li>[!UICONTROL 주요 장애물] (2)</li> 
    </ul> 
   <p><b>메모</b></p>
    <p>[!UICONTROL Journal Entry] 보고서에서 [!UICONTROL Condition] 필드가 추적되면 [!UICONTROL New] 및 [!UICONTROL Old Number Values]에 해당 이름 대신 조건과 연결된 번호가 표시됩니다. 원래 작업 또는 문제에 대해 조건이 정의되지 않은 경우 나중에 업데이트하면, 업데이트를 캡처하는 저널 항목에 [!UICONTROL Condition] 필드의 [!UICONTROL Old Number Value]이 -2,147,483,648로 표시됩니다. 이 문서에서 "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]" 및 "[!UICONTROL Journal Entry]"도 참조하십시오. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태 업데이트]</td> 
   <td> <p>이 필드에는 작업, 프로젝트 또는 문제의 현재 상태가 표시됩니다. 이 옵션은 작업, 프로젝트 또는 문제의 소유자가 [!UICONTROL 업데이트 상태] 필드에 제공한 최신 업데이트와 새 조건을 표시합니다.</p> <p>조건 업데이트에 대한 설명은 [!UICONTROL 조건 업데이트] 열에 표시되지 않고 기본 업데이트만 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제약 조건 날짜]</td> 
   <td> <p>[!UICONTROL Must Start On]과 같이 특정 날짜에 연결된 [!UICONTROL Task Constraint]를 사용하는 경우 해당 특정 날짜가 작업의 [!UICONTROL Constraint Date]가 됩니다.</p> <p>다음 작업 제약 조건은 [!UICONTROL 제약 조건 날짜] 필드를 업데이트합니다.</p> 
    <ul> 
     <li>[!UICONTROL은(는) 다음에 시작해야 합니다.]</li> 
     <li>[!UICONTROL 다음까지 완료]</li> 
     <li>[!UICONTROL 늦지 않게 시작]</li> 
     <li>[!UICONTROL 다음 이후에 시작]</li> 
    </ul> <p><b>팁</b></p>   
     <ul> 
      <li> <p>[!UICONTROL Fixed Dates]의 [!UICONTROL Constraint]이(가) 있는 작업에 [!UICONTROL Constraint Date]가 없습니다. </p> </li> 
      <li> <p> [!UICONTROL 제한 날짜]는 보고서 또는 사용자 지정된 보기에서만 볼 수 있습니다.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제약 조건 일]</td> 
   <td> <p>Must Start On과 같이 특정 날짜에 연결된 템플릿 작업에서 작업 제한 사항을 사용하는 경우 해당 특정 날짜가 템플릿 작업의 제한 일자가 됩니다.</p> <p>다음 작업 제약 조건은 [!UICONTROL Constraint Day] 필드를 업데이트합니다.</p> 
    <ul> 
     <li>[!UICONTROL은(는) 다음에 시작해야 합니다.]</li> 
     <li>[!UICONTROL 다음까지 완료]</li> 
     <li>[!UICONTROL 늦지 않게 시작]</li> 
     <li>[!UICONTROL 다음 이후에 시작]</li> 
    </ul> <p><b>팁</b></p> <p>  [!UICONTROL 제한조건 일]은 보고서 또는 사용자 지정된 보기에서만 볼 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제약 조건 유형]</td> 
   <td> <p>작업의 예약 경향. 예를 들어 [!UICONTROL As Soon Possible]은 작업을 가능한 한 빨리 시작하도록 예약하며, [!UICONTROL Finish No Later]는 작업을 [!UICONTROL Constraint Date] 및 그 이후에 완료하도록 예약합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상황별 메뉴]</td> 
   <td>화면 왼쪽에 있는 메뉴로, 항목이 활성 컨텐츠와 상관 관계를 맺도록 변경됩니다. 예를 들어 사용자가 프로젝트를 볼 때 [!UICONTROL 상황별 메뉴]에 프로젝트 관련 정보 및 도구에 대한 링크가 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>문제가 프로젝트 또는 작업으로 변환될 때 문제의 [!UICONTROL 기본 담당자]인 사용자에 대한 정보를 표시하는 프로젝트 또는 작업 보고서의 필드입니다. 필드는 [!UICONTROL 프로젝트 세부 사항] 섹션에도 표시되며, 여기에서는 변환된 문제의 [!UICONTROL 기본 담당자]의 이름을 표시합니다. 이 문서에서 "[!UICONTROL 기본 담당자]"도 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 비용]</td> 
   <td> <p>프로젝트, 작업 또는 문제를 완료할 때 지출해야 하는 통화 금액입니다. </p> <p>프로젝트와 관련된 인건비, 경비, 위험에 대한 다양한 유형의 비용을 추적할 수 있습니다.비용 추적에 대한 자세한 내용은 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/track-costs.md">비용 추적</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 비용 유형]</td> 
   <td>작업의 경우 [!UICONTROL 비용 유형]에 따라 작업의 비용 발생 방법이 결정됩니다. 일부 예에는 [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] 및 [!UICONTROL User Hourly plus Fixed]가 있습니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 간 종속성]</td> 
   <td> <p>한 프로젝트의 작업이 다른 프로젝트의 작업에 종속됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">프로젝트 간 전임 작업 만들기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 사용자 지정 데이터]</td> 
   <td> <p>조직에 고유한 데이터. 조직은 다음을 사용자 지정할 수 있습니다. [!DNL Workfront] 사용자 정의 양식 및 사용자 정의 필드를 만들어 적용. 이러한 사용자 지정 정보를 통해 KPI, 감사 및 수요 혼합에 대한 보고를 수행할 수 있습니다. </p> <p>[!UICONTROL 사용자 지정 데이터]는 다음에 연결할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 사용자]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 문서]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL 반복]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 데이터 유형]</td> 
   <td>[!UICONTROL 사용자 지정 데이터] 필드를 텍스트, 날짜, 숫자 또는 통화로 데이터베이스에 저장할지 여부를 지정하는 옵션입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 표시 유형]</td> 
   <td>사용자 정의 필드의 필드 표시 유형입니다. 예로는 [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons] 등이 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 필드]</td> 
   <td>사용자가 여러 선택 사항 중에서 선택할 수 있도록 해 주는 사용자 지정 데이터의 경우 사용자가 선택할 수 있는 값입니다. 사용자 지정 옵션은 [!UICONTROL 드롭다운], [!UICONTROL 다중 선택 드롭다운], [!UICONTROL 라디오 단추] 및 [!UICONTROL 확인란]에서만 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 정의 양식 레이블]</td> 
   <td>사용자 지정 옵션과 함께 사용자 지정 표시 유형을 사용하는 경우 이는 해당 사용자 지정 옵션의 드롭다운 메뉴, 확인란 또는 라디오 버튼에 표시되는 사용자 인터페이스 텍스트입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 값]</td> 
   <td>사용자 지정 옵션과 함께 사용자 지정 필드를 사용할 때 특정 옵션에 대해 데이터베이스에 저장되는 값입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 보기]</td> 
   <td>목록의 각 개체에 대해 표시되는 데이터 필드 또는 열의 정의입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Workfront 인스턴스를 사용하는 조직</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 대시보드]</td> 
   <td> <p> 보고서 또는 보고서 객체 보기에 이 필드를 추가하여 보고서가 목록에 나열된 대시보드를 표시할 수 있습니다. </p> <p> 이 필드를 사용하여 특정 대시보드에 나열된 보고서를 필터링할 수도 있습니다. </p> <p> 보고서 객체 보고서에 대시보드 정보를 포함하는 방법에 대한 자세한 내용은 이 문서의 "대시보드에 나열된 보고서 이해" 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">보고서 액세스 및 구성</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 데이터 유형]</td> 
   <td>"[!UICONTROL 사용자 지정 데이터 유형]"을(를) 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지연 일수]</td> 
   <td> <p>[!UICONTROL 실제 완료 일자]가 누락된 경우 이 필드는 [!UICONTROL 계획된 시작]과 [!UICONTROL 오늘] 간의 날짜 차이를 보여 줍니다.</p> <p>[!UICONTROL 실제 완료 일자]가 있는 경우 [!UICONTROL 실제 완료 일자]와 [!UICONTROL 계획된 완료 일자] 간의 날짜 차이도 표시합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 기본 일정]</td> 
   <td> <p>조직 내의 사용자 및 프로젝트에 할당할 사용자 정의 가능한 기본 작업 시간입니다. </p> <p>일정은 사용자에게 할당된 작업의 계획, 시작 및 완료 날짜를 계산하는 데 사용됩니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 결과물]</td> 
   <td>프로젝트 완료 시 제공되어야 하는 수량 가능한 상품 또는 서비스.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>접수 프로세스의 채점 및 우선 순위 지정.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 부서 목표]</td> 
   <td>부서 내 운영 지표 개선에 중점을 두는 특정 부서만의 목표입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종속성]</td> 
   <td>한 작업이 상태를 변경해야 다른 작업이 상태를 변경해야 하는 두 작업 간의 연결도 상태를 변경할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종속성 유형]</td> 
   <td> <p>작업과 해당 전임 작업 간의 일정 관계 유형. 예를 들어 [!UICONTROL Finish-Start]가 있습니다. 두 번째 작업을 시작하려면 먼저 첫 번째 작업을 완료해야 합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">작업 종속성 유형 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문서]</td> 
   <td>내의 개체에 첨부된 모든 파일 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문서 버전]</td> 
   <td> <p>동일한 문서가 동일한 오브젝트에 업로드될 때마다 버전 번호가 지정됩니다. 사용자는 이전 버전의 문서에 대한 몇 가지 옵션을 보고 변경할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">문서 버전 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 기간]</td> 
   <td> <p>작업 문제 또는 프로젝트 완료에 할당된 시간 창([!UICONTROL 계획 시작]과 계획 완료 사이의 일 수로 결정됨).</p> 
    <ul> 
     <li>작업의 경우 기간 유형이 단순하지 않으면 기간은 편집 가능한 필드입니다. 작업의 기간 유형이 단순이거나 작업 제한 사항이 고정 일자이면 기간은 Workfront에서 수행하는 계산입니다.</li> 
     <li>문제의 경우 기간은 항상 편집 가능한 필드이며 문제를 해결해야 하는 예상 일 수를 나타내야 합니다.</li> 
     <li>프로젝트의 경우 기간은 다음에 의해 수행되는 계산입니다. [!DNL Workfront] 그리고 가장 이른 작업의 계획된 시작과 프로젝트에 대한 최신 작업의 [!UICONTROL 계획된 완료] 간의 일 수 차이를 나타냅니다.</li> 
    </ul> <p>작업에 대한 [!UICONTROL Duration]과 [!UICONTROL Planned Duration] 간의 차이에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">작업에 대한 [!UICONTROL Planned Duration] 및 [!UICONTROL Duration] 간의 차이</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 기간(분)]</td> 
   <td>이 필드에는 [!UICONTROL Duration] 필드와 동일한 정보가 일 대신 분 단위로 표시됩니다. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>반복 작업 상위의 [!UICONTROL 작업 세부 사항] 및 [!UICONTROL 작업 편집] 상자에 표시됩니다. 각 반복 작업의 기간을 표시합니다. 반복 작업 만들기에 대한 자세한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>. </p> <p> <span>개별 반복 작업에서 수정된 기간은 이 필드에 표시된 값을 표시하지 않습니다.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 기간 유형]</td> 
   <td> <p>작업을 완료하는 데 필요한 작업이 작업 기간 동안 할당자에게 할당되는 방법을 나타내는 작업 필드입니다. 작업의 [!UICONTROL Duration], [!UICONTROL Work Required]와 할당된 리소스가 작업을 완료하는 데 소비해야 하는 시간 또는 [!UICONTROL Allocation] 간의 관계를 나타냅니다. </p> <p>이 필드는 작업의 [!UICONTROL Details] 탭에 나타납니다. </p> <p>작업의 기간 유형에 대한 옵션은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL 계산된 할당]</li> 
     <li>[!UICONTROL 계산된 작업]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL Duration] 및 [!UICONTROL Duration Type] 개요</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>전원 검색에서 시간을 측정하는 데 사용되는 단위입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>사용자 수와 작업을 완료하는 데 걸리는 시간 사이의 관계입니다. 사용자를 추가하면 작업을 완료하는 데 예약된 총 시간은 감소하지만 작업 기간은 동일하게 유지됩니다. 예를 들어, 작업이 땅콩 덩어리를 포격하는 경우, 더 많은 사람을 추가하면 예정된 시간은 줄어들지만, 일별 기간은 동일하게 유지됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 경과 시간]</td> 
   <td> <p>[!UICONTROL Elapsed time]은 작업의 [!UICONTROL Duration]에 대한 시간 단위입니다. 휴일, 주말 및 휴가를 포함하는 작업의 [!UICONTROL 계획된 시작 일자]와 [!UICONTROL 계획된 완료 일자] 사이의 시간입니다. 즉, 경과 시간은 역일이 경과된 때이다. </p> <p>[!DNL Workfront] 은 작업 기간에 대해 다음과 같은 경과 시간 단위를 지원합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 경과 시간(분)]</p> </li> 
     <li> <p>[!UICONTROL 경과 시간]</p> </li> 
     <li> <p>[!UICONTROL 경과 일수]</p> </li> 
     <li> <p>[!UICONTROL 경과 주]</p> </li> 
     <li> <p>[!UICONTROL 경과 월]</p> </li> 
    </ul> <p>경과 시간을 포함한 작업 기간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL Duration] 및 [!UICONTROL Duration Type] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종료 날짜]</td> 
   <td> <p> [!UICONTROL 요금] 보고서에서 프로젝트 수준의 작업 역할에 대한 새 청구 요금이 종료되는 날짜입니다. 이 일자 이전의 프로젝트와 연계된 시간에 이 청구 요금을 곱하여 프로젝트의 수익을 계산합니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 참여]</td> 
   <td>작업, 프로젝트, 팀 또는 조직에 대한 헌신과 믿음이 줄어드는 시기를 나타내는 [!UICONTROL 작업 성과 지표](WPI)입니다. 이것은 여러분이 그 믿음과 헌신을 되살리기 위해 행동해야 한다는 것을 나타냅니다. WPI는 다음과 같은 간단한 질문을 통해 측정됩니다. "기대했던 바를 이해했습니까? 네가 맡은 일이 조직에 영향을 미쳤니? 일을 잘하셨습니까?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>회사 목표 지표에 기여하는 다양한 분야의 목표.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트]</td> 
   <td>프로젝트 또는 작업의 모든 변경 사항.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 핸들러]</td> 
   <td>이벤트가 발생할 때 발생하는 자동화된 작업. 일반적인 예로는 자동화된 이메일 알림이 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 알림]</td> 
   <td>이벤트 처리기에서 생성된 이메일입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>작업 또는 프로젝트에 대한 비인적 비용.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>일반적으로 이는 라이선스 유형 또는 이러한 라이선스를 가진 사용자입니다. 이러한 라이선스 유형을 가진 사용자는 시스템에서 정보를 검토할 수 있는 권한만 갖습니다. 그들은 적극적으로 일에 참여할 수 없다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 외부 시스템]</td> 
   <td>지정된 기록 시스템 외부에 저장되고 관리되는 모든 서비스 또는 소프트웨어.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL 필드]</td> 
   <td><p>모든 Workfront 개체 또는 이 개체와 관련된 정보가 데이터베이스에 나타납니다. </p>
   <p>예를 들어 "project", "user", "hour"는 필드뿐만아니라 Workfront 개체입니다. "Name", "status", "owner", "start date"는 위의 오브젝트와 연결된 Workfront 필드입니다. </p>

<p>개체를 참조할 때 "개체"와 "필드"라는 용어가 서로 교환되어 사용될 수 있습니다.</p>
   <p>보고 범위에서 "필드"는 보고서에 캡처할 객체 또는 객체에 대한 정보를 나타냅니다.</p>

<p><b>메모</b></p>

<p>텍스트 추가 보고에서 필드는 데이터베이스에 나타나는 개체 또는 해당 정보를 참조합니다.</p>
   <p>사용자 인터페이스에 표시되는 이름이 데이터베이스의 필드 이름과 다른 경우가 있습니다. 예를 들어 "issue"는 Workfront 인터페이스에 있는 개체의 이름이지만, "opTask"는 Workfront 데이터베이스에 있는 개체(또는 필드)의 이름입니다. </p> 
   <p> 텍스트 모드 보고서, 보기, 필터 또는 그룹화를 작성할 때 또는 계산된 필드를 만들 때 데이터베이스에 나타나는 필드를 사용하는 것이 중요합니다.</p>

<p>자세한 내용은 <a href="../../../wf-api/general/api-explorer.md">API 탐색기</a> 및 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">텍스트 모드 개요</a>.</p>

<p>기본적으로 Workfront에는 개체와 해당 정보를 정의하는 필드 세트가 함께 제공됩니다. 사용자 정의 필드를 만들어 객체를 정의할 수도 있지만 사용자 정의 객체를 만들 수는 없습니다.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>화면에 표시되는 정보를 정의하는 보고서 또는 목록 요소의 기본 구성 요소 중 하나입니다. 보고 요소에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> <p>필터는 보고서 또는 [!DNL Workfront] 패널 목록(예: 프로젝트, 작업 또는 문제)</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>에서 인건비, 경비 및 수익 데이터를 관리하는 프로세스 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 고정 비용]</td> 
   <td>프로젝트에 대한 고정 금액을 정의할 수 있습니다. 이는 프로젝트를 완료하는 데 필요한 금액을 나타내는 프로젝트의 [!UICONTROL 계획된 비용]의 일부입니다. 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 고정 수입]</td> 
   <td>프로젝트에 대한 고정 수익 금액을 정의할 수 있습니다. 이는 프로젝트를 완료할 경우 가져올 수 있는 금액을 나타내는 프로젝트의 [!UICONTROL 계획된 수익]의 일부입니다. 매출에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 플래그]</td> 
   <td> <p> 이 필드는 [!UICONTROL 상태 아이콘]과 동일하지만 다음 보기에만 사용할 수 있습니다. </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> 자세한 내용은 이 문서 를 참조하십시오. <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더]</td> 
   <td>폴더는 객체와 연관된 문서나 보고서를 구성하는 데 사용됩니다.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE](전시간에 해당)</td> 
   <td>자원이 작업에 사용 가능한 시간을 나타내는 FTE(Full Time Equivalent)입니다. 
   [!UICONTROL FTE] 필드는 다음 영역에 표시됩니다. 
  <ul>
   <li> 사용자 프로필(사용자 편집 또는 생성 시) </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner](Workfront Scenario Planner에 추가 라이센스 필요) </li>
   <li> 사용자 목록 및 보고서 </li> </ul>

<p>[!UICONTROL FTE]은(는) 최대 1의 십진수여야 하며 0일 수 없습니다. </p>
   <p> [!UICONTROL FTE]가 1이면(프로필에 정의된 대로 사용자의 [!UICONTROL FTE] 필드에 대한 기본값임) 리소스(사용자 또는 역할)가 가용성을 계산하는 일정을 기반으로 전체 시간을 작동함을 의미합니다. </p>
   <p>Workfront 관리자는 사용자의 가용성을 확인하는 데 사용할 일정을 결정합니다.  </p>
   <ul>
   <li> [!UICONTROL 기본 일정]을 사용하면 Workfront은 프로필에 있는 사용자의 [!UICONTROL FTE]을(를) 사용하여 가용성을 계산합니다. </li>
   <li> 사용자 일정이 사용될 때 Workfront은 사용자의 휴무, [!UICONTROL Work Time] 값 및 [!UICONTROL Default Schedule]의 시간을 사용하여 사용자의 [!UICONTROL FTE]을(를) 계산합니다. </li> </ul>

<p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>.  </p>
   <p>에서 일정 만들기에 대한 자세한 내용은 [!DNL Workfront], 참조 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">일정 만들기</a>. </p>

<p><b>메모</b></p>
   <p>[!UICONTROL Scenario Planner]의 모든 계산에 대해 Workfront은 다음 값을 사용합니다. 1 [!UICONTROL FTE] = 8 시간.</p>
   <p>자세한 내용은 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">[!UICONTROL Scenario Planner] 시작</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 간트 차트]</td> 
   <td> <p>프로젝트의 작업이 현재 예약되어 있을 때 계획된 또는 예상 날짜를 기반으로 하는 달력 보기에서 프로젝트 날짜의 시각적 타임라인입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 목표]</td> 
   <td><p>에는 두 가지 목표 개념이 있습니다 [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>프로젝트 목표</b>: 프로젝트의 관련 이해 관계자가 동의한 비즈니스 목표 세트 프로젝트 목표는 프로젝트의 비즈니스 사례에 포함됩니다. </p> <p>목록 또는 보고서에 프로젝트 목표를 표시할 수 없지만 API를 통해 액세스할 수 있습니다. </p> <p>비즈니스 사례 프로젝트 목표에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">비즈니스 사례 목표 만들기 </a>. </p> </li> 
     <li> <p><b>전략적 목표</b>: 전략적 목표는 특정 기간에 대한 작업 전략을 계획하기 위해 만드는 목표입니다. 다음을 사용하여 이러한 유형의 목표를 생성할 수 있습니다. [!DNL Workfront Goals]. 조직에서 추가 라이선스를 구입해야 하며 전략적 목표를 만들려면 이 기능에 대한 액세스 권한이 있어야 합니다. [!DNL Workfront Goals] 추가 라이선스만 제공됩니다.</p> 
     <p>자세한 내용은 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>. </p> 
     <p>목표 또는 프로젝트 보고서에 전략적 목표를 표시하고 API를 통해 해당 목표에 액세스할 수 있습니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 목표 계층]</td> 
   <td> <p>[!UICONTROL Goal] 및 [!UICONTROL Project] 보고서에서 이 필드는 다른 목표에 맞춰질 때 전략 목표가 속한 계층의 목표를 표시하는 컬렉션 필드입니다. 목표는 ▸ 구분 기호로 구분됩니다. </p> <p>이 필드에는 목표와 목표의 부모만 표시됩니다. 하위 목표는 표시되지 않습니다. </p> <p>의 목표 정렬에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">의 목표 정렬 개요 [!DNL Workfront Goals]</a>. </p> 
   <p>이 필드는 조직이 를 구입한 경우에만 볼 수 있습니다. [!DNL Workfront Goals]. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 목표 성공 점수]</td> 
   <td> [!UICONTROL 프로젝트 보고서]에서 이 필드는 [!UICONTROL Business] 사례와 관련된 프로젝트 수준 목표를 참조하는 데 사용됩니다. 현재 더 이상 사용되지 않는 필드이며 기능과 연결되어 있지 않습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 목표] </td> 
   <td> <p>[!UICONTROL 프로젝트] 보고서에서 이 필드는 프로젝트와 관련된 모든 전략적 목표를 표시하는 컬렉션 필드입니다. 목표는 쉼표로 구분됩니다.</p> <p>이 필드는 조직이 를 구입한 경우에만 볼 수 있습니다. [!DNL Workfront Goals]. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. 의 전략적 목표 및 프로젝트 목표에 대한 자세한 내용 [!DNL Workfront]이 문서에서 "[!UICONTROL 목표]"를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전역 인터페이스 환경 설정]</td> 
   <td>모든 사용자에게 영향을 주는 인터페이스 설정입니다. [!UICONTROL 사용자 인터페이스 환경 설정]으로 [!UICONTROL 전역 인터페이스 환경 설정]을 덮어쓸 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>동일한 객체에 액세스할 수 있는 사용자 컬렉션(동일한 부서 또는 사업부)입니다. 사용자 외에도 그룹은 포트폴리오, 프로그램, 프로젝트 및<span> 프로젝트 템플릿,</span> 회사, 팀, 일정, 레이아웃 템플릿 및 타임시트 프로필.</p> <p>그룹별로 개체에 대한 권한을 부여할 수도 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> <p>다음 유형 중 하나의 객체 목록 또는 보고서에서 [!UICONTROL 그룹] 필드를 사용하여 특정 그룹과 관련된 해당 유형의 객체를 나열할 수 있습니다. 사용자, 포트폴리오, 프로그램, 프로젝트 <span>프로젝트 템플릿</span>, 회사, 팀, 일정, 레이아웃 템플릿 또는 타임시트 프로필.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 그룹 관리자]</td> 
   <td> <p>객체, 액세스 및 지정된 사용자 그룹의 사용자를 관리하는 사용자입니다.</p> <p> [!UICONTROL 그룹] 보고서에서 이 필드에는 그룹에서 [!UICONTROL 그룹 관리자]로 지정된 사용자 이름이 표시됩니다. 그룹 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>관리 액세스 권한이 있는 [!UICONTROL 그룹]</td> 
   <td> <p> [!UICONTROL 레이아웃 템플릿], [!UICONTROL 타임시트 프로필] 또는 [!UICONTROL 일정 보고서]에서 이 필드에는 그룹 관리자가 템플릿을 수정할 수 있는 액세스 권한을 가진 그룹이 표시됩니다. 이 필드로 이 보고서를 필터링할 수도 있습니다. </p> <p> 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 그룹화]</td> 
   <td> <p>일반 기준으로 목록의 정보를 분류하는 데 사용되는 보고 요소입니다.</p> <p>자세한 내용은 이 문서의 "[!UICONTROL Groupings]" 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전달 날짜]</td> 
   <td> <p>작업을 작업에 사용할 수 있게 되는 날짜입니다. [!UICONTROL 전달 날짜]는 계산이며 수동으로 설정할 수 없습니다. <br>[!UICONTROL 전달 날짜]에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL 작업 전달 날짜] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 도움말 데스크]</td> 
   <td>의 [!UICONTROL Requests] 영역을 설명하는 대체 이름 [!DNL Workfront]. [!UICONTROL 요청] 영역을 사용하여 고객 지원 티켓, 프로젝트 요청, 헬프 데스크 티켓 등을 처리할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소유자]</td> 
   <td>[!UICONTROL Hour] 보고서에서 [!UICONTROL Owner]는 시간이 속하는 사용자입니다. 이는 실제로 시간을 기록하는 사용자와 다릅니다. 이러한 두 엔티티는 경우에 따라 두 명의 서로 다른 사용자가 될 수 있습니다. <br>다른 사용자의 시간 로깅에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">로그 시간</a>.</td> 
  </tr>

<tr> 
   <td>시간 상태</td> 
   <td> <p>사용자가 작업, 문제 또는 프로젝트에 대해 기록하는 실제 시간에 대해 Workfront에서 설정한 속성입니다. </p>

시간 항목은 Workfront에서 다음 상태 중 하나를 가질 수 있습니다.
<ul>
   <li><b>제출됨</b>: 시간이 프로젝트, 작업 또는 문제에 기록되었습니다. 청구 기록에 포함되어 있거나 아직 청구 기록에 추가되지 않았습니다.</li>
   <li><b>승인됨</b>: 시간이 기록되었으며 프로젝트 소유자가 승인했습니다. 청구 기록에 포함되어 있거나 아직 청구 기록에 추가되지 않았습니다.</li> 
   <li><b>승인되지 않음</b>: 시간이 기록되었으며 프로젝트 소유자에 의해 거부되었습니다. 청구 기록에 포함되어 있거나 아직 청구 기록에 추가되지 않았습니다.</li>
   <li><b>청구됨</b>: 시간이 기록되어 청구 기록에 추가되고 청구 기록 상태가 청구됨으로 표시되었습니다. 프로젝트 소유자의 승인이 필요하지 않았습니다.</li>
   <li><b>청구됨 및 승인됨</b>: 시간이 기록되고 프로젝트 소유자가 승인했으며 청구 기록 상태가 청구됨으로 표시되었습니다.</li>
   </ul>


<p>시간이 청구 기록의 일부인 경우 시간 상태는 시간이 승인되었는지 또는 시간이 속한 청구 기록이 청구되었는지 여부를 나타냅니다. 시간 항목의 시간 상태는 시간 목록 또는 보고서에만 표시됩니다. </p>

<p>청구 기록에 시간을 추가하는 방법에 대한 자세한 내용은 문서의 "청구 기록에 시간 추가" 섹션을 참조하십시오 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >청구 기록 만들기</a>.</p>

<p>프로젝트 시간 승인에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >프로젝트 승인 시간 필요</a>.</p>

<p><b>팁</b></p>

<p>작업 항목에 직접 기록되지 않는 일반 시간은 시간 상태를 표시하지 않습니다. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL 시간 유형]</td> 
   <td> <p>사용자가 작업, 문제 또는 프로젝트에 대해 기록하는 실제 시간에 대해 설정할 수 있는 속성입니다. [!UICONTROL Vacation] 및 [!UICONTROL Time Off]와 같이 작업에 직접 연결되지 않은 기록된 시간에 대한 속성이기도 합니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">시간 유형 관리</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID는 의 모든 오브젝트와 연결된 영숫자 표시기입니다. [!DNL Workfront]. 에서 각 개체를 고유하게 식별합니다 [!DNL Workfront] 데이터베이스. 보고서나 목록에 있는 각 객체의 ID를 볼 수 있습니다. </p> <p><b>팁</b></p>   <p>개체 페이지의 URL에서 ID를 볼 수도 있습니다. 예를 들어 [!UICONTROL 프로젝트 세부 사항] 페이지에 액세스하면 프로젝트 ID가 다음 URL에 요약된 번호와 비슷하게 보일 수 있습니다.</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 개별 목표]</td> 
   <td>팀 목표의 지표에 기여하지만 개인 또는 경력 개발과 관련이 없는 개인 목표.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 상속 액세스]</td> 
   <td>액세스 권한이 객체에서 다른 객체로 전파될 수 있도록 하는 공유 기능입니다. 예를 들어 프로젝트 사용자의 프로그램 및 포트폴리오 레코드에 정의된 액세스 권한 상속</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>다음에서 [!DNL Workfront Scenario Planner]를 통해 플랜을 보다 쉽게 관리할 수 있도록 플랜을 여러 개의 이니셔티브로 나눌 수 있습니다. <span>[!UICONTROL Initiative] 보고서를 작성하고 [!UICONTROL Project] 보고서의 [!UICONTROL Initiative] 정보에 액세스할 수 있습니다.</span></p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>다음 [!DNL Initiative] 보고서가 다음에 표시되지 않음 [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스. API를 통해 [!UICONTROL Initiatives]에 액세스할 수 없습니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 이니셔티브 작업 역할]</span> </td> 
   <td> <p><span>[!UICONTROL 이니셔티브 작업 역할] 보고서 유형은에서 계획 이니셔티브와 연관된 작업 역할에 대한 정보를 표시합니다. [!DNL Workfront Scenario Planner].</span> </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p><span>이 보고서 유형은 다음에 표시되지 않습니다. [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 이니셔티브 작업 역할 시간]</span> </td> 
   <td> <p><span> [!UICONTROL 이니셔티브 작업 역할] 보고서에서 이니셔티브의 작업 역할과 연관된 시간 수를 표시합니다.</span> </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>이 필드와 [!UICONTROL 이니셔티브 작업 역할] 보고서 유형은 [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이니셔티브 작업 역할 수]</td> 
   <td> <p>[!UICONTROL 이니셔티브 작업 역할] 보고서에서 이니셔티브와 연관된 특정 작업 역할의 수를 표시합니다.</p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>이 필드와 [!UICONTROL 이니셔티브 작업 역할] 보고서 유형은 [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이니셔티브 마지막 게시 날짜]</td> 
   <td> <p>계획 이니셔티브가 프로젝트에 마지막으로 게시된 날짜를 표시하는 [!UICONTROL 이니셔티브], [!UICONTROL 이니셔티브 작업 역할] 및 [!UICONTROL 프로젝트] 보고서의 필드입니다. 이니셔티브를 게시하여 프로젝트를 만들거나 이니셔티브에 연결된 프로젝트를 업데이트할 수 있습니다.</p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p><span>이니셔티브 게시에 대한 자세한 내용은</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">에서 프로젝트를 만들고 업데이트하기 위한 시나리오 게시 [!DNL Workfront Scenario Planner]</a>. 이 필드는 다음 위치에 표시되지 않습니다. [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 인라인 검색]</td> 
   <td>한 개의 특정 필드에 대해 가능한 항목을 찾기 위해 양식을 완료하는 과정에서 수행된 검색입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 인터페이스 설정]</td> 
   <td>사용자 지정 보기, 필터, 그룹화, 목록 컨트롤 등을 정의할 수 있는 응용 프로그램 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL이 회사 목표]</p></td> 
   <td> <p>위치 [!DNL goal reports], 조직이 목표에 그 소유자로 지정되었는지 여부를 나타내기 위해 각 전략 목표에 대한 "[!UICONTROL True]/ [!UICONTROL False]" 값이 표시됩니다. </p> 
   <p>이 필드는 조직이 를 구입한 경우에만 볼 수 있습니다. [!DNL Workfront Goals]. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 문제]</td> 
   <td> <p>일반적으로 작업 또는 프로젝트의 완료를 방해하는 데 문제가 있음을 나타내는 계획되지 않은 작업 항목입니다. 추가 작업 노력 고려를 위해 평가되고 평가됩니다.</p> <p>[!UICONTROL Issue]는 [!UICONTROL 헬프 데스크] 요청일 수도 있습니다. [!UICONTROL Change Orders], [!UICONTROL Requests] 및 [!UICONTROL Bugs]도 [!UICONTROL Issues]입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 문제 관리]</td> 
   <td> <p>문제 유형의 정의와 각 유형과 연관된 라우팅, 분류 또는 트래픽 프로세스를 제어하는 프로세스 및 규칙입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 문제 소유자]</td> 
   <td>문제 평가 및 완료를 담당하는 팀 또는 사용자입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 반복]</td> 
   <td>팀이 사전 정의된 산출물 세트를 생성하는 기간.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업 역할]</td> 
   <td> <p>사용자의 일상적인 직무 기능 및 책임을 식별하는 데 사용됩니다. 작업 역할을 작업 항목에 할당하여 특정 사용자에게 할당하지 않고 작업 프로세스를 완료하는 데 필요한 기술을 식별할 수 있습니다. </p> <p>사용자는 두 개 이상의 역할을 가질 수 있습니다. 예를 들면 그래픽 디자이너 또는 컨설턴트가 있습니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL 저널 게시물]</p> </td> 
   <td> <p>프로젝트, 작업, 문제 및 기타 개체의 [!UICONTROL Updates] 영역에 나타나는 추적된 필드의 시스템 업데이트에 대한 정보를 알려주는 보고 가능한 개체입니다.</p> <p>자세한 내용은 다음을 참조하십시오. <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL 업데이트] 영역에 대한 보고서</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban 플래그]</td> 
   <td> <p>[!UICONTROL Task] 보고서 또는 [!UICONTROL Issue] 보고서에서 [!UICONTROL Kanban Flag] 필드는 [!UICONTROL Kanban 보드]의 스토리에 설정된 플래그 상태를 표시합니다. 가능한 값은 [!UICONTROL On Track], [!UICONTROL Ready to Pull] 및 [!UICONTROL Blocked]입니다.</p> <p>[!UICONTROL Kanban story board]의 스토리에 플래그 상태를 설정하는 방법에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">[!UICONTROL Kanban 보드]의 스토리에 플래그 사용</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>기업이 주요 비즈니스 목표를 얼마나 효과적으로 달성하고 있는지 입증하는 측정 가능한 가치.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지연]</td> 
   <td>전임 작업의 [!UICONTROL 계획된 완료 일자] 이후 종속 작업이 시작될 수 있을 때까지 경과해야 하는 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지연 유형]</td> 
   <td> <p>[!UICONTROL Lag]를 계산하는 방법입니다. 다음과 같을 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 일수] (근무일)</li> 
     <li>[!UICONTROL 캘린더 일](휴일 무시)</li> 
     <li>[!UICONTROL 백분율]</li> 
     <li>[!UICONTROL 요일]</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">지연 유형 개요</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL 큰 썸네일]</td> 
   <td> <p> [!UICONTROL Document] 목록 또는 보고서에서 문서의 미리보기를 썸네일에 표시합니다. </p> <p>선택 <strong>[!UICONTROL 큰 썸네일]</strong> 보고서에서 400픽셀 폭의 축소판을 봅니다.</p> <p>축소판 크기는 목록 또는 보고서에서 열의 너비를 수정할 때 조정됩니다.</p> <p>이 문서에서 "[!UICONTROL Thumbnail]"도 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 10명 뷰어]</td> 
   <td> <p>보고서 목록에서 이 필드에는 가장 최근에 보고서를 본 최대 10명의 사용자 이름이 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 상태 메모]</td> 
   <td> <p>이 필드에는 객체 소유자가 객체에 대해 마지막으로 입력한 갱신이 표시됩니다. 이것은 객체에 대한 소유자의 가장 최근 활동이나 상호 작용입니다.</p> <p>다음 [!DNL Last Condition Note] 개체의 마지막 메모의 메모 텍스트가 삭제된 경우 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 재무 업데이트 날짜]</td> 
   <td>[!UICONTROL 프로젝트] 보고서에서 이 필드는 프로젝트 재무 상태가 마지막으로 계산되고 업데이트된 날짜와 시간을 캡처합니다. 프로젝트 재무 정보에 대한 내용은 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">프로젝트 재무 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 메모]</td> 
   <td> <p>이 필드에는 사용자가 객체에 마지막으로 입력한 업데이트가 표시됩니다. 객체에 대한 가장 최근 활동 또는 상호 작용입니다.</p> <p>개체의 마지막 메모 텍스트가 삭제된 경우 [!UICONTROL 마지막 메모] 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다.</p>
   <p>이 필드를 [!UICONTROL 작업] 보고서에 추가하면 하위 개체에 남아 있는 모든 업데이트(예: 문제, 하위 작업, 문서 등)가 — 작업이 이 열에 표시되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 조회자]</td> 
   <td> <p>보고서 목록에서 이 필드에는 보고서를 마지막으로 본 사용자에 대한 정보가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막으로 본 날짜]</td> 
   <td> <p>보고서 목록에서 이 필드에는 보고서가 마지막으로 표시된 날짜가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 레이아웃 템플릿]</td> 
   <td>지정된 사용자의 작업 공간에 표시되는 탭과 보고서를 식별하기 위해 시스템 관리자 또는 그룹 관리자가 정의합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레이아웃 유형]</td> 
   <td>[!UICONTROL 사용자 지정 보기]와 함께 [!UICONTROL 레이아웃 유형]은 [!UICONTROL 사용자 지정 보기]의 유형을 지정합니다. 현재는 목록만 사용할 수 있습니다. 나중에 [!UICONTROL 세부 사항](개체의 [!UICONTROL 세부 사항] 보기)을 사용할 수 있게 됩니다.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이브러리 작업]</td> 
   <td>응용 프로그램에서 [!UICONTROL Tasks] 및 [!UICONTROL Template Tasks]의 이름을 일관되게 지정하는 데 사용되는 단일 작업의 템플릿입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이선스 유형]</td> 
   <td>[!UICONTROL 액세스 수준]에 할당된 라이선스 유형입니다. [!UICONTROL Full User], [!UICONTROL Limited User] 또는 [!UICONTROL Requester]입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이선스 제한 계획]</td> 
   <td> <p>[!UICONTROL 그룹] 보기 또는 보고서에서 이 필드는 해당 그룹이 [!UICONTROL 홈 그룹]으로 지정된 사용자에게 할당할 수 있는 최대 [!UICONTROL 계획] 라이선스 수를 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이선스 제한 작업]</td> 
   <td> <p>[!UICONTROL 그룹] 보기 또는 보고서에서 이 필드는 해당 그룹이 [!UICONTROL 홈 그룹]으로 지정된 사용자에게 할당할 수 있는 최대 [!UICONTROL 작업] 라이선스 수를 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>을(를) 생성할 수 있는 라이선스 유형 [!DNL Access Level] 문제를 제출하고, 메모를 입력하고, 문서를 업로드할 수 있는 보기 전용 권한이 포함된 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 목록 컨트롤]</td> 
   <td> <p>사용자 지정 필터, 보기 및 그룹화를 개별 사용자에게 연결하거나 모든 사용자에게 전역적으로 연결할 수 있는 [!UICONTROL 인터페이스 설치]의 일부입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>[!UICONTROL Project]의 [!UICONTROL 업데이트 유형] 중 하나입니다. 이 설정을 사용하면 "[!UICONTROL Recalculated Timelines]"를 클릭할 때만 [!UICONTROL Project Projected] 및 [!UICONTROL Planned] 타임라인을 업데이트할 수 있습니다. 이렇게 설정된 프로젝트는 야간 재계산 프로세스 중 및 프로젝트의 작업이 업데이트될 때 무시됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 [!UICONTROL 업데이트 유형] 선택 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>현재 로그인한 사용자를 나타냅니다. </p> <p>다른 사용자와 공유할 때 보고서를 더 일반적으로 만들려면 필터에서 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 항상 정보가 사용자 지정되므로 로그인하는 사용자에 따라 서로 다른 정보를 표시하는 보고서만 만들 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최대 사용자]</td> 
   <td> <p>사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이(가) 제거되어 필드를 업데이트할 수 없습니다. </p> <p>의 이전 릴리스에서 [!DNL Workfront], 작업 역할을 만들거나 편집할 때 이 필드를 업데이트할 수 있습니다. 각 프로젝트의 역할과 연결할 수 있는 총 사용자 수를 표시합니다. 프로젝트에서 할당할 수 있는 사용자 수에 제한이 없는 경우 값 0이 허용됩니다. </p>일부 보고서와 목록에는 여전히 필드가 표시되지만 표시된 정보를 업데이트할 수 없습니다. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 이정표]</td> 
   <td> <p>작업이 완료되었을 때 프로젝트의 키 포인트가 달성되었음을 나타내기 위해 작업과 연결할 수 있는 마커입니다. 일반적으로 이정표를 사용하여 프로젝트의 단계 또는 중요한 활동 세트와 같은 중요한 이벤트를 표시할 수 있습니다. [!UICONTROL 이정표]는 일반적으로 상위 작업과 연결됩니다. 작업에 마일스톤을 첨부하려면 먼저 마일스톤을 만들어야 합니다. 이정표에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">마일스톤 경로 만들기</a> 및 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">작업과 마일스톤 연결</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마일스톤 경로]</td> 
   <td>[!UICONTROL 이정표] 컬렉션. [!UICONTROL 마일스톤 경로]는 프로젝트에서 특정 유형의 [!UICONTROL 마일스톤]이 있는 프로젝트와 다른 세트의 [!UICONTROL 마일스톤]이 있는 프로젝트를 구별하는 데 사용됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 마일스톤 작업]</td> 
   <td>측정할 보고 가능한 이벤트를 나타내도록 플래그가 지정된 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>의 시나리오 내에서 한 단계 [!DNL Workfront Fusion] 연결된 앱을 기반으로 일부 기능을 수행합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 내 기본 역할]</td> 
   <td> <p>필터에서 참조되는 경우 로그인한 사용자와 동일한 [!UICONTROL 기본 역할]을 가진 사용자 또는 로그인한 사용자의 [!UICONTROL 기본 역할]에 할당된 작업 항목이 표시됩니다.</p> <p>다른 사용자와 공유할 때 보고서를 더 일반적으로 만들려면 필터에서 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 항상 정보가 사용자 지정되므로 로그인하는 사용자에 따라 서로 다른 정보를 표시하는 보고서만 만들 수 있습니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 내 홈 팀]</td> 
   <td> <p>필터에서 참조되는 경우 이 필드에는 로그인한 사용자의 [!UICONTROL 홈 팀]에 속한 사용자나 로그인한 사용자의 [!UICONTROL 홈 팀]에 할당된 작업 항목이 표시됩니다. </p> <p>다른 사용자와 공유할 때 보고서를 더 일반적으로 만들려면 필터에서 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 항상 정보가 사용자 지정되므로 로그인하는 사용자에 따라 서로 다른 정보를 표시하는 보고서만 만들 수 있습니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 명명 규칙]</td> 
   <td>데이터를 사용하여 프로젝트, 작업 및 결과물의 이름을 생성하는 조직 전체의 규칙 세트입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 기본 통합]</td> 
   <td>수동 코딩 또는 API 구성이 필요 없는 통합입니다. 또한 "기본 제공" 통합이라고도 합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 탐색 메뉴]</td> 
   <td>[!UICONTROL Workfront]의 기본 영역에 대한 링크가 있는 애플리케이션의 위쪽 가운데 패널입니다.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>[!UICONTROL Journal Entry] 보고서에서 [!UICONTROL Old Number Value]을(를) 대체하는 필드의 업데이트된 값이 표시됩니다.
   자세한 내용은 이 문서의 "[!UICONTROL Old Number Value]"를 참조하십시오.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL 청구 불능 경비]</td> 
   <td> <p>고객에게 청구 가능으로 표시되지 않은 비용. 이는 계획된 비용이거나 실제 비용일 수 있습니다.</p> <p>뷰 및 보고서에 추가할 수 있는 계획된 청구 불가능한 비용 및 실제 청구 불가능한 비용 필드를 사용할 수 있습니다. 프로젝트 또는 작업 세부 정보 페이지에는 표시되지 않습니다.</p>
   <p>다음 유형의 보고서에서 이러한 필드를 찾을 수 있습니다.</p>
   <ul>
   <li>기준선</li>
   <li>템플릿</li>
   <li>프로젝트(재무 데이터)</li>
   </ul>
   <p>경비를 청구 가능 경비로 표시하는 방법에 대한 자세한 내용은 다음을 참조하십시오. <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">프로젝트 경비 관리</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL 비근무일]</td> 
   <td>할당 완료에 할당되지 않은 날짜. 일반적으로 휴가일, 휴일 또는 주말입니다. API 탐색기에서 용어 표시. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참고]</td> 
   <td>에 대한 댓글 또는 업데이트 [!DNL Workfront] 개체.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 메모 텍스트]</td> 
   <td> <p>모든 객체에 대해 사용자가 입력한 업데이트 텍스트가 표시됩니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 연결된 목표 수]</td> 
   <td> <p>[!UICONTROL Project] 보고서에서 이 수는 프로젝트와 관련된 전략적 목표의 수입니다. 프로젝트를 전략적 목표와 연관시키는 방법에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">의 목표에 프로젝트 추가  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>전략적 목표에 대한 자세한 내용은 이 문서의 "[!UICONTROL 목표]"도 참조하십시오.</p> 
   <p>이 필드는 조직이 를 구입한 경우에만 볼 수 있습니다. [!DNL Workfront Goals]. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!UICONTROL Adobe Workfront 목표]의 목표에 프로젝트 추가</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 개체]</td> 
   <td> <p>표시되는 정보 [!DNL Adobe Workfront] 는 다음에 저장된 개체로 표시됩니다 [!DNL Workfront] 데이터베이스. 개체는 Workfront의 정보를 유도하는 요소입니다. 객체의 몇 가지 예는 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 문서]</li> 
     <li>[!UICONTROL 대시보드]</li> 
     <li>[!UICONTROL 보고서]</li> 
     <li>[!UICONTROL 그룹]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL 사용자]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL 사용자 정의 양식]</li>
     <li>[!UICONTROL 사용자 정의 필드]</li>  
     <li>[!UICONTROL 시간]</li> 
     <li>[!UICONTROL 청구 요금]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL 템플릿 작업]</li>

<p><b>메모</b></p>
  <p>이 목록은 광범위하지 않습니다. </p>

</ul> <p>자세한 내용은 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">[!UICONTROL Adobe Workfront]의 개체 이해</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 개체 유형]</td> 
   <td>모든 사용자 정의 양식이 포함된 보고서나 목록을 만드는 경우 이 필드를 보기 또는 필터로 사용하여 각 양식과 연결된 개체 유형을 확인할 수 있습니다. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>[!UICONTROL 분개 기입] 보고서에서 필드의 원래 값이 업데이트되기 전에 표시됩니다. 필드의 값이 업데이트되면 [!UICONTROL Journal Entry] 보고서에 [!UICONTROL New Number Value](으)로 표시됩니다. 자세한 내용은 "[!UICONTROL New Number Value]"도 참조하십시오.</td> 
  </tr>
  <tr> 
   <td>변경 시에만 [!UICONTROL]</td> 
   <td> <p>[!UICONTROL 프로젝트 업데이트] 유형 중 하나입니다. 이 옵션을 선택하면 프로젝트 또는 프로젝트 내 작업에 대한 업데이트 또는 변경이 수행될 때만 [!UICONTROL Project Projected] 및 [!UICONTROL Planned] 타임라인이 업데이트됩니다. 매일 밤 프로젝트를 업데이트하지는 않습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형 선택 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업]</td> 
   <td> <p>의 [!UICONTROL Issue] 이름입니다. [!DNL Workfront] 데이터베이스, 텍스트 모드 보고서 또는 계산된 사용자 지정 데이터에 사용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>완료되지 않았지만 진행 중인 문제 또는 작업.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조직 차트]</td> 
   <td>조직도의 약어입니다. 조직의 계층 구조를 보여 주는 차트입니다. 또한 [!UICONTROL 사용자]의 [!UICONTROL 회사] 및 [!UICONTROL 보고] 관계를 표시하고 설정할 수 있는 [!UICONTROL 사용자] 세부 정보 화면의 탭에도 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조직 설정]</td> 
   <td>조직의 [!UICONTROL Company], [!UICONTROL Groups] 및 [!UICONTROL Security Profiles]을(를) 정의합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 기타 그룹]</td> 
   <td> <p>사용자를 나열하는 보고서 또는 보기에서 이 필드에는 각 사용자가 구성원으로 있는 모든 그룹이 표시됩니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 통화 재정의]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할과 연결된 통화입니다. 다음을 수행하여 [!UICONTROL Setup] 영역에서 설정된 [!UICONTROL 기본 통화]를 재정의합니다. [!DNL Workfront] 관리자. </p> 
     <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 통화 청구/시간 재정의]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할의 선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 청구 요금입니다.</p> 
     <p> 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 통화 비용/시간 재정의]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할의 선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 비용률입니다. </p> 
     <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 소유자]</td> 
   <td>지정된 객체의 완료를 담당하는 사용자입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 소유자 유형]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 목표] 보고서에 전략적 목표에 할당된 소유자 유형이 표시됩니다. 다음은 목표 소유자 유형입니다.</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL 팀] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>목표 소유자가 조직일 때는 이 필드에 값이 표시되지 않습니다. </p> 
     <p>이를 위해서는 추가 라이센스가 필요합니다. 다음에 대한 정보: [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 개요</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 매개 변수]</td> 
   <td> <p>[!UICONTROL 매개 변수]는 사용자 지정 필드입니다. 시스템의 모든 매개 변수 또는 사용자 지정 필드에 대한 보고서를 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위]</td> 
   <td>보고서에서 이 필드에는 객체의 상위 항목에 대한 정보가 표시됩니다. 예를 들어 [!UICONTROL issue] 보고서에는 문제가 로그된 작업 또는 프로젝트에 대한 정보가 표시될 수 있고, 작업 보고서에는 직접 상위 작업 또는 프로젝트에 대한 정보가 표시될 수 있습니다. 에서 부모가 있을 수 있는 개체에 대한 자세한 내용 [!DNL Workfront]문서의 "상호 종속성 및 개체 계층" 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">의 오브젝트 이해 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위 지연]</td> 
   <td>[!UICONTROL 상위 작업] 시작과 [!UICONTROL 하위 작업] 시작 사이에 경과해야 하는 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위 작업]</td> 
   <td>[!UICONTROL 요약 작업]이라고도 합니다. 하위 작업([!UICONTROL 하위 작업]이라고도 함)이 있는 작업입니다. 상위 작업의 [!UICONTROL Duration], [!UICONTROL Work Required] 및 [!UICONTROL Percent Complete]는 하위 작업에서 계산됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 시간제 리소스]</td> 
   <td>시스템에 정의된 기본 일정보다 용량이 적은 사용 허가된 사용자입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료율]</td> 
   <td> <p>작업, 프로젝트 또는 문제와 관련된 작업의 완료율을 보여 주는 프로젝트, 작업 또는 문제 필드.</p> <p>문제 및 작업 시 이 필드를 수동으로 업데이트할 수 있습니다. </p> <p>프로젝트 및 상위 작업의 경우 이 필드는 모든 작업 작업에서 롤업되므로 수동으로 업데이트할 수 없습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">프로젝트 [!UICONTROL 완료율] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>일반적으로 항목에 대한 작업을 완료하거나 항목을 볼 수 있도록 부여되는, 오브젝트의 사용자에게 부여되는 권한. 다음에 대한 권한을 부여할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL 보고서]</li> 
     <li>[!UICONTROL 대시보드]</li> 
     <li>[!UICONTROL 문서]</li> 
     <li>[!UICONTROL 사용자 지정 Forms]</li> 
     <li>[!UICONTROL 보기]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL 그룹화]</li> 
    </ul> <p>자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">오브젝트에 대한 공유 권한 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획]</td> 
   <td> <p>다음에서 전체 라이선스 유형: [!DNL Workfront] 시스템. 의 모든 기능에 액세스하려면 사용자에게 이 권한이 있어야 합니다. [!DNL Workfront].</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan](위치: [!DNL Scenario Planner])</td> 
   <td> <p>플랜은 를 사용하여 작업할 때 주요 객체입니다. [!DNL Workfront] 시나리오 플래너. 회사의 장단기 미래에 대한 전략을 개략적으로 설명하고 각 상위 수준의 결과를 파악하여 계획에 추가할 수 있습니다. [!DNL Workfront] 시나리오 플래너. </p> <p>표시할 수 없습니다. [!DNL Scenario Planner] 보고서에서 플랜에 액세스할 수 없습니다. [!DNL Workfront] API. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획]</td> 
   <td> <p>어떤 일이 발생하기로 예정된 시간 프레임입니다. 에서 프로젝트, 작업 또는 문제를 만드는 경우 [!DNL Workfront], 계획된 시작 및 종료 날짜와 계획된 시간 프레임을 설정합니다. 이 값은 항목이 완료되는 데 걸리는 시간에 대한 원래 의도 또는 예상치를 나타냅니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 이익]</td> 
   <td>이는 프로젝트 관리자가 프로젝트를 완료하면 조직에 금전적 이익이 발생하는지 여부를 예상하기 위한 수동 입력입니다. 이 값을 지정하는 것은 프로젝트에 대한 [!UICONTROL 비즈니스 사례] 작성의 일부일 수 있습니다. 이 값을 업데이트하려면 프로젝트에 대한 [!UICONTROL 관리] 권한이 있어야 합니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 계획된 예산 시간]</td> 
   <td> <p>[!UICONTROL 예산 시간] 보고서에서 [!UICONTROL Resource Planner]의 프로젝트 또는 [!UICONTROL 작업 역할]에 대한 예산 시간을 표시합니다. </p> <p>[!UICONTROL Resource Planner]에서의 프로젝트 또는 역할 예산 편성에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!UICONTROL Project] 및 [!UICONTROL Role] 보기를 사용하는 [!UICONTROL Resource Planner]의 예산 리소스</a>. [!UICONTROL 예산 시간] 보고서에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">보고서: 예산 시간</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 완료 일자]</td> 
   <td> <p>선택한 날짜로 [!UICONTROL 계획된 완료 일자]를 수동으로 설정할 수 있습니다. [!UICONTROL 계획된 완료 일자]를 설정하지 않은 경우 [!DNL Workfront] 자동으로 설정합니다. 자동으로 설정된 경우 [!UICONTROL 계획된 완료 일자]는 [!UICONTROL 계획된 시작 일자] + [!UICONTROL 기간]입니다.</p> <p>자세한 내용은 다음 문서를 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">[!UICONTROL 계획된 완료 일자] 작업의 개요</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">프로젝트 [!UICONTROL 계획된 완료 일자] 설정</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 비용]</td> 
   <td> <p>프로젝트의 [!UICONTROL 계획된 인건비]와 [!UICONTROL 계획된 경비]의 합계입니다. 프로젝트에 대한 [!UICONTROL 계획된 위험 비용]은 포함되지 않습니다.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 기간]</td> 
   <td> <p>작업의 [!UICONTROL Planned Duration]은 일반적으로 작업의 [!UICONTROL Duration]과 동일합니다. 작업의 [!UICONTROL 계획된 시작] 및 [!UICONTROL 계획된 완료 일자] 간의 일 차이를 나타냅니다. </p> <p>작업에 [!UICONTROL Duration] 유형이 [!UICONTROL Effort Driven]인 경우 작업에 할당하는 리소스 수에 따라 [!UICONTROL Planned Duration]이(가) 작업의 [!UICONTROL Duration]과 다를 수 있습니다. </p> <p>예를 들어 [!UICONTROL Construction Driven]의 [!UICONTROL Duration] 유형이 있는 작업의 [!UICONTROL Duration]이 3일이고 전체 일정이 있는 리소스 하나를 작업에 할당하면 [!UICONTROL Planned Duration]도 3일입니다. 전체 시간 일정이 있는 세 개의 리소스를 동일한 작업에 할당하면 [!UICONTROL Duration]은 3일로 유지되지만 [!UICONTROL Planned Duration]은 1일이 됩니다. [!UICONTROL Planned Duration]은 작업의 [!UICONTROL Planned Start] 및 [!UICONTROL Planned Completion] 날짜도 변경하여 새 [!UICONTROL Planned Duration]을 반영합니다. 그 결과 프로젝트의 타임라인에도 영향을 미칩니다. </p> <p>작업에 대한 [!UICONTROL Duration]과 [!UICONTROL Planned Duration] 간의 차이에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">작업에 대한 [!UICONTROL Planned Duration] 및 [!UICONTROL Duration] 간의 차이</a>.</p> <p>프로젝트 및 문제에는 [!UICONTROL 계획된 기간]이 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 기간(분)]</td> 
   <td> <p>프로젝트 또는 문제의 [!UICONTROL 계획된 기간(분)]은 프로젝트 또는 문제의 [!UICONTROL 기간(분)]입니다. </p> <p>작업에 [!UICONTROL 계획된 기간(분)] 필드가 없습니다. </p> <p>[!UICONTROL 템플릿 작업]에는 작업의 [!UICONTROL 계획된 기간(분)]을 분 단위로 표시하는 [!UICONTROL 계획된 기간(분)] 필드가 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 경비]</td> 
   <td> <p>프로젝트 또는 작업에 대해 기록된 모든 비용에 대한 [!UICONTROL 계획 금액]의 합계입니다.</p> <p><b>예</b></p>
   <p>작업 1의 경비를 만들고 [!UICONTROL 계획된 비용] 필드에 $600.00을 입력하면 이 작업의 [!UICONTROL 계획된 비용]은 $600.00입니다. </p> 
   <p>프로젝트의 경우 [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 계획된 경비]를 계산합니다.</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 시간]</td> 
   <td> <p>이 필드는 [!UICONTROL projects], [!UICONTROL tasks] 및 문제 영역, 프로젝트, 작업 또는 문제에 대한 보고서 및 [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] 및 [!UICONTROL Utilization] 보고서와 같은 리소스 관리 도구에 표시됩니다. </p> <p>프로젝트 소유자가 각 작업 또는 문제를 완료하는 데 걸리는 예상 시간이 표시됩니다. 프로젝트의 경우 일반적으로 프로젝트 작업의 [!UICONTROL 계획된 시간] 롤업입니다. </p> <p>[!UICONTROL 계획된 시간] 필드는 보는 위치에 따라 다른 정보를 표시할 수 있습니다. 계획된 시간에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획된 시간 개요</a>.</p> <p>계획된 시간은 다음 위치에 분 단위로 저장됩니다. [!DNL Workfront] 데이터베이스. 이 필드를 사용하여 계산을 작성할 때 시간이 분으로 표시되는지 고려해야 합니다.<br></p> <p>기본적으로 계획된 시간은 작업 항목 기간 내의 모든 일과 작업에 할당된 모든 자원에 대해 동일하게 분배됩니다. 사용자는 작업 항목에 대한 일일 계획된 시간 수 또는 각 할당자에 대한 개별 계획된 시간을 업데이트할 수 있습니다.</p> <p>이 필드의 업데이트는 프로젝트, 작업 및 문제에 따라 다릅니다. </p> 
    <ul> 
     <li> <p>문제의 경우 이 필드를 수동으로 업데이트할 수 있습니다. 문제 계획 시간이 프로젝트 계획 시간에 추가되지 않습니다. </p> <p><b>팁</b></p> <p>문제 보고서에서 [!UICONTROL 계획된 시간] 필드 중 하나가 [!UICONTROL 작업] 필드로 바뀝니다. 필드에는 문제에 대한 계획된 시간 수가 표시됩니다. 자세한 내용은 이 표의 "work" 또는 "[!UICONTROL Work]" 필드를 참조하십시오. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>작업의 [!UICONTROL Calculated Assignment] 또는 [!UICONTROL Simple]이 작업의 [!UICONTROL Duration Type]인 경우 이 필드를 수동으로 업데이트할 수 있습니다. 이 필드는 다음 방법으로 계산됩니다. [!DNL Workfront] 작업의 [!UICONTROL Duration Type]이(가) [!UICONTROL Calculated Work] 또는 [!UICONTROL Effort Driven]인 경우.<br>[!UICONTROL 작업 기간]에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL Duration] 및 [!UICONTROL Duration Type] 개요</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>프로젝트의 경우 [!DNL Workfront] 프로젝트의 모든 작업에서 모든 계획된 시간을 추가하여 계획된 시간을 계산합니다. </p> </li> 
    </ul> <p><b>팁</b></p> <p>텍스트 모드를 사용하고 추가 필드를 참조하여 [!UICONTROL 프로젝트], [!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에 [!UICONTROL 계획된 시간]을 표시할 수도 있습니다. 자세한 내용은 "<code>work</code>", "[!UICONTROL Work]" 및 "<code>workRequiredExpression</code>이 테이블의 "필드. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 인건비]</td> 
   <td> 
    <p>작업의 경우 사용자 또는 역할의 시간당 요금에 사용자 또는 역할에 할당된 시간을 곱한 값입니다.</p> <p>프로젝트의 경우 모든 작업의 총 [!UICONTROL 계획된 인건비]입니다.</p> <p>사용자 또는 역할 사용 비율은 해당 작업에 대해 선택한 비용 유형에 따라 다릅니다. </p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 수익]</td> 
   <td> <p>작업 및 프로젝트는에서 [!UICONTROL 계획된 수익]에 대한 값을 표시할 수 있습니다. [!DNL Workfront]. [!UICONTROL 계획된 수익]은 프로젝트에서 작업의 [!UICONTROL 계획된 시간]과(와) 관련된 금액을 나타냅니다. 프로젝트의 경우 프로젝트의 [!UICONTROL 고정 수입]도 포함할 수 있습니다. </p> <p>작업의 경우 [!UICONTROL 계획된 시간]과(와) 관련된 매출입니다. 모든 작업의 계획된 시간은 프로젝트 [!UICONTROL 계획된 시간] 계산에 기여하기 위해 프로젝트의 계획된 시간으로 롤업됩니다. </p> 
   <p>[!DNL Workfront] 다음 공식을 사용하여 작업 및 프로젝트에 대한 [!UICONTROL 계획된 수익]을 계산합니다.</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>[!UICONTROL 프로젝트 세부 사항] 영역과 프로젝트 보고서에 표시되는 [!UICONTROL 계획된 수익] 프로젝트는 [!UICONTROL 사용률] 보고서에 표시되는 계획된 수익과 다릅니다. </p> <p>[!UICONTROL 프로젝트 세부 정보] 영역의 [!UICONTROL 계획된 수익]은 프로젝트의 고정 수익과 작업 수익을 반영합니다. [!UICONTROL 활용성 보고서]의 [!UICONTROL 계획된 수익]은 프로젝트의 작업에만 연결된 [!UICONTROL 계획된 수익]을 표시합니다. </p> 
     <p><b>예</b></p>  
      <p>프로젝트에 $20 시간당 비율의 컨설턴트에게 10시간이 할당된 작업이 1개 있고 프로젝트에 $100 [!UICONTROL 고정 수입]이 있는 경우 [!UICONTROL 사용률] 보고서에는 [!UICONTROL 계획 수입](작업의 시간과 연결된 [!UICONTROL 계획 수입])에 대해 $200이 표시됩니다. [!UICONTROL 프로젝트 세부 정보] 섹션에는 작업의 $300([!UICONTROL 계획된 수익] 및 프로젝트의 고정 수익이 표시됩니다. </p> 
    <p>의 수익 추적에 대한 정보 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">청구 및 수익 개요</a>. </p> 
    <p>[!UICONTROL 사용률 보고서의 [!UICONTROL 계획된 수익] 계산에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">자원 가동률 정보 보기 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 위험 비용]</td> 
   <td> <p>프로젝트 발생 확률을 인수분해하는 모든 위험의 총 [!UICONTROL 잠재적 비용]. 이 금액은 프로젝트의 [!UICONTROL 계획된 비용]에 포함되지 않습니다.</p> <p>프로젝트의 [!UICONTROL 계획된 위험 비용]은 다음 공식에 의해 계산됩니다.</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 포털 프로필]</td> 
   <td>에 표시되는 관리자 정의 탭 및 포털 섹션 컬렉션 [!DNL Workfront] 애플리케이션 [!UICONTROL Home] 및 기타 대시보드.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 포털 섹션]</td> 
   <td>대시보드 또는 포털 페이지에 있는 탭의 한 구성 요소. 일반적으로 단일 보고서, 차트, 달력 또는 주요 정보 목록입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 포털 탭]</td> 
   <td>최대 3개의 포털 섹션이 포함된 포털 또는 대시보드의 탭.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>통합 특성이 있는 프로젝트 모음입니다. 이러한 프로젝트는 일반적으로 동일한 리소스, 예산 또는 시간대에 대해 경쟁합니다. Portfolio을 프로그램으로 나누고 Portfolio에 추가하기 전에 프로젝트를 프로그램과 연결할 수 있습니다.</p> <p>포트폴리오에 대한 자세한 내용은 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">의 Portfolio 개요 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 관리]</td> 
   <td>컬렉션 또는 관련 프로그램 및 프로젝트 노력을 관리하는 데 중점을 둔 연습 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 최적화 도구]</td> 
   <td>A [!DNL Workfront] 포트폴리오 내에서 프로젝트를 평가하고 우선 순위를 지정하는 데 도움이 되는 도구입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 소유자]</td> 
   <td>포트폴리오에 대한 우선 순위 지정 및 예산을 담당하는 관련자입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 잠재적 위험 비용]</td> 
   <td>목록 및 보고서에서 찾을 수 있는 프로젝트 필드입니다. 이 보고서는 프로젝트와 관련된 위험이 발생할 경우 이에 대한 잠재적 비용을 보여줍니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">잠재적 위험 비용 계산 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 전임 작업]</td> 
   <td> <p>종속 작업을 완료하기 전에 완료해야 하는 작업입니다. 또한 다른 작업에 대해 [!UICONTROL 종속성]으로 표시된 작업입니다. 전임 작업은 계획자가 다른 작업이 완료된 후 작업을 시작하는 것과 같이 시퀀스 종속성 논리를 설정할 수 있도록 해줍니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">작업 전임 작업 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기본 회사]</td> 
   <td>사용자 설정에 지정된 대로 사용자가 속한 회사입니다. 회사는 프로젝트와 연계될 수도 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기본 담당자]</td> 
   <td><p>[!UICONTROL 기본 담당자]는 문제 작성자이며 다음에 의해 자동으로 지정됩니다. [!DNL Workfront] 다른 사용자가 문제를 만드는 경우. 다음을 보유한 경우 이 필드를 수동으로 업데이트할 수 있습니다. [!DNL Manage] 문제에 대한 권한. 문제에는 기본 담당자가 하나만 있을 수 있습니다.</p> 
   <p>기본 연락처를 변경하면 원래 기본 연락처로 지정된 사용자도 문제에 대한 [!UICONTROL 관리] 액세스 권한을 갖게 됩니다.</p>
   <p>문제를 작업 또는 프로젝트로 전환할 때 문제의 [!UICONTROL 기본 담당자]로 지정된 사용자가 프로젝트 또는 작업의 [!UICONTROL 전환된 문제 작성자]가 됩니다. 문제가 전환된 후 문제의 [!UICONTROL 기본 담당자]가 업데이트되면 [!UICONTROL 전환된 문제 작성자]는 전환이 발생한 순간에 문제의 [!UICONTROL 기본 담당자]로 유지됩니다. 이 문서에서 "[!UICONTROL 전환된 문제 작성자]"도 참조하십시오.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 우선 순위]</td> 
   <td>작업, 문제 또는 프로젝트에 중요한 정도를 지정할 수 있는 값입니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>[!UICONTROL Note] 또는 [!UICONTROL Document]에서 이 옵션을 사용하면 대부분의 뷰어에게 해당 개체가 숨겨집니다. 개인 도움말 요청 대기열의 경우 프로젝트 팀의 사용자만 [!UICONTROL 요청] 영역을 통해 해당 대기열(또는 프로젝트)에 문제를 제출할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로필]</td> 
   <td>사용자 계정에 대한 모든 정보.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 프로그램]</td> 
   <td> <p>잘 정의된 이점을 얻기 위해 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 하위 집합입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 프로그램 관리]</td> 
   <td>프로젝트 간 종속성, 위험, 문제, 요구 사항 및 솔루션을 관리하여 프로그램을 건강하게 유지하고 정의된 프로그램 이점을 얻을 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 프로그램 소유자]</td> 
   <td>프로젝트 목표가 회사 목표에 부합하도록 활동을 감독 및 조직할 책임이 있는 관련자.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 진행률]</span> </td> 
   <td> <p>[!UICONTROL Goal] 보고서에서 전략적 목표가 완료에 얼마나 가까운지 백분율을 표시합니다. 진행률은 숫자로 표시됩니다. 전략적 목표에 대한 자세한 내용은 이 표의 "[!UICONTROL Goal]"을 참조하십시오.</p> <p>이 필드는 조직이 를 구입한 경우에만 볼 수 있습니다. [!DNL Workfront] 목표. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 의 목표에 프로젝트 추가 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 진행 상태]</td> 
   <td> <p>프로젝트, 작업 및 목표 보고서에서 이 필드에는 프로젝트, 작업 또는 전략 목표의 진행 상태가 표시됩니다. 자세한 내용은 다음 문서를 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">프로젝트 진행 상태 개요</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">작업 진행 상태 개요</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">의 목표 진행 및 상태 개요 [!DNL Adobe Workfront Goals]</a> </p>
     <p>다음에 대한 [!UICONTROL Goal] 보고서 및 [!UICONTROL 진행 상태] [!DNL goals] 필드는 조직이 를 구입한 경우에만 표시됩니다. [!DNL Workfront Goals]. 의 전략적 목표에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL 프로젝트]</td> 
   <td> <p>특정 일정 내에 완료해야 하며 특정 예산과 리소스 수를 사용해야 하는 많은 양의 작업입니다. 관리하기 쉽도록 하려면 프로젝트를 일련의 작업으로 나눕니다. 모든 작업을 완료하면 프로젝트가 완료됩니다. 프로젝트 계획에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">프로젝트 계획 개요</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 할당 계획 시간]</td> 
   <td> <p>[!UICONTROL 이니셔티브 작업 역할] 보고서에서 프로젝트의 작업 또는 문제에 할당된 작업 역할과 연관된 [!UICONTROL 계획된 시간] 수를 표시합니다. 이 필드와 [!UICONTROL 이니셔티브 작업 역할] 보고서 유형은 [!DNL Workfront] 귀사에서 를 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Workfront Scenario Planner] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 세부 정보]</td> 
   <td>현재 프로젝트 상태에 대한 세부 정보.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 예산 비용]</td> 
   <td> <p> 목록 및 보고서에 표시되는 프로젝트의 [!UICONTROL 예산 비용]입니다.</p><p>이 문서에서 "[!UICONTROL 예산 비용]"도 참조하십시오.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 프로젝트 관리]</td> 
   <td>프로젝트 생성, 분류 및 이름 지정에 대한 임계값을 제어하는 정책 세트입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 프로젝트 오버헤드]</td> 
   <td>[!UICONTROL Hour] 보고서에서 이 필드는 시간 유형이 [!UICONTROL Project Time]인 기록된 시간에 연결된 재무 정보용으로 예약되어 있습니다. 프로젝트에는 고유한 청구 요금이 있을 수 있으며 한 시간이 프로젝트에 직접 기록되면 해당 요금이 계산에 사용됩니다. 프로젝트 설정을 기반으로 프로젝트의 통화가 다를 수 있으며 해당 시간에 대한 통화 전환이 있을 수 있습니다. [!UICONTROL 프로젝트 오버헤드] 개체는 [!DNL Workfront] 정보를 얻으려면</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 소유자]</td> 
   <td>프로젝트의 범위, 타임라인 및 할당을 관리하는 책임이 있는 사용자. 변경 주문, 재무 변경 및 산출물에 대한 기본 승인자.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 계획]</td> 
   <td>프로젝트 일정을 개발 및 유지 관리하는 프로세스입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 스폰서]</td> 
   <td>각 사용자의 관계가 지정되어야 하는 관련자 프로필입니다. 위치 [!DNL Workfront], 이는 [!UICONTROL 액세스 수준]으로 지정됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 팀]</td> 
   <td> <p>프로젝트에 할당된 사용자 또는 역할의 컬렉션</p> <p>자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">프로젝트 팀 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 추적]</td> 
   <td>프로젝트의 상태 및 범위를 측정하는 데 사용되는 데이터</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예상]</td> 
   <td> <p>작업, 문제 또는 프로젝트의 계획된 시간 및 완료율을 기반으로 한 작업 완료 시점의 예상 타임스탬프입니다.</p> <p>작업, 문제 또는 프로젝트의 날짜 또는 [!UICONTROL Duration]을 나타냅니다. 일반적으로 일부 작업이 이미 완료되었거나 시간이 경과한 후 작업 항목의 수명에 더 적합한 날짜와 기간을 지정합니다. </p> <p>예를 들어 작업의 [!UICONTROL 예상 완료 날짜]는 다음과 같은 날짜입니다. [!DNL Workfront] 은(는) 지금까지 작업에 얼마나 많은 작업이 수행되었는지, 작업에 몇 명이 할당되었는지, 시작일 이후 시간이 얼마나 지났는지 등을 기반으로 작업이 완료될 것으로 예상합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 기한]</td> 
   <td> <p>[!UICONTROL Document Version] 개체가 포함된 보고서([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)의 경우, 이 필드에는 증명 기한의 요일, 날짜, 시간 및 연도가 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 결정]</td> 
   <td> <p>[!UICONTROL Document Version] 개체가 포함된 보고서([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)에서 이 필드는 증명의 결정 상태(보류 중, 변경 필수 또는 승인됨)를 표시합니다</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 이름]</td> 
   <td> <p>[!UICONTROL Document Version] 개체가 포함된 보고서([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)에서 이 필드에 증명 이름이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 페이지]</td> 
   <td> <p>[!UICONTROL Document Version] 개체가 포함된 보고서([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)에서 이 필드는 증명에 포함된 페이지 수를 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 진행 상황]</td> 
   <td> <p>[!UICONTROL Document Version] 개체(예: [!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서)가 포함된 보고서에는 증명의 진행 상태([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Composed], [!UICONTROL Decision Made])가 표시됩니다.</p> <p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">증명 진행 개요</a> 위치: <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">증명 진행 상황 및 상태 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명]</td> 
   <td>이미지, 텍스트 문서, 비디오 또는 대화형 웹 컨텐츠에서 변경해야 하는 컨텐츠에 한 명 이상의 사용자가 표시 및 주석을 다는 검토 프로세스입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>[!UICONTROL Note] 또는 [!UICONTROL Document]에서 이 옵션을 사용하면 다른 사용자 또는 외부 사용자도 해당 오브젝트에 액세스할 수 있습니다 [!DNL Workfront]. [!UICONTROL 도움말 요청 큐]의 경우 [!UICONTROL Public]은 프로젝트에 문제를 제출할 수 있는 모든 사용자가 [!UICONTROL 요청] 영역을 통해 문제를 제출할 수 있음을 의미합니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>조직 내 작업 품질에 대한 인식.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>헬프 데스크 대기열 또는 [!UICONTROL 도움말 요청 대기열]이라고도 합니다. 사용자가 문제를 제출할 수 있도록 [!UICONTROL 요청] 영역에 게시된 프로젝트입니다. 일반적으로 대기열은 [!UICONTROL Bugs], [!UICONTROL Project Requests] 등과 같은 특정 주제에 대해 만들어집니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 큐 속성]</td> 
   <td>이러한 설정은 [!UICONTROL 요청] 영역에 게시되는 프로젝트에 대한 문제 제출 규칙을 정의합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대기열 주제]</td> 
   <td> <p>문제를 제출하는 사용자가 주제를 선택할 수 있도록 하는 [!UICONTROL 도움말 요청 큐]의 속성입니다. 주제는 다음과 같은 작업을 수행할 수 있습니다.</p> 
    <ul> 
     <li>사용자 정의 데이터 양식과 연결되어야 합니다.</li> 
     <li>선택한 항목에 설정된 라우팅 규칙을 통해 문제를 사용자, 역할 또는 팀에 자동으로 할당합니다.</li> 
     <li>선택한 주제에 설정된 라우팅 규칙을 통해 문제를 다른 프로젝트 또는 대기열로 이동합니다.</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">대기열 주제 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>[!UICONTROL 액세스 수준] 보고서에서 [!UICONTROL 액세스 수준]의 [!UICONTROL 등급]을 수동으로 표시할 수 있습니다. 이렇게 하면 다음과 같은 이점이 있습니다. [!DNL Workfront] 관리자: 각 액세스 수준과 연관된 복잡성 수준을 시각적으로 식별합니다. 예를 들어, 더 복잡한([!UICONTROL 계획] 수준) 액세스 수준에 대해서는 더 낮은 숫자를 제공하고 덜 복잡한([!UICONTROL 요청자] 수준) 액세스 수준에 대해서는 더 높은 숫자를 제공할 수 있습니다. 표준 액세스 수준의 등급을 지정할 수는 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 준비]</td> 
   <td> <p>작업 보고서의 이 필드는 [!UICONTROL 애자일] 작업이 백로그에서 [!UICONTROL 준비]로 표시되었는지 여부를 나타냅니다. 이 플래그는 [!UICONTROL Agile] 팀에 할당된 작업인 [!UICONTROL Agile] 작업에만 적용됩니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL 반복 빈도]</td> 
   <td> <p>반복 작업 상위의 [!UICONTROL 작업 세부 사항] 또는 [!UICONTROL 작업 편집] 상자에 표시되는 필드입니다. 반복 작업이 발생하는 빈도입니다. 반복 작업 만들기에 대한 자세한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참조 번호]</td> 
   <td> <p>프로젝트, 작업 및 문제는 생성될 때 고유 참조 번호와 자동으로 연결됩니다. 프로젝트, 작업 또는 문제의 [!UICONTROL Details] 페이지나 목록 또는 보고서에서 [!UICONTROL 참조 번호]를 볼 수 있습니다. </p> <p><b>팁</b><p><br>참조 번호는 항상 고유하므로 두 항목의 이름이 같은 경우 참조 번호를 유추할 수 있습니다. </p> <p>[!DNL Workfront] 시스템 수준에서 순차적 참조 번호를 자동으로 생성합니다. 각 프로젝트, 작업 또는 문제는 시퀀스에서 사용 가능한 다음 번호를 가져옵니다. <br></p> <p>예를 들어 사용자 A가 작업을 생성하는 경우 [!DNL Workfront] 은(는) 참조 번호 100을(를) 작업에 자동으로 할당할 수 있습니다. 사용자 B가 이 직후에 문제를 만들면 [!DNL Workfront] 문제에 참조 번호 101을 지정합니다. 참조 번호는 수동으로 편집할 수 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 거부 문제]</td> 
   <td>프로젝트 또는 작업 보고서에서 프로젝트 또는 작업에 대한 승인이 거부될 때 발생하는 문제입니다. 거부 문제에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">작업 항목에 대한 승인 프로세스 만들기</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 남은 위험 비용]</td> 
   <td> <p>프로젝트의 [!UICONTROL 계획된 위험 비용]과 프로젝트에 대한 모든 위험의 총 [!UICONTROL 실제 비용] 간의 차이를 표시하는 프로젝트 필드입니다. </p> <p>프로젝트에 대한 [!UICONTROL 남은 위험 비용]은 다음 공식을 사용하여 계산됩니다.</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 재계획]</td> 
   <td>문제를 복구하거나 극복하기 위해 프로젝트 날짜 변경. 예를 들어 몇 달 동안 보류된 프로젝트는 정확한 날짜를 반영하도록 재계획해야 합니다. 프로젝트의 날짜 또는 작업의 날짜를 조정하는 수동 작업입니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 보고서]</td> 
   <td>주어진 항목에 대한 정보가 포함된 차트 또는 표 [!DNL Workfront] 객체 및 관련 속성.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>중앙화된 단일 대기열에서 트리거되며 진행 중인 작업 노력과 관련이 없는 문제 유형입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 요청 큐]</td> 
   <td>트래픽 및 분류 프로세스에서 관리되는 문제의 백로그입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 요청 속도]</td> 
   <td>요청을 접수 및 완료하는 데 걸리는 총 작업 주기 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 요청자]</td> 
   <td>일반적으로 라이선스 유형입니다. 요청자 라이선스가 있는 사용자는 시스템에서 발생할 새 작업에 대한 요청을 제출할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>사용자의 개인 시간에 지정된 일수로, 사용자가 작업에 사용할 수 없음을 나타냅니다. "[!UICONTROL 비근무일]"을(를) 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 해결]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 문제를 참조하십시오. </p> <p>보고서에 해결 중 오브젝트를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능 및 해결 중 객체 정보 보기</a> 위치: <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 및 해결 가능한 객체 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 확인]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 프로젝트를 참조하십시오. </p> <p>보고서에 해결 중 오브젝트를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능 및 해결 중 객체 정보 보기</a> 위치: <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 및 해결 가능한 객체 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 해결 작업]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 작업을 참조하십시오. </p> <p>보고서에 해결 중 오브젝트를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능 및 해결 중 객체 정보 보기</a> 위치: <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 및 해결 가능한 객체 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>에 존재하는 사용자 또는 역할 [!DNL Workfront] 및 은(는) 프로젝트 팀, 작업 및 문제에 할당됩니다. 이들은 프로젝트, 작업 또는 문제와 관련된 작업을 완료할 책임이 있습니다. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management]는 가용성에 따라 자원의 사용을 정확하게 예측할 수 있는 엔터프라이즈 도구 세트로서, 수행해야 할 작업이 정시 및 예산으로 완료될 수 있도록 합니다. </p> <p>자원 관리 툴을 사용하여 자원에 대한 장기 용량 및 단기 스케줄링 요구 사항을 계획할 수 있습니다. </p> <p>의 리소스 관리에 대한 자세한 내용 [!DNL Workfront], 참조 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">리소스 관리 시작</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 리소스 관리자 ID]</td> 
   <td><p>프로젝트 보고서에서 특정 리소스 관리자를 찾기 위한 필터를 만들 때 이 옵션을 사용할 수 있습니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 리소스 관리자]</td> 
   <td> <p>프로젝트 보고서 또는 목록 보기에서 이 필드는 프로젝트에서 리소스 관리 활동을 수행하도록 지정된 사용자를 표시하는 정보 필드입니다.  보고서에서 "[!UICONTROL Resource Managers]"를 사용하면 프로젝트의 각 리소스 관리자를 쉼표로 구분한 리소스 관리자 목록이 표시됩니다. 주어진 프로젝트에서 최대 30개의 리소스 관리자를 지정할 수 있습니다.</p> <p>자세한 내용은 이 문서 를 참조하십시오. <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">프로젝트 또는 템플릿에 대한 리소스 관리자 지정 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 리소스 플래너 예산 시간] </td> 
   <td>프로젝트 예산 시간 및 [!UICONTROL 리소스 플래너]에서 프로젝트와 관련된 리소스입니다. 이 문서에서 "[!UICONTROL 예산 시간]"도 참조하십시오. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>고급 [!DNL Workfront] 프로젝트, 작업 역할 또는 사용자 간의 리소스를 보고 관리할 수 있는 도구입니다. 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 리소스 플래너 예산 인건비]</td> 
   <td> <p>리소스 플래너를 사용하여 프로젝트 작업 역할에 대해 예산 책정된 시간과 관련된 비용입니다. </p> <p>이 문서의 "예산 인건비"도 참조하십시오. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL 리소스 풀]</td> 
   <td> <p>리소스 풀은 프로젝트와 연결할 수 있는 사용자 컬렉션입니다. 동일한 리소스 풀의 사용자는 일반적으로 동일한 부서에 속하거나, 유사한 기술 또는 상호 보완적인 기술을 보유하고 있거나, 동일한 예산으로 자금이 조달됩니다. 여러 리소스 풀을 프로젝트 또는 사용자에게 연결할 수 있습니다. 리소스 풀은 프로젝트에만 할당되거나 여러 프로젝트에서 공유할 수 있습니다.</p> 
   <p>리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a>.</p> 
   <p>프로젝트 보고서에서 리소스 풀은 프로젝트와 연결된 모든 풀을 표시합니다. 이 개체는 그룹화에 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>특정 기간 동안 사용 가능한 시간 수와 보고서의 각 사용자에 대해 예약된 시간을 표시하는 보고서. 또한 [!UICONTROL Average Hours Per Day] 및 할당 백분율로도 계산됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>위치 [!DNL Workfront Goals]: 결과는 목표에 대한 진행 표시기입니다. 수동으로 업데이트하는 숫자, 백분율 값 또는 통화 금액일 수 있습니다. 보고서에 결과를 표시할 수 없으며 [!DNL Workfront] API. 활동에 대한 자세한 내용은 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront 목표에서 결과 및 활동 시작</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>작업 또는 프로젝트에 대한 청구 가능 금액. 금액은 시간별, 고정 또는 두 가지 모두를 조합하여 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>수익 유형은 태스크가 수익을 발생시키는 방법을 결정합니다. 일부 예에는 [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly] 및 [!UICONTROL Role Hourly w/Cap]이 있습니다. 의 수익 추적에 대한 정보 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>일반적으로 라이선스 유형입니다. [!UICONTROL Reviewer] 라이센스가 있는 사용자는 시스템에서 작업 항목을 검토하고 승인할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 위험]</td> 
   <td> <p>이는 의 다음 개념을 의미할 수 있습니다. [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>프로젝트의 위험 정도를 나타내는 프로젝트의 필드입니다. 위험 수준에 따라 프로젝트 실행의 우선 순위를 지정할 수 있습니다. 프로젝트는 다음과 같은 위험 수준을 가질 수 있습니다.</p> <p>- [!UICONTROL 매우 낮음]</p> <p>- [!UICONTROL 낮음]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL 높음]</p> <p>- [!UICONTROL 매우 높음]</p> <p>프로젝트에 대해 표시하는 위험 수준은 사용자 지정할 수 없습니다. </p> <p> 프로젝트의 위험 업데이트에 대한 자세한 내용은 문서의 "프로젝트 설정" 섹션을 참조하십시오 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a>. 보고서에 프로젝트의 위험 필드를 표시할 수 있습니다. </p> </li> 
     <li> <p>프로젝트 수명 중에 발생할 수 있는 이벤트로, 프로젝트의 비용, 범위 또는 일정에 대한 잠재적인 영향을 식별합니다. 프로젝트에 대한 잠재적 위험을 정의하고 프로젝트의 비즈니스 사례를 작성할 때 발생할 확률 또는 비용을 연관시킵니다. 프로젝트의 비즈니스 사례에 위험을 추가하는 방법에 대한 자세한 내용은 "프로젝트에 대한 위험 만들기 및 편집"을 참조하십시오. </p> <p>보고서에 [!UICONTROL 비즈니스 사례]에 정의된 위험을 표시할 수 없습니다. 보고서와 목록에는 여러 유형의 위험 비용만 표시할 수 있습니다. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 위험 비용]</td> 
   <td> <p>프로젝트의 위험과 관련된 비용입니다. 다음은 보고서에 표시할 수 있는 프로젝트와 관련된 위험 비용입니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 실제 비용]: 발생한 위험에 대한 실제 비용을 표시하는 위험에 대한 필드입니다. 보고서와 목록 외에도 위험을 편집하거나 만들 때 [!UICONTROL 위험 편집] 상자에서 위험을 찾을 수 있습니다. </p> <p>프로젝트, 작업 또는 문제 비용에 대해서는 이 문서의 "[!UICONTROL 실제 비용]"을 참조하십시오. </p> </li> 
     <li> <p>[!UICONTROL 계획된 위험 비용]: 프로젝트에 대한 모든 [!UICONTROL 잠재적 위험 비용]의 합계를 표시하는 프로젝트의 필드입니다. 이 문서의 "[!UICONTROL 계획된 위험 비용]"도 참조하십시오. </p> <p>잠재적 위험 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">잠재적 위험 비용 계산 </a>. </p> </li> 
     <li> <p>[!UICONTROL 남은 위험 비용]: 모든 위험의 [!UICONTROL 실제 비용] 합계와 [!UICONTROL 계획된 위험 비용] 간의 차이를 표시하는 프로젝트의 필드입니다. 이 문서의 "남은 위험 비용"을 참조하십시오. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 위험 관리]</td> 
   <td>위험을 식별, 완화 및 모니터링하는 프로세스</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 역할]</td> 
   <td>이 문서에서 "[!UICONTROL 작업 역할]"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라우팅]</td> 
   <td>일반적으로 대기열 주제 또는 대기열의 기본 경로(라우팅 규칙)로 인해 문제를 자동으로 할당하거나 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라우팅 규칙]</td> 
   <td>문제를 사용자, 역할 또는 팀에 자동으로 할당하거나 문제를 다른 프로젝트 또는 대기열 주제로 이동하는 프로젝트 및 대기열 주제에 대한 설정입니다. 라우팅 규칙은 일반적으로 도움말 요청 대기열에서 수신 문제를 자동으로 할당하는 데 사용됩니다.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 저장된 검색]</td> 
   <td>검색 기준이 저장된 검색입니다. 저장된 검색을 사용하면 검색 기준을 다시 입력할 필요 없이 동일한 검색을 쉽게 다시 실행할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 시나리오](위치: [!DNL Workfront Fusion]) </td> 
   <td> <p>시나리오는 앱/서비스 간에 데이터를 전송하고 변환하는 방법을 나타내는 일련의 단계(모듈)로 구성됩니다.</p> <p>의 시나리오에 대한 정보 [!DNL Workfront Fusion], 참조 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 시나리오 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario](위치: [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>다음에서 [!DNL Scenario Planner]: 시나리오는 계획의 사본입니다. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 자세한 내용은 [!DNL Workfront Scenario Planner], 참조 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>시나리오 만들기에 대한 내용은 다음을 참조하십시오. <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">에서 계획 시나리오 만들기 및 비교 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 일정]</td> 
   <td>근무 시간을 포함한 주별 근무 일정은 휴일(예: 휴일) 및 예외 일(예: 토요일 근무일)과 결합됩니다. Yiu는 일정을 프로젝트 및 사용자와 연결할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>[!UICONTROL Modified Shift]라고도 합니다. 스케줄에 정의된 정규 주별 근무 시간과 대비하여 예약된 일수. 예를 들어, 월요일부터 금요일까지 근무하도록 일정이 잡힌 토요일은 [!UICONTROL 일정 면제]가 됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예약된 보고서]</td> 
   <td> <p>보고서 보고서를 작성할 때 보고서가 [!UICONTROL 예약된 보고서] 필드를 사용하여 배달되도록 예약된 경우 보고서 일정에 대한 정보를 표시할 수 있습니다. 이 필드에는 글머리 기호 목록에 각 보고서의 각 일정에 대해 하나씩 여러 값이 표시됩니다. 보고서 예약에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">보고서 게재 개요</a>.</p> <p>이 필드는 여러 값을 표시하므로 그룹화에서 사용할 수 없습니다. 필터 또는 보기에서만 액세스할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범위 변경]</td> 
   <td>[!UICONTROL Task Duration] 또는 [!UICONTROL Predecessors]가 변경된 경우와 같이, 활성화된 경우 프로젝트 또는 작업 범위가 변경될 때마다 메모를 생성하는 [!UICONTROL Audit Trail]입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>표시를 위해 사용자 지정 데이터를 구성하기 위해 고유한 헤더가 있는 화면의 영역입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 섹션 구분]</td> 
   <td>섹션 사이의 간격 또는 테두리.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>사용자가 다른 개체가 아닌 시스템의 특정 개체와 상호 작용할 수 있도록 하는 설정입니다. 이 문서에서 "[!UICONTROL 액세스 수준]"도 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 설치]</td> 
   <td>관리자가 시스템 구성 및 환경 설정을 설정할 수 있는 영역입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 심각도]</td> 
   <td> <p>[!UICONTROL 심각도]는 항목이 작업 완료에 미치는 영향을 나타냅니다. 예를 들어 [!UICONTROL 심각도]가 높은 문제는 작업의 완료를 완전히 차단할 수 있지만 [!UICONTROL 심각도]가 낮은 문제는 단순한 미용 문제일 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 문제 심각도 업데이트</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 심각도]</td> 
   <td>이 문서에서 "[!UICONTROL 심각도]"를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 공유]</td> 
   <td>다른 사용자가 의 특정 항목을 보거나 편집할 수 있도록 허용하는 작업 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack 날짜]</td> 
   <td>작업 보기 또는 보고서에서 [!UICONTROL Slack 날짜]에는 작업이 프로젝트의 [!UICONTROL 완료 날짜]에 영향을 미칠 수 있는 정확한 날짜가 표시됩니다. 작업의 [!UICONTROL Slack 날짜]에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">작업 Slack 날짜 개요</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 스마트 할당]</td> 
   <td> <p>사용자에게 작업 또는 문제를 할당할 때, [!DNL Workfront] 작업을 완료할 수 있는 시간 및 프로젝트와의 관계를 기반으로 작업을 완료할 최고의 사용자를 나타내는 권장 사항([!UICONTROL 스마트 할당])을 만듭니다.</p> <p>자세한 내용은 을 참조하십시오. <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">스마트 할당 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>다른 객체의 상위 객체를 나타냅니다. 예를 들어 작업에 첨부된 문서의 이름은 [!UICONTROL Document] 보고서 또는 뷰의 [!UICONTROL Source] 필드에 있고, 프로젝트에 기록된 문제의 이름은 문제 보고서 또는 뷰의 [!UICONTROL Source] 필드에 있습니다. </p> 
   <p>다음 보고서에는 상위 객체에 대한 정보를 볼 수 있는 소스 열이 표시됩니다.</p>
  <ul><li>문제 보고서</li>
    <li>시간 보고서</li>
    <li>문서 보고서 </li>
    </ul>
   <p>사용자에게 문제, 시간 또는 문서의 상위 오브젝트에 대한 권한이 없는 경우 보고서가 표시되도록 구성되었거나 다른 사용자의 액세스 권한과 함께 제공되도록 구성된 경우에도 보고서의 소스 열이 비어 있습니다. </p>
   <p> 보고서에 상위 객체에 대한 정보를 표시하려면 상위 객체에 대한 열을 추가하여 상위 객체의 이름을 표시할 수 있습니다. </p>
    <p>예를 들어 소스 열이 있는 보고서에 다음 중 하나를 추가할 수 있습니다. </p>
    <ul><li>문서 또는 시간 보고서에 대한 프로젝트 이름, 작업 이름 또는 문제 이름 열입니다.</li>
    <li>문제 보고서에 대한 프로젝트 이름 또는 작업 이름 열입니다. </li> </ul>
    자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">다른 사용자의 액세스 권한으로 보고서 실행 및 전달</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 시작 날짜]</td> 
   <td> <p>항목에 대한 작업이 시작되도록 설정된 날짜. 다음 위치에 몇 가지 시작 일자가 있습니다. [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL 계획]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL 예상] </li> 
    </ul> <p>[!UICONTROL 요금 보고서]에서 프로젝트 수준의 작업 역할에 대한 새 청구 요금이 시작되는 날짜입니다. 이 일자 이후의 프로젝트와 연계된 시간에 이 청구 요금을 곱하여 프로젝트의 수익을 계산합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태]</td> 
   <td> <p>작업 항목 또는 전략 목표의 워크플로 위치를 표시하는 데 사용되는 표시기입니다.</p> <p>프로젝트의 경우 [!UICONTROL 상태]는 프로젝트가 다음과 같은지 여부를 나타내는 프로젝트의 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL 보류 중] </li> 
     <li>[!UICONTROL 완료] </li> 
     <li>[!UICONTROL 중단]</li> 
    </ul> <p>프로젝트 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">시스템 프로젝트 상태 목록 액세스</a>.</p>
    <p>작업의 경우 [!UICONTROL 상태]는 작업이 다음과 같은지 여부를 나타내는 작업의 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL 진행 중]</li> 
     <li>[!UICONTROL 완료]</li> 
    </ul> <p>작업 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">시스템 작업 상태 목록 액세스</a></p> <p>문제의 경우 [!UICONTROL 상태]는 이 문제가 다음과 같은지 여부를 나타내는 문제의 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL 진행 중]</li> 
     <li>[!UICONTROL 피드백 대기 중]</li> 
     <li>[!UICONTROL 보류 중]</li> 
     <li>[!UICONTROL 확인됨]</li> 
     <li>[!UICONTROL이 해결되지 않음]</li> 
     <li>[!UICONTROL을 복제할 수 없음]</li> 
     <li>[!UICONTROL 검증 완료]</li> 
     <li>[!UICONTROL 다시 열림]</li> 
    </ul> <p>문제 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록 액세스</a>.</p> 
    <p>전략적 목표의 경우 [!UICONTROL 상태]는 목표가 다음과 같은지 여부를 나타내는 목표의 설정입니다.</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL 초안]</li> 
      <li>[!UICONTROL 비활성]</li> 
      <li>[!UICONTROL 닫힘]</li> 
     </ul> 
     <p>전략적 목표에 대한 자세한 내용은 이 문서의 "[!UICONTROL Goals]" 또는 "[!UICONTROL Goals]"도 참조하십시오. </p> 
     <p>전략적 목표의 경우 이 필드는 조직이 를 구입한 경우에만 표시됩니다. [!DNL Workfront Goals]. 을 사용한 전략적 목표 관리에 대한 정보 [!DNL Workfront Goals], 참조 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태 변경]</td> 
   <td>[!UICONTROL 감사 추적]. 사용자가 프로젝트, 작업 또는 문제의 상태를 변경할 때 메모가 생성됩니다.</td> 
  </tr> 
  <tr> 
   <td>상태 아이콘</td> 
   <td> <p>기본 제공 [!UICONTROL 상태 아이콘] 필드를 보기의 열로 추가하여 다음과 같이 개체에 대한 주요 지점을 보다 명확하게 볼 수 있습니다.</p> 
    <ul> 
     <li>오브젝트에 문서가 첨부되어 있습니다.</li> 
     <li>오브젝트가 승인 프로세스와 연결되어 있습니다.</li> 
     <li>개체에는 연결된 추가 메모가 있습니다.</li> 
     <li>경비는 청구 가능 또는 환급 가능 </li> 
     <li>작업이 중요 경로에 있습니다.</li> 
     <li>사용자가 회사, 팀에 속하거나 다른 시간대에 있습니다. </li> 
    </ul> <p>다음 개체 보기에 [!UICONTROL 상태 아이콘] 필드를 추가할 수 있습니다. </p> 
    <ul> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL 템플릿 작업]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL 문서]</li> 
     <li>[!UICONTROL 사용자]</li> 
    </ul> <p>자세한 내용은 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태 업데이트]</td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 이 필드는 개체 소유자가 '[!UICONTROL 업데이트]' 영역에 제공한 가장 최근 상태 업데이트를 보여줍니다. 프로젝트의 경우 프로젝트 소유자가 작성한 댓글이고, 작업 및 문제의 경우 할당자가 작성한 댓글입니다.</p> 
   <p> 개체의 상태를 업데이트할 때 작성한 주석은 [!UICONTROL 상태 업데이트] 열에 표시되지 않습니다.</p> <p>'[!UICONTROL New],' '[!UICONTROL In Process]' 및 '[!UICONTROL Complete]' 상태를 표시하려면 [!UICONTROL Status] 열을 사용하십시오.</p> <p>상태에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">작업 상태 업데이트</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태]</td> 
   <td>이 문서에서 "[!UICONTROL 상태]"를 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 스토리보드]</td> 
   <td>스토리(애자일 방법론의 작업)의 상태와 완료로 진행되는 방식을 나타내는 차트입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 스토리 시간]</td> 
   <td>스토리의 난이도 또는 복잡성을 측정하는 데 사용되는 지표입니다. 애자일 팀은 시간 또는 점수 중 어느 것을 사용할지 선택할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 스토리 포인트]</td> 
   <td>스토리의 난이도 또는 복잡성을 측정하는 데 사용되는 지표입니다. 애자일 팀은 시간 또는 점수 중 어느 것을 사용할지 선택할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>조직 또는 조직의 작동 방식을 변경하는 장기적인 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>포트폴리오 및 프로그램 전반에서 회사 목표를 측정하고 정렬합니다.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>텍스트 모드 인터페이스를 사용할 때 보고서 열에 사용됩니다. </p>
   <p>다음 <code>[!UICONTROL stretch]</code> 는 보기에서 필요하지 않은 추가 공간을 차지하는 열을 식별하는 데 사용됩니다. 일반적인 사용자를 위한 작업 영역의 사용자 인터페이스 폭은 약 850픽셀이다. 즉, 보기가 850픽셀 중 600픽셀을 차지하는 4개의 열(각각 150픽셀)이 있는 보기입니다. UI에 250개의 추가 픽셀이 있으며, 이 픽셀은 스트레치 비율이 제공된 열에 추가됩니다. </p>
   <p>추가 코드 행을 사용하면 열 스트레치가 적용됩니다. <code>[!UICONTROL usewidths=true]</code> 뷰에 있는 하나 이상의 열에 대해 설명합니다. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL 구독자]</td> 
   <td> <p>프로젝트, 작업 또는 문제를 구독하는 사용자.</p> <p>보고서에서 이 필드를 사용하면 구독자 목록이 표시되고 각 구독자는 쉼표로 구분됩니다.</p> <p>자세한 내용은 이 문서 를 참조하십시오. <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">의 항목 구독 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 요약 작업]</td> 
   <td>이 문서에서 "[!UICONTROL 상위 작업]"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 하위 작업]</td> 
   <td>상위 작업 아래에 있는 하위 작업.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 시스템 거버넌스]</td> 
   <td>시스템의 변경 및 유지 관리를 제어하는 정책 세트</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>서로 다른 컴퓨팅 시스템과 소프트웨어 응용 프로그램을 함께 연결하여 통합된 전체로서 기능하는 프로세스입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업]</td> 
   <td> <p>최종 목표 달성(프로젝트 완료)을 위한 단계로 수행해야 하는 활동.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">작업 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 특성]</td> 
   <td>작업과 연결되고 작업에 대한 특정 세부 정보를 나타내는 기타 필드 또는 개체입니다. 일부 예는 [!UICONTROL 계획된 완료 일자] 및 [!UICONTROL 상태]입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>"[!UICONTROL 제약 조건 유형]" 및 "[!UICONTROL 제약 조건 날짜]"를 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업 관리]</td> 
   <td>작업 생성, 할당, 종료 및 가시성에 대한 임계값을 제어하는 정책 세트</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업 소유자]</td> 
   <td>작업 수행 및 완료 추정을 담당하는 팀 또는 사용자</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 팀]</td> 
   <td> <p>유사한 목표 또는 비즈니스 목표를 위해 작업하는 사용자의 컬렉션입니다. 이러한 사용자는 팀을 작업 항목에 할당하여 일괄적으로 작업 항목에 할당할 수 있습니다.</p> <p>팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>.</p> <p>프로젝트에는 프로젝트의 작업과 관련된 모든 사용자 또는 역할이 포함된 [!UICONTROL 프로젝트 팀]이 있을 수 있습니다.</p> <p>프로젝트 팀에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>프로젝트 템플릿은 가장 반복 가능한 프로젝트에 대한 일반적인 개요입니다. 프로젝트 템플릿을 만들 때 작업, 대기열 주제, 사용자 정의 양식, 문서 또는 승인을 정의하여 새 프로젝트를 만들어야 할 시간을 절약할 수 있습니다. </p> <p>기존 프로젝트에 템플릿을 첨부하거나 템플릿을 사용하여 새 프로젝트를 작성할 수 있습니다. 템플릿에 지정된 모든 정보는 템플릿을 사용하여 생성된 프로젝트로 전송됩니다. </p> <p>템플릿에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">프로젝트 템플릿 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 템플릿 작업]</td> 
   <td>템플릿의 일부인 작업입니다. 템플릿 작업은 템플릿을 사용하여 생성된 프로젝트의 작업이 됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>특정 주제와 관련된 [!UICONTROL Note] 및 회신 컬렉션.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> [!UICONTROL Document] 목록 또는 보고서에서 문서의 미리보기를 썸네일에 표시합니다. </p> <p> 선택 <strong>[!UICONTROL Thumbnail]</strong>  보고서에서 33~66픽셀 너비의 축소판을 봅니다. </p> <p>축소판 크기는 목록 또는 보고서에서 열의 너비를 수정할 때 조정됩니다.</p> <p>이 문서에서 "[!UICONTROL Large Thumbnail]"도 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 휴무]</td> 
   <td>사용자가 프로필에 휴무를 표시했을 때를 보기 위해 [!UICONTROL 휴무] 보고서를 작성할 수 있습니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 타임시트]</td> 
   <td> <p>사용자가 프로젝트, 작업 또는 문제에서 작업한 실제 시간이나 회의 또는 교육과 같이 작업과 관련되지 않은 다른 활동에 소요된 시간을 입력할 수 있는 타임카드. 근무 시간을 입력하는 것 외에도 시간 유형을 사용하여 시간 입력을 정의함으로써 시간이 작업과 관련된 시간인지 또는 간접비 시간에 해당하는지 여부를 나타낼 수도 있습니다. 타임시트에 대한 자세한 내용은 <a href="../../../timesheets/timesheets/timesheets-overview.md">타임시트 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 타임시트 프로필]</td> 
   <td> <p>[!UICONTROL 타임시트 프로필]은 [!DNL Workfront] 를 사용하여 연관된 사용자의 타임시트를 자동으로 생성합니다. </p> <p>각 타임시트가 만들어질 때 각 타임시트에 적용할 여러 설정을 구성할 수 있습니다. 이러한 설정 중 일부는 타임시트를 만드는 빈도(주별, 격주, 월별 두 번 또는 월별), 타임시트의 시작일, 타임시트 승인자, 사용자가 기록된 시간과 연결할 수 있는 사용 가능한 [!UICONTROL 시간 유형] 등입니다.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL 최상위 ID] </td> 
   <td> <p>이 필드에서는 목록이나 보고서의 최상위 수준 그룹과 해당 하위 그룹에 대한 데이터를 식별하고 필터링할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최상위 이름] </td> 
   <td> <p>이 필드를 사용하면 목록 또는 보고서의 [!UICONTROL 보기]에서 최상위 수준 그룹 및 하위 그룹에 대한 데이터를 식별할 수 있습니다.</p> <p>[!UICONTROL 최상위 ID] 필드를 사용하여 이 작업을 수행할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 총 시간]</td> 
   <td> <p>[!UICONTROL 프로젝트 보고서]에서 이 필드에는 마지막으로 프로젝트 재정이 계산된 프로젝트의 모든 시간에 대한 반올림된 합계가 표시됩니다. [!UICONTROL 실제 시간]은 프로젝트에 기록된 정확한 시간을 반영합니다. 일반적으로 [!UICONTROL 실제 시간]은 [!UICONTROL 총 시간]과 일치해야 합니다. [!UICONTROL 총 시간]이 [!UICONTROL 실제 시간] 필드와 다르게 나타나면 프로젝트의 재무 정보를 다시 계산해야 합니다.</p> <p>프로젝트 재무 다시 계산에 대한 자세한 내용은 문서 를 참조하십시오 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">프로젝트 재무 다시 계산</a>.</p> <p>타임시트 [!UICONTROL Standard] 보기에서 이 필드는 타임시트에 표시된 날짜에 대한 항목에 기록된 총 시간을 나타냅니다. 이 기본 제공 보기의 타임시트에 대한 [!UICONTROL 총 시간] 필드는 타임시트 시작 날짜와 종료 날짜 사이의 시간 차이를 동적으로 계산하는 "[!UICONTROL hoursDuration]" 필드를 참조합니다. 사용자가 타임시트의 시간대에서 사용 가능한 시간보다 많은 시간을 기록하는 경우 [!UICONTROL 총 시간] 열을 빨간색으로 표시하는 데 사용됩니다. 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">타임시트의 총 시간 보기</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 추적 모드]</td> 
   <td> <p>작업의 속성입니다. 작업의 예상 타임라인을 업데이트하는 방법과 시기를 결정합니다. For example:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update]를 사용하려면 작업을 수동으로 업데이트해야 합니다. 그렇지 않으면 [!UICONTROL Behind Schedule]이 된 다음 [!UICONTROL Late]이 됩니다.</li> 
     <li>[!UICONTROL 자동 완료]는 기한 또는 [!UICONTROL 계획된 완료 일자]가 지나면 작업을 자동으로 완료합니다.</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">작업 추적 모드 개요</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 트리거]</td> 
   <td>시나리오를 시작하는 이벤트입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 작업]</td> 
   <td>상태가 [!UICONTROL Late], [!UICONTROL Behind Schedule] 또는 [!UICONTROL At Risk]인 불완전한 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 미할당 작업]</td> 
   <td>사용자, 역할 또는 팀에 할당되지 않은 작업.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 업데이트 유형]</td> 
   <td> <p>프로젝트의 예상 타임라인이 다시 계산되는 시기를 결정하는 프로젝트의 설정입니다. [!UICONTROL 업데이트 유형]에는 다음 값이 있을 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 자동 및 변경 시]</li> 
     <li>[!UICONTROL 자동 전용]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형 선택 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>다음에서 생성된 계정 [!DNL Workfront] 사용자가 로그인하여 시스템과 상호 작용할 수 있도록 합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL 사용자 위임]</p> </td> 
   <td> <p>다음을 알려주는 보고 가능한 객체</p> 
    <ul> 
     <li>작업, 문제 및 프로젝트 승인을 위임한 사용자</li> 
     <li>작업, 문제 및 프로젝트 승인이 위임된 사용자</li> 
     <li>위임 시작 및 종료 시기</li> 
    </ul> <p>자세한 내용은 다음을 참조하십시오. <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">사용자 위임 보고서 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 인터페이스]</td> 
   <td>의 모든 시각적 및 대화형 측면 [!DNL Workfront] 응용 프로그램.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 인터페이스 환경 설정]</td> 
   <td>[!UICONTROL 사용자 인터페이스 설치]. [!DNL Workfront] 관리자는 이러한 설정을 변경하여 사용자 인터페이스의 측면을 사용자 지정할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 사용률]</td> 
   <td>지정된 스케줄, PTO 및 현재 작업량을 기준으로 한 사용자 또는 역할의 가용성.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>사용자(리소스)가 할당되거나 초과 할당된 방식을 보여 주는 보고서와 결합된 검색입니다. 이 문서의 "[!UICONTROL 리소스 사용률]"을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>오브젝트 이름</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>총 작업 주기 시간(작업을 완료하는 데 걸리는 시간)과 원래 커밋된 시간(작업 대 커밋 비율)에 작업이 수행되는 빈도를 측정합니다.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 보기]</td> 
   <td> <p>보기는 보고서나 개체 목록의 열을 수정할 수 있는 보고 요소를 나타냅니다.</p> 
   <p> 또한 보기는 액세스 수준이나 해당 객체에 대한 권한 공유 수준에 따라 객체에 대한 정보만 볼 수 있는 사용자의 권한을 의미합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 보기 아이콘]</td> 
   <td> <p> 이 필드는 상태 아이콘과 동일하지만 다음 보기에서만 사용할 수 있습니다. </p> 
    <ul> 
     <li> [!UICONTROL 문서] </li> 
    </ul> <p> 자세한 내용은 이 문서 를 참조하십시오. <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지난 달 조회수]</td> 
   <td> <p>보고서 목록에는 지난 달 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지난 분기 조회수]</td> 
   <td>보고서 목록에는 지난 분기 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >보고서 사용 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>보고서 목록에는 지난 해 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이번 달 조회수]</td> 
   <td> <p>보고서 목록에는 이번 달 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL이 이번 분기 조회수]</td> 
   <td>보고서 목록에는 이 분기 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 올해의 조회수]</td> 
   <td>보고서 목록에는 올해 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 이 문서 를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">보고서 사용 보기</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> 보고서에서 [!UICONTROL 텍스트 모드] 인터페이스를 사용할 때 각 열의 너비를 픽셀 단위로 지정할 수 있는 코드 행입니다. Workfront에서는 각 필드에 대해 제안된 너비를 제공하지만 필드 유형과 형식에 따라 조정할 수 있습니다.
추가 항목을 사용해야 합니다. <code>[!UICONTROL usewidths=true]</code> 열에 지정된 너비를 적용하는 코드 줄입니다. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 텍스트 모드에서 다음 문을 사용하면 프로젝트, 작업 또는 문제의 계획된 시간이 표시됩니다.</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>텍스트 모드 사용에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">텍스트 모드 구문 개요</a>. </p> 
   <p><b>팁</b> 
   <p>문제 보고서에서 [!UICONTROL 계획된 시간] 필드 중 하나를 추가하면 <code>work </code>보고서에 대한 필드. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>두 가지 기본 라이센스 유형 중 하나. [!UICONTROL Plan]보다 적은 액세스 권한을 가지고 있지만 시스템에서 만들고 업데이트할 수 있습니다. 작업 라이선스가 있는 사용자는 [!UICONTROL External], [!UICONTROL Reviewer] 또는 [!UICONTROL Requester] 라이선스 소유자보다 더 많은 권한을 갖습니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> <p>작업은 프로젝트, 작업 또는 문제에 대한 [!UICONTROL 계획된 시간] 수를 의미할 수 있습니다. 자세한 내용은 이 표의 "[!UICONTROL work]" 필드를 참조하십시오. </p> <p><b>팁</b></p> <p> 문제 보고서에서 [!UICONTROL 계획된 시간] 필드 중 하나를 추가하면 <code>work </code>보고서에 대한 필드. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 분석 구조]</td> 
   <td>상위/하위 관계를 기반으로 프로젝트 팀이 실행할 작업의 계층 구조.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 작업 노력] </td> 
   <td> 
    <p>프로젝트 관리자는 [!UICONTROL 계획된 시간] 대신 이 필드를 사용하여 작업을 완료하는 데 필요한 노력을 예상할 수 있습니다. 이 필드는 다음 조건이 충족될 때만 표시됩니다.</p> 
     <ul> 
      <li> <p>작업에 [!UICONTROL Simple Duration Type]이(가) 있습니다. </p> <p><b>팁</b></p> <p> [!UICONTROL 기간 유형] 작업을 다른 유형으로 업데이트하면 이 필드가 숨겨집니다. </p> </li> 
      <li>프로젝트 관리자가 프로젝트의 작업 [!UICONTROL 계획된 시간] 필드를 자동으로 계산하기 위해 [!UICONTROL 작업 노력 사용]을 사용하도록 설정했습니다. </li> 
     </ul> 
     <p>[!UICONTROL 계획된 시간] 대신 [!UICONTROL 작업 노력]을 사용하여 작업 노력을 추정하는 방법에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 노력 개요</a>. </p> 
     <p>작업 보고서와 목록에 이 필드를 표시할 수 있습니다.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 작업 항목]</td> 
   <td> <p>이 필드는에서 작업 또는 문제를 참조합니다. [!DNL Workfront]. </p> <p>[!UICONTROL 작업 항목] 보고서에는 작업과 문제에 대한 정보가 모두 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 혼합]</td> 
   <td>비즈니스를 실행하기 위해 할당된 작업과 비즈니스를 변경하기 위해 할당된 작업의 비율의 [!UICONTROL 작업 성과 지표](WPI). 혼합 WPI를 사용하면 전략에 실제 작업 할당이 적용되었는지 여부를 조직 수준에서 이해할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 리소스]</td> 
   <td>작업 또는 추적 시간을 수신할 수 있는 시스템 담당자의 지정입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 역할 및 책임]</td> 
   <td>지정된 문제, 작업, 프로젝트, 프로그램 또는 포트폴리오의 범위, 실행 및 승인을 관리하기 위한 소유자 및 이해 당사자를 정의합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 SLA]</td> 
   <td>모든 이해 당사자가 동의한 수량화 가능한 지표입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 이해 당사자]</td> 
   <td>작업 요청 결과에 대한 기득권을 가진 사용자 컬렉션.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 터치포인트]</td> 
   <td>관련자 간 커뮤니케이션에 대한 디지털 기록.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 성능 지표] </td> 
   <td> <p>혼합 비율, 용량, 속도, 품질 및 참여</p> <p>WPI는 [!UICONTROL Work Performance Indicator]의 일반 약어입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 프로세스]</td> 
   <td> <p>작업을 수신하고 우선 순위를 지정하고 실행하는 방법입니다. 일반적으로 작업을 실행하는 방식을 "워크플로" 또는 "프로젝트 계획"(날짜, 전임 작업 관계 등이 있는 작업 목록)이라고 합니다. </p> <p>작업 프로세스의 예로는 단일 에셋의 프로덕션 또는 다중 에셋 캠페인의 게재가 있을 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 워크플로우 템플릿]</td> 
   <td>[!UICONTROL Proof Approval] 보고서에서 이 필드에는 증명에 첨부된 모든 워크플로 템플릿이 표시됩니다. 첨부된 템플릿이 없으면 열이 비어 있습니다.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>사용자가 오버헤드를 포함하지 않고 실제 작업에 사용할 수 있는 FTE([!UICONTROL FTE]) 시간의 백분율을 나타냅니다. [!UICONTROL Work Time]은(는) 최대 1의 십진수여야 하며 0일 수 없습니다. 예를 들어, 실제 작업에 대한 20% 가용성은 0.2입니다.</p>
   </p>필드의 기본값은 1이며, 사용자가 전체 [!UICONTROL FTE]를 실제 프로젝트 관련 작업에 사용함을 나타냅니다.  </p>
   <p>시스템은 이 숫자를 사용하여 실제 프로젝트 관련 작업에 대한 사용자의 가용성을 계산합니다. </p>
   <p> 일정 예외 및 휴무는 사용자 용량에도 영향을 줄 수 있습니다. </p>
   <p>Workfront에서 일정을 만드는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">일정 만들기</a>. </p>
    <p>Workfront은 [!UICONTROL 설정] 영역의 리소스 관리 기본 설정에 따라 사용자의 가용성을 계산합니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">리소스 관리 환경 설정 구성</a>. </p> 
   <p>사용자를 편집하거나 만들 때 사용자의 [!UICONTROL Work Time]을 업데이트할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">사용자 프로필 편집</a></p> 
   <b>팁</b> 
   <p>[!UICONTROL Work Time] 값을 1로 설정하여 사용자가 프로젝트 관련 작업에 해당하는 전체 시간을 사용할 수 있음을 나타냅니다.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>Workfront 설명서에서 이 용어는 일정에 따라 작업에 할당된 시간을 설명하는 데 사용됩니다.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 텍스트 모드에서 다음 문을 사용하면 프로젝트, 작업 또는 문제의 계획된 시간 수 다음에 "시간"이라는 단어가 표시됩니다.</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>텍스트 모드 사용에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">텍스트 모드 구문 개요</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
