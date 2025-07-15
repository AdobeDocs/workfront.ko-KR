---
title: 레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿에서 사용자가 Adobe Workfront 전체의 왼쪽 패널 영역에 표시되는 내용을 사용자 지정할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의

<!--Audited: 10/2024-->

레이아웃 템플릿에서 [!DNL Adobe Workfront] 전체에서 왼쪽 패널 영역에 표시되는 내용을 사용자 지정할 수 있습니다.

예를 들어 작업을 볼 때 사용자가 왼쪽 패널에 표시되는 항목 중 하나를 결정할 수 있습니다.

![브랜딩 왼쪽 패널](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>순서 및 가시성에 대한 변경 사항은 모바일 앱에 반영됩니다.

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td><p>임의</p>
   <p>메인 메뉴에 사용자 정의 응용 프로그램을 추가하는 것은 Adobe App Builder에 대해 라이선스가 부여된 조직에서만 가능합니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p>
  <p> 현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront]의 영역에 대한 왼쪽 패널 사용자 지정:

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. ![사용자에게 표시되는 항목 사용자 지정](assets/dropdown-arrow.png) 아래의 아래쪽 화살표 **[!UICONTROL 아래쪽 화살표]**&#x200B;를 클릭한 다음 왼쪽 패널을 사용자 지정할 개체 유형 또는 [!DNL Workfront] 영역의 이름을 클릭합니다.

   왼쪽 패널을 사용자 지정할 수 있는 개체 형식과 [!DNL Workfront] 영역이 다음 표에 나열되어 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>개체 유형 또는 [!DNL Workfront] 영역</th> 
      <th>사용자가 다음을 클릭하면...</th> 
      <th>레이아웃 템플릿에 표시한 후 사용자에게 표시되는 왼쪽 패널의 섹션:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL 프로젝트]</td> 
      <td>프로젝트 이름</td> 
      <td>[!UICONTROL 작업], [!UICONTROL 프로젝트 세부 사항], [!UICONTROL 비즈니스 사례], [!UICONTROL 업데이트], [!UICONTROL 문서], [!UICONTROL 문제], [!UICONTROL 위험], [!UICONTROL 승인], [!UICONTROL 기준 요소], [!UICONTROL 청구 요금], [!UICONTROL 청구 기록], [!UICONTROL 비용], [!UICONTROL 시간], [!UICONTROL 업무 균형자], [!UICONTROL 사용자], [!UICONTROL 사용자] 사용률], [!UICONTROL 대기열 세부 정보], [!UICONTROL 라우팅 규칙], [!UICONTROL 대기열 주제], [!UICONTROL 주제 그룹], [!UICONTROL 지표], [!UICONTROL Planning]*, [!UICONTROL 사용자 정의 응용 프로그램]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 작업]</td> 
      <td>작업 이름</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Predecessors], [!UICONTROL Custom Application]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 문제]</td> 
      <td>문제의 이름</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issue Details], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL 사용자 정의 응용 프로그램]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>포트폴리오 이름</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio] [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates], [!UICONTROL Planning]*, [!UICONTROL 사용자 정의 응용 프로그램]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 프로그램]</td> 
      <td>프로그램 이름</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Planning]*, [!UICONTROL 사용자 정의 응용 프로그램]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>프로젝트 템플릿의 이름</td> 
      <td>[!UICONTROL 템플릿 작업], [!UICONTROL 템플릿 세부 사항], [!UICONTROL 업데이트], [!UICONTROL 문서], [!UICONTROL 위험], [!UICONTROL 비용], [!UICONTROL 사람], [!UICONTROL 승인], [!UICONTROL 청구 요금], [!UICONTROL 대기열 세부 사항], [!UICONTROL 라우팅 규칙], [!UICONTROL 대기열 주제], [!UICONTROL 주제 그룹]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 템플릿 작업]</td> 
      <td>템플릿 작업의 이름</td> 
      <td>[!UICONTROL 업데이트], [!UICONTROL 문서], [!UICONTROL 템플릿 작업 세부 정보], [!UICONTROL 하위 작업], [!UICONTROL 경비], [!UICONTROL 승인], [!UICONTROL 전임 작업]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL 청구 기록]</td> 
      <td>프로젝트에 대한 청구 기록의 이름</td> 
      <td>[!UICONTROL 청구 기록 세부 정보], [!UICONTROL 청구 가능 시간], [!UICONTROL 청구 가능 경비], [!UICONTROL 고정 수입]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 프로젝트]</td> 
      <td>[!UICONTROL 주 메뉴]의 프로젝트 <img src="assets/projects-in-main-menu.png"> <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL 프로젝트]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>요청 이름</td> 
      <td>[!UICONTROL New Request], [!UICONTROL Submitted Requests], [!UICONTROL All Requests], [!UICONTROL Draft]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 대시보드]</td> 
      <td>대시보드 이름</td> 
      <td>[!UICONTROL 내 대시보드], [!UICONTROL 공유 대시보드], [!UICONTROL 모든 대시보드]<p><b>참고</b>: [!DNL Adobe Workfront Classic]에서 레이아웃 템플릿을 사용하여 [!UICONTROL 보고서] 영역에 대한 사용자 지정 탭을 만든 경우 이 탭의 맨 아래에 표시됩니다. 사용자의 경우 [!UICONTROL 대시보드] 영역의 왼쪽 패널 하단에 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 스크럼 팀]</td> 
      <td>스크럼 팀의 이름</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current Iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL 팀 설정]</p> <p><strong>참고:</strong> <strong>[!UICONTROL 현재 반복]</strong> 항목은 반복에 하나 이상의 작업 또는 문제가 있는 경우에만 왼쪽 패널에 표시됩니다.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban 팀]</td> 
      <td>Kanban 팀의 이름</td> 
      <td>[!UICONTROL 업무 균형자], [!UICONTROL Kanban board], [!UICONTROL 백로그], [!UICONTROL 업데이트], [!UICONTROL 팀 설정]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall 팀]</td> 
      <td>Waterfall 팀의 이름입니다</td> 
      <td>[!UICONTROL 업무 균형자], [!UICONTROL 업데이트], [!UICONTROL 팀 요청], [!UICONTROL 팀 설정]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 반복]</td> 
      <td>반복 이름</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   *이 영역을 프로젝트, 포트폴리오 및 프로그램의 왼쪽 패널에 추가하려면 귀사에서 Workfront Planning에 대해 추가 라이선스를 구입해야 합니다. 자세한 내용은 [Adobe Workfront 계획 개요](/help/quicksilver/planning/general/planning-overview.md)를 참조하십시오.

   **사용자 정의 응용 프로그램은 별도로 만들어야 기본 메뉴 옵션으로 사용할 수 있습니다. 자세한 내용은 [Adobe App Builder을 사용하여 Workfront용 사용자 지정 응용 프로그램 만들기](/help/quicksilver/app-builder/app-builder.md)를 참조하십시오.


