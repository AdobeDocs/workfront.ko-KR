---
title: 우선 순위 만들기 및 사용자 지정
description: Workfront의 설정 영역에서 프로젝트, 작업 및 문제의 우선 순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제를 중요시합니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 2%

---

# 우선 순위 만들기 및 사용자 정의

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront의 설정 영역에서 프로젝트, 작업 및 문제의 우선 순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제를 중요시합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기존 우선 순위 맞춤화

Workfront 관리자는 Workfront에서 제공하는 기본 우선 순위를 다음과 같이 수정할 수 있습니다.

* 우선 순위 이름을 변경합니다.
* 우선 순위 재정렬.

  우선 순위를 다시 정렬하는 방법에 대한 자세한 내용은 [프로젝트, 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

* 기본 우선 순위를 변경합니다.

  기본 우선 순위를 변경하는 기능에 대한 자세한 내용은 [프로젝트, 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

* 우선 순위에 대한 설명을 편집합니다.
* 각 우선 순위에 대한 색상을 설정합니다.

  결과를 **우선 순위**(으)로 그룹화할 때 우선 순위 색상이 차트 보고서에 사용됩니다.

  차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오.

* 우선 순위를 삭제합니다.

  기존 우선순위를 삭제할 때는 대체 우선순위를 선택해야 합니다.

* 우선 순위를 숨깁니다.

  우선 순위를 숨기는 기능에 대한 자세한 내용은 [프로젝트, 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

  >[!NOTE]
  >
  >각 개체에 대해 Workfront 계정에 하나 이상의 우선 순위가 있어야 합니다.

각 객체 유형(프로젝트, 작업 및 문제)에 대해 기본적으로 제공되는 우선순위는 동일합니다.

* 없음
* 낮음
* 일반
* 높음
* 긴급

## 프로젝트, 작업 또는 문제에 대한 우선 순위 만들기 {#create-a-priority-for-a-project-task-or-issue}

Workfront에서 제공하는 기본 우선 순위 외에도 조직의 요구 사항을 반영하기 위해 고유한 우선 순위를 추가할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **우선 순위**&#x200B;를 클릭합니다.

1. 우선 순위를 만들려는 개체 유형의 탭을 클릭합니다(**프로젝트**, **작업** 또는 **문제**).
1. 표 맨 아래에 있는 **새 행**&#x200B;을 클릭합니다.
1. 우선 순위에 대해 다음 옵션을 구성합니다.

   * **우선 순위 이름**: 우선 순위 이름을 입력하십시오.
   * **중요도**: 새 우선 순위를 추가할 때 기본적으로 숫자가 할당됩니다. 이 번호가 사용자의 요구 사항과 일치하지 않는 경우 이 번호를 편집합니다.

     각 우선 순위의 중요 번호는 고유해야 합니다. 우선 순위 번호는 프로젝트, 작업 또는 문제의 중요성을 반영합니다. 가장 높은 번호는 가장 높은 우선 순위에 해당합니다.

     우선 순위를 저장한 후에는 이 번호를 편집할 수 없습니다.

   * **색상**: 우선 순위의 색상을 선택합니다.

     우선 순위 색상은 차트 보고서 및 애자일 팀 설정에 사용됩니다. 차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오. 애자일 팀 설정에 대한 자세한 내용은 [애자일 팀 만들기](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)를 참조하십시오.

   * **기본 우선 순위**: 새로 만든 모든 프로젝트, 작업 또는 문제에 Workfront을 자동으로 적용할 우선 순위를 선택하십시오.

     **보통**&#x200B;은(는) Workfront의 모든 개체에 대한 기본 우선 순위입니다.

     숨겨진 우선 순위를 기본값으로 설정할 수 없습니다.

     기본 우선 순위는 ![기본 우선 순위 아이콘](assets/default-icon.png) 아이콘으로 표시됩니다. 새 기본값을 선택하려면 다음 중 하나를 수행합니다.

      * 우선 순위 이름 옆의 확인란을 선택하고 화면 하단의 작업 표시줄에서 **기본값으로 설정**&#x200B;을 선택합니다.
      * 우선 순위 이름 위로 마우스를 가져간 후 표시되는 **자세히** 메뉴를 클릭합니다. **기본값으로 설정**&#x200B;을 선택합니다.

        새 기본 우선 순위에는 아이콘으로 레이블이 지정됩니다.

   * **설명**: 우선 순위에 대한 설명을 입력하여 해당 함수를 설명하십시오.
   * **선택 항목 숨기기**: 더 이상 필요하지 않은 우선 순위를 숨기려면 **예**&#x200B;를 선택합니다.

     숨겨진 우선 순위는 Workfront의 어디에도 표시되지 않으므로 사용자가 프로젝트, 작업 또는 문제에 대해 우선 순위를 선택할 수 없습니다.

     >[!IMPORTANT]
     >
     >더 이상 사용하지 않을 우선 순위를 삭제하는 대신 숨기는 것이 좋습니다. 이렇게 하면 우선 순위가 이미 완료된 개체에 대한 모든 이전 데이터를 유지하면서 나중에 다른 사람이 우선 순위를 사용하지 못하도록 할 수 있습니다.

1. (선택 사항) 우선 순위를 원하는 순서로 드래그 앤 드롭하여 목록 순서를 변경합니다.

   이렇게 하면 프로젝트, 작업 또는 문제에 대해 표시되는 순서가 변경됩니다. **중요도** 번호는 변경되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.

프로젝트, 작업 및 문제에 우선 순위를 적용하는 방법에 대한 지침은 다음 문서를 참조하십시오.

* [프로젝트 우선 순위 이해 및 업데이트](../../../manage-work/projects/planning-a-project/project-priority.md)
* [작업 우선 순위 업데이트](../../../manage-work/tasks/task-information/task-priority.md)
* [문제 우선 순위 업데이트](../../../manage-work/issues/issue-information/update-issue-priority.md)
