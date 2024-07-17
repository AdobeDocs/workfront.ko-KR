---
content-type: reference
product-area: projects
navigation-topic: financials
title: 예산 비용 계산
description: 활용성 보고서로 예산 CostTracking 프로젝트 진행 계산""
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# 예산 비용 계산

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

프로젝트의 예산 비용은 프로젝트를 계획할 때 예상한 대로 프로젝트와 연관된 총 비용입니다.

## 프로젝트의 예산 비용 개요

프로젝트의 예산 비용을 수동으로 변경할 수 없습니다. Adobe Workfront은 다음 공식을 사용하여 예산 비용을 계산합니다.

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 위의 계산에서 **리소스 플래너 예산 인건비**&#x200B;는 프로젝트의 작업 역할과 관련된 비용입니다.

  비즈니스 사례 또는 리소스 플래너의 리소스 예산 책정에서 프로젝트의 예산 인건비를 추적할 수 있습니다.

  >[!TIP]
  >
  >  비즈니스 사례에서 프로젝트의 예산 인건비는 보고서 및 목록에 리소스 플래너 예산 인건비로 표시됩니다.

  예산 인건비에 대한 자세한 내용은 문서 [프로젝트 예산 인건비 및 예산 시간 이해](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)를 참조하십시오.

* 위의 계산에서 **예산 경비**&#x200B;는 비즈니스 사례의 경비 영역 또는 프로젝트의 경비 탭에서 계산되므로 프로젝트의 경비와 연결된 계획된 경비입니다.\
  프로젝트 비용에 대한 자세한 내용은 문서 [프로젝트 비용 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md)를 참조하십시오.

* 위의 계산에서 **고정 비용**&#x200B;은(는) 프로젝트 세부 정보 섹션의 재무 영역에 정의된 대로 프로젝트 비용과 연결된 고정 금액입니다.\
  프로젝트의 재무 하위 탭에 대한 자세한 내용은 문서 [프로젝트 재무 영역의 정보 관리](../../../manage-work/projects/project-finances/manage-project-finance-area.md)를 참조하십시오.

>[!NOTE]
>
>Workfront은 프로젝트 통화를 사용하여 모든 비용 정보를 계산합니다. 리소스 플래너에서 리소스에 대한 예산 시간을 지정하는 경우 프로젝트 통화 변경 옵션이 비활성화됩니다.
>
>프로젝트 통화 변경에 대한 자세한 내용은 문서 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md)을 참조하십시오.

## 프로젝트의 예산 비용 찾기

비즈니스 사례 또는 리소스 플래너의 리소스 예산 편성 영역에 반영된 예산 원가는 다음과 같은 이름으로 Workfront의 다음 영역에 표시됩니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>예산 비용 표시 이름</strong></td> 
     <td><strong>Workfront 지역</strong></td> 
    </tr> 
    <tr> 
     <td>예산 비용</td> 
     <td> <p>비즈니스 사례 요약</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>비용</td> 
     <td> <p>Portfolio 최적화 도구</p> <p>팁: 모든 프로젝트 예산 비용 값의 합계는 포트폴리오의 예산 비용입니다.</p> </td> 
    </tr> 
    <tr> 
     <td>프로젝트 예산 비용</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>프로젝트 보고서</p> <p>프로젝트(재무 데이터) 보고서</p> <p>작업 보고서</p> <p>문제 보고서</p> <p>예산 시간 보고서</p> <p>보고서 만들기에 대한 자세한 내용은 문서 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>를 참조하십시오.</p> </td> 
    </tr> 
   </tbody> 
  </table>
