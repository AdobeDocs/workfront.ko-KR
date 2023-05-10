---
content-type: reference
navigation-topic: workfront-navigation
title: 용어 설명 [!DNL Adobe Workfront] 용어
description: 다음 [!DNL Adobe Workfront] 용어집에서는 Adobe Workfront에서 일반적으로 사용되는 용어를 나열합니다.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 7b5b0fd95e39f37153e36abb4e3b8e738ac26d21
workflow-type: tm+mt
source-wordcount: '19399'
ht-degree: 0%

---

# 용어 설명 [!DNL Adobe Workfront] 용어

>[!IMPORTANT]
>
>이 문서는 [!DNL Adobe Workfront] 애플리케이션, [!DNL Workfront] 설명서 또는 작업 계획 및 관리에 대해 일반적으로 설명하는 경우 현재 이 정보를 업데이트하고 있으므로 이 테이블이 완료되지 않을 수 있습니다. 이 정보를 철저히 고려할 때 이 면책조항을 제거합니다.

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
   <td>[!UICONTROL Access Level]</td> 
   <td>사용자가 Workfront 내에서 다른 개체 및 도구와 상호 작용하는 방법을 결정하는 사용자 프로필입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>이전 작업에서 작업을 수행할 수 없고 나중에 계획된 시작 날짜가 있는 작업 제약 조건이 없는 현재 프로젝트의 불완전한 작업입니다. 다시 말해, 그것은 오늘 작동할 수 있다.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>in [!DNL Workfront Goals]인 경우 활동은 목표에 대한 진행률 표시기입니다. 수동으로 업데이트하는 진행률 표시줄이나 목표와 연결된 프로젝트가 될 수 있습니다. 보고서에 활동을 표시할 수 없으며 [!DNL Workfront] API. 활동에 대한 자세한 내용은 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront 목표의 결과 및 활동 시작</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 비용]</td> 
   <td> <p>작업 및 문제의 경우 작업 또는 문제에 할당된 리소스의 시간당 비용 비율과 관련하여 로그된 실제 시간과 연관된 비용입니다. 프로젝트의 경우 프로젝트의 작업 및 문제로부터 얻은 모든 [!UICONTROL 실제 비용]입니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 비용]</td> 
   <td> <p>프로젝트 또는 작업에 대해 기록된 모든 비용에 대한 [!UICONTROL 실제 금액]의 합계입니다.</p> <b>예 </b>
   <p>작업 1에 대한 비용을 생성하고 [!UICONTROL 실제 금액] 필드에 $600.00을 입력하면 이 작업에 대한 [!UICONTROL 실제 비용]은 $600.00입니다. </p> 
   <p>프로젝트의 경우, [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 비용] 계산:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 실제 시간]</td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 [!UICONTROL 실제 시간]은 프로젝트, 작업 또는 문제에 로그온한 모든 시간의 합계입니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span> 작업 1의 [!UICONTROL 업데이트] 탭에서 '로그 시간'을 클릭하고 25시간을 입력한 경우 작업 1의 실제 시간 = 25시간입니다. </p> <p>[!DNL Workfront] 다음 공식을 사용하여 상위 작업 또는 프로젝트에 대한 [!UICONTROL 실제 시간]을 계산합니다.</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 실제 인건비]</td> 
   <td> <p>작업 또는 프로젝트에 투자한 노드와 연관된 [!UICONTROL 실제 비용]입니다. </p> <p>작업의 경우, [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 노무비]를 계산합니다.</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>작업에 [!UICONTROL Cost Type]의 [!UICONTROL User Hourly]가 있는 경우, [!DNL Workfront] 는 사용자 비율을 사용합니다. 작업에 [!UICONTROL Cost Type]의 [!UICONTROL Role Hourly]가 있는 경우, [!DNL Workfront] 작업 역할 비율을 사용하여 [!UICONTROL 실제 노무비]를 계산합니다. </p> <p>프로젝트의 경우, [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 실제 노무비]를 계산합니다.</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>예를 들어, 사용자가 [!UICONTROL User 시간별] [!UICONTROL Cost Type]으로 작업에 대해 5시간을 로그하고 시간당 요금이 $100인 경우 [!UICONTROL Actual Labor Cost]는 $500입니다.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>프로젝트 또는 작업의 [!UICONTROL Actual Revenue]는 프로젝트 또는 작업의 [!UICONTROL Actual Hours]와 연결된 금액입니다. </p> <p>의 매출 추적에 대한 정보 [!DNL Workfront]를 참조하십시오. <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 실제 시작]</td> 
   <td>사용자가 객체에 할당된 작업 중에 진행 중인 객체를 변경하는 타임스탬프입니다.</td> 
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
   <td>[!UICONTROL Agile] 방법론</td> 
   <td>다양한 기능 팀을 통한 요구 사항 및 솔루션의 협업 진화에 기반한 방법론 유형입니다. 이 기능은 고정된 타임라인에 따라 유연성과 변화를 장려합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>백로그에서 예상 작업을 가져와서 [!UICONTROL 반복]이라고 하는 일정 시간 내에 작업하므로 기존 팀과 다릅니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>이 항목이 [!UICONTROL 필터]에서 참조되면 이 필드에는 로그인한 사용자가 속한 팀에 속하는 사용자 또는 로그인한 사용자가 속한 팀에 할당된 작업 항목이 표시됩니다. </p> <p>다른 사용자와 보고서를 공유할 때 보다 일반적인 보고서를 만들려면 필터에 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 정보가 항상 사용자 지정되므로 로그인한 사람에 따라 다른 정보를 표시하는 보고서만 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당 날짜]</td> 
   <td> <p>이 필드는 다음 유형의 보고서에서 찾을 수 있습니다.</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project](재무 데이터)</li> 
     <li>[!UICONTROL Budget Hour]</li> 
    </ul> <p>대상<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project(Financial Data)] 보고서: </p> 
    <ul> 
     <li>이해하려고 할 때 이 보고서 작성 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 리소스에 할당된 [!UICONTROL 계획 시간]의 양입니다.</li> 
     <li> <p>[!UICONTROL 할당 날짜]는 작업에 대한 [!UICONTROL 작업 역할]의 할당이 시작되는 주의 첫 번째 날(일요일)입니다. 리소스([!UICONTROL 작업 역할])에는 할당된 작업의 [!UICONTROL 기간] 동안 주 단위 수만큼 [!UICONTROL 할당 날짜]가 있을 수 있습니다. 작업이 여러 달에 걸쳐 있는 경우 작업이 작업의 [!UICONTROL 기간]에 속하는 경우 한 달의 첫 날이 [!UICONTROL 할당 날짜]가 될 수도 있습니다.</p> <p>예를 들어, 3주 이상 걸이고 90개의 [!UICONTROL Planning Hours]가 있는 작업에 [!UICONTROL Job Role]을 할당할 수 있습니다. 이러한 시간은 작업 기간 동안 균등하게 분산되며, 이 작업은 매일 작업 역할에 6개의 [!UICONTROL 계획 시간]을 할당합니다.</p> <p><em> [!UICONTROL 일별 계획 시간] = [!UICONTROL 총 계획 시간]/ [!UICONTROL Duration] 작업 중 [!UICONTROL Work Days] 수 </em> </p> <p>그 결과, 3개의 [!UICONTROL 할당 날짜]가 있으며, 이는 각각 특정 수의 [!UICONTROL 계획 시간]이 작업에 연결된 매주 일요일마다 하나씩 있습니다.<br>작업이 한 달의 마지막 주 중순에 시작되고 새 달의 시작 후 2주가 지나면 작업에 네 개의 [!UICONTROL 할당 날짜]가 생깁니다. 매주 일요일마다 작업 [!UICONTROL 기간] 동안 한 번, 그리고 새 달의 첫 날에 한 번.</p> <p>이 정보를 최대한 활용하려면 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 프로젝트(재무 데이터) 보고서 및 [!UICONTROL 할당 날짜]에 대한 매트릭스 그룹을 추가한 다음 가장 정확한 데이터에 대해 주간, 월별, 분기별 또는 연간을 그룹화합니다.<br>매트릭스 그룹 빌드에 대한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">매트릭스 보고서 만들기</a>.</p> </li> 
    </ul> <p>재무 정보는 연결된 데이터가 5년 미만인 경우에만 [!UICONTROL 프로젝트(재무 데이터)] 보고서에 채워집니다. 예를 들어, 작업 역할이 2015년 1월에 작업에 할당되었고 오늘이 2021년 9월인 경우 작업 역할에 대한 [!UICONTROL 할당 날짜]와 같은 재무 필드가 [!UICONTROL 프로젝트(재무 데이터)] 보고서에 채워지지 않습니다. </p> 
    <div> 
     <p>[!UICONTROL Budget Hour] 보고서의 경우:</p> 
     <ul> 
      <li>리소스 또는 Resource Planner의 프로젝트에 할당된 [!UICONTROL 예산책정 시간]의 양을 이해하려고 할 때 이 보고서를 작성합니다.</li> 
      <li> <p>[!UICONTROL 할당 날짜]는 [!UICONTROL Resource Planner]에서 시간을 편성한 주의 첫 번째 날(일요일)입니다. </p> <p>팁:   <p>1주가 2개월 동안 지속되는 경우 보고서에서 두 개의 행을 생성합니다. 첫 번째 요일(첫 번째 달의 일요일) 및 두 번째 행은 두 번째 월의 첫 번째 요일을 표시합니다. </p> <p>예를 들어, 6월 30일(일요일) - 7월 6일(토요일) 주에 대해 사용자에게 8시간의 예산을 책정하는 경우 두 행은 6월 30일과 7월 1일의 [!UICONTROL 할당 날짜]를 보여줍니다. </p> </p> <p>예산 책정 리소스에 대한 자세한 내용은 [!DNL Resource Planner], 문서를 참조하십시오 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">의 예산 리소스 [!DNL Resource Planner] [!UICONTROL Project] 및 [!UICONTROL Role] 보기 사용</a>.</p> <p>[!UICONTROL Budget Hour] 보고서 작성에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">보고서: 예산책정 시간</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 공지]</td> 
   <td> <p>시스템 내의 사용자에게 정보를 전달하는 방법입니다. 이 정보는 종종 [!DNL Workfront] 관리자 또는 관리자로부터 사용자에게 전달 </p> <p>자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">공지 보내기</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>앱은 일반적으로 소프트웨어 애플리케이션에 대한 커넥터를 나타내지만 데이터를 조작하는 특수 기능도 나타낼 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자 결정]</td> 
   <td> <p>[!UICONTROL 증명 승인] 보고서에서 이 필드에는 더 이상 활성 상태가 아닌 증명에 대한 증명 승인 결정이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자 단계]</td> 
   <td>[!UICONTROL 증명 승인 보고서]에서 이 필드에는 증명 현재 단계에 대한 정보가 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>작업, 문서 또는 작업표와 같은 특정 작업 항목에서는 감독자나 다른 사용자가 작업 항목에 대해 로그오프해야 할 수 있습니다. 이 승인 프로세스를 승인이라고 합니다. </p> <p>자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">승인 프로세스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인 날짜]</td> 
   <td>[!UICONTROL 증명 승인] 보고서에서 이 필드에는 증명을 승인한 날짜가 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 승인자]</td> 
   <td>지정된 작업 항목에 대해 로그오프해야 하는 사용자 또는 작업 역할이나 작업표의 시간 항목을 승인하는 사용자입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당됨]</td> 
   <td> <p>[!UICONTROL 작업 또는 문제] 보고서에서 이 필드에는 작업 또는 문제의 소유자 또는 [!UICONTROL 기본 할당자]가 표시됩니다. 이 필드별로 필터링하거나 그룹화할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>문제 또는 작업에 지정된 사용자, 작업 역할 또는 팀입니다. 프로젝트, 포트폴리오 또는 프로그램에는 배정이 있을 수 없습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업이나 문제에 할당된 모든 엔터티(사용자, 작업 역할, 팀)의 목록이 표시됩니다. [!UICONTROL Assignment Users] 및 [!UICONTROL Assignment Roles] 필드를 사용하여 이 필드를 필터링할 수 있습니다. 팀 필드를 사용하여 작업이나 문제에 지정된 팀별로 필터링할 수 있습니다. 보고서를 이 필드로 그룹화할 수 없습니다.</p> <p>[!UICONTROL Recycle Bin]에 배치된 작업 항목은 다음 항목이 있는 [!UICONTROL Assignment] 개체를 참조하는 일부 보고서에 계속 표시됩니다. [!DNL OR] 필터 한정자가 사용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 할당된 작업 역할에 대한 정보가 표시됩니다. 이 필드에는 [!UICONTROL 기본 소유자]와 작업 또는 문제에 할당된 다른 작업 역할이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당 상태]</td> 
   <td> <p>할당, 작업 또는 문제 보고서에서 [!UICONTROL 할당 상태]는 작업 항목에 할당된 사용자가 [!UICONTROL Work On It] 또는 [!UICONTROL 완료] 단추를 클릭하여 작업을 수락하거나 완료했는지 여부를 표시합니다. 다음 [!UICONTROL 할당 상태]가 있습니다.</p> 
    <ul> 
     <li><b>[!UICONTROL 요청]</b>: 사용자가 작업이나 문제에 할당되었지만 [!UICONTROL Work On It] 단추를 클릭하지 않고 아직 작업을 시작합니다.</li> 
     <li><b>[!UICONTROL Working]</b>: 사용자가 [!UICONTROL Work On It] 단추를 클릭하고 현재 이 항목에서 작업 중입니다. </li> 
     <li><b>[!UICONTROL Done]</b>: 사용자가 [!UICONTROL 완료] 단추를 클릭하고 항목에 대한 작업을 완료했습니다. </li> 
    </ul> <p>자세한 내용은 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It] 및 [!UICONTROL Done] 단추 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 지정된 팀에 대한 정보가 표시됩니다. 이 필드에는 [!UICONTROL 기본 소유자] 및 작업이나 문제에 지정된 다른 팀이 표시됩니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>[!UICONTROL 작업] 또는 [!UICONTROL 문제] 보고서에서 이 필드에는 작업 또는 문제에 할당된 사용자에 대한 정보가 표시됩니다. 이 필드에는 [!UICONTROL 기본 소유자]와 작업이나 문제에 할당된 다른 사용자가 표시됩니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 속성]</td> 
   <td>속성은 [!DNL Workfront] 개체.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>감사는 Workfront에서 발생한 작업을 기록하는 시스템 메시지입니다. 다음 감사 유형이 기록됩니다.</p> 
    <ul> 
     <li>[!UICONTROL 범위 변경]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL 상태 변경]</li> 
     <li>[!UICONTROL 참고]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL 오류 항목]</li> 
     <li>[!UICONTROL 상태 변경]</li> 
     <li>[!UICONTROL 구독 변경 사항]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 감사 추적]</td> 
   <td>기록된 변경 사항([!UICONTROL 감사 영역])을 통해 추적된 이벤트에 의해 자동으로 생성된 메모 모음입니다. 각 메모는 작업을 수행한 사람, 작업, 작업 시간을 기록합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>[!UICONTROL Project Update] 유형 중 하나입니다. 이렇게 하면 야간 재계산 프로세스가 실행되고 프로젝트 또는 프로젝트 내의 작업에 대한 업데이트가 있을 때 프로젝트의 예상 및 계획된 타임라인이 재계산됩니다. </p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형을 선택합니다 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>사용 가능</p></td> 
   <td> <p>이 용어는 "사용자 가용성" 또는 "리소스 가용성"과 관련하여 사용되며 리소스(사용자 또는 작업 역할)가 작동할 수 있는 시간을 보여줍니다. </p> 
   <p>Workfront은 시스템에서 리소스 관리 환경 설정의 설정에 따라 여러 필드를 사용하여 사용자 가용성을 계산합니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>. </p>
   <p>리소스 가용성에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">리소스 관리 시작</a></p>
   또는 "능력"을 사용하여 자원 가용성을 나타냅니다. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>[!UICONTROL Project Update] 유형 중 하나입니다. 이렇게 하면 야간 재계산 프로세스가 실행될 때 예상 및 계획된 타임라인이 재계산됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형을 선택합니다</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>일상적인 업무 목표 실행에 기여하는 "일상적인 업무" 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 백로그]</td> 
   <td>새로운 문제가 작업할 준비가 될 때까지 유지되는 민첩한 환경의 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>민첩한 환경에서 반복을 측정하는 데이터 소스입니다.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>청구할 수 있는 수익, 시간 또는 비용을 기록합니다. 이 정보는 외부 회계 시스템에서 송장을 생성하는 데 사용할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">청구 레코드 만들기</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>청구 레코드 상태</td> 
   <td> <p>청구 레코드 또는 시간 보고서에서 청구 레코드의 상태는 청구 레코드가 청구되었는지 여부를 나타냅니다. 청구된 청구 레코드와 연관된 시간을 편집하거나 프로젝트를 삭제할 수 없습니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >청구 레코드 만들기</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL 브랜딩]</td> 
   <td><p>사용자 지정 프로세스 [!DNL Workfront] 색상 및 로고를 사용하여 회사를 미러링하는 인터페이스를 제공하기 위한 것입니다.</p><p><strong>참고</strong><br>조직에 온보딩된 경우 [!DNL Adobe Experience Cloud], 브랜딩을 사용할 수 없습니다.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 탐색 표시]</td> 
   <td> <p>사용자가 애플리케이션에서 있는 페이지의 계층 위치를 보여주는 페이지 상단의 영역입니다.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">자세한 내용은 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">탐색 표시 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산 상태]</td> 
   <td> <p>더 이상 사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이 제거되어 필드를 업데이트할 수 없습니다. </p> <p>이 필드는 프로젝트가 [!UICONTROL Capacity Planner]에 추가되었는지 여부 및 이에 대한 예산 계산이 완료되었는지 여부를 표시합니다. [!UICONTROL Capacity Planner]가 [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL 예산책정된 완료 날짜]</td> 
   <td> <p>더 이상 사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이 제거되었습니다. 이 필드는 업데이트할 수 없습니다. </p>
   <p> 이 필드는 [!UICONTROL 프로젝트] 및 [!UICONTROL 작업] 보고서 및 목록에 계속 표시됩니다.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예산책정된 비용]</td>

