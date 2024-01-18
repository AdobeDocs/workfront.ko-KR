---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트, 작업 및 문제의 예상 완료 일자 개요
description: 예상 완료 일자는 프로젝트, 작업 또는 문제가 완료되는 시기를 실시간으로 나타내는 계산된 지표입니다. 프로젝트, 작업 또는 문제가 완료됨으로 표시되면 예상 완료 일자가 실제 완료 일자의 일자로 변경됩니다.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bac9856f3d0946b17e36797262d1a21f093ceadd
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 프로젝트, 작업 및 문제의 예상 완료 일자 개요

예상 완료 일자는 프로젝트, 작업 또는 문제가 완료되는 시기를 실시간으로 나타내는 계산된 지표입니다. 프로젝트, 작업 또는 문제가 완료됨으로 표시되면 예상 완료 일자가 실제 완료 일자의 일자로 변경됩니다.

다음 섹션에서는 프로젝트, 작업 및 문제에 대해 예상 완료 일자가 결정되는 방법과 이를 찾는 방법에 대해 설명합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>신규: 
   <ul><li><p>기여자 이상: 보고서에서 예상 완료 일자 보기</p></li> <li><p>보고서를 만들 수 있는 표준 라이선스</p></li> </ul>

<p>현재: 
   <ul><li><p>보고서에서 예상 완료 일자를 보려면 이상 검토</p></li> 
   <li><p>보고서 작성을 위한 플랜 라이선스</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>보고서를 만들려면 보고서, 대시보드, 캘린더에 대해 편집 액세스 권한이 있어야 합니다.</p> <p>보고서를 만들거나 목록 보기를 수정하려면 필터, 보기, 그룹화에 대한 편집 액세스 권한이 있어야 합니다</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Adobe Workfront에서 예상 완료 일자를 결정하는 방법

예상 완료 일자 는 계산된 필드이며 수동으로 변경할 수 없습니다.

예상 완료 일자를 결정하는 데 사용되는 기준은 보고 있는 객체에 따라 다릅니다.

* **프로젝트:** 프로젝트의 예상 완료 일자는 프로젝트에 대한 최신 작업의 예상 완료 일자와 동일합니다.

  예를 들어 완료율이 높을수록 작업의 예상 완료 일자가 현재 일자에 가깝게 이동합니다. 작업의 상태가 신규(New)이고 작업 계획 완료 일자(Planned Completion Date)가 가깝거나 지난 경우 예상 완료 일자가 미래로 이동합니다.

* **작업:** 작업에 대한 예상 완료 일자는 다음 기준에 따라 결정됩니다.

   * **작업 할당자가 작업에 대해 수행한 진행 상황 업데이트:** 진행률 업데이트에는 완료율 변경 및 작업 상태 변경 사항이 포함됩니다.
   * **커밋 일자:** 작업 할당자가 커밋 일자를 지정하는 경우 예상 완료 일자가 커밋 일자와 일치하도록 변경됩니다.

     커밋 일자에 대한 자세한 내용은 문서 를 참조하십시오 [커밋 일자 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **전임 작업:** 전임 작업에 지연이 없는 경우 예상 완료 일자는 계획된 완료 일자와 일치해야 합니다. 지연이 발생함에 따라 종속 작업에는 계획된 완료 일자보다 큰 예상 완료 일자가 표시됩니다.

     작업의 계획된 완료 일자에 대한 자세한 내용은 [작업 계획 완료 일자 개요](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >작업의 전임 작업에 실제 완료 일자가 있는 경우 종속 작업은 다음 시나리오에 설명된 대로 예상 완료 일자를 받습니다.
  >
  >
  >프로젝트에 태스크 A, 태스크 B 및 태스크 C가 있고 태스크 B가 태스크 A의 승계자이고 태스크 C가 태스크 B의 승계자이며, 실제 완료 일자가 태스크 A에 추가된 경우, 태스크 B에 대한 예상 완료 일자가 자동으로 재계산됩니다(단, **업데이트 유형** / 프로젝트가 자동 및 변경 시 로 설정되지만 작업 C에 대해서는 다시 계산되지 않습니다. 현재 Workfront은 성능상의 이유로 업데이트된 작업에서 한 수준 위 또는 아래 방향으로 작업의 예상 완료 일자를 계산합니다. 

* **문제:** 문제 예상 완료 일자는 처음에 문제 계획 완료 일자와 일치하도록 설정됩니다.

  문제 피할당자가 커밋 일자를 지정하면 예상 완료 일자와 계획된 완료 일자가 모두 커밋 일자와 일치하도록 변경됩니다.

  커밋 일자에 대한 자세한 내용은 문서 를 참조하십시오 [커밋 일자 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 예상 완료 일자 보기

보고서에서 프로젝트, 작업 및 문제의 예상 완료 일자를 볼 수 있습니다. Workfront의 다른 영역에서 프로젝트 및 작업의 예상 완료 일자를 볼 수 있습니다.

### 프로젝트의 예상 완료 일자 보기 {#view-the-projected-completion-date-of-a-project}

1. 예상 완료 일자를 조회할 프로젝트로 이동합니다.
1. 클릭 **프로젝트 세부 정보** 왼쪽 패널에서
1. 를 찾습니다. **예상 완료 일자** 의 필드 **개요** > **프로젝트 일자** 섹션.

### 작업의 예상 완료 일자 보기 {#view-the-projected-completion-date-of-a-task}

1. 예상 완료 일자를 조회할 태스크로 이동합니다.
1. 클릭 **작업 세부 정보** 왼쪽 패널에서
1. 를 찾습니다. **예상 완료 일자** 의 필드 **개요** > **작업 일자 및 제한** 섹션.

### 문제의 예상 완료 일자 보기 {#view-the-projected-completion-date-of-an-issue}

문제 보고서 또는 목록 보기에서 문제에 대한 예상 완료 일자를 볼 수 있습니다. 목록 보기를 만드는 것은 보고서에서 보기를 만드는 것과 비슷합니다.

예상 완료 일자가 포함된 문제 보고서를 생성하려면

1. 문서에 설명된 대로 문제 보고서 만들기 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 다음 항목 선택 **열(보기)** 탭.
1. 클릭 **열 추가**&#x200B;을(를) 입력한 후 시작 **예상 완료 일자** 다음에서 **이 열에 표시:** 필드.

1. 목록에 표시될 때 아래 **문제** 개체. 
1. **저장 및 닫기**&#x200B;를 클릭합니다.

   다음 **예상 완료 일자** 보고서의 열이 채워집니다. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
