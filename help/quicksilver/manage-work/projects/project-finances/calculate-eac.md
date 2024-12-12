---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: EAC(완료 시 추정 비용) 계산
description: 성과 지표인 EAC(완료 시 추정 비용)는 프로젝트 또는 작업이 완료될 때의 예상 총 비용을 나타냅니다.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# EAC(완료 시 추정 비용) 계산

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

성과 지표인 EAC(완료 시 추정 비용)는 프로젝트 또는 작업이 완료될 때의 예상 총 비용을 나타냅니다.

설정으로서 EAC 값을 계산하는 방법을 정의할 수 있습니다. 

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <p>새로운 기능: 밝게 또는 높음</p>
   <p>또는</p>
   <p>현재: 검토 이상</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>프로젝트 및 재무 데이터에 대한 액세스 보기</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 보기 권한이 있는 프로젝트에 대한 보기 이상의 권한</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## EAC 계산 방법 정의

프로젝트 시스템 환경 설정의 일부로 Adobe Workfront 관리자는 EAC를 계산하는 방법을 정의할 수 있습니다. EAC는 다음 두 가지 방법 중 하나로 계산할 수 있습니다.

* [프로젝트 수준에서 계산](#calculate-at-the-project-level)
* [작업 및 하위 작업에서 롤업](#roll-up-from-tasks-and-subtasks)

완료 시 예상 값을 계산하는 방법을 포함하여 Workfront에서 프로젝트 환경 설정을 설정하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

프로젝트 관리자는 프로젝트의 재무 하위 탭에서 프로젝트 수준에서 이 환경 설정을 변경할 수도 있습니다. 프로젝트의 재무 하위 탭을 편집하는 방법에 대한 자세한 내용은 [프로젝트 재무 영역의 정보 관리](../../../manage-work/projects/project-finances/manage-project-finance-area.md)를 참조하십시오.

### 프로젝트 수준에서 계산 {#calculate-at-the-project-level}

상위 태스크 및 프로젝트에 대한 EAC는 EAC 공식에 실제 시간/실제 인건비를 입력하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 비용이 포함됩니다.

### 작업 및 하위 작업에서 롤업 {#roll-up-from-tasks-and-subtasks}

상위 작업 및 프로젝트에 대한 EAC는 각 하위 작업에 대한 EAC를 합산하여 결정됩니다. 이 계산에는 상위 작업 또는 프로젝트에 직접 추가된 실제 시간/비용 및 경비가 제외됩니다.

## PIM(Performance Index Method)을 기반으로 EAC를 계산하는 방법

Workfront에서 EAC에 대한 계산은 프로젝트의 선택된 PIM(성능 인덱스 메서드)에 따라 다릅니다. 시스템 또는 프로젝트의 PIM 설정에 대한 자세한 내용은 [PIM(성능 인덱스 메서드) 설정](../../../manage-work/projects/project-finances/set-pim.md)을 참조하십시오.

* [시간 기반 PIM을 사용하여 EAC 계산](#calculate-eac-using-hour-based-pim)
* [비용 기반 PIM을 사용하여 EAC 계산](#calculate-eac-using-cost-based-pim)

### 시간 기반 PIM을 사용하여 EAC 계산 {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;원가 성과 지수 [원가 성과 지수 계산](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0인 경우, EAC = 총 계획된 시간 + 실제 시간. 이 문제는 시간이 캡처되었지만 프로젝트/작업이 0% 완료된 경우에 발생합니다.

CPI 계산에 대한 자세한 내용은 [CPI(비용 성과 지표) 계산](../../../manage-work/projects/project-finances/calculate-cpi.md)을 참조하십시오.

### 비용 기반 PIM을 사용하여 EAC 계산 {#calculate-eac-using-cost-based-pim}

프로젝트의 EAC는 다음 공식을 사용하여 계산됩니다.

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC 인건비 =  <em>IF</em> CPI 인건비 &lt;&gt; 0 다음 EAC 인건비 = 계획된 인건비 / CPI 인건비</pre><pre><em>ELSE</em> EAC  노무 = 계획 노무비 + 실제 노무비</pre><pre>CPI 노무 = 실제 인건비 &lt;&gt; 0인 경우 CPI 노무 = 총 예산 비용작업수행 / 실제 인건비</pre><pre>ELSE CPI 인건비 = 1 </pre>EAC를 계산할 때 다음 필드를 고려합니다.

* 수행된 총 예산 비용 작업(BCWP) = 계획된 작업의 예산 비용(예산 비용)과 지금까지 완료된 작업의 비율을 곱한 결과입니다.

  BCWP(수행된 총 예산 비용 작업)에 대한 자세한 내용은 [BCWP(수행된 예산 비용 작업) 계산](../../../manage-work/projects/project-finances/calculate-bcwp.md)을 참조하십시오.

   * **부모가 아닌 작업의 경우:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **상위 작업의 경우:**
수행된 총 예산 비용 작업 수 = 모든 직접 하위 작업에 대해 수행된 총 예산 비용 작업 수 필드의 합계.

   * **프로젝트의 경우:**
수행된 총 예산 비용 작업 수 = 모든 최상위 레벨 태스크(상위 및 독립형 태스크)에 대한 수행된 총 예산 비용 작업 수 필드의 합계 

* EAC 비용 = 발생하지 않은 계획된 비용 비용에 실제 비용 발생 비용을 추가한 결과. 이 값은 다음 공식에 의해 계산됩니다.

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * 발생 실제 비용 = 실제 금액 필드가 0보다 큰 모든 비용에 대한 계획된 금액 필드의 합계. 예를 들어, 태스크 1에 대한 경비를 생성하고 계획 금액 필드에 $500.00를 입력하고 실제 금액 필드에 0을 초과하는 금액(즉, $600.00)을 입력하면, 이 태스크에 대해 발생한 계획 경비 비용은 $500.00입니다.
   * 미발생 계획 비용 = 실제 금액 필드가 0인 모든 비용에 대한 계획 금액 필드의 합계. 예를 들어, 첫 번째 경비의 경우 계획된 금액 필드의 값이 $500.00이고 실제 금액의 값이 $600.00인 태스크 1에 대해 두 개의 경비를 생성하고 두 번째 경비의 경우 계획된 금액 필드의 값이 $300.00이고 실제 금액 필드의 값이 $0.00인 경우 이 태스크의 미발생 계획된 경비의 값은 $300.00입니다. 

## 프로젝트 또는 작업에서 EAC 찾기

1. EAC를 보려는 프로젝트 또는 작업으로 이동합니다.
1. EAC를 보는 위치에 따라 프로젝트 또는 작업의 왼쪽 패널에서 **프로젝트 세부 정보** 또는 **작업 세부 정보**&#x200B;을(를) 확장합니다.

1. **재무**&#x200B;을 클릭합니다. 

   EAC 값이 **완료 시 예상** 필드에 표시됩니다.

   ![](assets/eac-highlighted-on-project-350x112.png)
