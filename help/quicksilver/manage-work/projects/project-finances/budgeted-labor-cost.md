---
content-type: reference
product-area: projects
navigation-topic: financials
title: 프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해
description: 프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# 프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Adobe Workfront Resource Planner를 사용하여 작업에 필요한 자원을 예약할 수 있습니다.

프로젝트에서 작업하기 위해 자원의 예산을 책정함에 따라 Workfront은 시간당 비용을 기준으로 역할, 프로젝트 및 사용자에 대한 예산책정된 노무비를 계산합니다.

프로젝트의 Resource Planner 예산책정된 노무비는 프로젝트에서 작업을 완료하기 위해 지정된 Job 역할과 연관된 비용과 각 역할을 수행하여 작업을 완료할 수 있는 예상 시간(Resource Planner 예산책정 시간) 사이의 계산입니다.

>[!IMPORTANT]
>
>사용자에 대한 Resource Planner 예산책정된 노무비는 프로젝트의 비용에 영향을 주지 않습니다. 직무 역할에 대한 인건비 비용만 프로젝트 비용에 영향을 줍니다.

## Job 역할 및 프로젝트에 대한 예산책정된 노무비 개요

Workfront은 프로젝트에 대한 Job 역할의 예산책정된 노무비를 사용하여 프로젝트의 예산책정된 노무비를 계산합니다.

>[!TIP]
>
>비즈니스 케이스의 프로젝트의 예산책정된 노무비는 보고서 및 목록의 자원 계획자 예산책정된 노무비로 표시됩니다.

다음 **예산책정된 인건비** (또는 Resource Planner Budget Labor Cost) 프로젝트의 경우 다음 공식을 사용하여 계산됩니다.

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

위의 계산에서 사용되는 필드는 다음과 같습니다.

* 프로젝트의 자원 예산 책정 영역 또는 자원 계획자 영역에서 작업 역할에 대한 예산 책정된 시간.

   Resource Planner의 예산 책정 자원에 대한 자세한 내용은 문서의 &quot;Resource Planner의 예산 책정 리소스&quot; 섹션을 참조하십시오 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   Business Case의 Resource Budgeting 영역의 예산 책정 리소스에 대한 자세한 내용은 다음을 참조하십시오 [비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* 다음 **작업 역할의 시간당 비용 비율** 위의 계산에서는 프로젝트의 각 작업 역할과 연관된 비용을 나타냅니다.\
   Job 역할 생성 및 관리 및 원가율 연결에 대한 자세한 내용은 문서를 참조하십시오 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront은 프로젝트의 통화를 사용하여 모든 비용 정보를 계산합니다. 자원 계획자에서 자원에 대한 예산책정된 시간을 지정하는 경우 프로젝트 통화를 변경하는 옵션이 비활성화됩니다.\
>프로젝트 통화 변경에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md).

## 사용자를 위한 예산책정된 노무비 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>사용자 예산책정 노무비는 프로젝트의 예산책정된 노무비에 영향을 주지 않습니다. 프로젝트에 대한 Job 역할의 노무비만 프로젝트의 Resource Planner 예산 인건비 원가에 영향을 줍니다.
> 
>모든 사용자의 모든 노무비 합계는 사용자와 연관된 Job 역할의 Resource Planner 예산책정된 노무비와 같거나 같지 않을 수 있습니다.
>
>Resource Planner에서 사용자에 대한 예산 시간(시)을 예상하는 경우, 사용자와 연관된 비용은 사용자와 연관된 작업 역할의 비용입니다. 사용자 또는 해당 요금과 관련된 비용은 아닙니다.

사용자가 프로젝트의 Job 역할과 연관되어 있고 Resource Planner에서 해당 시간의 예산책정된 경우, Workfront에서 사용자가 보는 위치에 따라, Oracle Built Labor가 다음 이름으로 표시됩니다.

* [!UICONTROL **예산책정된 인건비**]: 해당 역할에 따른 업무 사례의 자원 예산 영역.

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: 원가로 프로젝트 및 역할 뷰에서 정보를 볼 때 리소스 계획자가 표시됩니다.

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

