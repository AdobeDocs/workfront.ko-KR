---
product-area: projects
navigation-topic: manage-tasks
title: 목록의 작업 편집
description: 목록에 표시된 필드를 편집하여 작업 목록에서 작업 정보를 편집할 수 있습니다. 작업을 편집하는 다른 방법에 대한 자세한 내용은 작업 편집을 참조하십시오.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# 목록의 작업 편집 {#edit-tasks-in-a-list}

목록에 표시된 필드를 편집하여 작업 목록에서 작업 정보를 편집할 수 있습니다. 작업을 편집하는 다른 방법에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 부여 또는 더 높은 권한 부여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 목록에서 작업 편집에 대한 고려 사항 {#considerations-about-editing-tasks-in-a-list}

목록에서 작업을 편집하는 것은 변경 사항이 프로젝트 타임라인에 미치는 영향에 대한 명확한 보기를 통해 동시에 여러 작업을 변경하는 빠른 방법입니다.

목록에서 작업을 편집할 때는 다음 사항을 고려하십시오.

* 편집 상자에서 작업을 편집할 때 작업에 대한 관리 권한이 필요한 것과 달리, 작업에 Contribute 권한만 있는 목록에서 작업을 편집할 수 있습니다. 이렇게 하면 작업에 대해 다음과 같은 제한된 정보를 편집할 수 있습니다.

   * 설명
   * 상태
   * 완료율
   * 사용자 지정 양식 정보

      >[!NOTE]
      >
      >필드를 업데이트할 권한이 있는 경우에만 목록에서 작업 사용자 지정 필드를 편집할 수 있습니다.

   * 로그 시간
   * 지정 수정
   * 재무 정보 보기
   * 비용, 작업 또는 문제 추가

* 다음 목록에서 작업을 편집할 수 있습니다.

   * 프로젝트의 작업 섹션
   * 프로젝트의 하위 작업 섹션
   * 작업 보고서

      >[!NOTE]
      >
      >기본적으로 Workfront에서는 하위 작업 섹션이나 작업 보고서에 변경 사항을 자동으로 작업에 저장합니다.

* Workfront에서 목록의 작업에 대한 변경 사항을 저장할 시기를 제어할 수 있습니다. 변경 사항을 자동으로 저장하거나 수동으로 저장할 수 있습니다.

   Workfront에서 목록의 작업에 대한 변경 사항을 저장할 때 구성에 대한 자세한 내용은 [목록에서 작업을 편집할 때 저장 옵션을 선택합니다](#select-a-save-option-when-editing-tasks-in-a-list) 섹션에 자세히 설명되어 있습니다.

## 목록에서 작업을 편집할 때 저장 옵션을 선택합니다 {#select-a-save-option-when-editing-tasks-in-a-list}

목록의 작업에 대한 변경 사항이 자동으로 저장되거나, 변경 내용이 발생할 때 또는 각 변경 사항을 수동으로 저장할지 결정할 수 있습니다.

>[!IMPORTANT]
>
>작업을 자동으로 저장하는지 수동으로 저장하는지에 따라 목록에서 작업을 편집하는 동안 다른 사람의 정보를 덮어쓸 수 있습니다. 다른 사용자와 동시에 수행하는 작업에 대한 변경 사항을 Workfront에서 저장하는 방법에 대한 자세한 내용은 [작업 목록 내의 동시 변경 사항 저장 개요](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

업데이트 유형으로 자동 또는 자동 및 변경 시(On Change)가 선택된 프로젝트의 목록에 변경 사항을 저장하면 Workfront은 모든 인프로젝트 및 교차 프로젝트 종속성과 함께 프로젝트 타임라인을 업데이트합니다. 프로젝트가 크거나 종속성이 많은 경우 타임라인 계산에 시간이 오래 걸릴 수 있습니다. 작업 목록을 편집하는 일부 방법은 변경 내용을 저장하기 위해 선택한 방법에 따라 다른 방법보다 빠를 수 있습니다.

Workfront에서 목록의 작업에 대한 변경 사항을 저장할 시기를 제어할 수 있습니다. 다음 시나리오가 있습니다. 

* 각 업데이트 후에 Workfront에서 변경 사항을 자동으로 저장하도록 할 수 있습니다.

   자세한 내용은 섹션을 참조하십시오 [목록에서 작업 편집 및 변경 내용 자동 저장](#edit-tasks-in-a-list-and-automatically-save-changes) 참조하십시오.

* 저장 단추를 수동으로 사용하여 한 번에 여러 변경 사항을 적용할 때 제어할 수 있습니다.

   자세한 내용은 섹션을 참조하십시오 [목록에서 작업을 편집하고 변경 내용을 수동으로 저장](#edit-tasks-in-a-list-and-manually-save-changes) 참조하십시오.

### 목록에서 작업 편집 및 변경 내용 자동 저장 {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>프로젝트에 2000개 이상의 작업이 있거나 종속성이 많은 경우 변경 사항 및 모든 프로젝트 종속성이 느려질 수 있습니다.

작업 목록 변경 사항을 자동으로 저장할 때 다음 사항을 고려하십시오.

* 사용자 정의 뷰를 작업 목록에 적용하고 업데이트할 액세스 권한이 있는 모든 작업 관련 필드를 편집할 수 있습니다.
* 자동 저장된 변경 사항은 되돌릴 수 없습니다. 기본 설정입니다.
* Workfront은 프로젝트 업데이트 유형이 자동 또는 자동 및 변경일 때 변경 때마다 프로젝트의 타임라인과 모든 프로젝트 내 및 프로젝트 간 종속성을 자동으로 다시 계산합니다. 프로젝트 업데이트 유형에 대한 자세한 내용은 [프로젝트 업데이트 유형을 선택합니다](../../../manage-work/projects/manage-projects/select-project-update-type.md).

목록에서 작업을 편집하고 변경 내용을 자동으로 저장하려면 다음을 수행합니다.

1. 프로젝트로 이동한 다음 **작업** 섹션을 참조하십시오.
1. 을(를) 클릭합니다. **계획 모드 메뉴** ![](assets/qs-list-mode-or-save-mode-icon-small.png) 목록의 맨 위에서 **자동 저장** 옵션이 선택되어 있습니다.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 수동으로 업데이트할 수 있는 권한이 있는 필드를 편집합니다.

   ![](assets/inline-editing-a-task-350x26.png)

1. (선택 사항) 누르기 **Esc** 변경 사항을 취소하려면
1. 작업 및 프로젝트 타임라인에 변경 내용을 저장하려면 Enter 키를 누릅니다.
1. (선택 사항) 수정할 작업을 마우스 오른쪽 단추로 클릭합니다.

   또는

   을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon-task-list.png) 작업 이름의 오른쪽에 있습니다.

1. (선택 사항) 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>새 탭에서 열기</strong></td> 
      <td>새 브라우저 탭에서 작업을 엽니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>편집</strong></td> 
      <td><p>를 엽니다. <strong>작업 편집</strong> 상자를 엽니다. 여기에서 작업을 편집할 수 있습니다.</p><p>작업 편집에 대한 자세한 내용은 <a href="#edit-tasks-in-a-list" class="MCXref xref">목록의 작업 편집</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">삭제</td> 
      <td><p>작업을 삭제합니다.</p><p>작업 삭제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">작업 삭제</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">한 수준 내리기</td> 
      <td><p>작업을 한 수준별로 들여씁니다. </p><p>이 옵션은 독립 실행형 작업에만 표시됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">수준 올리기</td> 
      <td><p>한 단계별로 작업을 내던집니다. </p><p>이 옵션은 하위 작업에만 표시됩니다. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">위에 작업 삽입</td> 
      <td>선택한 작업 위에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래에 작업 삽입</td> 
      <td>선택한 작업 아래에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">복제</td> 
      <td><p>동일한 프로젝트 내에 작업의 중복 버전을 만듭니다. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">복사 위치:</td> 
      <td><p>작업을 다른 프로젝트에 복사합니다.</p><p>작업 복사 및 복제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">작업 복사 및 복제</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">이동 위치:</td> 
      <td><p>작업을 다른 프로젝트로 이동합니다.</p><p>작업 이동에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">작업 이동</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   변경 사항은 자동으로 저장되며 되돌릴 수 없습니다.

### 목록에서 작업을 편집하고 변경 내용을 수동으로 저장 {#edit-tasks-in-a-list-and-manually-save-changes}

목록에 있는 작업에 대한 변경 사항을 수동으로 저장할 수 있습니다. 이러한 방식으로 변경 사항을 저장하면 저장하기 전에 변경 사항을 취소할 수 있습니다.

>[!TIP]
>
>* 하위 작업 섹션이나 작업 보고서에서 작업을 편집할 때는 목록에 있는 작업에 변경한 내용을 되돌릴 수 없습니다.
>* 되돌릴 수 있는 변경 사항의 수에는 제한이 없습니다. 작업의 원래 상태에 도달할 때까지 하나씩 모두 되돌릴 수 있습니다.
>


작업 목록에 변경 사항을 수동으로 저장할 때는 다음 사항을 고려하십시오.

* 작업 목록 변경 사항을 수동으로 저장하려면 작업과 프로젝트를 모두 관리할 권한이 필요합니다.
* 프로젝트를 편집할 수 없습니다. 프로젝트를 편집하는 옵션이 비활성화됩니다.
* 프로젝트 헤더에 있는 정보는 업데이트할 수 없습니다. 작업 목록에서 변경 사항을 수동으로 저장할 때만 다음 작업을 수행할 수 있습니다.

   * 프로젝트에 가입합니다.
   * 프로젝트를 즐겨찾기 목록에 추가합니다.
   * 목록에서 해당 이름을 클릭하여 작업을 엽니다.

* 작업을 일괄적으로 편집합니다. 여러 작업을 선택하면 편집 아이콘이 비활성화됩니다.
* Workfront은 변경 사항을 저장한 후에만 작업에 대한 변경 사항에 대한 알림을 트리거합니다.

목록에 있는 작업에 대한 변경 사항을 수동으로 저장하는 방법에는 두 가지가 있습니다. 이러한 두 가지 방법은 아래에 설명되어 있습니다.

* [수동 Save Standard 옵션을 선택하면 작업 목록에 변경 내용을 수동으로 저장합니다.](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [수동 타임라인 계획 저장 옵션을 선택하면 작업 목록에 변경 내용을 수동으로 저장합니다](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 수동 Save Standard 옵션을 선택하면 작업 목록에 변경 내용을 수동으로 저장합니다. {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>프로젝트에 2000개 이상의 작업이 있거나 종속성이 많은 경우 작업에 대해 수행한 변경 사항과 이러한 변경 사항이 모든 프로젝트 종속성에 미치는 영향을 시각적으로 식별하는 데 시간이 걸릴 수 있습니다. 이 경우 프로젝트에 2,000개 이상의 작업이 있거나 종속성이 많은 경우 변경 사항을 저장하는 데 시간이 더 걸릴 수 있습니다.

Manual save Standard 옵션을 선택한 후 목록에서 작업을 업데이트할 때는 다음 사항을 고려하십시오.

* 작업 목록에 사용자 지정 보기를 적용하고 해당 보기에서 관리할 권한이 있는 작업 관련 필드를 편집할 수 있습니다.
* Workfront은 프로젝트 업데이트 유형이 자동 또는 자동 및 변경일 때 저장 을 클릭하면 프로젝트의 타임라인과 모든 프로젝트 내 및 프로젝트 간 종속성을 계산합니다. 프로젝트 업데이트 유형에 대한 자세한 내용은 [프로젝트 업데이트 유형을 선택합니다](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Manual save Standard 옵션을 선택할 때 목록에서 작업을 편집하려면 다음과 같이 하십시오.

1. 프로젝트로 이동한 다음 **작업** 섹션에 자세히 설명되어 있습니다.
1. 을(를) 클릭합니다. **계획 모드** 메뉴 ![](assets/qs-list-mode-or-save-mode-icon-small.png) 목록의 맨 위에서 을(를) 선택하고 을(를) 선택합니다. **수동 저장**&#x200B;를 클릭한 다음 **표준** > **적용**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   도구 모음 설정이 변경 사항을 실행 취소, 다시 실행 및 저장하는 옵션과 함께 표시됩니다.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 수동으로 업데이트할 권한이 있는 필드 안을 클릭합니다. 필드를 편집할 수 있게 되고 사용자가 변경할 수 있습니다.

   ![](assets/inline-editing-a-task-350x26.png)

1. 변경 사항을 일시적으로 저장하려면 Enter 키를 누릅니다.
1. (선택 사항) **실행 취소 아이콘** ![](assets/undo-icon-on-task-list.png) 변경 사항을 취소하고 필드를 원래 상태로 되돌리기 위해
1. (선택 사항 및 조건부) **다시 실행 아이콘** ![](assets/redo-icon-on-task-list.png) 변경 사항을 복원하려면 되돌릴 수 없습니다.

1. (선택 사항) 수정할 작업을 마우스 오른쪽 단추로 클릭합니다.

   또는

   을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon-task-list.png).

1. (선택 사항) 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>새 탭에서 열기</strong> </td> 
      <td>새 브라우저 탭에서 작업을 엽니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">삭제</td> 
      <td>작업 삭제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">작업 삭제</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">한 수준 내리기</td> 
      <td> <p>작업을 한 수준별로 들여씁니다. </p> <p>이 옵션은 독립 실행형 작업에만 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수준 올리기</td> 
      <td> <p>한 단계별로 작업을 내던집니다. </p> <p>이 옵션은 하위 작업에만 표시됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">위에 작업 삽입</td> 
      <td>선택한 작업 위에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래에 작업 삽입</td> 
      <td>선택한 작업 아래에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">복제</td> 
      <td> <p>동일한 프로젝트 내에 작업의 중복 버전을 만듭니다. </p> <p>작업 복사 및 복제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">작업 복사 및 복제</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront은 작업 타임라인을 변경할 때 모든 프로젝트 내 및 프로젝트 간 종속성을 업데이트합니다.
1. 클릭 **저장** 작업 변경 사항을 영구적으로 유지하고 프로젝트의 타임라인을 저장하려면 을 선택합니다.

#### 수동 타임라인 계획 저장 옵션을 선택하면 작업 목록에 변경 내용을 수동으로 저장합니다 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

변경 사항을 저장하고 모든 프로젝트 종속성이 더 빠릅니다. 이 기능은 2,000개 이상의 작업이 있는 프로젝트에서는 사용할 수 없습니다.

>[!IMPORTANT]
>
>종속성이 많은 작업이 수백 개 이상인 대규모 작업 목록을 편집할 때는 이 옵션을 사용하는 것이 좋습니다. 이 옵션을 사용하면 수동 저장 옵션을 사용하는 것보다 훨씬 빠르게 변경 사항을 시각적으로 식별할 수 있습니다.

작업 목록에서 수동 타임라인 계획 저장 옵션을 사용할 때는 다음 사항을 고려하십시오.

* 2000개 이상의 작업이 있는 프로젝트에 수동 타임라인 계획 저장 옵션을 적용할 수 없습니다.
* 사용자 지정 보기, 필터 또는 그룹을 작업 목록에 적용할 수 없습니다. 보기, 필터 및 그룹화 드롭다운 메뉴와 Agile 보기 아이콘이 비활성화됩니다. 기본적으로 적용되는 보기에는 제한된 수의 필드가 포함되어 있습니다.
* 프로젝트 업데이트 유형이 자동 또는 자동 및 변경일 때 각 변경 후 프로젝트의 타임라인과 모든 프로젝트 내 종속성이 자동으로 계산됩니다.
* 프로젝트 업데이트 유형이 자동 또는 자동 및 변경일 때 저장을 클릭하면 프로젝트 간 종속성이 계산됩니다. 프로젝트 업데이트 유형에 대한 자세한 내용은 [프로젝트 업데이트 유형을 선택합니다](../../../manage-work/projects/manage-projects/select-project-update-type.md).

수동 타임라인 계획 저장 옵션을 사용할 때 목록에서 작업을 편집하려면

1. 프로젝트로 이동한 다음 **작업** 섹션을 참조하십시오.
1. 을(를) 클릭합니다. **계획 모드** 메뉴 ![](assets/qs-list-mode-or-save-mode-icon-small.png) 목록의 맨 위에서 을(를) 선택하고 을(를) 선택합니다. **수동 저장**&#x200B;를 클릭한 다음 **타임라인 계획**> **적용**.

   이 옵션은 2,000개 이상의 작업이 있는 프로젝트의 경우 흐리게 표시됩니다.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >이 페이지에서 멀리 이동하면 Workfront이 자동 저장 옵션을 다시 활성화합니다.

   목록에서 다음 변경 사항을 확인합니다.

   * 보기, 그룹화 및 필터 드롭다운 메뉴가 제거되고 보기가 다음 필드로 바뀝니다.

      * 작업 번호
      * 작업 이름
      * 제한 유형
      * 기간
      * 계획된 시작 일자
      * 계획된 완료 일자
      * 전임 작업
      * 할당
      * 상태
      * 완료율
   * 애자일 보기 아이콘이 제거됩니다.
   * 도구 모음 설정이 변경 사항을 실행 취소, 다시 실행 및 저장하는 옵션과 함께 표시됩니다.

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. 수동으로 업데이트할 수 있는 권한이 있는 필드를 편집합니다.

   ![](assets/inline-editing-a-task-350x26.png)

1. 변경 사항을 일시적으로 저장하려면 Enter 키를 누릅니다.
1. (선택 사항) **실행 취소 아이콘** ![](assets/undo-icon-on-task-list.png) 변경 사항을 취소하고 필드를 원래 상태로 되돌리기 위해
1. (선택 사항 및 조건부) **다시 실행 아이콘** ![](assets/redo-icon-on-task-list.png) 되돌릴 수 없습니다.

1. (선택 사항) 수정할 작업을 마우스 오른쪽 단추로 클릭합니다

   또는

   을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon-task-list.png).

1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>새 탭에서 열기</strong> </td> 
      <td>새 브라우저 탭에서 작업을 엽니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">삭제</td> 
      <td>작업 삭제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">작업 삭제</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">한 수준 내리기</td> 
      <td> <p>작업을 한 수준별로 들여씁니다. </p> <p>이 옵션은 독립 실행형 작업에만 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">수준 올리기</td> 
      <td> <p>한 단계별로 작업을 내던집니다. </p> <p>이 옵션은 하위 작업에만 표시됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">위에 작업 삽입</td> 
      <td>선택한 작업 위에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">아래에 작업 삽입</td> 
      <td>선택한 작업 아래에 작업을 삽입합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">복제</td> 
      <td> <p>동일한 프로젝트 내에 작업의 중복 버전을 만듭니다. </p> <p>작업 복사 및 복제에 대한 자세한 내용은 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">작업 복사 및 복제</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront은 작업 타임라인을 변경할 때 모든 프로젝트 내 및 프로젝트 간 종속성을 업데이트합니다.
1. 클릭 **저장** 작업 변경 사항을 영구적으로 유지하고 프로젝트의 타임라인을 저장하려면 을 선택합니다.

## 요약을 사용하여 목록의 작업 편집

1. 편집할 작업이 포함된 프로젝트로 이동합니다.
1. 클릭&#x200B;**작업** 왼쪽 패널에 표시됩니다.

   프로젝트의 작업 목록이 표시됩니다.

1. 자세히 메뉴를 클릭합니다 ![](assets/more-icon-task-list.png) 작업 이름 다음에 을 클릭합니다. **요약 열기**. 편집할 작업을 선택한 다음 **요약 열기 아이콘** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) 목록의 오른쪽 상단에서.

   다음 **요약** 엽니다.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (선택 사항) **X 아이콘** 요약 오른쪽 상단에서 패널을 닫고 작업을 인라인으로 편집합니다.

   목록에서 작업을 편집하는 방법에 대한 단계를 따라 작업을 인라인 편집하십시오.

   목록에서 작업 편집에 대한 자세한 내용은 [목록에서 작업 편집에 대한 고려 사항](#considerations-about-editing-tasks-in-a-list) 참조하십시오.

1. (선택 사항)에서 작업에 대한 업데이트를 입력합니다. **업데이트** 영역.
1. 다음 아이콘 또는 영역을 클릭하여 작업으로 이동하고 작업 수준에서 정보를 편집합니다.

   | 문서 | 클릭 **추가하려면 여기를 클릭하십시오.** 을 눌러 작업에 문서를 추가합니다. |
   |---|---|
   | 세부 정보 | 을(를) 클릭하여 작업에 대한 정보를 업데이트합니다. |
   | 사용자 정의 양식 | 사용자 지정 Forms을 추가 또는 제거하거나 양식의 정보를 업데이트하려면 을(를) 클릭합니다. |
   | 시간 | 를 클릭하여 시간을 기록합니다. |
   | 승인 | 작업 승인을 추가하려면 을 클릭합니다. |

   {style=&quot;table-layout:auto&quot;}

1. 작업 업데이트를 마치면 브라우저에서 뒤로 단추를 클릭하여 작업 목록으로 돌아갑니다.

## 일괄 작업 편집

여러 작업을 한 번에 편집할 수 있습니다. 작업을 편집할 수 있도록 작업에 대한 관리 권한이 있는지 확인합니다.

1. 일괄적으로 편집할 작업이 포함된 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 다음을 확인합니다. **자동 저장** 옵션이 선택되어 있습니다.

   >[!IMPORTANT]
   >
   >작업을 수동으로 저장할 때는 작업을 일괄적으로 편집할 수 없습니다.

   목록의 작업에 변경 내용을 저장하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [목록에서 작업 편집에 대한 고려 사항](#considerations-about-editing-tasks-in-a-list) 참조하십시오.

1. 작업 목록에서 여러 작업을 선택합니다.
1. 을(를) 클릭합니다. **편집 아이콘** ![](assets/qs-edit-icon.png).

   다음 **작업 편집** 대화 상자가 열립니다.

1. 선택한 모든 작업에 대해 변경할 정보를 지정합니다.

   모든 작업에 대한 정보를 편집하는 것은 하나의 작업에 대한 정보를 편집하는 것과 동일합니다. 작업 기간을 편집하려면 선택한 작업에 동일한 작업 제약 조건이 있어야 합니다. 그렇지 않으면 **기간** 필드가 채워지지 않습니다.

   작업 편집에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >선택한 모든 작업에 대해 변경하는 정보는 을 제외하고 개별 작업에 대한 기존 정보를 덮어씁니다. **지정** 필드. 일괄 편집에서 새 담당자를 추가하면 해당 할당자가 선택한 모든 작업에 추가됩니다. 선택한 작업에 다른 할당자가 할당되면 일괄 편집을 통해 추가된 작업 외에 할당된 상태로 유지됩니다.

1. 클릭 **사용자 지정 Forms** 을 클릭하여 선택한 모든 작업에 첨부된 사용자 지정 양식을 편집합니다. 활성 사용자 지정 양식만 목록에 표시됩니다.

   선택한 작업에 일반적인 사용자 지정 양식이 없는 경우 이 섹션에는 양식이 표시되지 않습니다.

   선택한 모든 작업에 첨부된 양식의 필드만 편집할 수 있고 편집할 수 있는 권한이 있습니다.

1. (선택 사항) 사용자 지정 Forms 섹션에서 **사용자 지정 표현식 다시 계산** 선택한 작업에 첨부된 사용자 지정 양식에 있는 모든 계산된 사용자 지정 필드가 최신 상태인지 확인하는 옵션입니다.
1. 클릭 **변경 내용 저장**.

   이제 선택한 모든 작업에 모든 변경 사항이 표시됩니다.

사용자 지정 양식의 벌크 편집에 대한 자세한 내용은 [개체에 첨부된 사용자 지정 양식 관리](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
