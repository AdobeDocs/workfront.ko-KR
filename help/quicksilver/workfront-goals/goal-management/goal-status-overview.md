---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 상태 개요
description: 목표 상태는 목표가 활성 상태이고 현재 진행 상황을 기록하는지 또는 비활성 상태인지, 초안 상태인지, 이미 달성되었는지 여부를 나타냅니다.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 4%

---

# Adobe Workfront 목표의 목표 상태 개요

>[!IMPORTANT]
>
>이 문서에 설명된 기능을 사용하려면 조직에 다음 사항이 있어야 합니다.
>
>* 새 플랜 및 라이선스 구조의 경우:
>
>   * 궁극적인 Workfront 플랜
>    
>* 현재 플랜 및 라이선스 구조의 경우:
>
>   * Pro 이상의 Workfront 플랜
>   * Workfront 라이선스 외에 Adobe Workfront Goals 라이선스.
>
>Workfront Goals 라이선스에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오.
> 
>Workfront 목표에 액세스하는 방법에 대한 자세한 내용은 [Workfront 목표 사용 요구 사항](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md)을 참조하십시오.

## Workfront 목표에서 목표 상태를 업데이트할 때 고려 사항

* 사용자가 만들었거나 사용자와 공유된 목표의 상태를 수동으로 업데이트할 수 없습니다. 목표의 상태는 목표에 대해 수행하는 작업에 따라 업데이트됩니다. 예를 들어, 목표를 활성화하면 초안 상태가 활성으로 변경됩니다.
* 일부 제한 사항이 있으며 다음 규칙에 따라 목표 상태를 다른 상태로 변경할 수 없는 경우도 있습니다.

  | 부터/ 까지 | 초안 | 활성 | 비활성 | 마감됨 |
  |---|---|---|---|---|
  | 초안 | - | 예 | 아니요 | 아니요 |
  | 활성 | 아니요 | - | 예 | 예 |
  | 비활성 | 아니요 | 예 | - | 아니요 |
  | 마감됨 | 아니요 | 예 | 아니요 | - |

* 닫힌 목표를 열면 목표의 진행 상황도 업데이트됩니다.
* 목표에 대해 수행하는 특정 작업도 해당 상태를 업데이트합니다. 목표 상태를 업데이트하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)
   * [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md)
   * [Adobe Workfront 목표에서 목표 삭제 및 비활성화](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Adobe Workfront 목표의 목표 닫기 및 다시 열기](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront 목표의 목표 상태 개요

Workfront 목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오.

목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md)를 참조하십시오.

목표는 Workfront 목표에서 다음 상태 중 하나를 가질 수 있습니다.

* [초안](#draft)
* [활성](#active)
* [비활성](#inactive)
* [마감됨](#closed)

### 초안 {#draft}

* 새로 생성된 목표의 기본 상태입니다. 목표 만들기에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)를 참조하십시오.
* Workfront 목표는 초안 목표에 대한 진행률을 기록하지 않습니다.
* 초안 목표의 진행 상황을 업데이트할 수 없습니다.
* 진행 정보가 부족하기 때문에 초안 목표를 닫거나 비활성화할 수 없습니다.
* 초안 목표는 다른 목표의 진행 상황 계산에 기여하지 않으며 그래프에서 고려하지 않습니다.
* 초안 목표는 다음 Workfront 목표 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)


>[!IMPORTANT]
>
>목표의 상태를 다른 상태로 변경하면 목표를 다시 초안 상태에 배치할 수 없습니다.

### 활성 {#active}

* 초안 목표를 결과 또는 활동과 연관시키거나 다른 목표를 정렬하는 경우에만 활성화 할 수 있습니다. 목표를 활성화하면 상태가 활성으로 변경됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md)를 참조하십시오.
* Workfront 목표 는 활성 목표에 대한 진행 상황을 기록합니다.
* 활성 목표는 다른 목표의 진행률 계산에 기여하며, 그래프에서 고려됩니다.
* 활성 목표는 Workfront 목표의 다음 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션
   * 활성 목표의 진행 상태가 그래프로 표시됩니다

* 마감됨 또는 비활성 목표를 다시 활성화할 수 있습니다.

### 비활성 {#inactive}

* 소유자가 활성 목표에 대한 작업을 일시적 또는 영구적으로 중단하면 비활성화할 수 있습니다. 기록 정보를 위해 보관할 수 있습니다. 목표의 상태가 비활성으로 업데이트됩니다.

  목표 비활성화에 대한 자세한 내용은 문서 [Adobe Workfront 목표에서 목표 삭제 및 비활성화](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)의 &quot;목표 비활성화&quot; 섹션을 참조하십시오.

* 초안 목표나 마감된 목표는 비활성화할 수 없습니다.
* 비활성 목표를 다시 활성화하고 계속 작업할 수 있습니다.
* Workfront 목표는 비활성 목표에 대한 진행률을 계산하지 않습니다.
* 비활성 목표의 진행 상황을 업데이트할 수 없습니다.
* 비활성 목표는 다른 목표의 진행률 계산에 기여하지 않으며 그래프에서 고려하지 않습니다.
* 비활성 목표는 초안 목표와 달리 한 번 활성화되었기 때문에 진행 기록이 있습니다.
* 비활성 목표는 Workfront 목표의 다음 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)

### 마감됨 {#closed}

* 목표를 달성했거나 더 이상 이 목표를 작업하고 있지 않으며 앞으로도 목표를 마감할 것임을 표시하려는 경우 목표를 마감할 수 있습니다. 목표 종료에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 종료 및 다시 열기](../../workfront-goals/goal-management/close-and-reopen-goals.md)를 참조하십시오.

  >[!TIP]
  >
  >아직 달성하지 못한 목표에 대해 나중에 작업할 계획이라면 상태를 [종료됨] 대신 [비활성]으로 변경하는 것이 좋습니다.

* 초안 목표와 같이 활성화되지 않은 목표는 닫을 수 없습니다.
* 마감된 목표를 다시 열고 작업을 계속할 수 있습니다.
* Workfront 목표가 종료된 목표에 대한 진행률 기록을 중단합니다.
* 마감된 목표의 진행률은 업데이트할 수 없습니다.
* 마감된 목표는 Workfront 목표의 다음 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)
   * 종료된 목표의 정보도 그래프 섹션에서 고려됩니다.
