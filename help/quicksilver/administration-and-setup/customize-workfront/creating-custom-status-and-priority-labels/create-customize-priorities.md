---
title: 우선순위 만들기 및 사용자 지정
description: Workfront의 설정 영역에서 프로젝트, 작업 및 문제에 대한 우선순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제에 중요함을 제공합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 우선순위 만들기 및 사용자 지정

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront의 설정 영역에서 프로젝트, 작업 및 문제에 대한 우선순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제에 중요함을 제공합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기존 우선순위 사용자 지정

Workfront 관리자는 Workfront에 제공된 기본 우선순위를 다음과 같이 수정할 수 있습니다.

* 우선순위 이름을 변경합니다.
* 우선순위 순서를 재정리합니다.

   우선순위 순서 조정 방법에 대한 자세한 내용은 [프로젝트 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue).

* 기본 우선순위를 변경합니다.

   기본 우선 순위 변경 기능에 대한 자세한 내용은 [프로젝트 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue).

* 우선순위에 대한 설명을 편집합니다.
* 우선 순위마다 색상을 설정합니다.

   우선순위 색상은 결과를 그룹화할 때 차트 보고서에 사용됩니다 **우선순위**.

   차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 우선순위를 삭제합니다.

   기존 우선순위를 삭제할 때는 교체 우선순위를 선택해야 합니다.

* 우선순위를 숨깁니다.

   우선순위 숨기기 기능에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >각 개체에 대해 Workfront 계정에 하나 이상의 우선 순위가 있어야 합니다.

각 객체 유형(프로젝트, 작업 및 문제)에 대해 기본적으로 제공되는 우선순위는 동일합니다.

* 없음
* 낮음
* 기본
* 높음
* 긴급

## 프로젝트 작업 또는 문제에 대한 우선 순위 만들기 {#create-a-priority-for-a-project-task-or-issue}

Workfront에서 제공하는 기본 우선순위 외에도 조직의 요구 사항을 반영하도록 고유한 우선순위를 추가할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **우선순위**.

1. 우선 순위를 만들 개체 유형의 탭을 클릭합니다(**프로젝트**, **작업**, 또는 **문제**).
1. 클릭 **새 우선 순위 추가**.
1. 새 우선 순위에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">우선 순위 이름</td> 
      <td>우선 순위 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">중요도 점수</td> 
      <td> <p>새 우선순위를 추가할 때 기본적으로 숫자가 할당됩니다. 본인의 요구 사항과 일치하지 않는 경우 이 번호를 편집합니다.</p> <p>다음 <strong>중요도</strong> 각 우선 순위의 번호는 선택한 개체에 대해 고유해야 합니다.<br>우선 순위 수는 프로젝트, 작업 또는 문제의 중요성을 반영합니다. 가장 높은 숫자는 가장 높은 우선 순위에 해당합니다.</p> <p><b>참고</b>: 우선 순위를 저장한 후에는 중요도 번호를 편집할 수 없습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>우선 순위에 맞는 색을 선택하십시오.</p> <p>우선순위 색상은 차트 보고서와 Agile Team Settings에 사용됩니다. 차트 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">보고서에 차트 추가</a>.</p> <p>Agile 팀 설정에 대한 자세한 내용은 의 를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 우선 순위</td> 
      <td> <p>라디오 단추를 선택하여 이 우선순위가 기본 우선 순위인지 여부를 결정합니다.</p> <p>우선순위가 <strong>기본 우선순위</strong>Workfront의 모든 프로젝트, 작업 또는 문제에 대해 자동으로 선택됩니다. <strong>일반</strong> 는 Workfront의 모든 객체에 대한 기본 우선 순위입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>해당 기능을 설명하는 우선 순위에 대한 설명을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">숨기기</td> 
      <td> <p>우선 순위를 숨기려면 이 상자를 선택합니다.</p><p>을(를) 선택하는 경우 <b>숨기기</b> 선택 사항: Workfront에서 우선순위가 표시되지 않고 사용자가 프로젝트, 작업 및 문제에 대해 선택할 수 없습니다.</p> 
      <p><b>중요 사항</b>: 더 이상 사용하지 않을 우선순위를 삭제하는 대신 숨기는 것이 좋습니다. 이를 숨기면, 이 우선 순위로 완성된 개체의 모든 역사적 데이터를 유지할 수 있으며, 향후 이 우선 순위를 선택할 수 없게 합니다. </p>
      <p>선택적으로, 원하는 순서로 끌어다 놓아 우선순위의 목록 순서를 변경할 수 있습니다. 그러면 프로젝트, 작업 및 문제에 대해 표시되는 순서가 변경됩니다. 이렇게 해도 <b>중요도</b> 번호. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

프로젝트, 작업 및 문제에 우선순위를 적용하는 방법에 대한 지침은 다음 문서를 참조하십시오.

* [프로젝트 우선순위 이해 및 업데이트](../../../manage-work/projects/planning-a-project/project-priority.md)
* [작업 우선 순위 업데이트](../../../manage-work/tasks/task-information/task-priority.md)
* [업데이트 문제 우선 순위](../../../manage-work/issues/issue-information/update-issue-priority.md)