1. **[!UICONTROL 왼쪽 패널]** 목록에서 다음 중 하나를 수행하여 선택한 [!DNL Workfront] 영역 또는 개체 유형에 대해 왼쪽 패널에 표시되는 사용자를 결정합니다.

   * 왼쪽 패널에서 섹션을 표시하거나 숨기려면 **표시** ![표시 아이콘](assets/add-secondary-nav-item.png) 또는 **숨기기** ![숨기기 아이콘](assets/delete-secondary-nav-item.png) 아이콘을 클릭합니다. **표시** 또는 **숨기기** 아이콘이 없는 항목은 숨길 수 없습니다.

   * 왼쪽 패널에서 순서를 변경하려면 ![이동 아이콘](assets/move-icon---dots.png)을 끕니다.

   >[!NOTE]
   >
   >**[!UICONTROL 사용자에게 표시되는 항목 사용자 지정]** 드롭다운 목록의 다음 항목은 왼쪽 패널 이외의 영역을 참조합니다.
   >* [!UICONTROL 목록]
   >* [!UICONTROL 요약 패널]
   >* [!UICONTROL 홈]
   >* [!UICONTROL 브랜딩]
   > 
   >추가 영역을 사용자 지정하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.
   >
   >* [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [레이아웃 템플릿을 사용하여 [!UICONTROL 요약 패널 사용자 지정]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [레이아웃 템플릿을 사용하여 홈 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Brand Adobe [!DNL Workfront] 레이아웃 템플릿 사용](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (선택 사항) 조직의 대시보드 중 하나에 연결되는 왼쪽 패널 항목을 추가하려면 **[!UICONTROL 사용자 지정 섹션 추가]**&#x200B;를 클릭하고 항목에 대한 **[!UICONTROL 사용자 지정 섹션 제목]**&#x200B;을 입력한 다음 대시보드를 추가하십시오.

   대시보드 항목은 왼쪽 패널 하단에 나타납니다. 사용자가 왼쪽 패널에서 대시보드 항목 위로 마우스를 가져가면 해당 대시보드 항목 옆에 입력한 사용자 정의 섹션 제목이 표시됩니다.

   >[!NOTE]
   >
   >사용자는 사용자 정의 대시보드 항목을 자신의 왼쪽 패널에 추가할 수 있습니다. 레이아웃 템플릿에 사용자 정의 대시보드 항목을 추가하면 항목이 추가한 항목 외에도 덮어쓰거나 재설정하지 않고 표시됩니다. 이는 사용자 지정 대시보드 항목이 있는 새 레이아웃 템플릿에 사용자를 할당하는 경우에도 마찬가지입니다. 사용자가 왼쪽 패널을 사용자 지정하는 방법에 대한 자세한 내용은 [사용자 지정 탭 또는 섹션 만들기](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)를 참조하십시오.
   >
   >대시보드에 대한 자세한 내용은 [대시보드](../../../reports-and-dashboards/dashboards/dashboards-overview.md)를 참조하십시오.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >언제든지 [!UICONTROL **저장**]&#x200B;을 클릭하여 진행 상황을 저장할 수 있습니다. 그러면 레이아웃 템플릿 편집기가 닫히고 나중에 템플릿을 계속 수정할 수 있습니다.