<td> <p>프로젝트에 대한 예산 책정 자원과 연관된 비용입니다. </p>
   <p>필드는 다음 영역에 표시됩니다 [!DNL Workfront] 다음 이름 아래:</p>
   <ul>
   <li><strong>[!UICONTROL 예산책정된 비용]</strong>: ([!UICONTROL Business Case Summary] 패널)</li>
   <li><strong>[!UICONTROL Cost]</strong>: ([!UICONTROL Cost]로 정보를 볼 때 [!UICONTROL Utilization] 영역)</li>
   <li><strong>[!UICONTROL Project Budget Cost]</strong>: 목록 및 보고서</li>
   </ul>   
    <p>프로젝트에 대한 [!UICONTROL 예산책정된 비용]은 다음 공식을 사용하여 계산됩니다.</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>[!UICONTROL 예산책정된 비용] 계산에 대한 자세한 내용을 알고, [!DNL Workfront]를 참조하십시오. <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">프로젝트 예산책정 원가 계산</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 예산책정된 시간]</td> 
   <td> <p>프로젝트에서 완료하는 데 필요한 작업에 대한 예산을 책정한 시간. 이 필드는 프로젝트 또는 프로젝트 리소스에 대해 [!UICONTROL Business Case](또는 [!UICONTROL Resource Planner]에서)의 [!UICONTROL Resource Budgeting] 영역에 설정한 시간을 참조합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">프로젝트에 대한 [!UICONTROL 예산책정된 노무비] 및 [!UICONTROL 예산책정된 시간] 이해</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 예산책정 사용자 정보 [!DNL Resource Planner], 문서를 참조하십시오 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">의 예산 리소스 [!DNL Resource Planner] [!UICONTROL Project] 및 [!UICONTROL Role] 보기 사용</a>. </p> 
    <p>[!UICONTROL Business Case] 또는 [!UICONTROL Resource Planner]의 [!UICONTROL Resource Budgeting] 영역에 설정된 시간이 다음 영역에 표시됩니다 [!DNL Workfront] 및 를 입력합니다.</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL 예산책정된 시간] 표시 이름</strong></td> 
        <td><strong>영역 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Hours]가 본 [!UICONTROL Resource Planner]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 예산책정된 시간]</td> 
        <td> <p>활용률 보고서 [!UICONTROL 시간] 보기</p> <p>[!UICONTROL 사용률] 보고서에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL Resource Utilization] 보고서 개요</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. 시간]</td> 
        <td> <p>[!UICONTROL Budget Hour] 보고서</p><p>예산책정된 시간 보고서의 [!UICONTROL 예산책정된 시간] 개체는 사용되지 않는 리소스 관리 도구에 관련된 정보를 참조합니다. "[!UICONTROL Bud만 해당. 이 보고서의 "시간" 필드는 [!UICONTROL Resource Planner] 또는 프로젝트 [!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역에 설정된 시간을 나타냅니다. </p> <p>보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner 예산책정 시간] </td> 
        <td> <p>다음 보고서에서 찾을 수 있습니다.</p>
        <ul>
        <li>[!UICONTROL Project] 보고서
        <li>[!UICONTROL Project(Financial Data)] 보고서
        <li>[!UICONTROL Task] 보고서
        <li>[!UICONTROL Issue] 보고서
        <li>[!UICONTROL Budget Hour] 보고서</li>
        </ul>
         <p>보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>의 [!UICONTROL Budget Hours]에 대한 기타 모든 언급 [!DNL Adobe Workfront] 는 Workfront에서 제거된 더 이상 사용되지 않는 기능을 사용하여 예산책정된 시간을 나타냅니다 . 이 필드는 보기 전용 필드이며 현재 리소스 예산 책정 도구를 사용할 때 현재 정보로 업데이트되지 않습니다. </p>
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
   <td>[!UICONTROL 예산책정된 인건비]</td> 
   <td> <p>이 비용은 리소스 관리자로서 프로젝트에서 완료해야 하는 작업에 대한 작업 역할에 예산을 편성하는 시간과 관련된 비용입니다. </p> <p>프로젝트 보고서의 [!UICONTROL 예산책정된 노무비]는 다음 공식을 사용하여 계산됩니다.</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>이 필드는 다음을 의미할 수 있습니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역 또는 프로젝트의 작업 역할 비용과 연관된 [!UICONTROL Resource Planner]에 표시되는 인건비 비용입니다. [!UICONTROL Budget Labor Cost] 계산에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL 예산책정된 노무비 이해] 및 프로젝트에 대한 [!UICONTROL 예산책정 시간]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>프로젝트에서 프로젝트에 연결된 이니셔티브에서 예상되는 [!UICONTROL People Cost]를 반영하는 [!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역에 표시되는 인건비 [!DNL Scenario Planner] 시나리오 계획자를 사용하여 프로젝트 자원의 예산을 책정하는 경우 이니셔티브에 대한 자세한 내용은 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">시나리오 플래너의 이니셔티브 개요</a>. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> </li> 
     <p>다음 이름 아래에 다음 영역이 표시됩니다.</p>
   <ul>
   <li><strong>[!UICONTROL 예산책정된 인건비]</strong>: ([!UICONTROL Business Case]의 [!UICONTROL Resource Budgeting] 영역)에서 사용할 수 있습니다.
   <li><strong>[!UICONTROL 예산책정된 비용]</strong>: ([!UICONTROL Utilization] 보고서 [!UICONTROL Cost] 보기)
   <p>자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 사용률 정보 보기 </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: 에서 [!DNL Resource Planner] 프로젝트 또는 [!DNL Role] 보기, 비용별 보기
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: 다음 보고서에서 다음을 수행합니다. 
   <ul>
    <li>[!UICONTROL Project] 보고서</li>
    <li>[!UICONTROL Project(Financial Data)] 보고서</li>
    <li>[!UICONTROL Task] 보고서</li>
    <li>[!UICONTROL Issue] 보고서</li>
    <li>[!UICONTROL Budget Hour] 보고서</li> 
    </ul>
    <p>보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p>
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
   <td>[!UICONTROL 예산책정 시작 날짜]</td> 
  <td> <p>더 이상 사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이 제거되었습니다. 이 필드는 업데이트할 수 없습니다.</p>
  <p>이 영역들은 [!DNL Workfront]. </p> 
  <p>필드는 [!UICONTROL project] 및 [!UICONTROL 작업] 보고서 및 목록에 계속 표시됩니다.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>완료된 작업과 남은 작업의 시각적 표현을 제공하는 라인 차트입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>프로젝트를 [!UICONTROL Idea] 상태에서 [!UICONTROL Planning] 상태로 이동해야 하는지 여부를 평가하는 데 사용되는 도구입니다. 즉, [!UICONTROL 비즈니스 사례]는 특히 프로젝트를 포트폴리오의 다른 프로젝트와 비교할 때 프로젝트를 시작하고 완료할 가치가 있는지 여부를 조직에서 결정하는 데 도움이 됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">프로젝트에 대한 [!UICONTROL Business Case] 만들기 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budget Hours]</td> 
   <td> <p>더 이상 사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이 제거되었습니다. 이 필드는 업데이트할 수 없습니다.</p> <p>이 필드는 여전히 프로젝트에서 표시되며 [!UICONTROL 작업] 목록 및 보고서는 보고서에 표시됩니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>작업 [!UICONTROL 기간] 유형 중 하나입니다. 이렇게 하면 작업의 [!UICONTROL 기간] 및 [!UICONTROL 작업 필요]를 기반으로 작업에 할당된 사용자가 작업에 할당되는 8시간 작업일의 백분율이 계산됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL 기간] 및 [!UICONTROL 기간 유형] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>작업 [!UICONTROL 기간 유형] 중 하나입니다. [!UICONTROL Duration] 및 사용자 [!UICONTROL Assignment] 백분율(8시간 근무일을 기반으로 함)이 주어지면 작업에 대한 [!UICONTROL 작업 필요]가 계산됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL 기간] 및 [!UICONTROL 기간 유형] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>에는 두 가지 유형의 달력이 있습니다 [!DNL Workfront]: [!UICONTROL 홈 달력] 및 달력 보고서.</p> <p>[!UICONTROL 홈 달력]은 사용자가 사용 가능한 시간(시)에 대해 작업 로드를 관리할 수 있는 개인 달력입니다 [!DNL Workfront]. 사용자는 [!UICONTROL Home Calendar]를 [!DNL Outlook] ([!DNL Google] 및 [!DNL Microsoft] 통합 출시). </p> <p>[!UICONTROL Home Calendar]에 대한 자세한 내용은 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] 보기</a>.</p> <p>달력 보고서는 사용자가 기한, 작업 상태 및 이벤트가 지정된 사용자를 포함하여 이벤트의 날짜 및 기타 중요한 세부 사항을 볼 수 있는 동적 보고서입니다.</p> <p> 달력 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">달력 보고서 개요</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL 시작 가능]</td> 
   <td> <p>이 필드는 작업이 작업을 시작할 준비가 되었는지 여부를 나타냅니다. 작업의 [!UICONTROL 시작 가능] 필드에서 작업을 시작할 준비가 되면 [!UICONTROL True]로 설정됩니다. </p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">작업에 대한 "[!UICONTROL 시작 가능]" 개요</a>.</p> 
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
   <td> <p>리소스가 작업에 할당할 수 있는 가용 시간입니다. "가용성"을 참조하십시오. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>카테고리는 사용자 지정 양식입니다. 이 객체에 대한 보고서를 작성할 수 있으며, 다른 객체 보고서에도 표시할 수 있습니다. 일부 개체에는 사용자 지정 양식이나 카테고리가 있을 수 없습니다. 다음 개체에는 사용자 지정 양식이 있을 수 있습니다. <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범주 이름]</td> 
   <td> <p>다음 객체 중 어느 하나의 객체에 대한 뷰에 열로 추가하면 해당 객체와 연관된 모든 사용자 정의 양식 목록이 표시됩니다.</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL 작업]<br></li> 
     <li>[!UICONTROL 문제]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>계획 작업을 정의, 이해 및 범위, 일정, 비용 및 자원 요소의 변경에 적용하는 데 중점을 둔 실무 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 변경 순서]</td> 
   <td>계약 범위에 대한 요청된 변경을 개략적으로 설명하는 프로젝트에 대해 제기된 문제 유형입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>프로젝트 [!UICONTROL 업데이트 유형] 중 하나입니다. 프로젝트 또는 작업에서 작업 또는 편집 작업이 수행될 때 [!UICONTROL 프로젝트 예상] 및 [!UICONTROL 계획됨] 타임라인만 업데이트합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변경 순서]</td> 
   <td> <p>일반적으로 프로젝트를 완료하기 전에 계획되지 않은 작업의 양을 수행해야 함을 나타내는 [!UICONTROL 문제] 유형 중 하나입니다.</p> <p>[!UICONTROL 문제] 유형에 대한 자세한 내용은 문서의 "기본 문제 유형" 섹션을 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">기본 문제 유형 사용자 지정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 하위 작업]</td> 
   <td>[!UICONTROL Parent Task] ([!UICONTROL Summary Task])의 [!UICONTROL Subtask]인 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>[!UICONTROL Subtasks]에 대한 [!UICONTROL Parent Task]([!UICONTROL Summary Task])의 컬렉션입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cookies] 및 [!UICONTROL Training]</td> 
   <td>학습 모듈, 인증, 표준 또는 학습 커뮤니티입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>사용자가 작업 결과물에 대한 기대치를 설정할 수 있는 통신 도구입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 커밋 날짜]</td> 
   <td>사용자가 작업 결과물에 대한 기대치를 설정할 수 있는 커뮤니케이션 도구입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] 및 [!UICONTROL Reporting]</td> 
   <td>프로젝트, 프로그램 또는 포트폴리오의 예외 및 상태를 검토하는 표준</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>[!UICONTROL Company]는 [!DNL Workfront]. </p> 
   <p> 사용자나 프로젝트를 하나의 회사와 연결할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">회사 만들기 및 편집</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료 날짜]</td> 
   <td> <p>프로젝트, 작업 또는 문제가 완료되도록 설정된 날짜입니다. 에는 몇 가지 유형의 [!UICONTROL 완료 날짜]가 있습니다 [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL 실제 완료 날짜]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">프로젝트 개요 [!UICONTROL 실제 완료 날짜] </a>.</li> 
     <li>[!UICONTROL 계획된 완료 날짜]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">프로젝트 [!UICONTROL 계획된 완료 날짜] 설정</a> 및 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">작업 개요 [!UICONTROL 계획된 완료 날짜]</a>.</li> 
     <li>[!UICONTROL 예상 완료 날짜]. 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">프로젝트, 작업 및 문제에 대한 [!UICONTROL 예상 완료 날짜] 개요</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료일]</td> 
   <td>[!UICONTROL Template] 시작 날짜를 기준으로 [!UICONTROL Template Task] 또는 [!UICONTROL Template]이 완료되어야 하는 날짜입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 완료 모드]</td> 
   <td> <p>이는 프로젝트가 [!UICONTROL 완료]로 표시되는 방식을 나타냅니다. 이 파일에는 두 개의 값이 있을 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Manual]: 사용자는 프로젝트 상태를 [!UICONTROL 완료]로 변경해야 합니다.</li> 
     <li>[!UICONTROL Automatic]: 프로젝트의 모든 작업이 100% 완료이고 모든 문제가 닫히면 프로젝트 상태가 자동으로 [!UICONTROL 완료]로 변경됩니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>작업, 문제 또는 프로젝트의 진행 상황을 시각적으로 나타냅니다.</p> <p>프로젝트의 경우 프로젝트 소유자가 조건을 수동으로 설정하거나 [!DNL Workfront]를 설정하는 것이 좋습니다. </p> <p>프로젝트 조건에 사용할 수 있는 값은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Troubleshooting]</li> 
    </ul> <p>프로젝트 조건에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL 프로젝트 조건] 및 [!UICONTROL 조건 유형] 개요</a>.</p>
     <p>작업 및 문제 조건을 보고서에 표시할 수 있는 숫자와 연결할 수 있습니다. 아래 목록에는 작업 및 문제 조건에 대한 기본 이름과 숫자가 표시됩니다. 시스템 관리자는 조건 이름을 업데이트할 수 있으며 다른 숫자로 새 조건을 추가할 수 있습니다. 숫자를 조건과 연결하면 편집할 수 없습니다.  </p> 
     <p>작업의 경우 작업 소유자가 조건을 수동으로 설정합니다. 작업 조건에 사용할 수 있는 값은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL 부드럽게 이동] (0)<br></li> 
     <li> [!UICONTROL 몇 가지 문제] (1)<br></li> 
     <li>[!UICONTROL 주요 장애물] (2)</li> 
    </ul> <p>작업 조건에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">작업 및 문제에 대한 [!UICONTROL 조건] 업데이트</a>.</p> <p>문제의 경우 문제 소유자가 조건을 수동으로 설정합니다. 문제 조건에 사용할 수 있는 값은 다음과 같습니다.<br></p> 
    <ul> 
     <li>[!UICONTROL 부드럽게 이동] (0)<br></li> 
     <li>[!UICONTROL 몇 가지 문제] (1)<br></li> 
     <li>[!UICONTROL 주요 장애물] (2)</li> 
    </ul> 
   <p><b>메모</b></p>
    <p>[!UICONTROL Journal Entry] 보고서에서 [!UICONTROL Condition] 필드를 추적하면 [!UICONTROL New] 및 [!UICONTROL Old Number Values]에 해당 이름 대신 조건에 연결된 숫자가 표시됩니다. 조건이 원래 작업 또는 문제에 대해 정의되지 않고 나중에 업데이트하면 업데이트를 캡처하는 분개 입력에 [!UICONTROL Condition] 필드의 [!UICONTROL Old Number Value]가 -2,147,483,648로 표시됩니다. 이 문서에서 "[!UICONTROL 새 번호 값]", "[!UICONTROL 이전 번호 값]" 및 "[!UICONTROL 저널 항목]"도 참조하십시오. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조건 업데이트]</td> 
   <td> <p>이 필드는 작업, 프로젝트 또는 문제의 현재 상태를 보여 줍니다. 이 옵션은 작업, 프로젝트 또는 문제 소유자가 새 조건과 함께 [!UICONTROL 업데이트 상태] 필드에서 제공한 최신 업데이트를 보여줍니다.</p> <p>조건 업데이트에 대해 수행된 주석이 [!UICONTROL 조건 업데이트] 열에 표시되지 않습니다. 기본 업데이트만 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제약 조건 날짜]</td> 
   <td> <p>[!UICONTROL 시작 날짜]와 같이 특정 날짜에 연결된 [!UICONTROL 작업 제약 조건을 사용하는 경우 해당 특정 날짜는 작업의 [!UICONTROL 제한 날짜]가 됩니다.</p> <p>다음 작업 제약 조건은 [!UICONTROL 제약 조건 날짜] 필드를 업데이트합니다.</p> 
    <ul> 
     <li>[!UICONTROL을 시작해야 함]</li> 
     <li>[!UICONTROL이 종료되어야 함]</li> 
     <li>[!UICONTROL 시작 후]</li> 
     <li>[!UICONTROL Start No Early]</li> 
    </ul> <p>팁:   
     <ul> 
      <li> <p>[!UICONTROL Constraint]가 [!UICONTROL Fixed Date]인 작업에 [!UICONTROL Constraint Date]가 없습니다. </p> </li> 
      <li> <p> [!UICONTROL 제한 날짜]는 보고서나 사용자 지정 보기에서만 볼 수 있습니다.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>시작 시기 등과 같이 특정 일에 연결된 템플릿 작업에서 작업 제한을 사용하는 경우 해당 특정 날이 템플릿 작업의 제한 일이 됩니다.</p> <p>다음 작업 제약 조건은 [!UICONTROL 제약 조건 일] 필드를 업데이트합니다.</p> 
    <ul> 
     <li>[!UICONTROL을 시작해야 함]</li> 
     <li>[!UICONTROL이 종료되어야 함]</li> 
     <li>[!UICONTROL 시작 후]</li> 
     <li>[!UICONTROL Start No Early]</li> 
    </ul> <p>팁: [!UICONTROL Constraint Day]는 보고서나 사용자 지정 보기에서만 볼 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제약 조건 유형]</td> 
   <td> <p>작업의 예약 경향. 예를 들어 [!UICONTROL 가능한 한 빨리] 은(는) 작업이 가능한 한 빨리 시작되도록 예약하고, [!UICONTROL Finish No Launch]는 [!UICONTROL Constraint Date] 또는 그 이후까지 작업을 완료하도록 예약합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL 작업 제약 조건] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Context Menu]</td> 
   <td>화면 왼쪽에 있는 메뉴로서 항목이 활성 컨텐츠와 상호 연관되도록 변경됩니다. 예를 들어 사용자가 프로젝트를 보고 있으면 [!UICONTROL 상황별 메뉴]에 프로젝트 관련 정보 및 도구에 대한 링크가 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변환된 문제 작성자]</td> 
   <td>문제가 프로젝트 또는 작업으로 변환될 때 문제의 [!UICONTROL 기본 연락처]인 사용자에 대한 정보를 표시하는 프로젝트 또는 작업 보고서의 필드입니다. 이 필드는 변환된 문제에 대한 [!UICONTROL 기본 연락처]의 이름을 표시하는 [!UICONTROL 프로젝트 세부 정보] 섹션에도 표시됩니다. 이 문서에서 "[!UICONTROL 기본 연락처]"도 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>프로젝트, 작업 또는 문제를 완료할 때 사용해야 하는 통화 금액입니다. </p> <p>프로젝트와 관련된 다양한 유형의 인건비, 비용, 위험을 추적할 수 있습니다.비용 추적에 대한 자세한 내용은 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/track-costs.md">비용 추적</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 비용 유형]</td> 
   <td>작업의 경우 [!UICONTROL 비용 유형]은 작업이 비용을 발생시키는 방법을 결정합니다. 일부 예로는 [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] 및 [!UICONTROL User Hourly plus Fixed]가 있습니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 간 종속성]</td> 
   <td> <p>한 프로젝트의 작업은 다른 프로젝트의 작업에 따라 달라집니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">프로젝트 간 선행 작업 만들기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 사용자 지정 데이터]</td> 
   <td> <p>조직에 고유한 데이터. 조직은 다음을 사용자 지정할 수 있습니다 [!DNL Workfront] 사용자 지정 양식 및 사용자 지정 필드를 만들어 애플리케이션을 만듭니다. 이 사용자 지정 정보를 통해 KPI, 감사 및 수요 혼합에 대한 보고를 수행할 수 있습니다. </p> <p>[!UICONTROL 사용자 지정 데이터]를 다음에 연결할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL 반복]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 데이터 유형]</td> 
   <td>[!UICONTROL 사용자 지정 데이터] 필드가 데이터베이스에 텍스트, 날짜, 숫자 또는 통화로 저장되는지 지정하는 옵션입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 표시 유형]</td> 
   <td>사용자 지정 필드의 필드 표시 유형입니다. 예를 들면 [!UICONTROL 드롭다운], [!UICONTROL 텍스트 필드], [!UICONTROL 텍스트 영역], [!UICONTROL 라디오 단추] 등이 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 필드]</td> 
   <td>사용자가 여러 옵션 중에서 선택할 수 있는 사용자 지정 데이터의 경우, 사용자가 선택할 수 있는 값입니다. 사용자 지정 옵션은 [!UICONTROL 드롭다운], [!UICONTROL 다중 선택 드롭다운], [!UICONTROL 라디오 단추] 및 [!UICONTROL 확인란]에서만 유효합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 양식 레이블]</td> 
   <td>사용자 지정 옵션과 함께 사용자 지정 표시 유형을 사용하는 경우 드롭다운 메뉴, 확인란 또는 해당 사용자 지정 옵션의 라디오 단추에 표시되는 사용자 인터페이스 텍스트입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>사용자 지정 옵션과 함께 사용자 지정 필드를 사용할 때 특정 옵션을 위해 데이터베이스에 저장되는 값입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 지정 보기]</td> 
   <td>목록의 각 개체에 대해 표시되는 데이터 필드 또는 열의 정의입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Workfront 인스턴스를 사용하는 조직.</td> 
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
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> 보고서 또는 보고서 객체 목록에 이 필드를 추가하여 보고서가 목록에 나열되는 대시보드를 표시할 수 있습니다. </p> <p> 이 필드를 사용하여 특정 대시보드에 나열된 보고서를 필터링할 수도 있습니다. </p> <p> 보고서 개체 보고서에 대한 대시보드 정보를 포함하는 방법에 대한 자세한 내용은 문서의 "대시보드에 나열된 보고서 이해" 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">보고서 액세스 및 구성</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 데이터 유형]</td> 
   <td>"[!UICONTROL 사용자 지정 데이터 유형]"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>이 필드는 [!UICONTROL 실제 완료 날짜]가 누락된 경우 [!UICONTROL 계획된 시작]과 [!UICONTROL 오늘] 간의 날짜 차이를 보여줍니다.</p> <p>또한 [!UICONTROL 실제 완료 날짜]가 있을 때 [!UICONTROL Actual Completion]과 [!UICONTROL Planning Completion] 간의 날짜 차이를 표시합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 기본 일정]</td> 
   <td> <p>조직 내의 사용자 및 프로젝트에 지정할 사용자 지정 가능한 기본 작업 시간입니다. </p> <p>예약은 사용자에게 할당된 작업의 계획, 시작 및 완료 날짜를 계산하는 데 사용됩니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 산출물]</td> 
   <td>프로젝트 완료 시 제공되어야 하는 수량화 가능한 상품이나 서비스.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>흡입 프로세스의 점수 및 우선순위.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 부서 목표]</td> 
   <td>부서 내 운영 지표 개선에 중점을 둔 특정 부서의 목표</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종속성]</td> 
   <td>한 작업이 상태를 변경해야 다른 작업이 상태를 변경할 수 있는 두 작업 간의 링크도 상태를 변경할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종속성 유형]</td> 
   <td> <p>작업과 이전 작업 간의 예약 관계 유형입니다. 한 예는 [!UICONTROL Finish-Start]입니다. 두 번째 작업을 시작하려면 먼저 첫 번째 작업이 완료되어야 합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">작업 종속성 유형 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>내의 객체에 첨부된 모든 파일 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>동일한 문서에 동일한 객체가 업로드될 때마다 버전 번호가 할당됩니다. 사용자는 이전 버전의 문서에 대한 여러 옵션을 보고 변경할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">문서 버전 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>작업 문제 또는 프로젝트 완료를 위해 할당된 시간([!UICONTROL 계획 시작]과 계획 완료 사이의 일 수로 결정됨)</p> 
    <ul> 
     <li>작업의 경우 작업 기간 유형이 단순하지 않은 경우 지속 시간은 편집 가능한 필드입니다. 작업의 기간 유형이 단순 또는 작업 제한이 고정 날짜인 경우 기간은 Workfront에서 수행하는 계산입니다.</li> 
     <li>문제의 경우 지속 시간은 항상 편집 가능한 필드이며 문제를 해결해야 하는 예상 일 수를 나타냅니다.</li> 
     <li>프로젝트의 경우 기간은 [!DNL Workfront] 그리고 가장 이른 작업의 계획 시작과 프로젝트에 대한 최신 작업의 [!UICONTROL 계획 완료] 간의 일 차이를 나타냅니다.</li> 
    </ul> <p>작업에 대한 [!UICONTROL 기간]과 [!UICONTROL Planning Duration]의 차이점에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">작업에 대한 [!UICONTROL Planning Duration]과 [!UICONTROL Duration] 간의 차이점</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 기간(분)]</td> 
   <td>이 필드에는 [!UICONTROL 기간] 필드와 같은 정보가 일 대신 분 단위로 표시됩니다. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>이는 반복 작업의 상위의 [!UICONTROL 작업 세부 사항] 및 [!UICONTROL 작업 편집] 상자에 표시됩니다. 각 반복 작업의 기간을 표시합니다. 반복 작업 만들기에 대한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>. </p> <p> <span>개별 반복 작업에서 수정된 기간은 이 필드에 표시된 값을 표시하지 않습니다.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 기간 유형]</td> 
   <td> <p>작업을 완료하는 데 필요한 작업이 작업 기간 동안 할당자에게 할당되는 방법을 나타내는 작업 필드입니다. 작업의 [!UICONTROL 기간], [!UICONTROL 작업 필요], 시간 또는 [!UICONTROL 할당] 간의 관계를 나타냅니다. 할당된 리소스는 작업에 소비하여 완료해야 합니다. </p> <p>이 필드는 작업의 [!UICONTROL 세부 사항] 탭에 표시됩니다. </p> <p>옵션은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Tivity Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL 기간] 및 [!UICONTROL 기간 유형] 개요</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>전원 검색에서 시간을 측정하는 데 사용되는 단위입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tivity Driven]</td> 
   <td>사용자 수와 작업을 완료하는 데 걸리는 시간 사이의 관계입니다. 사용자를 더 추가하면 작업이 완료되도록 예약된 총 시간이 감소하지만 작업 기간은 동일하게 유지됩니다. 예를 들어, 만약 일이 땅콩 한 배럴에 일을 한다면, 더 많은 사람을 추가한다면, 일정이 줄어들게 되지만, 1일에 걸리는 기간은 동일하게 유지됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time]은 작업의 [!UICONTROL Duration]에 대한 시간 단위입니다. 휴일, 주말 및 타임오프를 포함하는 작업의 [!UICONTROL 계획 시작 날짜]와 [!UICONTROL 계획 완료 날짜] 사이의 시간입니다. 즉, 경과 시간은 달력 일수의 경과입니다. </p> <p>[!DNL Workfront] 작업 기간 동안 다음과 같은 경과 시간 단위를 지원합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>경과 시간을 포함하여 작업 기간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL 기간] 및 [!UICONTROL 기간 유형] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종료 날짜]</td> 
   <td> <p> [!UICONTROL 비율] 보고서에서 프로젝트 레벨에서 작업 역할에 대한 새 청구 비율이 종료되는 날짜입니다. 이 일자 이전의 프로젝트와 연관된 시간을 이 청구 비율로 곱하여 프로젝트의 수익을 계산합니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>작업, 프로젝트, 팀 또는 조직에 대한 약정 및 신뢰도가 저하되는 시기를 나타내는 [!UICONTROL 작업 성과 지표](WPI)입니다. 이것은 여러분이 그 믿음과 약속을 되살리기 위해 행동해야 한다는 것을 나타냅니다. WPI는 간단한 질문으로 측정됩니다. "당신은 당신이 무엇을 기대했는지 이해했습니까? 당신이 맡은 일이 조직에 영향을 미칩니까? 정말 잘했어요?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>회사 목표의 지표에 기여하는 교차 기능 목표입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>프로젝트 또는 작업의 변경 사항.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 처리기]</td> 
   <td>이벤트가 발생할 때 발생하는 자동화된 작업입니다. 일반적인 예는 자동화된 이메일 알림입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 알림]</td> 
   <td>이벤트 처리기에서 생성된 전자 메일입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>작업 또는 프로젝트에 대한 비인적 비용</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>일반적으로 라이센스 유형 또는 이러한 라이센스가 있는 사용자이며 시스템에서 정보를 검토할 수만 있습니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 외부 시스템]</td> 
   <td>지정된 기록 시스템 외부에서 저장 및 관리되는 모든 서비스 또는 소프트웨어</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>모든 Workfront 개체 또는 이와 연관된 정보가 데이터베이스에 표시됩니다. </p>
   <p>예를 들어 "project", "user", "hour"는 모두 Workfront 객체뿐만 아니라 필드입니다. "Name", "status", "owner", "start date"는 위의 객체와 연관된 Workfront 필드입니다. </p>

