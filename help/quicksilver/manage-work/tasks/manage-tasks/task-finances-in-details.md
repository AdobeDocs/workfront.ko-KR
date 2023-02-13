---
product-area: projects
navigation-topic: manage-tasks
title: 작업 세부 정보 섹션의 작업 재무 관리
description: 작업 세부 정보 섹션의 작업 재무 관리
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# 작업 세부 정보 섹션의 작업 재무 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

작업 세부 사항 섹션의 개요 영역에 액세스하여 작업의 재무 정보를 보거나 편집할 수 있습니다. 이 영역에서는 보거나 편집할 수 있는 제한된 수의 필드가 있습니다. 작업에 대한 모든 재무 정보 편집에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 액세스 편집</p> <p>재무 데이터 이상에 대한 액세스 보기</p> <p>작업에 대한 재무 정보를 편집하려면 재무 데이터에 대한 편집 액세스 권한이 있어야 합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 보기 이상을 포함하는 작업에 대한 권한 보기</p> <p>작업에 대한 재무 정보를 편집하려면 재무 편집을 포함하는 작업에 대한 관리 권한이 있어야 합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 세부 정보 섹션에서 작업 재무 편집

1. 작업을 보려는 프로젝트로 이동합니다.

   >[!NOTE]
   >
   >작업을 찾으려면 해당 작업을 검색하고 이름을 클릭하여 작업에 액세스할 수도 있습니다. Workfront에서 개체 검색에 대한 자세한 내용은 [Adobe Workfront 검색](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 보려는 작업 이름을 클릭합니다.
1. 클릭 **작업 세부 사항**.
1. (선택 사항) **모두 축소** 작업 세부 사항 페이지의 오른쪽 상단에 있는 아이콘을 클릭합니다.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 작업 세부 사항 섹션의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 클릭 **재무** 작업에 대한 재무 정보를 확장하고 조회하려면

   을(를) 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) 세부 사항 섹션의 오른쪽 위 모서리에서 **재무**.

1. 필드를 한 번 클릭하거나 **+추가** 를 눌러 빈 필드에 정보를 추가합니다.
1. 에서 다음 정보를 검토하거나 편집합니다 **재무** 영역 :

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
     <tr> 
      <td role="rowheader">계획된 비용</td> 
      <td> <p>계획 시간, 비용 유형 및 사용자 또는 작업 역할에 대한 시간별 비율을 기준으로 작업 비용을 표시하는 계산입니다. 추적 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 비용</td> 
      <td> <p> 실제 시간, 비용 유형 및 사용자 또는 작업 역할에 대한 시간별 비율을 기준으로 작업 비용을 표시하는 계산입니다. 추적 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 수익</td> 
      <td> <p>계획된 시간, 매출 유형 및 사용자 또는 작업 역할에 대한 시간별 비율을 기반으로 작업과 연관된 수익을 표시하는 계산입니다. 추적 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 매출</td> 
      <td> <p>실제 시간, 매출 유형 및 사용자 또는 작업 역할에 대한 시간별 비율을 기반으로 작업과 연관된 수익을 표시하는 계산입니다. 추적 비용에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">비용 추적</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>특정 시간에 작업이 수행되는 방식을 보여주는 작업 성능 지표입니다. 이 값은 프로젝트의 성능 색인 방법에 따라 계산됩니다.<br>자세한 내용은 다음 문서를 참조하십시오.</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">원가 성과 지수 계산(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">SPI(일정 성과 인덱스) 계산 </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">원가 스케줄 성과 인덱스 계산(CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 시 예상(EAC)</td> 
      <td> <p>완료된 작업의 총 비용을 보여주는 계산입니다. 완료 시 추정에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">완료 시 예상 계산(EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 재무 섹션에서 필드를 편집하는 경우 **Save****Changes**.
