---
title: 우선 순위 만들기 및 사용자 지정
description: Workfront의 설정 영역에서 프로젝트, 작업 및 문제의 우선 순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제를 중요시합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 우선 순위 만들기 및 사용자 지정

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront의 설정 영역에서 프로젝트, 작업 및 문제의 우선 순위를 제어할 수 있습니다. 우선 순위는 Adobe Workfront의 프로젝트, 작업 또는 문제를 중요시합니다.

## 액세스 요구 사항

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기존 우선 순위 맞춤화

Workfront 관리자는 Workfront에서 제공하는 기본 우선 순위를 다음과 같이 수정할 수 있습니다.

* 우선 순위 이름을 변경합니다.
* 우선 순위 재정렬.

  우선 순위를 다시 정렬하는 방법에 대한 자세한 내용은 [프로젝트 작업의 우선 순위 만들기 또는 문제](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

* 기본 우선 순위를 변경합니다.

  기본 우선 순위를 변경하는 기능에 대한 자세한 내용은 [프로젝트 작업 또는 문제에 대한 우선 순위 만들기](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

* 우선 순위에 대한 설명을 편집합니다.
* 각 우선 순위에 대한 색상을 설정합니다.

  결과를 **우선 순위**(으)로 그룹화할 때 우선 순위 색상이 차트 보고서에 사용됩니다.

  차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오.

* 우선 순위를 삭제합니다.

  기존 우선순위를 삭제할 때는 대체 우선순위를 선택해야 합니다.

* 우선 순위를 숨깁니다.

  우선 순위를 숨기는 기능에 대한 자세한 내용은 [프로젝트 작업의 우선 순위 만들기 또는 문제](#create-a-priority-for-a-project-task-or-issue)를 참조하십시오.

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

Workfront에서 제공하는 기본 우선 순위 외에도 조직의 요구 사항을 반영하기 위해 고유한 우선 순위를 추가할 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **우선 순위**&#x200B;를 클릭합니다.

1. 우선 순위를 만들려는 개체 유형의 탭을 클릭합니다(**프로젝트**, **작업** 또는 **문제**).
1. **새 우선 순위 추가**&#x200B;를 클릭합니다.
1. 새 우선 순위에 대해 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">우선 순위 이름</td> 
      <td>우선 순위의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">중요도 점수</td> 
      <td> <p>새 우선 순위를 추가할 때는 기본적으로 숫자가 할당됩니다. 이 번호가 사용자의 요구 사항과 일치하지 않는 경우 이 번호를 편집합니다.</p> <p>각 우선 순위의 <strong>중요도</strong> 번호는 선택한 개체에 대해 고유해야 합니다.<br>우선 순위 숫자는 프로젝트, 작업 또는 문제의 중요도를 반영합니다. 가장 높은 숫자는 가장 높은 우선 순위와 일치합니다.</p> <p><b>참고</b>: 우선 순위를 저장한 후에는 중요도 번호를 편집할 수 없습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>우선 순위의 색상을 선택합니다.</p> <p>우선 순위 색상은 차트 보고서 및 애자일 팀 설정에 사용됩니다. 차트 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">보고서에 차트 추가</a>를 참조하십시오.</p> <p>애자일 팀 설정에 대한 자세한 내용은에서 를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 우선 순위</td> 
      <td> <p>라디오 버튼을 선택하여 기본 우선 순위인지 여부를 결정합니다.</p> <p>우선 순위가 <strong>기본 우선 순위</strong>(으)로 지정된 경우 Workfront의 모든 프로젝트, 작업 또는 문제에 대해 자동으로 선택됩니다. <strong>보통</strong>은(는) Workfront의 모든 개체에 대한 기본 우선 순위입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>우선 순위에 대한 설명을 추가하여 해당 기능을 설명합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">숨기기</td> 
      <td> <p>우선 순위를 숨기려면 이 상자를 선택합니다.</p><p><b>숨기기</b> 옵션을 선택하면 우선 순위가 Workfront의 어디에도 표시되지 않으며 사용자가 프로젝트, 작업 및 문제에 대해 우선 순위를 선택할 수 없습니다.</p> 
      <p><b>중요</b>: 더 이상 사용하지 않을 우선 순위를 삭제하는 대신 숨기는 것이 좋습니다. 이 우선 순위를 사용하여 완료된 개체의 모든 기록 데이터를 숨기면 나중에 해당 우선 순위를 선택할 수 없게 됩니다. </p>
      <p>원하는 순서로 끌어다 놓아 우선순위의 목록 순서를 변경할 수 있습니다(선택적). 이렇게 하면 프로젝트, 작업 및 문제에 대해 표시되는 순서가 변경됩니다. <b>중요도</b> 번호는 변경되지 않습니다. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

프로젝트, 작업 및 문제에 우선 순위를 적용하는 방법에 대한 지침은 다음 문서를 참조하십시오.

* [프로젝트 우선 순위 이해 및 업데이트](../../../manage-work/projects/planning-a-project/project-priority.md)
* [작업 우선 순위 업데이트](../../../manage-work/tasks/task-information/task-priority.md)
* [문제 우선 순위 업데이트](../../../manage-work/issues/issue-information/update-issue-priority.md)
