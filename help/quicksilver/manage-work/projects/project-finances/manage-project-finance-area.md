---
product-area: projects
navigation-topic: financials
title: 프로젝트 재무 영역의 정보 관리
description: 프로젝트 재무 영역의 정보 관리
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# 프로젝트 재무 영역의 정보 관리

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

프로젝트 세부 정보 섹션의 재무 영역에 액세스하여 프로젝트의 재무 정보를 보거나 편집할 수 있습니다. 이 영역에서는 보거나 편집할 수 있는 제한된 수의 필드가 있습니다. 프로젝트에 대한 모든 정보 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 보기 이상의 액세스</p> <p>프로젝트 및 재무 데이터에 대한 액세스를 편집하여 프로젝트의 재무 정보를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 보기 권한을 포함하는 프로젝트 이상의 권한 보기</p> <p>프로젝트에 대한 재무 정보를 편집할 재무 관리를 포함하는 프로젝트에 대한 권한을 관리합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 재무 영역 개요

재무 영역에서 정보를 보거나 편집할 때 다음 사항을 고려하십시오.

* 프로젝트 세부 정보의 재무 영역에서 찾을 수 있는 재무 정보는 태스크에서 프로젝트 레벨로 롤업되는 값과 프로젝트에 직접 입력된 정보를 나타냅니다. 일부 재무 정보는 작업 레벨뿐만 아니라 프로젝트에서 관리할 수 있습니다.
* 프로젝트에서 재무 영역을 보려면 프로젝트에 대한 보기 권한과 액세스 레벨의 재무 데이터에 대한 액세스 권한이 있어야 합니다.
* 재무 영역에서 정보를 편집하려면 프로젝트에 대한 관리 권한과 액세스 수준에서 재무 데이터에 대한 액세스 권한이 있어야 합니다. 그러나 프로젝트 소유자만 이 영역에 대한 정보를 편집해야 합니다.

## 프로젝트에 대한 재무 정보 보기

1. 프로젝트로 이동합니다.
1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) 세부 사항 섹션의 오른쪽 위 모서리에서 **재무**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Workfront 관리자가 레이아웃 템플릿을 구성한 방법에 따라 개요 섹션이 맨 먼저 나열되지 않고 이 경우 축소될 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 프로젝트의 재무 영역에서 다음 필드를 봅니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">성과 지수 방법</td> 
      <td> Workfront에서 근로값 지표를 계산하는 데 사용하는 방법을 제어합니다. 몇 시간 또는 비용을 기반으로 할 수 있습니다. <br>PIM에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">PIM(성능 인덱스 메서드) 설정</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI / SPI / CSI</td> 
      <td> <p>특정 시간에 프로젝트가 수행되는 방식을 보여주는 프로젝트 성능 지표입니다. 이 값은 성능 인덱스 방법을 기반으로 계산됩니다.<br>자세한 내용은 다음 문서를 참조하십시오. </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">원가 성과 지수 계산(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">SPI(일정 성과 인덱스) 계산 </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">원가 스케줄 성과 인덱스 계산(CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 시점 예측</td> 
      <td> PIM(성능 인덱스 방법)이 시간 기반인 경우 프로젝트 예상 총 비용(시간 단위)이며, PIM(성능 인덱스 방법)이 비용 기반인 경우 통화 값으로 표시됩니다.<br>완료 시 예상 계산에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">완료 시 예상 계산(EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">예산</td> 
      <td>이것은 프로젝트의 예산 세트입니다. 프로젝트 소유자가 수동으로 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">고정 비용</td> 
      <td>프로젝트에서의 다른 활동과는 무관하게 프로젝트에서의 고정 비용입니다. 프로젝트 소유자가 수동으로 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 비용</td> 
      <td>계획 시간 및 작업 할당자와 연관된 비율(작업 역할 또는 사용자)을 기준으로 프로젝트의 예상 비용입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 비용</td> 
      <td>그 프로젝트에서 발생하는 모든 비용. 실제 원가는 모든 실제 원가의 합계입니다. 인건비 비용(실제 시간 및 작업 역할과 연관된 비율 기준 또는 작업 역할을 로깅하는 사용자 기준), 비용 및 고정 비용을 프로젝트 또는 태스크와 연결할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">고정 수입</td> 
      <td>프로젝트 일정에 따라 예상 수익을 설정합니다. 고정 수익은 프로젝트 소유자가 수동으로 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 수익</td> 
      <td>계획 시간 및 작업 할당자와 연관된 비율(Job 역할 또는 사용자)을 기준으로 예상되는 예상 소득</td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 수익</td> 
      <td>실제 시간 및 작업 할당자와 연관된 비율(Job 역할 또는 사용자)을 기준으로 프로젝트의 실제 소득</td> 
     </tr> 
     <tr> 
      <td role="rowheader">청구된 수익</td> 
      <td> <p>청구 레코드에 캡처된 클라이언트 또는 다른 당사자에게 청구되는 수익입니다. 청구 레코드에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">청구 레코드 만들기</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## 프로젝트에 대한 재무 정보 편집

