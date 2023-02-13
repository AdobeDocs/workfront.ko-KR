---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront 목표의 목표 상태 개요
description: 목표 상태는 목표가 활성 상태이고 현재 진행 상태를 기록하는지 또는 비활성 상태인지, 초안 상태인지 또는 이미 달성되었는지 여부를 나타냅니다.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Adobe Workfront 목표의 목표 상태 개요

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>이 문서에 설명된 기능을 사용하려면 조직에 다음 내용이 있어야 합니다.
>
>* Pro 이상 [Adobe Workfront 플랜](https://www.workfront.com/plans).
>* Workfront 라이선스 외에 Adobe Workfront 목표 라이선스.
>
>Workfront 목표 라이센스에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오.

Workfront 목표 액세스에 대한 자세한 내용은 [Workfront 목표 사용 요구 사항](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


목표 상태는 목표가 활성 상태이고 현재 진행 상태를 기록하는지 또는 비활성 상태인지, 초안 상태인지 또는 이미 달성되었는지 여부를 나타냅니다.

## Workfront 목표에서 목표 상태를 업데이트할 때 고려 사항

* 생성했거나 사용자와 공유된 목표의 상태는 수동으로 업데이트할 수 없습니다. 목표에 대해 수행하는 작업에 따라 목표 상태가 업데이트됩니다. 예를 들어, 목표를 활성화하면 초안 상태가 활성으로 변경됩니다.
* 일부 제한 사항이 있으며, 다음 규칙에 따라 목표 상태를 다른 상태로 변경할 수 없는 경우가 있습니다.

   | 시작/종료 | 초안 | 활성 | 비활성 | 마감됨 |
   |---|---|---|---|---|
   | 초안 | - | 예 | 아니요 | 아니요 |
   | 활성 | 아니요 | - | 예 | 예 |
   | 비활성 | 아니요 | 예 | - | 아니요 |
   | 마감됨 | 아니요 | 예 | 아니요 | - |

* 폐쇄된 목표를 열면 목표의 진행 속도도 업데이트됩니다.
* 목표에 대해 수행하는 특정 작업도 해당 상태를 업데이트합니다. 목표 상태를 업데이트하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md)
   * [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md)
   * [Adobe Workfront 목표에서 목표 삭제 및 비활성화](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Adobe Workfront 목표에 목표를 닫고 다시 엽니다.](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront 목표의 목표 상태 개요

Workfront 목표 만들기에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).

목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).

목표는 Workfront 목표에 다음 상태 중 하나를 가질 수 있습니다.

* [초안](#draft)
* [활성](#active)
* [비활성](#inactive)
* [마감됨](#closed)

### 초안 {#draft}

* 새로 만든 목표에 대한 기본 상태입니다. 목표 만들기에 대한 내용은 [Adobe Workfront 목표에서 목표 만들기](../../workfront-goals/goal-management/create-goals.md).
* Workfront 목표는 초안 목표에 대한 진행 상황을 기록하지 않습니다.
* 초안 목표 진행 상태는 업데이트할 수 없습니다.
* 진행 정보가 없으므로 초안 목표를 닫거나 비활성화할 수 없습니다.
* 초안 목표는 다른 목표의 진행 계산에 기여하지 않으며 그래프에서 고려하지 않습니다.
* 다음과 같은 Workfront 목표 영역에 포함된 초안 목표가 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)


>[!IMPORTANT]
>
>목표의 상태를 다른 상태로 변경하면 목표를 다시 초안 상태로 배치할 수 없습니다.

### 활성 {#active}

* 초안 목표를 결과, 활동 또는 목표에 연결하는 경우에만 활성화하거나 다른 목표를 맞출 수 있습니다. 목표를 활성화하면 상태가 활성으로 변경됩니다. 목표 활성화에 대한 자세한 내용은 [Adobe Workfront 목표에서 목표 활성화](../../workfront-goals/goal-management/activate-goals.md).
* Workfront 목표는 활성 목표에 대한 진행 상황을 기록합니다.
* 활성 목표는 다른 목표의 진행 계산에 기여하며 그래프에서 고려됩니다.
* 활성 목표는 다음 Workfront 목표 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션
   * 활성 목표의 진행 상태가 그래프로 표시됩니다

* 폐쇄됨 또는 비활성 목표를 다시 활성화할 수 있습니다.

### 비활성 {#inactive}

* 소유자가 일시적으로 또는 영구적으로 작업을 중지한 경우 활성 목표를 비활성화할 수 있습니다. 역사적 정보를 위해 보관하시면 됩니다 목표 상태를 비활성으로 업데이트합니다.

   목표 비활성화에 대한 자세한 내용은 문서의 &quot;목표 비활성화&quot; 섹션을 참조하십시오 [Adobe Workfront 목표에서 목표 삭제 및 비활성화](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* 초안 또는 닫힌 목표는 비활성화할 수 없습니다.
* 비활성 목표를 다시 활성화하고 계속 작업할 수 있습니다.
* Workfront 목표는 비활성 목표에 대한 진행 상태를 계산하지 않습니다.
* 비활성 목표의 진행 상태는 업데이트할 수 없습니다.
* 비활성 목표는 다른 목표의 진행 계산에 기여하지 않으며 그래프에서 고려하지 않습니다.
* 비활성 목표는 초안 목표와 달리 한때 활성 상태였기 때문에 진행 기록이 있습니다.
* 비활성 목표는 다음 Workfront 목표 영역에 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)

### 마감됨 {#closed}

* 목표를 달성했는지 또는 더 이상 작업을 하지 않았는지 또는 향후에 목표에 도달했는지를 나타내고자 할 때 목표를 닫을 수 있습니다. 목표 종료에 대한 자세한 내용은 [Adobe Workfront 목표에 목표를 닫고 다시 엽니다.](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >아직 달성되지 않은 목표에 대해 나중에 작업할 계획이라면, 상태를 마감됨 대신 비활성 상태로 변경하는 것이 좋습니다.

* 초안 목표와 같이 활성화되지 않은 목표를 닫을 수 없습니다.
* 닫힌 목표를 다시 열고 작업을 계속할 수 있습니다.
* Workfront 목표는 닫힌 목표에 대한 진행 상황을 기록하는 것을 중지합니다.
* 닫힌 목표의 진행 상태는 업데이트할 수 없습니다.
* 다음 Workfront 목표 영역에 닫힌 목표가 표시됩니다.

   * 목표 목록
   * 목표 정렬 섹션(정렬된 목표로만)
   * 닫힌 목표에 대한 정보도 그래프 섹션에 고려합니다.
