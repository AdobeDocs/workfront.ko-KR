---
navigation-topic: financials
title: 청구 기록 만들기
description: 수익 및 추적 경비를 설정하는 것 외에도 청구해야 하는 정보에 대한 청구 기록을 프로젝트에 만들 수 있습니다.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: fc82ce4b5abb2cd7411d62ac8bb428bc5337386f
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 1%

---

# 청구 기록 만들기

<!-- Audited: 6/2025 -->

수익 및 추적 경비를 설정하는 것 외에도 청구해야 하는 정보에 대한 청구 기록을 프로젝트에 만들 수 있습니다.

작업에 대한 청구 기록을 생성할 수 없으며 프로젝트에 대한 청구 기록만 생성할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>프로젝트 및 재무 데이터에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 관리 권한으로 프로젝트에 대한 권한 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 청구 기록 개요

청구 기록은 프로젝트에 대한 첨부 파일로 생성되며 프로젝트의 재무 데이터와 프로젝트 태스크의 재무 정보를 포함합니다.

청구 기록 사용을 계획할 때는 다음 사항을 고려하십시오.

* 외부 공급업체 또는 파트너에게 프로젝트와 관련된 금액을 청구하려는 경우 청구 기록을 생성합니다. 고정 금액을 외부 출처에 청구하는 것 외에도, 프로젝트에 대한 작업량(기록된 시간부터)뿐만 아니라 발생한 비용 또는 고정 수입 금액을 외부 계약자에게 청구해야 하는 경우가 있습니다. 이 모든 정보를 동일한 청구 기록에 포함할 수 있습니다.
* 청구 기록이 청구됨으로 설정되면 편집할 수 없습니다.

  >[!IMPORTANT]
  >
  >이는 요금이 다르고 프로젝트에 대한 수입 및 경비 정보를 잠그려는 경우에 중요합니다. 청구 기록에 추가하고 청구됨으로 표시하면 시스템에서 요금이 업데이트될 때 업데이트되지 않습니다.

* 청구됨으로 표시된 청구 기록이 있는 프로젝트는 삭제할 수 없습니다.

## 청구 기록 만들기

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.
1. 왼쪽 패널에서 **청구 기록**&#x200B;을 클릭합니다.
1. **새 청구 기록**&#x200B;을 클릭합니다.
1. 표시되는 **새 청구 기록** 상자에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>(필수) 청구 기록에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">청구 상태</td> 
      <td> <p>이 레코드가 아직 청구되지 않은 경우 <strong>청구되지 않음</strong>을 선택합니다.</p> <p>청구 기록이 청구된 경우 <strong>청구됨</strong>을(를) 선택하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">청구 일자</td> 
      <td>달력 아이콘을 클릭하여 이 청구 기록이 청구된 날짜를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">PO 번호</td> 
      <td>이 청구 기록과 연관된 PO 번호를 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">인보이스 ID</td> 
      <td>이 청구 기록과 연관된 송장을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">추가 금액</td> 
      <td>청구 기록의 고정 금액을 입력합니다. 이 프로젝트에 대해 외부 고객, 계약자 또는 파트너에게 청구하려는 금액입니다. 청구 기록 상태가 청구됨으로 변경된 후에는 이 금액을 수정할 수 없습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **사용자 지정 Forms**&#x200B;에서 레코드에 추가할 청구 기록 사용자 지정 양식을 선택합니다.

   여기에서 청구 기록 사용자 정의 양식을 선택하려면 먼저 만들어야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. **저장 을 클릭합니다.** 청구 기록이 만들어졌습니다.

## 청구 기록에 청구 가능 시간, 경비 및 고정 수익 포함

### 청구 기록에 청구 가능 시간 포함 {#include-billable-hours-in-a-billing-record}

작업, 문제 또는 프로젝트에 기록된 시간을 청구 기록에 포함할 수 있습니다.

시간을 기록하는 사용자 또는 기본 작업 역할이 시간당 청구 요금과 연결된 경우 이 시간의 수익이 청구 기록에 추가됩니다.

