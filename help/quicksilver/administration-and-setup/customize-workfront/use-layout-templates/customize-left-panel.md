---
title: 레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿에서 Adobe Workfront 전체에서 왼쪽 패널 영역에 표시되는 내용을 사용자 지정할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의

레이아웃 템플릿에서 사용자가 왼쪽 패널 영역에 표시되는 내용을 사용자 지정할 수 있습니다 [!DNL Adobe Workfront].

예를 들어, 작업을 볼 때 왼쪽 패널에 표시되는 다음 항목 중 어느 항목을 결정할 수 있습니다.

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>순서 및 가시성에 대한 변경 사항이 모바일 앱에 반영됩니다.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> 시스템 수준에서 이러한 단계를 수행하려면 [!UICONTROL 시스템 관리자] 액세스 수준이 필요합니다.<p>그룹에 대해 해당 그룹을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 의 영역에 대해 왼쪽 패널 사용자 정의 [!DNL Workfront]:

1. 에 설명된 대로 레이아웃 템플릿 작업을 시작합니다. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 아래쪽 화살표를 클릭합니다 ![](assets/dropdown-arrow.png) 아래에 **[!UICONTROL 사용자에게 표시되는 항목 사용자 지정]**&#x200B;을 클릭한 다음 사용자 지정할 왼쪽 패널을 클릭합니다.

   >[!NOTE]
   >
   >에 대한 정보 [!UICONTROL 홈] 이 드롭다운 목록의 옵션은 다음을 참조하십시오 [사용자 지정 [!UICONTROL 홈] 및 [!UICONTROL 요약] 레이아웃 템플릿 사용](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). 목록 옵션에 대한 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 에서 **[!UICONTROL 왼쪽 패널]** 목록에서 다음 중 하나를 수행하여 사용자가 왼쪽 패널에 표시되는 옵션([!DNL Workfront] 영역 또는 객체 유형)을 선택한 경우

   * 표시 ![](assets/add-secondary-nav-item.png) 또는 숨기기 ![](assets/delete-secondary-nav-item.png) 항목. 없는 항목 ![](assets/add-secondary-nav-item.png) 또는 ![](assets/delete-secondary-nav-item.png) 숨길 수 없습니다.

   * 항목 드래그 ![](assets/move-icon---dots.png) 왼쪽 패널에서 주문을 변경하려면

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>옵션</th> 
      <th>사용자가 다음을 클릭하면...</th> 
      <th>다음 중 선택한 왼쪽 패널 항목이 표시됩니다.</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>프로젝트 이름</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Equontrol Coorettrol Entrails, [!WICONTROL Expenses [!COPAGES], [!UICONTROL, [!UICONTROL Experiences [!WICONTROL!COPAGES [!UICONTROL], [!UICONTROL Hours], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 작업]</td> 
      <td>작업 이름</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Prevideos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 문제]</td> 
      <td>문제 이름</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issue Details], [!UICONTROL Hours], [!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>포트폴리오의 이름</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfolio Details], [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>프로그램 이름</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>프로젝트 템플릿의 이름입니다</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Experiences], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Questions], [!UICONTROL Queue Details], [!UICONTROL [!UICONTROL Rules [!UICONTROL [!UICONTROL Routs] 큐 항목], [!UICONTROL 항목 그룹]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>템플릿 작업의 이름</td> 
      <td>[!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expermissions], [!UICONTROL Approvals], [!UICONTROL Prevideos]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>프로젝트에 대한 청구 레코드의 이름</td> 
      <td>[!UICONTROL 청구 레코드 세부 정보], [!UICONTROL 청구 가능 시간], [!UICONTROL 청구 가능한 비용], [!UICONTROL 고정 수익]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>프로젝트 <img src="assets/projects-in-main-menu.png"> ([!UICONTROL 기본 메뉴]에서) <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>요청 이름</td> 
      <td>[!UICONTROL 새 요청], [!UICONTROL 제출된 요청], [!UICONTROL 모든 요청], [!UICONTROL Draft]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>대시보드 이름</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b>참고</b>: 에서 레이아웃 템플릿을 사용하여 [!UICONTROL 보고서] 영역에 대한 사용자 지정 탭을 만든 경우 [!DNL Adobe Workfront Classic]로 설정되면 이 목록의 맨 아래에 표시됩니다. 사용자의 경우 왼쪽 패널 하단에 [!UICONTROL 대시보드] 영역을 표시합니다.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Screum Team]</td> 
      <td>스크럼 팀의 이름</td> 
      <td><p>[!UICONTROL 반복], [!UICONTROL 현재 반복], [!UICONTROL 백로그], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>참고:</strong> 다음 <strong>[!UICONTROL 현재 반복]</strong> 반복에 하나 이상의 작업이나 문제가 있는 경우 왼쪽 패널에만 항목이 표시됩니다.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 간판 팀]</td> 
      <td>간판 팀의 이름</td> 
      <td>[!UICONTROL 작업 로드 밸런서], [!UICONTROL 간판 보드], [!UICONTROL 백로그], [!UICONTROL 업데이트], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>폭포 팀명</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
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

   >[!NOTE]
   >
   >의 마지막 3개 항목 **[!UICONTROL 사용자에게 표시되는 항목 사용자 지정]** 드롭다운 목록([!UICONTROL 목록], [!UICONTROL 홈 및 요약], 및 [!UICONTROL 브랜딩])은 왼쪽 패널 이외의 영역을 구성하기 위한 것입니다. 자세한 내용은 다음 문서를 참조하십시오.
>   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [사용자 지정 [!UICONTROL 홈] 및 [!UICONTROL 요약] 레이아웃 템플릿 사용](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [브랜드 Adobe [!DNL Workfront] 레이아웃 템플릿 사용](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. (선택 사항) 조직의 대시보드 중 하나에 연결되는 왼쪽 패널 항목을 추가하려면 를 클릭합니다 **[!UICONTROL 사용자 지정 섹션 추가]**, 입력 **[!UICONTROL 사용자 지정 섹션 제목]** 항목에 대해 대시보드를 추가합니다.

   대시보드 항목은 왼쪽 패널 하단에 나타납니다. 사용자는 왼쪽 패널을 마우스로 가리키면 대시보드 항목 옆에 입력하는 사용자 지정 섹션 제목을 볼 수 있습니다.

   >[!NOTE]
   사용자는 자신의 왼쪽 패널에 사용자 지정 대시보드 항목을 추가할 수 있습니다. 레이아웃 템플릿에 사용자 지정 대시보드 항목을 추가하면 해당 항목이 덮어쓰거나 재설정하지 않고 해당 항목과 병합됩니다. 사용자 지정 대시보드 항목을 사용하여 새 레이아웃 템플릿에 사용자를 지정하는 경우에도 마찬가지입니다. 사용자가 왼쪽 패널을 사용자 지정하는 방법에 대한 자세한 내용은 [사용자 지정 탭 또는 섹션 만들기](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   대시보드에 대한 자세한 내용은 [대시보드](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 완료한 경우 을 누릅니다 **[!UICONTROL 저장]**.

   >[!TIP]
   을(를) 클릭합니다 [!UICONTROL 저장] 언제든지 진행 상태를 저장한 다음 나중에 계속 템플릿을 수정합니다.