<p>개체를 참조할 때 "개체" 및 "필드"라는 항목을 서로 교환하여 사용할 수 있습니다.</p>
   <p>보고 범위에서 "필드"는 보고서에서 캡처할 개체 또는 개체에 대한 정보를 참조합니다.</p>

<p><b>메모</b></p>

<p>텍스트 추가 보고에서 필드는 데이터베이스에 표시되는 객체 또는 해당 정보를 참조합니다.</p>
   <p>경우에 따라 사용자 인터페이스에 표시되는 이름이 데이터베이스의 필드 이름과 다릅니다. 예를 들어 "issue"는 Workfront 인터페이스에 있는 개체의 이름이지만 "opTask"는 Workfront 데이터베이스에 있는 개체의 이름(또는 필드)입니다. </p> 
   <p> 텍스트 모드 보고서, 보기, 필터 또는 그룹을 작성하거나 계산된 필드를 만들 때 데이터베이스에 나타나는 필드를 그대로 사용하는 것이 중요합니다.</p>

<p>자세한 내용은 <a href="../../../wf-api/general/api-explorer.md">API 탐색기</a> 및 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">텍스트 모드 개요</a>.</p>

<p>기본적으로 Workfront에는 개체 및 해당 정보를 모두 정의하는 필드 세트가 포함되어 있습니다. 사용자 정의 필드를 만들어 개체를 정의할 수도 있지만 사용자 정의 개체를 만들 수는 없습니다.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>보고서에 표시되는 정보를 정의하는 보고서 또는 목록 요소의 기본 빌딩 블록 중 하나입니다. 보고 요소에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> <p>필터는 보고서 또는 [!DNL Workfront] 프로젝트, 작업 또는 문제와 같은 패널 목록.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>의 인건비, 비용 및 수익 데이터를 관리하는 프로세스 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 고정 비용]</td> 
   <td>프로젝트에 대한 고정 비용을 정의할 수 있습니다. 프로젝트를 완료하는 데 필요한 금액을 나타내는 프로젝트의 [!UICONTROL 계획 비용]의 일부입니다. 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 고정 수익]</td> 
   <td>프로젝트에 대한 고정 수익 금액을 정의할 수 있습니다. 프로젝트를 완료하면 얻을 수 있는 금액을 나타내는 프로젝트의 [!UICONTROL 계획 수익]의 일부입니다. 매출에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 플래그]</td> 
   <td> <p> 이 필드는 [!UICONTROL 상태 아이콘]과 동일하지만 다음 보기에서만 사용할 수 있습니다. </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>폴더는 객체와 연관된 문서 또는 보고서를 구성하는 데 사용됩니다.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE](Full Time Equivalent)</td> 
   <td>자원을 작업에 사용할 수 있는 시간을 나타내는 Full Time Equivalent입니다. 
   다음 영역에 [!UICONTROL FTE] 필드가 표시됩니다. 
  <ul>
   <li> 사용자를 편집하거나 만들 때 사용자의 프로필 </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner](Workfront Scenario Planner에 대한 추가 라이센스가 필요) </li>
   <li> 사용자 목록 및 보고서 </li> </ul>

<p>[!UICONTROL FTE]는 최대 10진수여야 하며 0일 수 없습니다. </p>
   <p> 프로필에 정의된 대로 사용자 [!UICONTROL FTE] 필드의 기본값인 1의 [!UICONTROL FTE]는 리소스(사용자 또는 역할)가 가용성을 계산하는 일정에 따라 전체 시간(시간)을 작동함을 의미합니다. </p>
   <p>Workfront 관리자는 사용자의 가용성을 확인하는 데 사용할 일정을 결정합니다.  </p>
   <ul>
   <li> [!UICONTROL 기본 일정]을 사용하면 Workfront은 프로필에 있는 사용자의 [!UICONTROL FTE]를 사용하여 가용성을 계산합니다. </li>
   <li> 사용자 일정이 사용되는 경우 Workfront에서는 사용자의 시간 제한, [!UICONTROL 작업 시간] 값 및 [!UICONTROL 기본 일정]을 사용하여 사용자의 [!UICONTROL FTE]를 계산합니다. </li> </ul>

<p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">리소스 관리 환경 설정 구성</a>.  </p>
   <p>예약 작성에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">예약 만들기</a>. </p>

