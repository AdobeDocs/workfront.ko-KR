---
content-type: reference
product-area: projects
navigation-topic: financials
title: 예산책정된 비용 계산
description: 가동률 보고서를 사용하여 예산책정된 원가 추적 프로젝트 진행 계산"
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# 예산책정된 비용 계산

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

프로젝트의 예산책정된 원가는 프로젝트를 계획할 때 예상된 프로젝트와 연관된 총 원가입니다.

## 프로젝트의 예산책정된 원가 개요

프로젝트의 예산책정된 원가는 수동으로 변경할 수 없습니다. Adobe Workfront은 다음 공식을 사용하여 예산책정된 원가를 계산합니다.

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 다음 **자원 계획자 예산 노무비** 위의 계산에서는 프로젝트의 작업 역할과 연관된 비용이 있습니다.

   Business Case 또는 Resource Planner의 Resource Budgeting 영역에서 프로젝트의 예산책정된 노무비를 추적할 수 있습니다.

   >[!TIP]
   >
   >  비즈니스 케이스의 프로젝트의 예산책정된 노무비는 보고서 및 목록의 자원 계획자 예산책정된 노무비로 표시됩니다.

   예산책정된 인건비 비용에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 대한 예산책정된 노무비 및 예산책정 시간 이해](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* 다음 **예산책정된 비용** 위의 계산에서 프로젝트 비용과 연관된 계획 원가는 업무 사례의 비용 영역 또는 프로젝트의 비용 탭에서 계산되며,\
   프로젝트 비용에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 비용 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* 다음 **고정 비용** 위의 계산에서 프로젝트 상세내역 섹션의 재무 영역에 정의되어 있는 프로젝트 원가와 연관된 고정 금액이 있습니다.\
   프로젝트의 재무 하위 탭에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 재무 영역의 정보 관리](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront은 프로젝트의 통화를 사용하여 모든 비용 정보를 계산합니다. 자원 계획자에서 자원에 대한 예산책정된 시간을 지정하는 경우 프로젝트 통화를 변경하는 옵션이 비활성화됩니다.
>
>프로젝트 통화 변경에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md).

## 프로젝트의 예산책정된 비용 찾기

업무 사례의 자원 예산 영역 또는 자원 계획자가 반영되는 예산책정된 비용은 다음 이름 아래에 Workfront의 다음 영역에 표시됩니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>예산책정된 원가 표시명</strong></td> 
     <td><strong>Workfront 지역</strong></td> 
    </tr> 
    <tr> 
     <td>예산 비용</td> 
     <td> <p>비즈니스 사례 요약</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>비용</td> 
     <td> <p>Portfolio 최적화 프로그램</p> <p>팁: 모든 프로젝트 예산책정된 원가 값의 합계는 포트폴리오의 예산책정된 원가입니다.</p> </td> 
    </tr> 
    <tr> 
     <td>프로젝트 예산 비용</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>프로젝트 보고서</p> <p>프로젝트(재무 데이터) 보고서</p> <p>작업 보고서</p> <p>문제 보고서</p> <p>예산책정된 시간 보고서</p> <p>보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
