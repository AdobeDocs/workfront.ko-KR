---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 수행된 작업의 예산 비용 계산(BCWP)
description: BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 양을 나타내는 프로젝트 성능 지표입니다.
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 수행된 작업의 예산 비용 계산(BCWP)

## 수행된 작업의 예산 비용 개요(BCWP)

BCWP(Backed Cost of Work Performed)라고도 하는 Earned Value는 이 지표가 계산될 때 실제로 완료된 작업의 양을 나타내는 프로젝트 성능 지표입니다.

Adobe Workfront은 프로젝트 및 작업 모두에 대해 수행된 작업의 예산 비용(BCWP)을 계산합니다.

작업이나 프로젝트에서 BCWP 값을 검토할 때는 다음 사항을 고려하십시오.

* Workfront은 프로젝트의 PMI(성능 인덱스 메서드)에 대한 구성에 따라 작업에 대한 BCWP를 계산합니다.

   몇 시간이나 비용을 사용하여 PMI를 계산하도록 프로젝트를 구성할 수 있으며 BCWP도 동일한 값을 사용하여 계산됩니다.

   BCWP 계산 방법 구성에 대한 자세한 내용은 섹션을 참조하십시오 [BCWP 계산 방법 구성](#configure-how-bcwp-is-calculated) 참조하십시오.

* Workfront은 프로젝트의 모든 상위 작업과 개별 작업에서 모든 BCWP 값을 추가하여 프로젝트의 BCWP를 계산합니다.

   하위 작업의 값은 프로젝트의 BCWP에 추가되지 않습니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## BCWP 계산 방법 구성 {#configure-how-bcwp-is-calculated}

프로젝트의 PIM(성능 인덱스 방법)을 계산하는 방법을 구성하여 BCWP를 몇 시간 단위로 계산할지 또는 비용을 계산할지 여부를 구성할 수 있습니다.

1. 프로젝트로 이동하여 확장 **프로젝트 세부 사항** 왼쪽 패널에 표시됩니다.
1. 에서 **재무** 영역, 위치 **성능 인덱스 메서드** 필드를 입력하고 두 번 클릭하여 편집합니다.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 다음 옵션 중에서 선택합니다.

   | 옵션 | 계산 수행 방법 |
   |---|---|
   | 시간 기반 | Workfront은 작업의 계획된 시간을 사용하여 BCWP를 계산합니다. |
   | 비용 기반 | Workfront은 작업의 계획된 비용을 사용하여 BCWP를 계산합니다. |

1. 클릭 **변경 내용 저장**.

프로젝트 작업의 BCWP는 시간 또는 비용을 사용하여 계산됩니다.

## BCWP 계산

Workfront은 다음 공식을 사용하여 작업 또는 프로젝트에 대한 BCWP(수행된 작업의 예산 비용)를 계산합니다.

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

다음 값이 이러한 계산에 사용됩니다.

| 사용된 값 | 사용된 값에 대한 설명입니다 |
|---|---|
| 실제 완료율 | Workfront에 나타나는 작업의 실제 완료율입니다. |
| 작업 예산 | 작업의 계획 시간 또는 계획 비용에 대한 값입니다. |

예를 들어 작업의 실제 완료율이 25%이고 작업 예산 또는 계획 비용이 $10,000인 경우 작업에 대한 BCWP는 다음과 같습니다.

```
BCWP = 25% x $10,000 = $2,500
```

## 프로젝트 또는 작업의 BCWP를 찾습니다.

BCWP 열을 뷰에 추가하여 보고서나 목록에 수행된 작업 비용 예산책정 값을 볼 수 있습니다.

1. 작업 또는 프로젝트 목록으로 이동합니다.
1. 를 확장합니다. **보기** 메뉴 및 선택 **새 보기** 또는 **보기 사용자 지정**.

1. 클릭 **열 추가**.
1. 에서 **다음 열에 표시:** 필드 입력 시작 **BCWP** 목록에 표시될 때 클릭하여 선택합니다.

   ![](assets/bcwp-project-view.png)

1. 클릭 **보기 저장**.
1. BCWP 필드가 보기에 표시됩니다.
