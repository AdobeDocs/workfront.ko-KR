---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 예약된 작업의 예산 비용 계산(BCWS)
description: 계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업의 양을 나타내는 프로젝트 성능 지표입니다.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 2%

---

# 예약된 작업의 예산 비용 계산(BCWS)

## BCWS(예약된 작업의 예산 비용) 개요

계획된 값이라고도 하는 BCWS(Budgeted Cost of Work Scheduled)는 이 지표가 계산되는 시점에 완료해야 하는 작업의 양을 나타내는 프로젝트 성능 지표입니다.

Adobe Workfront은 프로젝트 및 작업 모두에 대해 BCWS(예약된 작업의 예산 비용)를 계산합니다.

작업 또는 프로젝트에서 BCWS에 대한 값을 검토할 때 다음 사항을 고려하십시오.

* Workfront은 프로젝트의 PIM(Performance Index Method)에 대한 구성을 기반으로 작업에 대한 BCWS를 계산합니다.

  시간이나 비용을 사용하여 PIM을 계산하도록 프로젝트를 구성할 수 있으며 BCWS도 동일한 값을 사용하여 계산됩니다.

  BCWS 계산 방법 구성에 대한 자세한 내용은 이 문서의 [BCWS 계산 방법 구성](#configure-how-bcws-is-calculated) 섹션을 참조하십시오.

* Workfront은 프로젝트의 모든 상위 작업 및 개별 작업에서 모든 BCWS 값을 추가하여 프로젝트에 대한 BCWS를 계산합니다.

  하위 작업의 값은 프로젝트의 BCWS에 추가되지 않습니다.

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
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>프로젝트에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>프로젝트에 대한 권한 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## BCWS 계산 방법 구성 {#configure-how-bcws-is-calculated}

프로젝트의 PIM(Performance Index Method) 계산 방법을 구성하여 BCWS를 시간 단위로 계산할지 비용 단위로 계산할지 구성할 수 있습니다.

1. 프로젝트로 이동한 다음 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭합니다.
1. **재무** 영역에서 **성과 지표 메서드** 필드를 찾아 두 번 클릭하여 편집합니다.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 다음 옵션 중에서 선택합니다.

   | 옵션 | 계산 수행 방법 |
   |---|---|
   | 시간 기반 | Workfront은 작업의 계획된 시간을 사용하여 BCWS를 계산합니다. |
   | 비용 기반 | Workfront은 작업의 계획된 비용을 사용하여 BCWS를 계산합니다. |


1. **변경 내용 저장**&#x200B;을 클릭합니다.

   프로젝트에 대한 작업의 BCWS는 시간 또는 비용을 사용하여 계산됩니다.

## BCWS 계산

Workfront은 다음 공식을 사용하여 작업 또는 프로젝트에 대한 BCWS(예정된 작업 비용)를 계산합니다.

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

다음 값이 이 계산에 사용됩니다.

| 값 사용됨 | 사용된 값 설명 |
|---|---|
| 계획된 완료율 | 작업 시작부터 오늘까지 경과된 시간을 살펴보면 작업의 완료율이 다음과 같습니다. |
| 작업 예산 | 작업의 계획된 시간 또는 계획된 비용에 대한 값입니다. |

예를 들어 오늘 2월 12일이고 작업이 2월 10일부터 2월 20일까지 지속되도록 예약된 경우 작업은 오늘 20% 완료되어야 합니다. 작업 예산(계획된 비용)이 $10,000인 경우 작업의 BCWS는 다음과 같습니다.

```
Task BCWS = 20% x $10,000 = $2,000
```

## 프로젝트 또는 작업에 대한 BCWS 찾기

BCWS 열을 보기에 추가하여 보고서 또는 목록에서 예약된 작업의 예산 비용 값을 볼 수 있습니다.

1. 작업 또는 프로젝트 목록으로 이동합니다.
1. **보기** 메뉴를 확장하고 **새 보기** 또는 **보기 사용자 지정**&#x200B;을 선택합니다.

1. **열 추가**&#x200B;를 클릭합니다.
1. **이 열에 표시:** 필드에서 **BCWS**&#x200B;을(를) 입력하고 목록에 표시될 때 클릭하여 선택합니다.

   ![](assets/bcws-in-project-view.png)

1. **보기 저장**&#x200B;을 클릭합니다.
1. **BCWS** 필드가 보기에 표시됩니다.
