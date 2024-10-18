---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업에 대한 완료율 보기 및 업데이트
description: 작업의 완료율을 업데이트하여 해당 작업의 완료 진행 상황을 나타낼 수 있습니다.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: e68972f7334a93f7fbd3db29919a2f2746ce64fe
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 작업에 대한 완료율 보기 및 업데이트

<!--Audited:01/2024-->

작업의 완료율을 업데이트하여 해당 작업의 완료 진행 상황을 나타낼 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업의 완료율을 업데이트할 수 있는 영역

다음 영역 중 하나에서 작업에 대한 완료율을 갱신할 수 있습니다.

* **작업 목록에서**: 완료율 열이 표시되면 작업의 완료율을 업데이트할 수 있습니다.\
  인라인 편집에 대한 자세한 내용은 [Adobe Workfront의 목록에서 인라인 편집 항목](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)을 참조하십시오.

* **마일스톤 보기에서**: 프로젝트 목록 또는 프로젝트 보고서에서 마일스톤 보기를 사용할 때 작업의 완료율을 업데이트할 수 있습니다. 자세한 내용은 [마일스톤 보기 사용](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)을 참조하세요.

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **작업 헤더에서**: 작업 헤더에서 작업의 완료율을 업데이트할 수 있습니다. 자세한 내용은 [작업 편집](../../tasks/manage-tasks/edit-tasks.md)을 참조하세요.

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **작업의 요약 패널에서**: 다음 영역에서 작업을 볼 때 요약 패널의 맨 위에 있는 작업의 완료율을 업데이트할 수 있습니다.

   * 작업 목록 또는 보고서
   * 타임시트
   * 워크로드 밸런서

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  자세한 내용은 [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)를 참조하세요.

* **홈**: 홈 영역의 요약 패널 또는 내 작업 위젯에서 작업 또는 문제의 완료율을 업데이트할 수 있습니다.

자세한 내용은 [새 홈 시작](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)을 참조하세요.

## 작업 완료율 업데이트에 대한 고려 사항

* 작업을 100% 완료로 표시하면 작업 상태가 완료로 업데이트됩니다.
* 상위 작업에 대해 다음과 같은 시나리오가 있습니다.
   * 프로젝트의 요약 완료 모드가 자동으로 설정되어 있고 하위 작업이 완료되지 않은 경우 상위 작업의 완료율을 100%로 업데이트할 수 없습니다.
   * 프로젝트의 요약 완료 모드가 수동으로 설정되고 하위 작업이 완료되거나 완료되지 않은 경우 상위 작업의 완료율을 100%로 업데이트할 수 있습니다.

  자세한 내용은 [프로젝트 편집](../manage-projects/edit-projects.md)을 참조하세요.

## 작업 완료율 업데이트

1. Workfront에서 다음 영역 중 하나로 이동합니다.

   * 작업 목록
   * 프로젝트 목록 및 마일스톤 보기 적용
   * 작업 페이지 액세스를 통한 작업
1. 완료율을 업데이트하려는 작업의 **완료율** 필드를 찾습니다.

   >[!TIP]
   >
   >  완료율 필드는 항상 요약 패널의 맨 위에 표시됩니다.


1. **완료율** 필드 내부를 클릭하고 0에서 100 사이의 숫자를 입력하십시오

   또는

   **완료율** 표시줄을 클릭하고 필요한 숫자로 드래그하여 사용 가능한 경우 완료한 작업의 양을 나타냅니다.

   >[!NOTE]
   >
   >작업의 100%가 완료되었다고 표시하면 작업의 상태도 완료로 업데이트됩니다.


1. 키보드에서 Enter 키를 눌러 완료율을 저장합니다.

프로젝트의 완료율도 자동으로 업데이트됩니다.