사용자가 다음 요구 사항을 충족하는 경우 업무 사례의 자원 예산 영역 또는 해당 역할에 따라 자원 계획자에 표시됩니다.

* 이 구성 요소는 프로젝트에서 작업 역할 중 하나에 연결됩니다.
* 자원 계획자에 지정된 예산책정된 시간이 있습니다.
* 프로필과 연관된 시간당 비용 비율이 있습니다.

   사용자에게 시간당 비용 비율을 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 사용자는 프로젝트와 연결된 리소스 풀 중 하나에 속합니다.

사용자의 예산책정된 노무비는 다음 공식으로 계산됩니다.

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 프로젝트의 예산책정된 노무비 찾기

업무 사례의 자원 예산 영역 또는 자원 계획자가 반영된 예산책정된 노무비는 다음 이름의 Workfront의 다음 영역에 표시됩니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>예산책정된 노무비 표시명</strong></td> 
     <td><strong>Workfront 지역</strong></td> 
    </tr> 
    <tr> 
     <td>예산 인건비</td> 
     <td>업무 사례의 자원 예산 영역</td> 
    </tr> 
    <tr> 
     <td>예산 비용</td> 
     <td><p>활용률 보고서 원가 보기</p><p>자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">활용률 정보 보기</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>원가별 자원 계획자 프로젝트 또는 역할 보기</td> 
    </tr> 
    <tr> 
     <td>자원 계획자 프로젝트 예산책정된 노무비</td> 
     <td> <p>프로젝트 보고서</p> <p>프로젝트(재무 데이터) 보고서</p> <p>작업 보고서</p> <p>문제 보고서</p> <p>예산책정된 시간 보고서</p> <p>보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Adobe Workfront 시나리오 계획자를 사용하여 프로젝트 자원을 예산을 책정하는 경우 업무 사례의 자원 예산 책정 영역에 있는 예산책정된 노무비는 프로젝트에 연결된 이니셔티브의 인력 원가와 동일합니다. 시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md). 시나리오 계획자를 사용한 예산 편성에 대한 자세한 내용은 [시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 프로젝트의 예산책정된 시간 찾기

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

예산책정된 시간은 프로젝트의 예산책정된 노무비(또는 Resource Planner 예산책정된 원가) 값에 영향을 줍니다.

프로젝트의 예산책정된 노무비는 프로젝트에서 작업을 완료하기 위해 지정된 Job 역할과 연관된 원가와 각 역할을 수행하여 작업을 완료할 수 있는 예상 시간(예산책정된 시간)입니다.

아래 표에 나열된 필드에서 Workfront의 예산책정 시간을 볼 수 있습니다.

>[!NOTE]
>
>Workfront에서 &quot;예산책정된 시간&quot;에 대한 다른 언급은 Workfront에서 제거된 더 이상 사용되지 않는 기능을 사용하여 책정된 시간을 의미합니다. 이 필드는 보기 전용 필드이며 현재 리소스 예산 책정 도구를 사용할 때 현재 정보로 업데이트되지 않습니다.

업무 사례의 Resource Budgeting 영역 또는 Resource Planner에 책정된 시간이 Workfront의 다음 영역과 다음 이름 아래에 표시됩니다.

* **시간**: 업무 사례의 자원 예산 영역
* **BDG**:시간별 리소스 계획자 보기
* **예산책정된 시간**: 활용률 보고서 시간 보기 자세한 내용은 [자원 사용률 정보 보기](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **버드 시간**: 예산책정된 시간 보고서

   예산책정된 시간 보고서의 예산책정된 시간 객체는 사용되지 않는 자원 관리 도구와 관련된 정보를 나타냅니다. &quot;버드&quot;만 이 보고서의 &quot;시간&quot; 필드는 프로젝트 업무 사례의 자원 계획자 또는 자원 예산 책정 영역에 책정된 시간을 나타냅니다.

   보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 **사용자 지정 보고서 만들기**.
* **자원 계획자 예산책정 시간**: 다음 보고서에서 다음을 수행합니다.

   * 프로젝트 보고서
   * 프로젝트(재무 데이터) 보고서
   * 작업 보고서
   * 문제 보고서
   * 예산책정된 시간 보고서
