---
content-type: reference
product-area: projects
navigation-topic: financials
title: 프로젝트의 예산 인건비 및 예산 시간 이해
description: 프로젝트의 예산 인건비 및 예산 시간 이해
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 0%

---

# 프로젝트의 예산 인건비 및 예산 시간 이해

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Adobe Workfront 리소스 플래너를 사용하여 작업에 대한 리소스 예산을 책정할 수 있습니다.

프로젝트에 대한 작업에 리소스 예산을 책정할 때 Workfront은 시간당 비용 값을 기반으로 역할, 프로젝트 및 사용자에 대한 예산 인건비를 계산합니다.

프로젝트의 리소스 플래너 예산 인건비는 프로젝트에서 작업을 완료하기 위해 할당된 작업 역할과 관련된 비용과 작업을 완료하는 데 각 역할을 사용할 수 있는 예상 시간(리소스 플래너 예산 시간) 사이의 계산입니다.

>[!IMPORTANT]
>
>리소스 플래너의 사용자 예산 인건비는 프로젝트의 인건비에 영향을 주지 않습니다. 직무 역할에 대한 인건비만이 프로젝트의 비용에 영향을 미친다.

## 작업 역할 및 프로젝트에 대한 예산 인건비 개요

Workfront은 프로젝트에서 작업 역할의 예산 인건비를 사용하여 프로젝트의 예산 인건비를 계산합니다.

>[!TIP]
>
>비즈니스 사례에서 프로젝트의 예산 인건비는 보고서 및 목록에 리소스 플래너 예산 인건비로 표시됩니다.

프로젝트의 **예산 인건비**(또는 리소스 플래너 예산 인건비)는 다음 공식에 따라 계산됩니다.

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

위의 계산에 사용된 필드는 다음을 참조합니다.

* 프로젝트 또는 리소스 플래너의 리소스 예산 책정에서 작업 역할에 대해 예산 책정된 시간.

  리소스 플래너의 리소스 예산 편성에 대한 자세한 내용은 문서 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)의 &quot;리소스 플래너의 리소스 예산 책정&quot; 섹션을 참조하십시오.

  비즈니스 사례의 리소스 예산 책정 영역에서 리소스 예산 편성에 대한 자세한 내용은 [비즈니스 사례의 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)을 참조하세요.

* 위의 계산에서 **작업 역할의 시간당 비용 비율**&#x200B;은(는) 프로젝트의 각 작업 역할과 관련된 비용을 나타냅니다.\
  작업 역할을 만들고 관리하며 비용 요율과 연결하는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) 문서를 참조하십시오.

>[!NOTE]
>
>Workfront은 프로젝트 통화를 사용하여 모든 비용 정보를 계산합니다. 리소스 플래너에서 리소스에 대한 예산 시간을 지정하는 경우 프로젝트 통화 변경 옵션이 비활성화됩니다.\
>프로젝트 통화 변경에 대한 자세한 내용은 문서 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md)을 참조하십시오.

## 사용자의 예산 인건비 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>사용자 예산 인건비는 프로젝트의 예산 인건비에 영향을 주지 않습니다. 프로젝트에 대한 작업 역할의 인건비만 프로젝트의 리소스 플래너 예산 인건비에 영향을 줍니다.
> 
>모든 사용자의 총 인건비는 사용자와 연관된 작업 역할의 리소스 플래너 예산 인건비와 동일하거나 동일하지 않을 수 있습니다.
>
>리소스 플래너의 사용자에 대한 예산 시간을 예상하는 경우, 사용자와 관련된 비용은 사용자와 관련된 작업 역할의 비용입니다. 사용자 또는 사용자 요금과 관련된 비용이 아닙니다.

사용자가 프로젝트의 작업 역할과 연결되어 있고 리소스 플래너에 시간이 예산 책정된 경우, 예산 책정된 인건비는 Workfront에서 볼 수 있는 위치에 따라 다음과 같은 이름으로 표시됩니다.