* [청구 기록에 추가할 수 있는 시간](#what-hours-can-be-added-to-a-billing-record)
* [청구 기록에 시간 추가](#add-hours-to-a-billing-record)

#### 청구 기록에 추가할 수 있는 시간 {#what-hours-can-be-added-to-a-billing-record}

다음 조건이 충족될 때 청구 기록에 시간을 추가할 수 있습니다.

* 작업, 문제 또는 프로젝트에 대한 시간이 기록되었습니다.
* 기록된 시간의 시간 유형이 매출로 표시됩니다.

  자세한 내용은 문서 [시간 유형 관리](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)를 참조하십시오.

* 시간을 기록하는 사용자가 해당 사용자 또는 기본 작업 역할과 연계된 시간당 청구 요금이 있는 경우 문제 또는 프로젝트에 기록된 모든 시간을 청구 기록에 추가할 수 있습니다.
* 작업에 시간이 기록된 경우 작업의 수익 유형은 다음과 같아야 합니다.

   * 수익 유형을 청구 불가능으로 설정할 수 없습니다.
   * 매출 유형 이 시간별 사용자로 설정된 경우 시간을 기록하는 사용자는 프로필에 시간당 청구 요금이 설정되어 있어야 합니다.
   * 수익 유형이 시간별 역할로 설정된 경우 시간을 기록하는 사용자의 기본 역할에는 시간당 청구 요금이 있어야 합니다.

     >[!NOTE]
     >
     >프로젝트 수준에서 작업 역할에 대한 청구 요율을 재정의할 수 있습니다.\
     >자세한 내용은 문서 [프로젝트 작업 역할 청구 요금 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)에서 프로젝트 수준의 작업 역할 청구 요금 오버라이드 섹션을 참조하십시오.

* 프로젝트 설정에서 이 프로젝트에 대한 승인 필요 옵션을 선택한 경우 프로젝트 소유자는 기록된 시간을 승인해야 합니다.\
  자세한 내용은 [프로젝트 승인 시간 필요](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md)를 참조하십시오.

#### 청구 기록에 시간 추가 {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.
1. 왼쪽 패널에서 **청구 기록**&#x200B;을 클릭합니다.
1. 청구 기록 **설명**&#x200B;을 클릭하여 **청구 기록 세부 정보** 탭을 엽니다.
1. 왼쪽 패널에서 **청구 가능 시간**&#x200B;을 클릭합니다.
1. 청구 기록에 포함할 수 있는 시간이 있으면 **시간 추가**&#x200B;를 클릭하세요. **청구 가능 시간 추가** 상자가 열립니다.

   >[!NOTE]
   >
   >기록된 시간이 없거나 기록된 시간이 청구 기록에 추가해야 하는 조건을 충족하지 않는 경우 **시간 추가** 단추가 표시되지 않습니다. 자세한 내용은 이 문서의 다음 섹션을 참조하십시오. [청구 기록에 추가할 수 있는 시간](#what-hours-can-be-added-to-a-billing-record).

1. 청구 기록에 포함할 시간 항목을 선택한 다음 **시간 추가**&#x200B;를 클릭합니다. 실제 시간 비용은 **청구 기록 합계**&#x200B;에 **청구 가능 시간** 금액으로 추가됩니다.

1. (선택 사항) **청구 기록 세부 정보**&#x200B;를 클릭하여 **청구 가능 시간** 및 **청구 기록 합계** 금액과 청구 기록 헤더의 청구 기록 합계를 검토합니다.

### 청구 기록에 청구 가능 경비 포함 {#include-billable-expenses-in-a-billing-record}

청구 기록에 청구 가능 경비를 추가하는 경우 작업과 프로젝트의 비용이 청구 가능으로 표시되는지 확인합니다. 청구 가능으로 표시되지 않은 경비는 청구 기록에 추가할 수 없습니다. 경비 추가에 대한 자세한 내용은 문서 [프로젝트 경비 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md)를 참조하십시오.

청구 기록에 청구 가능 경비를 추가하려면

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.
1. 왼쪽 패널에서 **청구 기록**&#x200B;을 클릭합니다.
1. 청구 기록 **설명**&#x200B;을 클릭하여 **청구 기록 세부 정보** 탭을 엽니다.
1. 왼쪽 패널에서 **청구 가능한 경비**&#x200B;를 클릭합니다.
1. (조건부) 작업 또는 프로젝트에 경비를 추가하고 청구 가능으로 표시한 경우 **경비 추가**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >경비가 있지만 청구 가능으로 표시되지 않으면 **경비 추가** 단추가 표시되지 않습니다. 실제 금액이 0보다 큰 청구 가능 비용만 청구 기록에 포함될 수 있습니다.

1. 청구 기록에 추가할 수 있는 청구 가능 경비를 선택한 다음 **경비 추가**&#x200B;를 클릭합니다.  실제 경비는 **청구 기록 합계**&#x200B;에 **청구 가능 경비** 금액으로 추가됩니다.

1. (선택 사항) **청구 기록 세부 정보**&#x200B;를 클릭하여 **청구 가능 경비** 및 **청구 기록 합계** 금액과 청구 기록 헤더의 청구 기록 합계를 검토합니다.

### 청구 기록에 고정 수익 포함 {#include-fixed-revenues-in-a-billing-record}

고정 수익을 사용할 수 있는 작업이 있는 경우 청구 기록에 고정 수익을 추가할 수 있습니다. 청구 기록에 추가할 수 있는 다른 유형의 작업 또는 프로젝트 수익이 없습니다. 수익 유형에 대한 자세한 내용은 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) 문서의 청구 및 수익 개요 섹션을 참조하십시오.

{{step1-to-projects}}

1. **프로젝트** 페이지에서 프로젝트를 선택하십시오.
1. 왼쪽 패널에서 **청구 기록**&#x200B;을 클릭합니다.
1. 청구 기록의 **설명**&#x200B;을 클릭하여 **청구 기록 세부 정보** 탭을 엽니다.
1. **고정 수입** 탭을 선택합니다.
1. 고정 수입을 작업에 추가한 경우 **고정 수입 추가**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >작업에 매출액이 있지만 [고정]으로 표시되지 않으면 **고정 매출액 추가** 단추가 표시되지 않습니다.

1. 청구 기록에 포함할 고정 수익이 있는 작업을 선택한 다음 **작업 추가**&#x200B;를 클릭합니다.  **고정 수입** 작업 금액이 **청구 기록 합계**&#x200B;에 **청구 가능 수입** 금액으로 추가됩니다.

1. (선택 사항) **청구 기록 세부 정보**&#x200B;를 클릭하여 **청구 가능 수익** 및 **청구 기록 합계** 금액과 청구 기록 헤더의 청구 기록 합계를 검토합니다.

## 청구 기록 편집

청구 기록을 생성하고 시간, 경비 및 수익을 추가한 후 청구됨으로 표시되기 전에 기존 기록의 일부 정보를 편집할 수 있습니다.

1. 청구 기록으로 이동합니다.
1. 왼쪽 패널에서 **청구 기록 세부 정보**&#x200B;를 선택합니다.
1. 사용 가능한 모든 필드의 정보를 편집합니다.

   또는

   오른쪽 상단의 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭한 다음 사용 가능한 필드에서 정보를 편집합니다.

   다음 내용을 업데이트합니다.

   * **설명**
   * **청구 일자**
   * **청구 상태**

     >[!TIP]
     >
     >청구 상태에 대해 **청구됨**&#x200B;을(를) 선택하면 변경 내용을 저장한 후에는 청구 기록을 편집할 수 없습니다.

   * **송장 ID**
   * **PO 번호**
   * **추가 금액**

   다음 필드는 편집할 수 없습니다.

   * **청구 가능 시간:** 청구 기록에 포함된 시간의 총 실제 매출입니다. 자세한 내용은 이 문서의 다음 섹션을 참조하십시오. [청구 기록에 청구 가능 시간 포함](#include-billable-hours-in-a-billing-record).

   * **청구 가능 경비**: 청구 기록에 포함된 청구 가능 경비의 실제 총액입니다. 자세한 내용은 이 문서의 다음 섹션을 참조하십시오. [청구 기록에 청구 가능한 경비 포함](#include-billable-expenses-in-a-billing-record).

   * **청구 가능 수익**: 청구 기록에 포함된 작업의 총 고정 수익입니다. 자세한 내용은 이 문서의 다음 섹션을 참조하십시오. [청구 기록에 고정 수입 포함](#include-fixed-revenues-in-a-billing-record).

   * **청구 기록 합계**: 청구 가능한 모든 금액의 합계입니다. 이는 다음 공식에 의해 계산됩니다.

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. **변경 내용 저장**&#x200B;을 클릭합니다.
