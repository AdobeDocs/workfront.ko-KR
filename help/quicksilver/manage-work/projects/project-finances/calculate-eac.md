---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 완료 시 예상 계산(EAC)
description: 성능 지표로, EAC(완료 시 예상) 는 프로젝트 또는 작업이 완료되었을 때 예상되는 총 비용을 나타냅니다.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 완료 시 예상 계산(EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

성능 지표로, EAC(완료 시 예상) 는 프로젝트 또는 작업이 완료되었을 때 예상되는 총 비용을 나타냅니다.

설정으로 EAC 값을 계산하는 방법을 정의할 수 있습니다. 

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
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 보기에 대한 권한이 있는 프로젝트에 대한 더 높은 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## EAC 계산 방법 정의

프로젝트 시스템 환경 설정의 일부로 Adobe Workfront 관리자가 EAC를 계산하는 방법을 정의할 수 있습니다. EAC는 다음 두 가지 방법 중 하나로 계산할 수 있습니다.

* [프로젝트 수준에서 계산](#calculate-at-the-project-level)
* [작업 및 하위 작업에서 롤업](#roll-up-from-tasks-and-subtasks)

완료 시 예상 계산 방법을 비롯하여 Workfront에서 프로젝트 환경 설정을 설정하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

프로젝트 관리자는 프로젝트의 재무 하위 탭에서 프로젝트 레벨에서 이 기본 설정을 변경할 수도 있습니다. 프로젝트의 재무 하위 탭 편집에 대한 자세한 내용은 [프로젝트 재무 영역의 정보 관리](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### 프로젝트 수준에서 계산 {#calculate-at-the-project-level}

상위 태스크 및 프로젝트에 대한 EAC는 EAC Formula에 실제 시간/실제 노무비를 입력하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 포함됩니다.

### 작업 및 하위 작업에서 롤업 {#roll-up-from-tasks-and-subtasks}

상위 태스크 및 프로젝트에 대한 EAC는 각 하위 태스크에 대한 EAC를 합하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 제외됩니다.

## PIM(성능 인덱스 방법)을 기반으로 EAC를 계산하는 방법

Workfront에서 EAC에 대한 계산은 프로젝트의 선택한 PIM(성능 인덱스 메서드)에 따라 다릅니다. 시스템 또는 프로젝트에 대한 PIM 설정에 대한 자세한 내용은 [PIM(성능 인덱스 메서드) 설정](../../../manage-work/projects/project-finances/set-pim.md).

* [시간 기반 PIM을 사용하여 EAC 계산](#calculate-eac-using-hour-based-pim)
* [비용 기반 PIM을 사용하여 EAC 계산](#calculate-eac-using-cost-based-pim)

### 시간 기반 PIM을 사용하여 EAC 계산 {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;원가 성과 인덱스인 경우 [원가 성과 지수 계산(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = 총 계획 시간 + 실제 시간 이 문제는 시간이 캡처되었지만 프로젝트/작업이 0% 완료된 경우에 발생합니다.

CPI 계산에 대한 자세한 내용은 [원가 성과 지수 계산(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### 비용 기반 PIM을 사용하여 EAC 계산 {#calculate-eac-using-cost-based-pim}

프로젝트의 EAC는 다음 공식을 사용하여 계산됩니다.

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC 노무 =  <em>IF</em> CPI 노무 &lt;&gt; 0 다음 EAC 노무 = 계획된 노무 비용/CPI 노무</pre><pre><em>ELSE</em> EAC 노무 = 계획된 노무비 + 실제 노무비</pre><pre>CPI 노무 = IF 실제 노무비 &lt;&gt; 0 CPI 노무 = TotalBudgetCostWorkPerformed / 실제 노무비</pre><pre>ELSE CPI 인건비 = 1 </pre>EAC를 계산할 때 다음 필드가 고려됩니다.

* 수행된 총 예산책정된 원가 작업 시간(BCWP) = 계획된 작업(예산책정된 비용)의 예산책정된 비용과 지금까지 완료된 작업 비율을 곱한 결과입니다.

   수행된 총 예산책정된 비용 작업 시간(BCWP)에 대한 자세한 내용은 [수행된 예산 원가 작업 계산(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **비상위 작업의 경우:**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **상위 작업의 경우:**
수행된 총 예산책정된 원가 작업 시간 = 모든 직접 하위 태스크에 대한 총 예산책정된 원가 작업 수행 필드의 합계입니다.

   * **프로젝트의 경우:**
수행된 총 예산책정된 원가 작업 시간 = 모든 최상위 레벨 태스크에 대한 총 예산책정된 원가 작업 수행 필드의 합계(상위 및 독립형 태스크). 

* EAC 비용 = 발생된 실제 비용 비용을 발생되지 않은 계획 비용 비용에 추가한 결과. 다음 수식으로 계산됩니다.

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * 발생된 실제 비용 원가 = 실제 금액 필드가 0보다 큰 모든 비용에 대한 계획 금액 필드의 합계입니다. 예를 들어, 태스크 1에 대한 비용을 생성하고 계획 금액 필드에 $500.00를 입력하고 실제 금액 필드에 금액 > 0을 입력하는 경우, 600달러) 이 작업에 대한 비용 발생 예정 비용은 $500.00입니다.
   * 발생되지 않은 계획 비용 = 실제 금액 필드가 0인 모든 비용에 대한 계획 금액 필드의 합계입니다. 예를 들어, 태스크 1에 대해 첫 번째 비용에 대해 계획 금액 필드의 값이 $500.00이고 실제 금액의 값이 $600.00이고 두 번째 비용에 대해 계획 금액 필드의 값은 $300.00이고 실제 금액 필드의 값은 $0.00인 경우, 이 태스크에 대해 발생되지 않은 계획 비용 값은 $300.00입니다. 

## 프로젝트 또는 작업에서 EAC 찾기

1. EAC를 보려는 프로젝트 또는 작업으로 이동합니다.
1. 확장 **프로젝트 세부 사항** 또는 **작업 세부 사항** EAC를 보는 위치에 따라 프로젝트 또는 작업의 왼쪽 패널에 표시됩니다.

1. 클릭 **재무**. 

   EAC 값은 **완료 시 예상** 필드.

   ![](assets/eac-highlighted-on-project-350x112.png)