<p><b>메모</b></p>
   <p>[!UICONTROL Scenario Planner]의 모든 계산에 대해 Workfront은 다음 값을 사용합니다. 1 [!UICONTROL FTE] = 8시간.</p>
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
   <td>[!UICONTROL Gantt 차트]</td> 
   <td> <p>프로젝트의 작업이 현재 예약되어 있는 계획 또는 예상 날짜를 기준으로 달력 보기에서 프로젝트 날짜의 시각적 타임라인입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 목표]</td> 
   <td><p>에는 두 가지 목표 개념이 있습니다 [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>프로젝트 목표</b>: 프로젝트의 관련 이해 관계자가 동의한 일련의 비즈니스 목표. 프로젝트 목표는 프로젝트의 비즈니스 사례의 일부입니다. </p> <p>목록 또는 보고서에 프로젝트 목표를 표시할 수 없지만 API를 통해 액세스할 수 있습니다. </p> <p>비즈니스 사례 프로젝트 목표에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">비즈니스 사례 목표 생성 </a>. </p> </li> 
     <li> <p><b>전략적 목표</b>: 전략적 목표는 특정 기간 동안 작업 전략을 계획하기 위해 생성하는 목표입니다. 를 사용하여 이러한 유형의 목표를 만들 수 있습니다 [!DNL Workfront Goals]. 조직은 추가 라이센스를 구입해야 하며 전략적 목표를 만들려면 이 기능에 액세스할 수 있어야 합니다. [!DNL Workfront Goals] 추가 라이센스에서만 사용 가능합니다.</p> 
     <p>자세한 내용은 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>. </p> 
     <p>목표 또는 프로젝트 보고서에 전략적 목표를 표시하고 API를 통해 액세스할 수 있습니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 목표 계층]</td> 
   <td> <p>[!UICONTROL 목표] 및 [!UICONTROL 프로젝트] 보고서에서 전략적 목표가 다른 목표에 도달할 때 속한 계층에 목표를 표시하는 수집 필드입니다. 목표는 구분 기호로 ▸. </p> <p>이 필드에는 목표 및 목표에 대한 부모만 표시됩니다. 하위 목표는 표시되지 않습니다. </p> <p>목표 정렬에 대한 자세한 내용 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">의 목표 정렬 개요 [!DNL Workfront Goals]</a>. </p> 
   <p>이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront Goals]. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Acquisition Score]</td> 
   <td> [!UICONTROL 프로젝트 보고서]에서 이 필드는 [!UICONTROL Business] 사례와 연관된 프로젝트 수준 목표를 참조하는 데 사용됩니다. 현재 이 필드는 더 이상 사용되지 않으며 기능과 연결되어 있지 않습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 목표] </td> 
   <td> <p>[!UICONTROL 프로젝트] 보고서에서 프로젝트와 연결된 모든 전략적 목표를 표시하는 수집 필드입니다. 목표는 쉼표로 구분됩니다.</p> <p>이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront Goals]. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. 의 전략적 목표 및 프로젝트 목표에 대한 자세한 정보 [!DNL Workfront]를 보려면 이 문서에서 "[!UICONTROL Goal]"을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>모든 사용자에게 영향을 주는 인터페이스 설정입니다. [!UICONTROL 사용자 인터페이스 환경 설정]은 [!UICONTROL 사용자 인터페이스 환경 설정]에서 덮어쓸 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>동일한 객체에 액세스할 수 있는 사용자(동일한 부서 또는 사업부에서 가능)의 모음입니다. 사용자 외에도 그룹을 포트폴리오, 프로그램, 프로젝트,<span> 프로젝트 템플릿,</span> 회사, 팀, 일정, 레이아웃 템플릿 및 작업표 프로필</p> <p>그룹별로 개체에 권한을 부여할 수도 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">그룹 개요</a>.</p> <p>다음 유형 중 하나의 객체 목록이나 보고서에서 [!UICONTROL 그룹] 필드를 사용하여 특정 그룹과 연관된 해당 유형의 객체를 나열할 수 있습니다. 사용자, 포트폴리오, 프로그램, 프로젝트 <span>프로젝트 템플릿</span>, 회사, 팀, 일정, 레이아웃 템플릿 또는 작업표 프로필</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 그룹 관리자]</td> 
   <td> <p>지정된 사용자 그룹의 개체, 액세스 및 사용자를 관리하는 사용자.</p> <p> [!UICONTROL 그룹] 보고서에서 이 필드는 그룹에 [!UICONTROL 그룹 관리자]로 지정된 사용자의 이름을 표시합니다. 그룹 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> [!UICONTROL 레이아웃 템플릿], [!UICONTROL 작업표 프로필] 또는 [!UICONTROL 일정 보고서]에서는 그룹 관리자가 템플릿을 수정할 수 있는 액세스 권한이 있는 그룹을 표시합니다. 이 필드로 이 보고서를 필터링할 수도 있습니다. </p> <p> 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">레이아웃 템플릿 만들기 및 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>목록의 정보를 일반적인 기준으로 분류하는 데 사용되는 보고 요소입니다.</p> <p>자세한 내용은 문서의 "[!UICONTROL 그룹화]" 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">보고 요소: 필터, 보기 및 그룹화</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 핸드오프 날짜]</td> 
   <td> <p>작업을 작업에 사용할 수 있게 되는 날짜입니다. [!UICONTROL 핸드오프 날짜]는 계산이며 수동으로 설정할 수 없습니다. <br>[!UICONTROL 핸드오프 날짜]에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL 작업 핸드오프 날짜] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>의 일부 [!DNL Workfront] 이는 모든 문제 대기열을 보유합니다. [!UICONTROL Help Desk]를 사용하여 고객 지원 티켓, 프로젝트 요청, 헬프데스크 티켓 등을 처리할 수 있습니다. 이는 [!UICONTROL Requests] 영역과 동일합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>[!UICONTROL Hour] 보고서에서 [!UICONTROL Owner]는 시간이 할당된 사용자입니다. 실제로 시간을 기록하고 있는 사용자와 다릅니다. 이러한 두 엔티티는 서로 다른 두 사용자일 수 있습니다. <br>다른 사용자의 로깅 시간에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">로그 시간</a>.</td> 
  </tr>

<tr> 
   <td>시간 상태</td> 
   <td> <p>사용자가 작업, 문제 또는 프로젝트에 대해 기록하는 실제 시간에 대해 Workfront이 설정하는 속성입니다. </p>

시간 항목에는 Workfront에서 다음 상태 중 하나가 있을 수 있습니다.
<ul>
   <li><b>제출됨</b>: 프로젝트, 작업 또는 문제에 로그온한 시간 이들은 청구 레코드의 일부이거나 아직 청구 레코드에 추가되지 않습니다.</li>
   <li><b>승인됨</b>: 시간이 기록되었으며 프로젝트 소유자가 승인했습니다. 이들은 청구 레코드의 일부이거나 아직 청구 레코드에 추가되지 않습니다.</li> 
   <li><b>승인되지 않음</b>: 프로젝트 소유자가 로그하여 거부한 시간입니다. 이들은 청구 레코드의 일부이거나 아직 청구 레코드에 추가되지 않습니다.</li>
   <li><b>청구됨</b>: 시간이 기록되고 청구 레코드에 추가되었으며 청구 레코드 상태가 청구됨으로 표시되었습니다. 프로젝트 소유자가 승인할 필요는 없습니다.</li>
   <li><b>청구됨 및 승인됨</b>: 시간이 기록되고 프로젝트 소유자가 승인했으며 청구 레코드 상태가 청구됨으로 표시되었습니다.</li>
   </ul>


<p>시간이 청구 레코드의 일부인 경우 시간 상태는 시간이 승인되었는지 또는 해당 시간이 속한 청구 레코드가 청구되었는지 여부를 나타냅니다. 시간 항목의 시간 상태는 1시간 목록이나 보고서에만 표시됩니다. </p>

<p>청구 레코드에 시간을 추가하는 방법에 대한 자세한 내용은 문서의 "청구 레코드에 시간 추가" 섹션을 참조하십시오 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >청구 레코드 만들기</a>.</p>

<p>프로젝트에 대한 시간 승인에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >프로젝트 승인 시간 필요</a>.</p>

<p><b>팁</b></p>

<p>작업 항목에 직접 기록되지 않은 일반 시간은 시간 상태를 표시하지 않습니다. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>사용자가 작업, 문제 또는 프로젝트에 대해 기록하는 실제 시간에 대해 설정할 수 있는 속성입니다. 또한 [!UICONTROL Vacation] 및 [!UICONTROL Time Off]와 같이 작업에 직접 연결되어 있지 않은 로그된 시간에 대한 속성입니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">시간 유형 관리</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID는 의 모든 개체와 연결된 영숫자 표시기입니다 [!DNL Workfront]. 이 변수는 [!DNL Workfront] 데이터베이스. 보고서에서 개체의 ID나 각 개체의 목록을 볼 수 있습니다. </p> <p>팁:   <p>개체 페이지의 URL에서 ID를 볼 수도 있습니다. 예를 들어, 프로젝트의 ID는 [!UICONTROL 프로젝트 세부 사항] 페이지에 액세스할 때 다음 URL에 요약된 숫자와 비슷합니다.</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 개별 목표]</td> 
   <td>개인 또는 경력 개발과는 관련이 없지만 팀 목표 지표에 기여하는 개별 목표.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 상속된 액세스]</td> 
   <td>액세스 권한이 객체에서 다른 객체로 전파되도록 하는 공유 함수입니다. 예를 들어 프로젝트 사용자는 프로그램 및 포트폴리오 레코드에 정의된 액세스를 상속합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>에서 [!DNL Workfront Scenario Planner]를 사용하면 계획을 여러 이니셔티브로 나누어 계획을 보다 쉽게 관리할 수 있습니다. <span>[!UICONTROL Initiative] 보고서를 작성하고 [!UICONTROL Project] 보고서에서 [!UICONTROL Initiative] 정보에 액세스할 수 있습니다.</span></p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>다음 [!DNL Initiative] 보고서가 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스. API를 통해 [!UICONTROL 이니셔티브]에 액세스할 수 없습니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative 작업 역할]</span> </td> 
   <td> <p><span>[!UICONTROL Initiative Job Role] 보고서 유형은에서 계획 이니셔티브와 연관된 작업 역할에 대한 정보를 표시합니다 [!DNL Workfront Scenario Planner].</span> </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p><span>이 보고서 유형은 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative 작업 역할 시간]</span> </td> 
   <td> <p><span> [!UICONTROL Initiative Job Role] 보고서에서 이니셔티브의 Job 역할과 연관된 시간 수를 표시합니다.</span> </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>이 필드 및 [!UICONTROL Initiative Job Role] 보고서 유형이 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative 작업 역할 수]</td> 
   <td> <p>[!UICONTROL Initiative Job Role] 보고서에는 이니셔티브와 연관된 특정 작업 역할의 수가 표시됩니다.</p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>이 필드 및 [!UICONTROL Initiative Job Role] 보고서 유형이 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative 마지막으로 게시된 날짜]</td> 
   <td> <p>[!UICONTROL Initiative], [!UICONTROL Initiative Job Role] 및 [!UICONTROL Project]의 필드는 계획 이니셔티브가 프로젝트에 마지막으로 게시된 날짜를 표시하는 필드입니다. 이니셔티브를 게시하여 프로젝트를 생성하거나 이니셔티브에 연결된 프로젝트를 업데이트할 수 있습니다.</p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> <p><span>이니셔티브 게시에 대한 자세한 내용은</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">에서 프로젝트를 만들고 업데이트하기 위한 시나리오를 게시합니다. [!DNL Workfront Scenario Planner]</a>. 이 필드는 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 인라인 검색]</td> 
   <td>양식을 완료하는 과정에서 하나의 특정 필드에 대해 가능한 항목을 찾기 위해 검색을 수행했습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>사용자 지정 보기, 필터, 그룹화, 목록 컨트롤 등을 정의할 수 있는 응용 프로그램의 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL은 회사 목표입니다.]</p></td> 
   <td> <p>in [!DNL goal reports]을 지정하면 조직이 목표에 소유자로 지정되었는지 여부를 나타내기 위해 각 전략적 목표에 대한 "[!UICONTROL True]/ [!UICONTROL False]" 값이 표시됩니다. </p> 
   <p>이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront Goals]. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 개요 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 문제]</td> 
   <td> <p>일반적으로 작업이나 프로젝트 완료를 방지하는 데 문제가 있음을 나타내는 계획되지 않은 작업 항목입니다. 그것은 보다 많은 작업 노력을 고려하여 평가 및 평가된다</p> <p>[!UICONTROL Issue]는 [!UICONTROL Help Desk] 요청일 수도 있습니다. [!UICONTROL Change Orders], [!UICONTROL Requests] 및 [!UICONTROL Bugs]도 [!UICONTROL Issues]입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>각 유형과 연관된 라우팅, 트레이지 또는 트래픽 프로세스의 정의와 문제 유형의 정의를 제어하는 프로세스 및 규칙입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>문제 삼중 및 완료를 담당하는 팀 또는 사용자입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>팀이 미리 정의된 결과물 세트를 생성하는 기간입니다.</td> 
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
   <td> <p>사용자의 일상적인 작업 기능 및 책임을 식별하는 데 사용됩니다. 작업 역할을 작업 항목에 지정하여 특정 사용자에게 작업 프로세스를 지정하지 않고 완료하는 데 필요한 기술을 식별할 수 있습니다. </p> <p>사용자는 두 개 이상의 역할을 가질 수 있습니다. 예를 들면 그래픽 디자이너 또는 컨설턴트가 있습니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>프로젝트, 작업, 문제 및 기타 개체의 [!UICONTROL 업데이트] 영역에 나타나는 추적된 필드에 대한 시스템 업데이트에 대한 정보를 알려주는 보고 가능한 개체입니다.</p> <p>자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL Updates] 영역에 대한 보고서</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 간판 플래그]</td> 
   <td> <p>[!UICONTROL Task] 보고서 또는 [!UICONTROL Issue] 보고서에서 [!UICONTROL Kanban Flag] 필드는 [!UICONTROL Kanboard]의 스토리에 설정된 플래그 상태를 표시합니다. 가능한 값은 [!UICONTROL On Track], [!UICONTROL Ready To Pull], [!UICONTROL이 차단되었습니다]입니다.</p> <p>[!UICONTROL 간판 스토리 보드의 스토리에 플래그 상태를 설정하는 방법에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">[!UICONTROL 간판 보드]의 스토리에 플래그를 사용합니다.</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>기업이 주요 비즈니스 목표를 얼마나 효과적으로 달성하고 있는지 보여주는 측정 가능한 가치</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>종속 작업을 시작할 때까지 이전 작업의 [!UICONTROL 계획된 완료 날짜]가 경과된 후 경과해야 하는 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>[!UICONTROL Lag]를 계산하는 방법입니다. 다음을 수행할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Days] (일 수)</li> 
     <li>[!UICONTROL Calendar Days](휴일 무시)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL 요일]</li> 
    </ul> <p>자세한 내용은 의 "[!UICONTROL Lag Types 개요]" 섹션을 참조하십시오. <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">지연 유형 개요</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 큰 축소판]</td> 
   <td> <p> [!UICONTROL 문서] 목록이나 보고서에서 문서의 미리 보기를 축소판으로 표시합니다. </p> <p>선택 <strong>[!UICONTROL 큰 축소판]</strong> 보고서에서 400픽셀 단위의 축소판을 보려면</p> <p>축소판의 크기는 목록 또는 보고서에서 열 너비를 수정할 때 조정됩니다.</p> <p>이 문서에서 "[!UICONTROL Thumbnail]도 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>보고서 목록에서 이 필드에는 가장 최근에 보고서를 본 최대 10명의 사용자가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>이 필드에는 객체 소유자가 객체에 마지막으로 입력한 업데이트 즉, 객체에 대한 소유자의 가장 최근 활동이나 상호 작용이 표시됩니다.</p> <p>다음 [!DNL Last Condition Note] 개체의 마지막 메모 텍스트가 삭제된 경우 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance 업데이트 날짜]</td> 
   <td>[!UICONTROL 프로젝트] 보고서에서 이 필드는 프로젝트 재정이 마지막으로 계산되고 업데이트된 날짜와 시간을 캡처합니다. 프로젝트 재정에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">프로젝트 재무 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막 참고]</td> 
   <td> <p>이 필드에는 사용자가 객체에 마지막으로 입력한 업데이트가 표시됩니다. 객체에 대한 가장 최근 활동이나 상호 작용입니다.</p> <p>개체의 마지막 메모 텍스트가 삭제된 경우 [!UICONTROL 마지막 참고] 열이 비어 있습니다. 객체에 새 메모를 입력하면 마지막 메모가 되고 열에 다시 표시됩니다.</p>
   <p>이 필드가 [!UICONTROL 작업] 보고서에 추가되면 문제, 하위 작업, 문서 등과 같은 하위 개체에 남아 있는 모든 업데이트가 발생합니다. 작업 — 이 열에 표시되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막으로 본 사람]</td> 
   <td> <p>보고서 목록의 이 필드에는 마지막으로 보고서를 본 사용자에 대한 정보가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 마지막으로 본 날짜]</td> 
   <td> <p>보고서 목록에서 이 필드는 보고서가 마지막으로 표시된 날짜를 표시합니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 레이아웃 템플릿]</td> 
   <td>시스템 관리자 또는 그룹 관리자가 특정 사용자의 작업 공간에 표시되는 탭과 보고서를 식별하도록 정의합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레이아웃 유형]</td> 
   <td>[!UICONTROL 사용자 지정 보기]와 함께 [!UICONTROL 레이아웃 유형]은 [!UICONTROL 사용자 지정 보기]의 유형을 지정합니다. 현재 목록만 사용할 수 있습니다. 나중에 [!UICONTROL Detail](개체의 [!UICONTROL Detail] 보기)를 사용할 수 있습니다.</td> 
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
   <td>[!UICONTROL Library Task]</td> 
   <td>응용 프로그램에서 [!UICONTROL 작업] 및 [!UICONTROL 템플릿 작업]의 일관된 이름을 제공하는 데 사용되는 단일 작업의 템플릿입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이선스 유형]</td> 
   <td>[!UICONTROL 액세스 수준]에 할당된 라이선스 유형입니다. [!UICONTROL Full User], [!UICONTROL Limited User] 또는 [!UICONTROL Requester]입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라이선스 제한 계획]</td> 
   <td> <p>[!UICONTROL 그룹] 보기 또는 보고서에서 이 필드는 [!UICONTROL 홈 그룹]으로 지정된 각 그룹을 가진 사용자에게 할당할 수 있는 최대 [!UICONTROL Plan] 라이센스 수를 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>[!UICONTROL 그룹] 보기 또는 보고서에서 이 필드는 [!UICONTROL 홈 그룹]으로 지정된 각 그룹을 가진 사용자에게 할당할 수 있는 최대 [!UICONTROL Work] 라이센스 수를 표시합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>라이센스 유형으로서 [!DNL Access Level] 여기에는 문제를 제출하고 메모를 입력하고 문서를 업로드할 수 있는 보기 전용 권한이 포함되어 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>사용자 지정 필터, 보기 및 그룹화를 개별 사용자에게 연결하거나 모든 사용자에게 전체적으로 연결할 수 있는 [!UICONTROL 인터페이스 설정]의 일부입니다.</p> </td> 
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
   <td> <p>[!UICONTROL Project]의 [!UICONTROL 업데이트 유형] 중 하나입니다. 이 설정을 사용하면 "[!UICONTROL 다시 계산 타임라인]"을 클릭할 때만 [!UICONTROL 프로젝트 예상] 및 [!UICONTROL 계획됨] 타임라인을 업데이트할 수 있습니다. 이러한 방식으로 설정된 프로젝트는 간단한 다시 계산 프로세스 및 프로젝트의 프로젝트 또는 작업이 업데이트되는 동안 무시됩니다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 [!UICONTROL Update Type]을 선택합니다. </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>현재 로그인한 사용자를 나타냅니다. </p> <p>다른 사용자와 보고서를 공유할 때 보다 일반적인 보고서를 만들려면 필터에 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 정보가 항상 사용자 지정되므로 로그인한 사람에 따라 다른 정보를 표시하는 보고서만 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최대 사용자]</td> 
   <td> <p>더 이상 사용되지 않는 필드입니다. 이 필드에 표시될 수 있는 모든 정보는 [!DNL Workfront] 이 제거되어 필드를 업데이트할 수 없습니다. </p> <p>이전 릴리스 [!DNL Workfront]작업 역할을 만들거나 편집할 때 이 필드를 업데이트할 수 있습니다. 각 프로젝트에서 역할과 연결할 수 있는 총 사용자 수가 표시됩니다. 프로젝트에서 할당할 수 있는 사용자 수를 제한하지 않고 0의 값을 사용할 수 있습니다. </p>일부 보고서 및 목록에서는 필드를 계속 볼 수 있지만 표시되는 정보는 업데이트할 수 없습니다. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 이정표]</td> 
   <td> <p>작업을 완료했을 때 프로젝트의 주요 지점이 달성되었음을 나타내기 위해 작업에 연결할 수 있는 마커입니다. 일반적으로 이정표를 사용하여 프로젝트의 단계 완료나 중요한 활동 세트와 같은 중요한 이벤트를 표시할 수 있습니다. [!UICONTROL Milestones]은 일반적으로 상위 작업과 연결됩니다. 작업에 이정표를 연결하려면 먼저 이정표를 만들어야 합니다. 이정표에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">이정표 경로 만들기</a> 및 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">작업과 이정표 연결</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이정표 경로]</td> 
   <td>[!UICONTROL milestones] 컬렉션. [!UICONTROL 이정표 경로]는 [!UICONTROL 이정표] 세트가 다른 프로젝트와 특정 유형의 [!UICONTROL 이정표]가 있는 프로젝트를 구분하는 데 프로젝트에서 사용됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 이정표 작업]</td> 
   <td>측정할 보고서 가능 이벤트를 나타내는 플래그 지정된 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>의 시나리오 내에서 단일 단계 [!DNL Workfront Fusion] 에서는 연결된 앱을 기반으로 일부 기능을 수행합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>이 항목이 필터에서 참조되면 로그인된 사용자와 동일한 [!UICONTROL 기본 역할]을 가진 사용자 또는 로그인한 사용자의 [!UICONTROL 기본 역할]에 할당된 작업 항목이 표시됩니다.</p> <p>다른 사용자와 보고서를 공유할 때 보다 일반적인 보고서를 만들려면 필터에 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 정보가 항상 사용자 지정되므로 로그인한 사람에 따라 다른 정보를 표시하는 보고서만 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>이 항목이 필터에서 참조되면 이 필드에는 로그인한 사용자의 [!UICONTROL 홈 팀]에 속하는 사용자 또는 로그인한 사용자의 [!UICONTROL 홈 팀]에 할당된 작업 항목이 표시됩니다. </p> <p>다른 사용자와 보고서를 공유할 때 보다 일반적인 보고서를 만들려면 필터에 이 필드를 사용하는 것이 좋습니다. 이렇게 하면 로그인한 사용자에 대해 정보가 항상 사용자 지정되므로 로그인한 사람에 따라 다른 정보를 표시하는 보고서만 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 이름 지정 규칙]</td> 
   <td>데이터를 사용하여 프로젝트, 작업 및 결과물의 이름을 생성하는 조직 전체의 규칙 세트입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>수동 코딩 또는 API 구성이 필요 없는 통합. 또한 "즉시 사용 가능한" 통합이라고도 합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 탐색 메뉴]</td> 
   <td>[!UICONTROL Workfront]의 기본 영역에 연결하는 애플리케이션의 맨 위 가운데 패널입니다.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL 새 숫자 값]</td> 
   <td>[!UICONTROL Journal Entry] 보고서에서 [!UICONTROL Old Number Value]를 대체하는 필드의 업데이트된 값이 표시됩니다.
   자세한 내용은 이 문서에서 "[!UICONTROL 이전 번호 값]"을 참조하십시오.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>지정 완료에 할당되지 않은 일수입니다. 보통 휴가일이거나 휴일이나 주말이에요</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참고]</td> 
   <td>에 대한 설명 또는 업데이트 [!DNL Workfront] 개체.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참고 텍스트]</td> 
   <td> <p>그러면 사용자가 객체에 입력한 업데이트 텍스트가 표시됩니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 연결된 목표 수]</td> 
   <td> <p>[!UICONTROL 프로젝트] 보고서에서 프로젝트와 연결된 전략적 목표 수입니다. 프로젝트를 전략적 목표와 연관시키는 방법에 대한 자세한 내용은 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">의 목표에 프로젝트 추가  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>전략 목표에 대한 자세한 내용은 이 문서에서 "[!UICONTROL Goal]"을 참조하십시오.</p> 
   <p>이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront Goals]. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!UICONTROL Adobe Workfront 목표]에서 목표에 프로젝트 추가</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>표시되는 정보 [!DNL Adobe Workfront] 는 [!DNL Workfront] 데이터베이스. 객체는 Workfront에서 정보를 유도하는 것입니다. 객체 중 일부는 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL 사용자 지정 양식]</li>
     <li>[!UICONTROL 사용자 지정 필드]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL 청구율]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL 템플릿 작업]</li>

