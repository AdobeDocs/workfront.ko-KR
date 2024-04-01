---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업에 대한 완료율 보기 및 업데이트
description: 작업의 완료율을 업데이트하여 해당 작업의 완료 진행 상황을 나타낼 수 있습니다.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 작업에 대한 완료율 보기 및 업데이트

<!--Audited:01/2024-->

작업의 완료율을 업데이트하여 해당 작업의 완료 진행 상황을 나타낼 수 있습니다.

## 액세스 요구 사항

작업을 수동으로 업데이트하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새 라이선스: Standard</p> 
   또는
   <p>현재 라이선스: 작업 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 작업의 완료율을 업데이트할 수 있는 영역

다음 영역 중 하나에서 작업에 대한 완료율을 갱신할 수 있습니다.

* **작업 목록에서**: 완료율 열이 표시되면 작업의 완료율을 업데이트할 수 있습니다.\
  인라인 편집에 대한 자세한 내용은 [Adobe Workfront 목록의 항목 인라인 편집](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **마일스톤 보기에서**: 프로젝트 목록 또는 프로젝트 보고서에서 마일스톤 보기를 사용할 때 작업의 완료율을 업데이트할 수 있습니다. 자세한 내용은 [마일스톤 보기 사용](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **작업 헤더**: 작업 헤더에서 작업의 완료율을 업데이트할 수 있습니다. 자세한 내용은 [작업 편집](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **작업의 요약 패널에서**: 다음 영역에서 작업을 볼 때 요약 패널의 맨 위에 있는 작업의 완료율을 업데이트할 수 있습니다.

   * 작업 목록 또는 보고서
   * 타임시트
   * 워크로드 밸런서

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  자세한 내용은 [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)


## 작업 완료율 업데이트에 대한 고려 사항

* 작업을 100% 완료로 표시하면 작업 상태가 완료로 업데이트됩니다.
* 상위 작업에 대해 다음과 같은 시나리오가 있습니다.
   * 프로젝트의 요약 완료 모드가 자동으로 설정되어 있고 하위 작업이 완료되지 않은 경우 상위 작업의 완료율을 100%로 업데이트할 수 없습니다.
   * 프로젝트의 요약 완료 모드가 수동으로 설정되고 하위 작업이 완료되거나 완료되지 않은 경우 상위 작업의 완료율을 100%로 업데이트할 수 있습니다.

  자세한 내용은 [프로젝트 편집](../manage-projects/edit-projects.md).

## 작업 완료율 업데이트

1. Workfront에서 다음 영역 중 하나로 이동합니다.

   * 작업 목록
   * 프로젝트 목록 및 마일스톤 보기 적용
   * 작업 페이지 액세스를 통한 작업
1. 를 찾습니다. **완료율** 완료율을 업데이트하려는 작업의 필드입니다.
1. 완료율 필드 안쪽을 클릭하고 0에서 100 사이의 숫자를 입력합니다.

   또는

   을(를) 클릭하고 드래그 **완료율** 가능한 경우 작업을 얼마나 완료했는지 나타내는 데 필요한 숫자를 입력합니다.

   >[!NOTE]
   >
   >작업의 100%가 완료되었다고 표시하면 작업의 상태도 완료로 업데이트됩니다.


1. 키보드에서 Enter 키를 눌러 완료율을 저장합니다.

프로젝트의 완료율도 자동으로 업데이트됩니다.