* [!UICONTROL **예산 인건비**]: 해당 역할의 비즈니스 사례에 대한 리소스 예산 영역입니다.

  ![비즈니스 사례의 예산 인건비](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: 비용별 프로젝트 및 역할 보기에서 정보를 볼 때 리소스 플래너입니다.

  ![리소스 계획의 예산 인건비](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

사용자는 각 역할의 비즈니스 사례의 리소스 예산 편성 영역에 표시되거나 다음 요구 사항을 충족하는 경우 리소스 플래너에 표시됩니다.

* 프로젝트에서 작업 역할 중 하나와 연결됩니다.
* 리소스 플래너에 지정된 예산 시간이 있습니다.
* 프로필과 연계된 시간당 비용 요금이 있습니다.

  사용자에게 시간당 비용 요금을 추가하는 방법에 대한 자세한 내용은 문서 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하십시오.

* 사용자는 프로젝트와 연결된 리소스 풀 중 하나의 일부입니다.

사용자의 예산 인건비는 다음 공식에 의해 계산됩니다.

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 프로젝트의 예산 인건비를 찾습니다.

비즈니스 사례 또는 리소스 플래너의 리소스 예산 편성 영역에 반영된 예산 인건비가 Workfront의 다음 영역에 다음과 같은 이름으로 표시됩니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>예산 인건비 표시명</strong></td> 
     <td><strong>Workfront 지역</strong></td> 
    </tr> 
    <tr> 
     <td>예산 인건비</td> 
     <td>비즈니스 사례의 리소스 예산 영역</td> 
    </tr> 
    <tr> 
     <td>예산 비용</td> 
     <td><p>활용률 보고서 비용 보기</p><p>자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">사용률 정보 보기</a> 를 참조하십시오.</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>원가별 리소스 플래너 프로젝트 또는 역할 보기</td> 
    </tr> 
    <tr> 
     <td>리소스 플래너 프로젝트 예산 인건비</td> 
     <td> <p>프로젝트 보고서</p> <p>프로젝트(재무 데이터) 보고서</p> <p>작업 보고서</p> <p>문제 보고서</p> <p>예산 시간 보고서</p> <p>보고서 만들기에 대한 자세한 내용은 문서 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>를 참조하세요.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Adobe Workfront 시나리오 플래너를 사용하여 프로젝트 리소스의 예산을 책정하는 경우, 비즈니스 사례의 리소스 예산 책정 영역에서 예산 책정된 인건비는 프로젝트에 연결된 이니셔티브의 인건비와 동일합니다. 시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오. 시나리오 플래너를 사용한 리소스 예산 편성에 대한 자세한 내용은 [시나리오 플래너를 사용한 비즈니스 사례의 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)을 참조하십시오.

## 프로젝트의 예산 시간을 찾습니다.

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

예산 시간은 프로젝트의 예산 인건비(또는 리소스 플래너 예산 비용) 값에 영향을 줍니다.

프로젝트의 예산 인건비는 프로젝트에서 작업을 완료하기 위해 할당된 작업 역할과 관련된 비용이며, 각 역할이 작업을 완료하는 데 소요될 수 있는 예상 시간(예산 시간)입니다.

아래 표에 나열된 필드에서 Workfront의 예산 시간을 볼 수 있습니다.

>[!NOTE]
>
>Workfront의 &quot;예산 시간&quot;에 대한 다른 언급은 Workfront에서 제거된 더 이상 사용되지 않는 기능을 사용하여 예산 책정된 시간을 나타냅니다. 이는 보기 전용 필드이며 현재 리소스 예산 책정 도구를 사용할 때 현재 정보로 업데이트되지 않습니다.

비즈니스 사례 또는 리소스 플래너의 리소스 예산 책정에서 책정된 시간은 Workfront의 다음 영역에 다음 이름으로 표시됩니다.

* **시간**: 비즈니스 사례의 리소스 예산 영역
* **BDG**:시간별 리소스 플래너 보기
* **예산 시간**: 사용률 보고서 시간 보기
자세한 내용은 [리소스 사용률 정보 보기](../../../resource-mgmt/resource-utilization/view-utilization-information.md)를 참조하십시오.
* **예산. 시간**: 예산 시간 보고서

  예산 시간 보고서의 예산 시간 개체는 더 이상 사용되지 않는 리소스 관리 도구와 관련된 정보를 참조합니다. 오직 &quot;싹&quot;만 이 보고서의 &quot;시간&quot; 필드는 프로젝트 비즈니스 사례의 리소스 플래너 또는 리소스 예산 책정에서 예산 책정된 시간을 나타냅니다.

  보고서 만들기에 대한 자세한 내용은 문서 **사용자 지정 보고서 만들기**&#x200B;를 참조하십시오.
* **리소스 플래너 예산 시간**: 보고서:

   * 프로젝트 보고서
   * 프로젝트(재무 데이터) 보고서
   * 작업 보고서
   * 문제 보고서
   * 예산 시간 보고서