<p><b>메모</b></p>
  <p>이것은 광범위한 목록이 아닙니다. </p>

</ul> <p>자세한 내용은 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">[!UICONTROL Adobe Workfront]의 개체 이해</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 개체 유형]</td> 
   <td>모든 사용자 지정 양식이 포함된 보고서나 목록을 만드는 경우 이 필드를 보기 또는 필터로 사용하여 각 양식과 연결된 개체 유형을 확인할 수 있습니다. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL 이전 숫자 값]</td> 
   <td>[!UICONTROL Journal Entry] 보고서에는 업데이트되기 전의 필드의 원래 값이 표시됩니다. 필드의 값이 업데이트되면 [!UICONTROL Journal Entry] 보고서에 [!UICONTROL 새 번호 값]으로 표시됩니다. 자세한 내용은 "[!UICONTROL 새 번호 값]"을 참조하십시오.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>[!UICONTROL 프로젝트 업데이트] 유형 중 하나입니다. 이 옵션을 선택하면 [!UICONTROL Project Projected] 및 [!UICONTROL Planning] 타임라인은 프로젝트 또는 프로젝트 내의 작업에 업데이트 또는 변경이 있을 때만 업데이트됩니다. 매일 밤 그 프로젝트를 업데이트하지는 않는다.</p> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형을 선택합니다 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op 작업]</td> 
   <td> <p>에서 [!UICONTROL Issues]의 이름입니다. [!DNL Workfront] 데이터베이스, 텍스트 모드 보고서 또는 계산된 사용자 지정 데이터에 사용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>완료되지 않지만 작업 중인 문제 또는 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>조직도의 약어입니다. 조직의 계층을 보여주는 차트입니다. 또한 [!UICONTROL 사용자] 세부 정보 화면의 탭에 [!UICONTROL 사용자]의 [!UICONTROL Company] 및 [!UICONTROL Reporting] 관계를 표시하고 설정할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 조직 설정]</td> 
   <td>조직의 [!UICONTROL Companies], [!UICONTROL Groups] 및 [!UICONTROL Security Profiles]를 정의합니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 기타 그룹]</td> 
   <td> <p>사용자를 나열하는 보고서 또는 보기에서 이 필드는 각 사용자가 멤버인 모든 그룹을 표시합니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할과 연관된 통화입니다. 이는 [!UICONTROL 설정] 영역에 설정된 [!UICONTROL 기본 통화]의 재정의입니다. [!DNL Workfront] 관리자 </p> 
     <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할의 선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 청구 비율입니다.</p> 
     <p> 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 통화 비용/시간 대체]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 작업 역할] 보고서에서 작업 역할의 선택한 [!UICONTROL 재정의 통화]를 사용하는 작업 역할의 시간당 비용입니다. </p> 
     <p>자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">작업 역할 만들기 및 관리</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>지정된 객체의 완료를 담당하는 사용자입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 목표] 보고서에는 전략적 목표에 할당된 소유자 유형이 표시됩니다. 다음은 목표 소유자 유형입니다.</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>목표 소유자가 조직인 경우 이 필드에 값이 표시되지 않습니다. </p> 
     <p>이 경우 추가 라이센스가 필요합니다. 에 대한 자세한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 개요</a>. </p> 
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
   <td> <p>[!UICONTROL 매개 변수]는 사용자 지정 필드입니다. 모든 매개 변수에 대한 보고서 또는 시스템의 사용자 지정 필드를 작성할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>보고서에서 이 필드는 개체의 상위에 대한 정보를 표시합니다. 예를 들어, [!UICONTROL 문제] 보고서에서는 문제가 기록되는 작업 또는 프로젝트에 대한 정보를 표시할 수 있습니다. 작업 보고서에는 직접 상위 작업 또는 프로젝트에 대한 정보가 표시될 수 있습니다. 에 부모가 있을 수 있는 객체에 대한 자세한 정보 [!DNL Workfront]를 참조하려면 문서의 "개체 간 종속성 및 계층" 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">의 개체 이해 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위 지연]</td> 
   <td>[!UICONTROL Parent Task] 시작과 [!UICONTROL Subtask] 시작 사이에 경과해야 하는 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위 작업]</td> 
   <td>[!UICONTROL 요약 작업]이라고도 합니다. 이 작업은 하위 작업([!UICONTROL 하위 작업]이라고도 함)이 있는 작업입니다. 상위 작업의 [!UICONTROL Duration], [!UICONTROL Work Required] 및 [!UICONTROL Percent Complete]는 하위 작업에서 계산됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>시스템에 정의된 기본 예약보다 용량이 적은 라이센스가 있는 사용자입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>작업, 프로젝트 또는 문제와 관련된 작업의 완료율을 표시하는 프로젝트, 작업 또는 문제 필드입니다.</p> <p>문제 및 작업 작업에 대해 이 필드를 수동으로 업데이트할 수 있습니다. </p> <p>프로젝트 및 상위 작업의 경우 이 필드는 모든 작업 작업의 롤업이며 수동으로 업데이트할 수 없습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">프로젝트 [!UICONTROL 완료율] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 권한]</td> 
   <td> <p>객체에 대한 작업을 완료하거나 항목을 볼 수 있도록 일반적으로 사용자에게 부여된 권한. 다음에 대한 권한을 부여할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL 프로그램]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL 그룹화]</li> 
    </ul> <p>자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 권한 공유 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획]</td> 
   <td> <p>는 [!DNL Workfront] 시스템. 사용자는에서 모든 기능에 액세스하려면 이 권한이 있어야 합니다 [!DNL Workfront].</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (다음 [!DNL Scenario Planner])</td> 
   <td> <p>계획은 [!DNL Workfront] 시나리오 플래너. 회사의 근장기적인 미래에 대한 전략에 대해 개략적으로 설명하고 각 높은 수준의 결과를 식별하고 이를 계획에 추가할 수 있습니다 [!DNL Workfront] 시나리오 플래너. </p> <p>표시할 수 없습니다 [!DNL Scenario Planner] 는 보고서에서 계획하며, [!DNL Workfront] API. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Scenario Planner] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획됨]</td> 
   <td> <p>어떤 것이 발생하도록 예약된 시간대입니다. 에서 프로젝트, 작업 또는 문제를 만들 때 [!DNL Workfront]을(를) 설정하고 계획 시작 및 종료 날짜와 계획 기간을 설정하고 계획 기간을 설정합니다. 이러한 값은 항목이 완료되는 데 걸리는 시간을 나타내는 원래 의도나 추정치를 나타냅니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planning Benefits]</td> 
   <td>프로젝트 관리자가 프로젝트를 완료하면 조직에 금전적 이점이 있는지 여부를 추정하기 위한 수동 입력입니다. 이 값을 지정하는 것은 프로젝트에 대한 [!UICONTROL Business Case] 작성을 수행하는 과정의 일부일 수 있습니다. 이 값을 업데이트하려면 프로젝트에 대한 [!UICONTROL 관리] 권한이 있어야 합니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 계획된 예산 시간]</td> 
   <td> <p>[!UICONTROL Scheduled Hour] 보고서에서 [!UICONTROL Resource Planner]에 있는 프로젝트 또는 [!UICONTROL Job Roles]에 대해 예산책정된 시간 크기를 표시합니다. </p> <p>[!UICONTROL Resource Planner]의 프로젝트 또는 역할 예산 지정에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!UICONTROL Project] 및 [!UICONTROL Role] 보기를 사용하는 [!UICONTROL Resource Planner]의 예산 리소스</a>. [!UICONTROL 예산책정된 시간] 보고서에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">보고서: 예산책정 시간</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 완료 날짜]</td> 
   <td> <p>[!UICONTROL 계획 완료 날짜]를 선택한 날짜로 수동으로 설정할 수 있습니다. [!UICONTROL 계획된 완료 날짜]를 설정하지 않으면, [!DNL Workfront] 자동으로 설정합니다. 자동으로 설정되면 [!UICONTROL 계획 완료 날짜]는 [!UICONTROL 계획 시작 날짜] + [!UICONTROL 기간]입니다.</p> <p>자세한 내용은 다음 문서를 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">작업 개요 [!UICONTROL 계획된 완료 날짜]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">프로젝트 [!UICONTROL 계획된 완료 날짜] 설정</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planning Cost]</td> 
   <td> <p>프로젝트의 [!UICONTROL Planning Labor Cost] 및 [!UICONTROL Planning Expense Cost]의 합계입니다. 프로젝트에 대한 [!UICONTROL 계획된 위험 비용]은 포함되지 않습니다.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 기간]</td> 
   <td> <p>작업의 [!UICONTROL 계획된 기간]은 일반적으로 작업의 [!UICONTROL 기간]과 동일합니다. 이 값은 작업의 [!UICONTROL 계획 시작]과 [!UICONTROL 계획 완료 날짜] 간의 일 차이를 나타냅니다. </p> <p>작업에 [!UICONTROL Duration] 유형이 [!UICONTROL Tivation Driven]인 [!UICONTROL Duration]이 있는 경우 작업에 할당하는 리소스 수에 따라 [!UICONTROL Planning Duration]이 작업의 [!UICONTROL Duration]과 다를 수 있습니다. </p> <p>예를 들어 [!UICONTROL Duration] 유형이 [!UICONTROL Effort Driven]인 작업에 [!UICONTROL Duration]이 3일이며 전체 시간표가 있는 리소스 하나를 작업에 할당하면 [!UICONTROL Planning Duration]도 3일입니다. 동일한 작업에 전체 시간표가 있는 세 리소스를 할당하면 [!UICONTROL 기간]은 3일 동안 유지되지만 [!UICONTROL Planning Duration]은 1일이 됩니다. [!UICONTROL Planning Duration]은 새 [!UICONTROL Planning Duration]을 반영하도록 작업의 [!UICONTROL Planning Start] 및 [!UICONTROL Planning Completed Completion] 날짜도 변경합니다. 따라서 프로젝트의 타임라인에도 영향을 받습니다. </p> <p>작업에 대한 [!UICONTROL 기간]과 [!UICONTROL Planning Duration]의 차이점에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">작업에 대한 [!UICONTROL Planning Duration]과 [!UICONTROL Duration] 간의 차이점</a>.</p> <p>프로젝트 및 문제에 [!UICONTROL 계획된 기간]이 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 기간 분]</td> 
   <td> <p>프로젝트 또는 문제에 대한 [!UICONTROL 계획된 기간 분]은 프로젝트의 [!UICONTROL 기간]이거나 분 단위입니다. </p> <p>작업에 [!UICONTROL Planning Duration Minutes] 필드가 없습니다. </p> <p>[!UICONTROL Template Tasks]에는 작업의 [!UICONTROL Planning Duration]을 분 단위로 표시하는 [!UICONTROL Planning Duration Minutes] 필드가 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 비용]</td> 
   <td> <p>프로젝트 또는 작업에 대해 기록된 모든 비용에 대한 [!UICONTROL 계획 금액]의 합계.</p> <p><b>예</b></p>
   <p>작업 1에 대한 비용을 생성하고 [!UICONTROL 계획 금액] 필드에 $600.00을 입력하면 이 작업에 대한 [!UICONTROL 계획 비용]은 $600.00입니다. </p> 
   <p>프로젝트의 경우, [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL 계획 비용]을 계산합니다.</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 시간]</td> 
   <td> <p>이 필드는 [!UICONTROL 프로젝트], [!UICONTROL 작업]에 표시되고 [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] 및 [!UICONTROL Utilization] 보고서와 같은 영역, 프로젝트, 작업 또는 문제에 대한 보고서, 리소스 관리 도구에 대해 설명합니다. </p> <p>프로젝트 소유자가 각 작업이나 문제가 완료되는 데 걸리는 시간을 보여 줍니다. 프로젝트의 경우 일반적으로 프로젝트의 작업에서 [!UICONTROL 계획 시간]의 롤업입니다. </p> <p>[!UICONTROL Planning Hours] 필드는 보기 위치에 따라 다른 정보를 표시할 수 있습니다. 계획된 시간에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">계획 시간 개요</a>.</p> <p>계획된 시간은 [!DNL Workfront] 데이터베이스. 이 필드를 사용하여 계산을 작성할 때는 시간이 분으로 표시되는지 확인해야 합니다.<br></p> <p>기본적으로 계획 시간은 작업 항목의 기간 내의 모든 일수와 작업에 지정된 모든 자원에 대해서도 동일하게 분배됩니다. 사용자는 작업 항목에 대한 일일 계획 시간 또는 각 할당자에 대한 개별 계획 시간을 갱신할 수 있습니다.</p> <p>이 필드를 업데이트하면 프로젝트, 작업 및 문제에 따라 다릅니다. </p> 
    <ul> 
     <li> <p>문제의 경우 이 필드를 수동으로 업데이트할 수 있습니다. 문제 계획 시간이 프로젝트 계획 시간에 추가되지 않습니다. </p> <p>팁: 문제 보고서에서 [!UICONTROL Planning Hours] 필드 중 하나가 [!UICONTROL Work] 필드로 바뀝니다. 이 필드는 문제에 대한 계획 시간 수를 표시합니다. 자세한 내용은 이 표의 "작업" 또는 "[!UICONTROL 작업]" 필드를 참조하십시오. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>작업의 경우 작업의 [!UICONTROL 기간 유형]이 [!UICONTROL Calculated Assignment] 또는 [!UICONTROL Simple]인 경우 이 필드를 수동으로 업데이트할 수 있습니다. 이 필드는 [!DNL Workfront] 작업의 [!UICONTROL Duration Type]이 [!UICONTROL Calculated Work] 또는 [!UICONTROL Activity Driven]인 경우<br>[!UICONTROL 작업 기간]에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">작업 [!UICONTROL 기간] 및 [!UICONTROL 기간 유형] 개요</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>프로젝트의 경우 [!DNL Workfront] 프로젝트의 모든 작업에서 모든 계획 시간을 추가하여 계획 시간을 계산합니다. </p> </li> 
    </ul> <p><b>팁</b></p> <p>텍스트 모드 및 참조 추가 필드도 사용하여 [!UICONTROL project], [!UICONTROL task] 또는 [!UICONTROL 문제] 보고서에 [!UICONTROL 계획 시간]을 표시할 수 있습니다. 자세한 내용은 "<code>work</code>", "[!UICONTROL Work]" 및 "<code>workRequiredExpression</code>" 필드를 생성할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 인건비]</td> 
   <td> 
    <p>작업의 경우 사용자 또는 역할의 시간별 비율과 사용자 또는 역할에 지정된 시간 수를 곱합니다.</p> <p>프로젝트의 경우 모든 작업의 총 [!UICONTROL Planning Labor Cost]입니다.</p> <p>사용자 또는 롤의 사용 여부는 지정된 작업에 대해 선택된 원가 유형에 따라 달라집니다. </p> <p>자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md">비용 추적</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planning Revenue]</td> 
   <td> <p>작업 및 프로젝트에는 [!UICONTROL Planning Revenue]에 대한 값이 표시될 수 있습니다 [!DNL Workfront]. [!UICONTROL Planning Revenue]는 프로젝트에 있는 작업의 [!UICONTROL Planning Hours]와 연결된 금액을 나타냅니다. 프로젝트의 경우 프로젝트의 [!UICONTROL 고정 수익]을 포함할 수도 있습니다. </p> <p>작업의 경우 [!UICONTROL Planning Hours] 작업과 연결된 수익입니다. 모든 작업의 계획 시간은 프로젝트 [!UICONTROL 계획 시간] 계산에 기여하기 위해 프로젝트의 계획 시간으로 롤업됩니다. </p> 
   <p>[!DNL Workfront] 다음 공식을 사용하여 작업 및 프로젝트에 대한 [!UICONTROL 계획 수익]을 계산합니다.</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>[!UICONTROL 프로젝트 세부 정보] 영역과 프로젝트 보고서에 표시되는 [!UICONTROL 계획 수익] 프로젝트는 [!UICONTROL 활용률] 보고서에 표시되는 계획 매출과 다릅니다. </p> <p>[!UICONTROL 프로젝트 세부 정보] 영역의 [!UICONTROL 계획 수익]은 프로젝트의 고정 수익과 작업 수입을 반영합니다. [!UICONTROL 활용률 보고서]의 [!UICONTROL 계획 수익]은 프로젝트의 작업에만 연결된 [!UICONTROL 계획 수익]을 표시합니다. </p> 
     <p><b>예</b></p>  
      <p>프로젝트에 10시간이 있고, 시간당 요금이 $20인 컨설턴트에 할당되고, 프로젝트에 $100가 있는 경우 [!UICONTROL 고정 수익] 보고서에는 [!UICONTROL Planning Revenue](작업 시간과 연관된 [!UICONTROL Planning Revenue]에 대해 $200가 표시됩니다.) [!UICONTROL 프로젝트 세부 정보] 섹션에는 작업의 [!UICONTROL 계획 수익] 및 프로젝트에 대한 고정 수익이 $300로 표시됩니다. </p> 
    <p>의 매출 추적에 대한 정보 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">청구 및 수익 개요</a>. </p> 
    <p>[!UICONTROL Utilization Report]의 [!UICONTROL Planning Revenue] 계산에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">자원 사용률 정보 보기 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 위험 비용]</td> 
   <td> <p>발생할 확률에 따라 프로젝트 팩토링에 대한 모든 위험의 [!UICONTROL 잠재적 비용]의 합계입니다. 이 금액은 프로젝트의 [!UICONTROL 계획 비용]에 포함되지 않습니다.</p> <p>프로젝트의 [!UICONTROL Planning Risk Cost]는 다음 공식을 사용하여 계산됩니다.</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>관리자가 정의한 탭과 포털 섹션 모음이며 [!DNL Workfront] 애플리케이션 [!UICONTROL 홈] 및 기타 대시보드.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 포털 섹션]</td> 
   <td>대시보드 또는 포털 페이지에 있는 탭의 구성 요소 중 하나. 일반적으로 단일 보고서, 차트, 달력 또는 주요 정보 목록입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal 탭]</td> 
   <td>최대 3개의 포털 섹션이 포함된 포털 또는 대시보드의 탭입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>통합 특성을 갖는 프로젝트 모음입니다. 이러한 프로젝트들은 일반적으로 동일한 자원, 예산 또는 시간 슬롯에 대해 경쟁합니다. Portfolio을 프로그램으로 나누고 프로젝트를 Portfolio에 추가하기 전에 프로그램과 연결할 수 있습니다.</p> <p>포트폴리오에 대한 자세한 내용은 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">의 Portfolio 개요 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 관리]</td> 
   <td>컬렉션 또는 관련 프로그램 및 프로젝트 작업을 관리하는 데 중점을 둔 실무 영역입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 최적화 프로그램]</td> 
   <td>A [!DNL Workfront] 포트폴리오 내의 프로젝트를 평가하고 우선 순위를 지정하는 데 도움이 되는 도구입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio 소유자]</td> 
   <td>포트폴리오의 우선 순위 지정 및 예산을 담당하는 이해 당사자입니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 잠재적인 위험 비용]</td> 
   <td>목록 및 보고서에서 찾을 수 있는 프로젝트 필드입니다. 이 경우 프로젝트와 관련된 위험에 대한 잠재적 비용이 표시됩니다. 자세한 내용은 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">잠재적 위험 비용 계산 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Previous]</td> 
   <td> <p>종속 작업이 완료되기 전에 완료해야 하는 작업입니다. 또한 다른 작업에 대해 [!UICONTROL 종속성]으로 표시된 작업입니다. 선행 작업을 통해 계획자는 다른 작업이 완료된 후 작업을 시작하는 등의 순서 종속성 논리를 설정할 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">작업 선행 작업 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>사용자가 속한 회사가 사용자 설정에서 지정된 대로 해당 사용자에 속합니다. 회사는 프로젝트와 연결할 수도 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기본 연락처]</td> 
   <td><p>[!UICONTROL Primary Contact]는 문제의 작성자이며 [!DNL Workfront] 누군가 문제를 만들면 있는 경우 이 필드를 수동으로 업데이트할 수 있습니다 [!DNL Manage] 문제에 대한 권한. 문제에 기본 연락처는 하나만 있을 수 있습니다.</p> 
   <p>기본 연락처를 변경하면 원래 기본 연락처로 지정된 사용자에게는 여전히 해당 문제에 대한 [!UICONTROL 관리] 액세스 권한이 있습니다.</p>
   <p>문제를 작업 또는 프로젝트로 변환할 때 의 [!UICONTROL 기본 연락처]로 지정된 사용자는 프로젝트 또는 작업의 [!UICONTROL Converted Issue Originator]가 됩니다. 문제가 변환된 후 문제에 대한 [!UICONTROL 기본 연락처]가 업데이트되면 전환이 발생한 시점에 [!UICONTROL Converted Issue Originator]가 문제의 [!UICONTROL 기본 연락처]로 유지됩니다. 이 문서에서 "[!UICONTROL Converted Issue Originator]"도 참조하십시오.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Task, Issue 또는 Project에 할당하여 중요도를 지정할 수 있는 값입니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>[!UICONTROL 참고] 또는 [!UICONTROL 문서]에서 이 옵션은 대부분의 뷰어에 해당 개체를 숨깁니다. 개인 도움말 데스크 큐의 경우, 큐 팀의 사용자만 [!UICONTROL 도움말 데스크] 영역을 통해 해당 큐에 문제를 제출할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>사용자 계정에 대한 모든 정보입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>잘 정의된 혜택을 얻기 위해 유사한 프로젝트를 함께 그룹화할 수 있는 포트폴리오 내의 하위 집합입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 프로그램 관리]</td> 
   <td>프로그램을 건전하게 유지하고 정의된 프로그램 이점을 달성하기 위한 프로젝트 간 종속성, 위험, 문제, 요구 사항 및 솔루션 관리</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 프로그램 소유자]</td> 
   <td>프로젝트 목표가 회사 목표에 부합하도록 활동을 감독 및 구성할 책임이 있는 이해 당사자</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>[!UICONTROL 목표] 보고서에는 전략적 목표가 완료되는 정도에 대한 백분율이 표시됩니다. 진행률 백분율이 숫자로 표시됩니다. 전략 목표에 대한 자세한 내용은 이 표의 "[!UICONTROL Goal]"을 참조하십시오.</p> <p>이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront] 목표. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 의 목표에 프로젝트 추가 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>프로젝트, 작업 및 목표 보고서에서 이 필드에는 프로젝트, 작업 또는 전략 목표에 대한 진행 상태가 표시됩니다. 자세한 내용은 다음 문서를 참조하십시오.</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">프로젝트 진행 상태 개요</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">작업 진행 상태 개요</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">목표 진행 상태 및 조건 개요 [!DNL Adobe Workfront Goals]</a> </p>
     <p>에 대한 [!UICONTROL Target] 보고서 및 [!UICONTROL Progress Status] [!DNL goals] 필드가 표시되는 것은 조직이 구매한 경우에만 볼 수 있습니다 [!DNL Workfront Goals]. 의 전략적 목표에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>특정 기간 내에 완료해야 하며 특정 예산과 자원을 사용해야 하는 많은 양의 작업. 관리할 수 있도록 프로젝트를 일련의 작업으로 나눕니다. 모든 작업을 완료하면 프로젝트가 완료됩니다. 프로젝트 계획에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">프로젝트 개요 계획</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 할당 계획 시간]</td> 
   <td> <p>[!UICONTROL Initiative Job Role] 보고서에는 프로젝트의 작업 또는 문제에 할당된 작업 역할과 연관된 [!UICONTROL Planning Hours] 수가 표시됩니다. 이 필드와 [!UICONTROL Initiative Job Role] 보고서 유형이 [!DNL Workfront] 회사가 구매하지 않은 경우 인스턴스 [!DNL Workfront Scenario Planner] 라이센스. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md">다음 [!DNL Workfront Scenario Planner] 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 세부 정보]</td> 
   <td>프로젝트의 현재 상태에 대한 세부 사항입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budget Cost]</td> 
   <td> <p> 목록 및 보고서에 표시되는 프로젝트의 [!UICONTROL 예산책정 비용]입니다.</p><p>이 문서에서 "[!UICONTROL Budget Cost]"도 참조하십시오.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>프로젝트 생성, 분류 및 이름 지정에 대한 임계값을 제어하는 정책 집합입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>[!UICONTROL Hour] 보고서에서 이 필드는 [!UICONTROL Project Time]의 시간 유형으로 기록된 시간과 연결된 재무 정보에 대해 예약됩니다. 프로젝트에 자체 청구 요금이 있을 수 있으며, 한 시간이 프로젝트에 직접 기록되면 해당 요금이 계산에 사용됩니다. 프로젝트 설정에 따라 프로젝트마다 다른 통화를 사용할 수 있으며, 해당 시간에 대한 통화 전환이 있을 수 있습니다. [!UICONTROL Project Overhead] 개체를 사용하면 [!DNL Workfront] 정보를 얻기 위해</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 소유자]</td> 
   <td>프로젝트의 범위, 타임라인 및 할당을 관리하는 사용자입니다. 변경 주문, 재무 변경 및 산출물에 대한 기본 승인자입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>프로젝트 일정을 개발 및 유지 관리하는 프로세스입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>각 사용자의 관계에 있어야 하는 지정된 이해 관계자 프로필입니다. in [!DNL Workfront]로 지정되며 [!UICONTROL 액세스 수준]으로 지정됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>프로젝트에 지정된 사용자 또는 역할 수집</p> <p>자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">프로젝트 팀 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 추적]</td> 
   <td>프로젝트의 상태와 범위를 측정하는 데 사용되는 데이터입니다</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>작업, 문제 또는 프로젝트의 계획된 시간 및 백분율을 기준으로 작업이 완료되는 시간의 예상 타임스탬프입니다.</p> <p>작업, 문제 또는 프로젝트의 날짜 또는 [!UICONTROL 기간]을 나타냅니다. 일반적으로 일부 작업이 이미 완료되었거나 시간이 경과한 후 작업 항목의 수명 동안 더 참인 날짜 및 기간을 지정합니다. </p> <p>예를 들어 작업의 [!UICONTROL 예상 완료 날짜]는 다음과 같은 날짜입니다 [!DNL Workfront] 은(는) 작업이 지금까지 수행된 작업 횟수, 할당된 사람 수 및 시작 날짜 이후 경과된 시간을 기준으로 작업이 완료될 것으로 예측합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 최종 기한]</td> 
   <td> <p>[!UICONTROL Document Version] 개체([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)가 들어 있는 보고서에는 이 필드에 증명 마감일의 요일, 날짜, 시간 및 연도가 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 결정]</td> 
   <td> <p>[!UICONTROL Document Version] 개체(예: [!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서)가 들어 있는 보고서에는 증명의 결정 상태(보류 중, 변경 사항 또는 승인됨)가 표시됩니다</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 이름]</td> 
   <td> <p>[!UICONTROL Document Version] 개체([!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서 등)가 들어 있는 보고서에는 이 필드에 증명 이름이 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 페이지]</td> 
   <td> <p>[!UICONTROL Document Version] 개체(예: [!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서)가 포함된 보고서의 경우 이 필드에는 증명에 포함된 페이지 수가 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 증명 진행률]</td> 
   <td> <p>[!UICONTROL Document Version] 개체(예: [!UICONTROL Document Version] 보고서 및 [!UICONTROL Proof Approval] 보고서)가 들어 있는 보고서에는 증명([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commended], [!UICONTROL Decisiontrol Decision Made])의 진행 상태가 표시됩니다.</p> <p>자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">증명 진행률 개요</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">증명 진행 및 상태 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>하나 이상의 사용자가 이미지, 텍스트 문서, 비디오 또는 대화형 웹 컨텐츠에서 변경해야 하는 컨텐츠에 표시하고 주석을 다는 검토 프로세스입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>[!UICONTROL 참고] 또는 [!UICONTROL 문서]에서 이 옵션을 사용하면 해당 개체를 다른 사용자 또는 외부 사용자가 액세스할 수 있습니다 [!DNL Workfront]. [!UICONTROL Help Desk Queue]의 경우 [!UICONTROL Public]은 문제를 제출할 수 있는 모든 사용자가 [!UICONTROL Help Desk] 영역을 통해 문제를 제출할 수 있음을 의미합니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>조직 내에서 업무 품질에 대한 인식.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>[!UICONTROL Help Desk Queue]라고도 합니다. 사용자가 문제를 제출할 수 있도록 [!UICONTROL 도움말 데스크] 영역에 게시된 프로젝트입니다. 일반적으로 큐는 버그, 프로젝트 요청 등과 같은 특정 주제에 대해 만들어집니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 큐 속성]</td> 
   <td>이러한 설정은 [!UICONTROL Help Desk]에 게시되는 프로젝트에 대한 문제 제출 규칙을 정의합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 큐 항목]</td> 
   <td> <p>문제를 제출하는 사용자가 항목을 선택할 수 있도록 하는 [!UICONTROL Help Desk Queue]의 속성입니다. 항목은 다음 작업을 수행할 수 있습니다.</p> 
    <ul> 
     <li>사용자 지정 데이터 양식과 연결</li> 
     <li>선택한 항목의 공정순서 규칙 세트를 통해 사용자, 역할 또는 팀에 문제를 자동으로 지정합니다.</li> 
     <li>선택한 항목의 라우팅 규칙 세트를 통해 문제를 다른 프로젝트 또는 대기열로 이동합니다.</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">큐 항목 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>[!UICONTROL 액세스 수준] 보고서에서 [!UICONTROL 액세스 수준]의 [!UICONTROL 등급]을 수동으로 표시할 수 있습니다. 이것은 다음과 같이 사용자에게 도움이 됩니다 [!DNL Workfront] 관리자는 각 액세스 수준과 연관된 복잡도 수준을 시각적으로 확인할 수 있습니다. 예를 들어, 더 복잡한 ([!UICONTROL Plan] 수준) 액세스 수준에 대해 더 낮은 숫자를 지정하고 덜 복잡한 ([!UICONTROL Quester] 수준) 액세스 수준에 더 높은 숫자를 지정할 수 있습니다. 표준 액세스 수준의 등급을 지정할 수 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>작업 보고서의 이 필드는 백로그에 [!UICONTROL Agile] 작업이 [!UICONTROL Ready]로 표시되었는지 여부를 나타냅니다. 이 플래그는 [!UICONTROL Agile] 작업에만 적용되며, 이 작업은 [!UICONTROL Agile] 팀에 할당된 작업입니다. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL 되풀이 빈도]</td> 
   <td> <p>반복 작업의 상위의 [!UICONTROL 작업 세부 사항] 또는 [!UICONTROL 작업 편집] 상자에 표시되는 필드입니다. 되풀이 작업이 발생하는 빈도입니다. 반복 작업 만들기에 대한 내용은 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">반복 작업 만들기</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참조 번호]</td> 
   <td> <p>프로젝트, 작업 및 문제는 만들 때 자동으로 고유한 참조 번호와 연결됩니다. 프로젝트, 작업 또는 문제에 대한 [!UICONTROL Details] 페이지나 목록이나 보고서에서 [!UICONTROL Reference Number]를 볼 수 있습니다. </p> <p><b>팁</b><p><br>참조 번호가 항상 고유하므로 두 항목의 이름이 같은 경우 참조 번호로 연기할 수 있습니다. </p> <p>[!DNL Workfront] 시스템 수준에서 순차적 참조 번호를 자동으로 생성합니다. 각 프로젝트, 작업 또는 문제는 시퀀스에서 다음 사용 가능한 번호를 가져옵니다. <br></p> <p>예를 들어 사용자 A가 작업을 만드는 경우 [!DNL Workfront] 자동으로 작업을 100의 참조 번호로 할당할 수 있습니다. 사용자 B가 이 후 문제를 만들면 [!DNL Workfront] 참조 번호 101에 문제를 지정합니다. 참조 번호는 수동으로 편집할 수 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 거부 문제]</td> 
   <td>프로젝트 또는 작업 보고서에서 프로젝트 또는 작업에 대한 승인이 거부될 때 생성되는 문제입니다. 거부 문제에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">작업 항목에 대한 승인 프로세스 생성</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 남은 위험 비용]</td> 
   <td> <p>프로젝트의 [!UICONTROL Planning Risk Cost] 및 프로젝트의 모든 위험에 대한 전체 [!UICONTROL Actual Cost] 간의 차이를 보여 주는 프로젝트 필드입니다. </p> <p>프로젝트에 대한 [!UICONTROL 나머지 위험 비용]은 다음 공식을 사용하여 계산됩니다.</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>수리 또는 문제 해결을 위해 프로젝트 날짜 변경 예를 들어, 몇 달 동안 보류된 프로젝트를 정확한 날짜를 반영하도록 다시 계획해야 합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>주어진 항목에 대한 정보가 포함된 차트 또는 테이블 [!DNL Workfront] 개체 및 관련 특성을 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>중앙 집중식 단일 큐에서 트리거되며 진행 중인 작업 작업과는 관련이 없는 문제 유형입니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 요청 큐]</td> 
   <td>트래픽 및 트레이시 프로세스에서 관리하는 문제의 백로그.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 요청 속도]</td> 
   <td>요청 취수와 완료에 소요되는 총 작업 주기 시간입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>일반적으로 라이센스 유형입니다. 요청자 라이센스를 가진 사용자는 시스템에서 새로운 작업이 수행되도록 요청할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예약 시간]</td> 
   <td>사용자의 개인 시간에 지정된 일수로, 사용자가 작업에 사용할 수 없음을 나타냅니다. "[!UICONTROL Non Work Days]"를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 해결]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 문제를 참조합니다. </p> <p>보고서에서 해결 개체를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능한 객체 정보 보기 및 해결</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 프로젝트 해결]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 프로젝트를 참조합니다. </p> <p>보고서에서 해결 개체를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능한 객체 정보 보기 및 해결</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 해결]</td> 
   <td> <p>문제 보고서에서 보기 또는 필터의 이 필드를 사용하여 문제를 해결하는 작업을 참조합니다. </p> <p>보고서에서 해결 개체를 표시하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">보고서에서 해결 가능한 객체 정보 보기 및 해결</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>시스템에 존재하며 프로젝트 팀 및 작업에 할당된 사용자 및/또는 역할.</td> 
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
   <td> <p>[!UICONTROL Resource Management]는 시간 및 예산에 따라 완료되도록 가용성에 따라 리소스의 사용을 정확하게 예측할 수 있는 엔터프라이즈 도구 세트입니다. </p> <p>리소스 관리 도구를 사용하여 리소스에 대한 장기 용량 및 단기 스케줄링 요구 사항을 계획할 수 있습니다. </p> <p>의 리소스 관리에 대한 자세한 내용 [!DNL Workfront]를 참조하십시오. <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">리소스 관리 시작</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager ID]</td> 
   <td><p>프로젝트 보고서에서 필터를 만들어 특정 리소스 관리자를 찾을 때 이 옵션을 사용할 수 있습니다. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager]</td> 
   <td> <p>프로젝트 보고서 또는 목록 보기에서 프로젝트에 대한 리소스 관리 활동을 수행하도록 지정된 사용자를 표시하는 정보 필드입니다.  보고서에서 "[!UICONTROL 리소스 관리자]"를 사용하면 프로젝트의 각 리소스 관리자가 쉼표로 구분되는 리소스 관리자 목록이 표시됩니다. 주어진 프로젝트에서 최대 30명의 자원 관리자를 지정할 수 있습니다.</p> <p>자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">프로젝트 또는 템플릿에 대한 자원 관리자 지정 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner 예산책정 시간] </td> 
   <td>[!UICONTROL Resource Planner]에서 프로젝트에 대한 예산책정된 시간 및 이와 연관된 리소스입니다. 이 문서에서 "[!UICONTROL Budget Hours]"도 참조하십시오. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>고급 [!DNL Workfront] 프로젝트, 작업 역할 또는 사용자 간에 리소스를 보고 관리할 수 있는 도구입니다. 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner 예산책정된 노무비]</td> 
   <td> <p>자원 계획자를 사용하여 프로젝트 Job 역할에 대해 책정된 시간과 연관된 비용입니다. </p> <p>이 문서에서 "예산책정된 인건비"도 참조하십시오. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL 리소스 풀]</td> 
   <td> <p>자원 풀은 프로젝트와 연결할 수 있는 사용자 모음입니다. 일반적으로 동일한 자원 풀의 사용자는 동일한 부서에 속하거나 유사한 기술이나 보완적 기술을 가지고 있거나 동일한 예산으로 자금을 조달합니다. 여러 리소스 풀을 프로젝트 또는 사용자에게 연결할 수 있습니다. 리소스 풀은 프로젝트에만 할당하거나 여러 프로젝트에서 공유할 수 있습니다.</p> 
   <p>리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a>.</p> 
   <p>프로젝트 보고서에서 리소스 풀은 프로젝트와 연결된 모든 풀을 표시합니다. 그룹화에서는 이 개체를 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>특정 기간 동안 사용할 수 있는 시간 수와 보고서의 각 사용자에 대해 예약된 시간을 표시하는 보고서입니다. 이는 [!UICONTROL 일별 평균 시간] 및 할당 백분율로도 계산됩니다.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>in [!DNL Workfront Goals]를 입력하면 목표에 대한 진행률 표시기가 표시됩니다. 수동으로 업데이트하는 숫자, 백분율 값 또는 통화 금액일 수 있습니다. 보고서에 결과를 표시할 수 없으며 를 통해 결과에 액세스할 수 없습니다 [!DNL Workfront] API. 활동에 대한 자세한 내용은 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront 목표의 결과 및 활동 시작</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>작업 또는 프로젝트에 대한 청구 가능한 금액입니다. 양은 시간별, 고정 또는 두 가지 조합일 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>매출 유형은 작업이 수익을 발생시키는 방법을 결정합니다. 일부 예로는 [!UICONTROL Fixed Hourly], [!UICONTROL Role 시간별] 및 [!UICONTROL Role Hour W/Cap] 등이 있습니다. 의 매출 추적에 대한 정보 [!DNL Workfront] 참조 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">청구 및 수익 개요</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>일반적으로 라이센스 유형입니다. [!UICONTROL Reviewer] 라이센스가 있는 사용자는 시스템에서 작업 항목을 검토하고 승인할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>이는 의 다음 개념을 참조할 수 있습니다 [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>프로젝트가 얼마나 위험한지를 나타내는 프로젝트의 필드입니다. 위험 수준에 따라 프로젝트 실행에 우선 순위를 지정할 수 있습니다. 프로젝트의 위험 수준은 다음과 같습니다.</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>프로젝트에 대해 표시하는 위험 수준은 사용자 지정할 수 없습니다. </p> <p> 프로젝트의 위험 요소 업데이트에 대한 자세한 내용은 문서의 "프로젝트 설정" 섹션을 참조하십시오 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a>. 프로젝트의 위험 필드를 보고서에 표시할 수 있습니다. </p> </li> 
     <li> <p>프로젝트 수명 중에 발생할 수 있는 이벤트로, 프로젝트의 비용, 범위 또는 일정에 영향을 줄 수 있습니다. 프로젝트에 잠재적 위험을 정의하고 프로젝트의 비즈니스 사례를 작성할 때 발생할 가능성 또는 비용을 연관시킵니다. 프로젝트의 비즈니스 사례에 위험 추가에 대한 자세한 내용은 "프로젝트에서 위험 요소 생성 및 편집"을 참조하십시오. </p> <p>[!UICONTROL Business Case]에 정의된 위험을 보고서에 표시할 수 없습니다. 보고서와 목록에는 몇 가지 유형의 위험 비용만 표시할 수 있습니다. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 위험 비용]</td> 
   <td> <p>프로젝트의 위험과 관련된 비용입니다. 다음은 보고서에 표시할 수 있는 프로젝트와 관련된 위험 비용입니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 실제 비용]: 발생한 위험에 대한 실제 비용을 보여주는 위험 필드. 보고서와 목록 외에 위험을 편집하거나 만들 때 [!UICONTROL 위험 편집] 상자에서 보고서를 찾을 수 있습니다. </p> <p>프로젝트, 작업 또는 문제 비용에 대해서는 이 문서에서 "[!UICONTROL 실제 비용]"을 참조하십시오. </p> </li> 
     <li> <p>[!UICONTROL 계획된 위험 비용]: 프로젝트에 대한 모든 [!UICONTROL 잠재적 위험 비용]을 표시하는 프로젝트의 필드입니다. 이 문서에서 "[!UICONTROL Planning Risk Cost]"도 참조하십시오. </p> <p>잠재적 위험 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">잠재적 위험 비용 계산 </a>. </p> </li> 
     <li> <p>[!UICONTROL 남은 위험 비용]: 모든 위험의 [!UICONTROL 실제 비용] 합계와 [!UICONTROL Planning Risk Cost] 간의 차이를 표시하는 프로젝트의 필드입니다. 이 문서에서 "남은 위험 비용"도 참조하십시오. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>위험을 식별, 완화 및 모니터링하는 프로세스입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 역할]</td> 
   <td>이 문서에서 "[!UICONTROL 작업 역할]"을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>일반적으로 대기열 항목 또는 대기열에 대한 기본 경로(공정순서 규칙)로 인해 문제를 자동으로 지정하거나 이동합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 라우팅 규칙]</td> 
   <td>사용자, 역할 또는 팀에 문제를 자동으로 할당하거나 문제를 다른 프로젝트 또는 큐로 이동한 프로젝트 및 큐의 설정입니다. 라우팅 규칙은 일반적으로 헬프데스크 큐에서 수신 문제를 자동으로 할당하는 데 사용됩니다.</td> 
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
   <td>검색 기준이 저장된 검색. 저장된 검색을 사용하면 검색 기준을 다시 입력하지 않고도 동일한 검색을 다시 쉽게 실행할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 시나리오] (위치 [!DNL Workfront Fusion]) </td> 
   <td> <p>시나리오는 앱/서비스 간에 데이터를 전송하고 변환하는 방법을 나타내는 일련의 단계(모듈)로 구성됩니다.</p> <p>의 시나리오에 대한 정보 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 시나리오 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario](다음 중) [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>에서 [!DNL Scenario Planner], 시나리오는 계획의 사본입니다. </p> <p>다음 [!DNL Scenario Planner] 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">다음 [!DNL Scenario Planner] 개요</a>. </p> <p>시나리오 만들기에 대한 내용은 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">에서 계획 시나리오를 만들고 비교합니다. [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>근무 시간을 포함한 주간 근무 스케줄과 휴가(휴일 등) 및 예외 일수(예: 토요일 근무 일수)가 결합됩니다. 일정은 프로젝트 및 사용자에게 적용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예약 면제]</td> 
   <td>[!UICONTROL Modified Shift]라고도 합니다. 일정에 의해 정의된 일반 주별 작업 시간과 달리 예약된 일수입니다. 예를 들어, 일정이 월요일부터 금요일까지 작업으로만 설정된 토요일은 [!UICONTROL 예약 면제]가 됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 예약된 보고서]</td> 
   <td> <p>보고서 보고서를 작성할 때 [!UICONTROL 예약된 보고서] 필드를 사용하여 보고서를 배달하도록 예약된 경우 보고서 예약에 대한 정보를 표시할 수 있습니다. 이 필드에는 각 보고서의 일정에 대해 하나씩 글머리 기호 목록에 여러 개의 값이 표시됩니다. 보고서 예약에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">보고서 배달 개요</a>.</p> <p>이 필드는 여러 값을 표시하므로 그룹화에는 사용할 수 없습니다. 필터나 보기에서만 액세스할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범위 변경]</td> 
   <td>[!UICONTROL Task Duration] 또는 [!UICONTROL Previous]가 변경되는 경우와 같이 활성 상태인 경우 프로젝트 또는 작업의 범위를 변경할 때마다 메모를 생성하는 [!UICONTROL Audit Trail]입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>표시용 사용자 지정 데이터를 구성하기 위해 만들어진 자체 헤더가 있는 화면의 영역입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>섹션 간 간격 또는 테두리.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>사용자가 시스템의 특정 객체와 상호 작용할 수 있도록 허용하는 설정입니다. 이 문서에서 "[!UICONTROL 액세스 수준]"도 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 설정]</td> 
   <td>관리자가 시스템 구성 및 환경 설정을 설정할 수 있는 영역입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity]는 항목이 작업 완료에 미치는 영향을 나타냅니다. 예를 들어, [!UICONTROL Severity]가 높은 문제는 작업 완료를 완전히 차단할 수 있지만 [!UICONTROL Severity]가 낮은 문제는 사소한 것일 수 있습니다.</p> <p>자세한 내용은 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 문제 심각도 업데이트</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td>이 문서에서 "[!UICONTROL Severity]"를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>다른 사용자가 의 특정 항목을 보거나 편집할 수 있도록 허용하는 작업 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack 날짜]</td> 
   <td>작업 보기 또는 보고서에서 [!UICONTROL Slack 날짜]는 작업이 프로젝트의 [!UICONTROL 완료 날짜]에 확실히 영향을 줄 수 있는 정확한 날짜를 표시합니다. 작업의 [!UICONTROL Slack 날짜]에 대한 자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">작업 Slack 날짜 개요</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>사용자에게 작업 또는 문제를 할당할 때, [!DNL Workfront] 은(는) 작업을 완료하는 데 사용할 수 있는 시간과 프로젝트에 대한 관계를 기준으로 가장 적합한 사용자가 누구인지에 대한 권장 사항([!UICONTROL Smart Assignments])을 제공합니다.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">스마트 할당 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>다른 개체의 부모 개체를 나타냅니다. 예를 들어 작업에 첨부된 문서의 이름은 [!UICONTROL Document] 보고서 또는 보기의 [!UICONTROL Source] 필드에 있습니다. 프로젝트에 의해 기록되는 문제는 문제 보고서 또는 보기의 [!UICONTROL 소스] 필드에 프로젝트 이름이 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 시작 날짜]</td> 
   <td> <p>항목에 대한 작업이 시작되도록 설정된 날짜입니다. 에는 몇 가지 시작 날짜가 있습니다 [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL 계획됨]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>[!UICONTROL 비율 보고서]에서 이것은 프로젝트 수준에서 작업 역할에 대한 새 청구 비율이 시작되는 날짜입니다. 프로젝트 관련 시간(이 일자 이후)에 이 청구 비율을 곱하여 프로젝트의 수익을 계산합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태]</td> 
   <td> <p>작업 항목 또는 전략적 목표에 대한 워크플로우 위치를 알리는 데 사용되는 표시기입니다.</p> <p>프로젝트의 경우 [!UICONTROL 상태]는 프로젝트가 다음 프로젝트인지 여부를 나타내는 프로젝트의 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>프로젝트 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">시스템 프로젝트 상태 목록에 액세스합니다</a>.</p>
    <p>작업의 경우 [!UICONTROL 상태]는 작업이 다음 작업인지 여부를 나타내는 작업의 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>작업 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">시스템 작업 상태 목록에 액세스합니다</a></p> <p>문제에 대해 [!UICONTROL 상태]는 이 문제가 다음 문제인지 여부를 나타내는 문제 설정입니다.</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL 피드백 대기 중]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL이 해결되지 않음]</li> 
     <li>[!UICONTROL을 복제할 수 없음]</li> 
     <li>[!UICONTROL 확인됨 완료]</li> 
     <li>[!UICONTROL 다시 열림]</li> 
    </ul> <p>문제 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스합니다</a>.</p> 
    <p>전략 목표의 경우 [!UICONTROL 상태]는 목표의 여부를 나타내는 목표의 설정입니다.</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>전략 목표에 대한 자세한 내용은 이 문서에서 "[!UICONTROL Goals]" 또는 "[!UICONTROL Goals]"를 참조하십시오. </p> 
     <p>전략적 목표의 경우 이 필드는 조직이 구매한 경우에만 표시됩니다 [!DNL Workfront Goals]. 을 사용하여 전략적 목표를 관리하는 방법에 대한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 개요</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태 변경]</td> 
   <td>[!UICONTROL 감사 추적]. 사용자가 프로젝트, 작업 또는 문제의 상태를 변경하면 메모가 생성됩니다.</td> 
  </tr> 
  <tr> 
   <td>상태 아이콘</td> 
   <td> <p>기본 제공 [!UICONTROL 상태 아이콘] 필드를 뷰에 열로 추가하여 다음과 같이 개체에 대한 주요 지점에 대한 가시성을 향상시킬 수 있습니다.</p> 
    <ul> 
     <li>객체에 문서가 첨부되어 있습니다</li> 
     <li>객체는 승인 프로세스와 연관됩니다</li> 
     <li>개체에는 연결된 추가 메모가 있습니다</li> 
     <li>비용은 청구가능 또는 환급 가능 합니다 </li> 
     <li>작업이 중요한 경로에 있습니다.</li> 
     <li>사용자가 회사, 팀에 속하거나 다른 시간대에 있습니다 </li> 
    </ul> <p>다음 개체의 보기에서 [!UICONTROL 상태 아이콘] 필드를 추가할 수 있습니다. </p> 
    <ul> 
     <li>[!UICONTROL 작업]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL 템플릿 작업]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>자세한 내용은 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태 업데이트]</td> 
   <td> <p>이 필드에는 사용자가 '[!UICONTROL 업데이트 상태]' 필드에서 제공한 최신 상태 업데이트가 표시됩니다. 상태 업데이트에 대한 주석이 [!UICONTROL 상태 업데이트] 열에 표시되지 않습니다.</p> <p>'[!UICONTROL New], '[!UICONTROL In Process]' 및 '[!UICONTROL Complete]' 상태를 표시하려면 [!UICONTROL Status] 열을 사용하십시오.</p> <p>상태 업데이트에 대한 주석이 [!UICONTROL 상태 업데이트] 열에 표시되지 않습니다.</p> <p>상태에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">작업 상태 업데이트</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상태]</td> 
   <td>이 문서에서 "[!UICONTROL 상태]"를 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>스토리 상태(민첩한 방법론의 작업)와 완료가 진행되는 방법을 나타내는 차트입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>스토리의 어려움이나 복잡성을 측정하는 데 사용되는 지표입니다. 애자일 팀은 시간 또는 포인트 사용 여부를 선택할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>스토리의 어려움이나 복잡성을 측정하는 데 사용되는 지표입니다. 애자일 팀은 시간 또는 포인트 사용 여부를 선택할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>조직 또는 조직이 작동하는 방식을 변경하는 장기 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>포트폴리오 및 프로그램에서 회사 목표 측정 및 조정</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>프로젝트, 작업 또는 문제를 구독하는 사용자.</p> <p>보고서에서 이 필드를 사용하면 구독자 목록이 표시되고 각 구독자는 쉼표로 구분됩니다.</p> <p>자세한 내용은 문서를 참조하십시오 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">의 항목에 가입 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 요약 작업]</td> 
   <td>이 문서에서 "[!UICONTROL Parent Task]"를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>상위 작업 아래에 있는 하위 작업입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>시스템의 변경 및 유지 관리를 제어하는 정책 집합입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>서로 다른 컴퓨팅 시스템과 소프트웨어 응용 프로그램을 물리적으로 또는 기능적으로 연결하여 전체 통합 작업을 수행하는 프로세스입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업]</td> 
   <td> <p>최종 목표(프로젝트 완료)를 달성하는 단계로 수행되어야 하는 활동.</p> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">작업 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 특성]</td> 
   <td>작업에 관련된 다른 필드 또는 개체이며 작업에 대한 특정 세부 정보를 나타냅니다. 일부 예로는 [!UICONTROL 계획된 완료 날짜] 및 [!UICONTROL 상태]가 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 제약 조건]</td> 
   <td>"[!UICONTROL 제약 조건 유형]" 및 "[!UICONTROL 제약 조건 날짜]"를 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>작업 생성, 할당, 종료 및 가시성에 대한 임계값을 제어하는 정책 집합입니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 작업 소유자]</td> 
   <td>작업의 작업 예상 및 완료를 담당하는 팀 또는 사용자</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>유사한 목표 또는 비즈니스 목표를 향해 작업하는 사용자 모음입니다. 이러한 사용자는 팀을 작업 항목에 할당하여 작업 항목에 일괄적으로 할당할 수 있습니다.</p> <p>팀에 대한 자세한 내용은 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">팀 개요</a>.</p> <p>프로젝트에는 프로젝트의 작업과 연결된 모든 사용자 또는 역할이 포함된 [!UICONTROL 프로젝트 팀]이 있을 수 있습니다.</p> <p>프로젝트 팀에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">프로젝트 팀 개요</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>프로젝트 템플릿은 가장 반복 가능한 프로젝트의 일반적인 개요입니다. 새 프로젝트를 작성해야 할 시간을 절약하기 위해 프로젝트 템플릿을 만들 때 작업, 대기열 항목, 사용자 정의 양식, 문서 또는 승인을 첨부할 수 있습니다. </p> <p>기존 프로젝트에 템플릿을 첨부하거나 템플릿을 사용하여 새 프로젝트를 작성할 수 있습니다. 템플릿에 지정된 모든 정보가 이 템플릿을 사용하여 생성된 프로젝트로 전송됩니다. </p> <p>템플릿에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">프로젝트 템플릿 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>템플릿의 일부인 작업입니다. 템플릿 작업은 템플릿을 사용하여 생성된 프로젝트의 작업이 됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 스레드]</td> 
   <td>특정 주제와 관련된 [!UICONTROL 참고] 및 해당 답글 모음입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> [!UICONTROL 문서] 목록이나 보고서에서 문서의 미리 보기를 축소판으로 표시합니다. </p> <p> 선택 <strong>[!UICONTROL Thumbnail]</strong>  보고서에서 33-66픽셀 크기의 축소판을 보려면 </p> <p>축소판의 크기는 목록 또는 보고서에서 열 너비를 수정할 때 조정됩니다.</p> <p>이 문서에서 "[!UICONTROL Large Thumbnail]"을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 시간 초과]</td> 
   <td>사용자가 프로필에서 시간 초과를 표시한 경우 볼 수 있도록 [!UICONTROL 시간 초과] 보고서를 작성할 수 있습니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업표]</td> 
   <td> <p>사용자가 프로젝트, 작업 또는 문제에 대해 작업한 실제 시간 또는 모임 또는 교육처럼 업무와 관련이 없는 다른 활동에 사용한 시간을 입력할 수 있는 타임카드입니다. 작업 시간을 입력할 수 있을 뿐만 아니라 시간 유형을 사용하여 시간 입력을 정의하여 시간이 작업 관련 시간인지 아니면 간접비 시간에 해당되는지를 나타낼 수도 있습니다. 작업표에 대한 자세한 내용은 <a href="../../../timesheets/timesheets/timesheets-overview.md">작업표 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업표 프로필]</td> 
   <td> <p>[!UICONTROL 작업표 프로필]은 [!DNL Workfront] 을 사용하여 연결된 사용자의 작업표를 자동으로 만듭니다. </p> <p>만든 각 작업표에 적용할 여러 설정을 구성할 수 있습니다. 이러한 설정 중 일부는 다음과 같습니다. 작업표를 작성할 빈도(매주, 2주, 2회, 월별 또는 월별), 작업표 시작일, 작업표 승인자, 사용 가능한 [!UICONTROL Hour Types]를 사용자가 기록된 시간과 연결할 수 있습니다.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL 상위 ID] </td> 
   <td> <p>이 필드에서는 목록이나 보고서에서 최상위 그룹 및 해당 하위 그룹에 대한 데이터를 식별하고 필터링할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 상위 이름] </td> 
   <td> <p>이 필드에서는 [!UICONTROL 보기]에서 목록이나 보고서에 대한 최상위 그룹 및 해당 하위 그룹에 대한 데이터를 식별할 수 있습니다.</p> <p>[!UICONTROL 상위 상위 ID] 필드를 사용하여 이 작업을 수행할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 총 시간]</td> 
   <td> <p>[!UICONTROL 프로젝트 보고서]에서 이 필드는 프로젝트 재정이 마지막으로 계산된 시간, 프로젝트의 모든 시간의 반올림된 합계를 표시합니다. [!UICONTROL 실제 시간]은 프로젝트에 기록된 정확한 시간을 반영합니다. 일반적으로 [!UICONTROL 실제 시간]은 [!UICONTROL 총 시간]과 일치해야 합니다. [!UICONTROL 총 시간]이 [!UICONTROL 실제 시간] 필드와 크게 다른 것으로 나타나면 프로젝트의 재정을 다시 계산해야 합니다.</p> <p>프로젝트 재정 재계산에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">프로젝트 재무 재계산</a>.</p> <p>작업표 [!UICONTROL Standard] 보기에서 이 필드는 작업표에 표시된 날짜에 대해 기록된 총 시간을 나타냅니다. 이 기본 제공 보기의 작업표에 대한 [!UICONTROL 총 시간] 필드는 작업표 시작 날짜와 종료 날짜 사이의 시간 차이를 동적으로 계산하는 "[!UICONTROL hoursDuration]" 필드를 참조합니다. 사용자가 작업표의 시간 프레임에서 사용 가능한 시간보다 더 많은 시간을 기록하면 [!UICONTROL 총 시간] 열을 빨간색으로 표시하는 데 사용됩니다. 자세한 내용은 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">작업표에서 총 시간 보기</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 추적 모드]</td> 
   <td> <p>작업의 특성입니다. 이에 따라 Task에 대해 Projected Timeline이 어떻게 업데이트되는지 결정됩니다. For example:</p> 
    <ul> 
     <li>[!UICONTROL 사용자가 업데이트해야 함]을 사용하려면 작업을 수동으로 업데이트해야 합니다. 그렇지 않으면 [!UICONTROL Behind Schedule], [!UICONTROL Late]가 됩니다.</li> 
     <li>[!UICONTROL Auto Complete]는 기한 또는 [!UICONTROL Planning Completion Date]가 전달되면 자동으로 작업을 완료합니다.</li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">작업 추적 모드 개요</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>시나리오를 시작하는 이벤트입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 작업]</td> 
   <td>[!UICONTROL Late], [!UICONTROL Behind Schedule] 또는 [!UICONTROL At Risk] 조건이 있는 불완전한 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 할당되지 않은 작업]</td> 
   <td>사용자, 역할 또는 팀에 할당되지 않은 작업입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 업데이트 유형]</td> 
   <td> <p>프로젝트의 예상 타임라인이 다시 계산되는 시기를 결정하는 프로젝트의 설정입니다. 옵션은 다음과 같습니다.</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>자세한 내용은 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">프로젝트 업데이트 유형을 선택합니다 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>에서 만든 계정 [!DNL Workfront] 사용자가 로그인한 다음 시스템과 상호 작용할 수 있도록 허용</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL 사용자 위임]</p> </td> 
   <td> <p>다음을 알려주는 보고 가능한 개체</p> 
    <ul> 
     <li>위임된 작업, 문제 및 프로젝트 승인이 있는 사용자</li> 
     <li>사용자에게 위임된 작업, 문제 및 프로젝트 승인이 있는 사용자</li> 
     <li>이러한 위임을 시작하고 종료하는 경우</li> 
    </ul> <p>자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">사용자 위임 보고서 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>의 모든 시각적 및 대화형 측면 [!DNL Workfront] 응용 프로그램.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL 사용자 인터페이스 설정]. [!DNL Workfront] 관리자는 이러한 설정을 변경하여 사용자 인터페이스의 측면을 사용자 지정할 수 있습니다.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>지정된 스케줄, PTO 및 현재 작업 로드를 기준으로 사용자 또는 역할의 가용성입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>사용자(리소스)가 할당되거나 과다 할당되는 방식을 보여주는 보고서와 결합되는 검색입니다. 이 문서에서 "[!UICONTROL Resource Utilization]"을 참조하십시오.</p> </td> 
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
   <td>총 작업 주기 시간(작업 완료에 걸리는 시간) 및 원래 약정된 시간(작업 대 커밋 비율)에서 작업이 수행되는 빈도를 측정합니다.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>보기는 보고서 또는 프로젝트, 작업 또는 문제 목록에서 열을 수정하는 데 사용하거나 액세스 수준 또는 권한 공유 수준에서 정보만 볼 수 있는 사용자의 권한을 나타내는 데 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 보기 아이콘]</td> 
   <td> <p> 상태 아이콘과 동일한 필드이지만 다음 보기에서만 사용할 수 있습니다. </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">보기의 기본 제공 상태 아이콘</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지난달 보기]</td> 
   <td> <p>보고서 목록에는 지난 달 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 지난 분기 보기]</td> 
   <td>보고서 목록에는 지난 분기 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >보고서 사용량 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>보고서 목록에는 지난 1년 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이번 달 보기]</td> 
   <td> <p>보고서 목록에는 이 달 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이 분기 보기]</td> 
   <td>보고서 목록에는 이 분기 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">보고서 사용량 보기</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 올해 보기]</td> 
   <td>보고서 목록에는 올해 동안 보고서를 본 횟수가 표시됩니다.<br>보고서 목록의 사용 정보에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">보고서 사용량 보기</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 텍스트 모드에서 다음 문을 사용하여 프로젝트, 작업 또는 문제의 계획 시간을 표시합니다.</p>
   <p></p><p></p> 
   <p>텍스트 모드 사용에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">텍스트 모드 구문 개요</a>. </p> 
   <p><b>팁</b> 
   <p>문제 보고서에서 [!UICONTROL 계획된 시간] 필드 중 하나를 추가하면 <code>work </code>필드를 보고서에 추가합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>두 가지 기본 라이센스 유형 중 하나입니다. 이렇게 하면 [!UICONTROL Plan]보다 적은 액세스 권한이 있지만 시스템에서 생성 및 업데이트를 수행할 수 있습니다. 이는 [!UICONTROL External], [!UICONTROL Reviewer] 또는 [!UICONTROL Requester] 라이센스 유형보다 성능이 뛰어납니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 라이선스 개요</a>.</p> <p>작업은 프로젝트, 작업 또는 문제에 대한 [!UICONTROL 계획 시간] 수를 참조할 수 있습니다. 자세한 내용은 이 표의 "[!UICONTROL 작업]" 필드를 참조하십시오. </p> <p>팁: 문제 보고서에서 [!UICONTROL 계획된 시간] 필드 중 하나를 추가하면 <code>work </code>필드를 보고서에 추가합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 분류 구조]</td> 
   <td>상위/하위 관계를 기반으로 프로젝트 팀이 실행할 작업의 계층 구조입니다.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 작업] </td> 
   <td> 
    <p>프로젝트 관리자는 [!UICONTROL Planning Hours] 대신 이 필드를 사용하여 작업을 완료하는 데 필요한 노력을 예상할 수 있습니다. 이 필드는 다음 조건을 충족할 때만 표시됩니다.</p> 
     <ul> 
      <li> <p>작업에 [!UICONTROL 단순 기간 유형]이 있습니다. </p> <p>팁: 작업 [!UICONTROL 기간 유형]을 다른 유형으로 업데이트하면 이 필드가 숨겨집니다. </p> </li> 
      <li>프로젝트 관리자가 [!UICONTROL 작업 사용]을 활성화하여 프로젝트의 작업 [!UICONTROL 계획 시간] 필드를 자동으로 계산합니다. </li> 
     </ul> 
     <p>[!UICONTROL Planning Hours] 대신 [!UICONTROL Work Pure]를 사용하여 작업 노력을 추정하는 방법에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">작업 시간 개요</a>. </p> 
     <p>작업 보고서 및 목록에 이 필드를 표시할 수 있습니다.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 작업 항목]</td> 
   <td> <p>이 필드는 [!DNL Workfront]. </p> <p>[!UICONTROL 작업 항목] 보고서에는 작업과 문제 모두에 대한 정보가 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management mix]</td> 
   <td>비즈니스를 운영하고 비즈니스를 변경하는 데 할당된 작업의 비율([!UICONTROL 작업 성능 지표] )입니다. Mix WPI를 사용하면 조직에 실제 작업 할당이 적용되는지 여부를 조직 수준에서 파악할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>작업 또는 추적 시간을 받을 수 있는 시스템에서 사용자 지정</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management 역할 및 책임]</td> 
   <td>지정된 문제, 작업, 프로젝트, 프로그램 또는 포트폴리오의 범위, 실행 및 승인을 관리할 소유자 및 이해 관계자 정의</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 관리 SLA]</td> 
   <td>모든 이해 관계자가 합의한 수량화 가능한 지표.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management 이해 관계자]</td> 
   <td>작업 요청의 결과에 대한 기득권을 가진 사용자 모음입니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management 터치포인트]</td> 
   <td>이해 당사자 간의 커뮤니케이션에 대한 디지털 기록</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 작업 성능 지표] </td> 
   <td> <p>혼용 비율, 용량, 속도, 품질 및 참여</p> <p>WPI는 [!UICONTROL Work Performance Indicator]의 일반적인 약어입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>작업을 수신, 우선 순위 지정 및 실행하는 메서드입니다. 작업을 실행하는 방식은 일반적으로 "워크플로우" 또는 "프로젝트 계획"이라고 합니다(날짜, 이전 관계 등이 있는 작업 목록). </p> <p>작업 프로세스의 예로는 단일 자산을 만들거나 다중 자산 캠페인을 전달하는 것이 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow Template]</td> 
   <td>[!UICONTROL 증명 승인] 보고서에서 이 필드에는 증명에 첨부된 모든 워크플로우 템플릿이 표시됩니다. 첨부된 템플릿이 없으면 열이 비어 있습니다.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>사용자가 오버헤드를 포함하지 않고 실제 작업에 사용할 수 있는 Full Time Equivalent([!UICONTROL FTE]) 시간의 백분율을 나타냅니다. [!UICONTROL Work Time]은(는) 최대 10진수 값이어야 하며, 0일 수 없습니다. 예를 들어 실제 작업의 20% 가용성은 0.2입니다.</p>
   </p>필드의 기본값은 1이며, 사용자가 실제 프로젝트 관련 작업에 전체 [!UICONTROL FTE]를 사용함을 나타냅니다.  </p>
   <p>시스템은 이 숫자를 사용하여 실제 프로젝트 관련 작업에 대한 사용자의 가용성을 계산합니다. </p>
   <p> 예약 예외 및 해제 시간은 사용자 용량에 영향을 줄 수 있습니다. </p>
   <p>Workfront에서 예약 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">예약 만들기</a>. </p>
    <p>Workfront은 [!UICONTROL 설정] 영역의 리소스 관리 환경 설정에 따라 사용자의 가용성을 계산합니다. 자세한 내용은 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">리소스 관리 환경 설정 구성</a>. </p> 
   <p>사용자를 편집하거나 만들 때 사용자의 [!UICONTROL 작업 시간]을 업데이트할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">사용자 프로필 편집</a></p> 
   <b>팁</b> 
   <p>사용자가 프로젝트 관련 작업에 사용할 수 있음을 나타내려면 [!UICONTROL 작업 시간] 값을 1로 설정합니다. 이 값은 전체 상응하는 전체 시간을 나타냅니다.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>Workfront 설명서에서 이 용어는 예약에 따라 작업에 할당된 시간을 설명하는 데 사용됩니다.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>프로젝트, 작업 또는 문제 보고서에서 텍스트 모드에서 다음 문을 사용하여 프로젝트, 작업 또는 문제의 계획 시간 수 다음에 "시간"이라는 단어가 표시됩니다.</p>
   <p></p><p></p>
    <p>텍스트 모드 사용에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">텍스트 모드 구문 개요</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