프로젝트 소유자는 프로젝트의 재무 하위 탭에 대한 정보를 편집할 수 있습니다.

Project Finance 하위 탭의 정보를 편집하려면

1. 소유자인 프로젝트로 이동합니다.

   >[!NOTE]
   >
   >다음 단계를 수행하려면 프로젝트에 대한 권한 관리 가 필요합니다. 프로젝트 소유자만 프로젝트의 재무 하위 탭을 변경할 것을 권장합니다.

1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) 세부 사항 섹션의 오른쪽 위 모서리에서 **재무** . 편집할 재무 영역이 열립니다.
1. 필드를 한 번 클릭하거나 **+추가** 를 눌러 빈 필드에 정보를 추가합니다.

   >[!TIP]
   >
   >Workfront에서 자동으로 계산하거나 필드에 대한 편집 권한이 없는 경우 편집할 수 없습니다.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. 아래 필드를 업데이트합니다.

   >[!NOTE]
   >
   >Workfront 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 프로젝트 세부 사항 섹션의 필드가 사용자 환경에서 다를 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">성과 지수 방법</td> 
      <td> <p>Workfront에서 프로젝트 성능 지표를 계산하는 데 사용하는 방법을 제어합니다. 관리자가 시스템 수준에서 설정하지만 프로젝트 수준에서 편집할 수도 있습니다. 다음 옵션 중 하나를 선택하십시오.</p> 
       <ul> 
        <li><strong>시간 기반:</strong>Workfront에서는 프로젝트의 CPI 및 EAC를 계산하는 데 계획 시간을 사용하고 프로젝트의 EAC는 시간 단위로 표시됩니다. </li> 
        <li><strong>비용 기반:</strong>Workfront은 프로젝트의 CPI 및 EAC를 계산할 때 계획 노무비를 사용하고 EAC는 통화 값으로 표시됩니다. 이 옵션을 선택하는 경우 작업 담당자(작업 역할 또는 사용자)가 비용 비율에 연결되어 있는지 확인합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">완료 시점 예측</td> 
      <td> <p>프로젝트 또는 작업이 완료될 때 예상되는 총 비용을 나타냅니다. 관리자가 시스템 수준에서 설정하지만 프로젝트 수준에서 편집할 수도 있습니다. 다음 옵션 중 하나를 선택하십시오.</p> 
       <ul> 
        <li><strong>프로젝트 수준에서 계산</strong>: 상위 태스크 및 프로젝트에 대한 EAC는 EAC Formula에 실제 시간/실제 노무비를 입력하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 포함됩니다.</li> 
        <li><strong>작업/하위 작업에서 롤업</strong>: 상위 태스크 및 프로젝트에 대한 EAC는 각 하위 태스크에 대한 EAC를 합하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 제외됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">예산</td> 
      <td>이 프로젝트에 대한 예산을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>고정 비용</strong> </td> 
      <td>이 프로젝트에 대한 고정 비용을 지정합니다. 여기에는 인건비 또는 비용 비용이 포함되지 않아야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>고정 수입</strong> </td> 
      <td> <p>이 프로젝트의 고정 수입을 지정합니다. 여기에는 파트너 또는 타사에 청구되는 청구 레코드에서 발생하는 수익이 포함되지 않아야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">프로젝트 통화</td> 
      <td> <p>시스템의 기본 통화와 다른 경우 이 프로젝트의 통화를 지정합니다. 시스템의 기본 통화는 Workfront 관리자가 정의합니다. Workfront에서 환율 설정에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">환율 설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **Save****Changes**.
