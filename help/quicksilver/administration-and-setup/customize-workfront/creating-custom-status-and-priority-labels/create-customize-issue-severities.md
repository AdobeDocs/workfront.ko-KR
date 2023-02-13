---
title: 문제 심각도 만들기 또는 사용자 지정
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 사용자는 몇 가지 기능을 사용하여 문제가 얼마나 심각한지를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도 중 하나를 사용자 지정하거나 사용자를 위해 새 심각도를 만들 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# 문제 심각도 만들기 또는 사용자 지정

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

사용자는 몇 가지 기능을 사용하여 문제가 얼마나 심각한지를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도 중 하나를 사용자 지정하거나 사용자를 위해 새 심각도를 만들 수 있습니다.

>[!NOTE]
>
>작업 및 프로젝트에 몇 가지 기능이 없습니다.

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

## 내장 문제 심각도

Workfront에는 5가지 기본 제공 문제 심각성이 있습니다.

* 표시용
* 혼란 야기
* 해결 방법이 있는 버그
* 해결 방법이 없는 버그
* 치명적인 오류

<p>이러한 심각도에 대해 다음을 편집할 수 있습니다.</p>

* 이름
* 색상

   심각도의 색상이 차트 보고서에 유지됩니다(문제 심각도별로 결과를 그룹화하는 경우). 차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 기본값은 심각도입니다

   기본 심각도에 대한 자세한 내용은 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity) 참조하십시오.
* 설명
* Workfront에서 심각도가 숨겨지는지 여부

   심각도 숨김에 대한 자세한 내용은 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity")

* 심각도 삭제

   이 작업을 수행하는 경우 교체 심각도를 선택해야 합니다.

## 문제 심각도 만들기 또는 편집 {#create-or-edit-an-issue-severity}

Workfront 관리자는 사용자의 요구 사항에 맞게 문제 심각도를 만들고 편집할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **세속**.

1. 새 심각도를 생성하는 경우 **새 심각도 추가**.
1. 새 심각도에 대해 다음 옵션을 구성하거나 기존 심각도에 대해 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">심각도 이름</td> 
      <td>심각도의 이름을 입력합니다</td> 
     </tr> 
     <tr> 
      <td role="rowheader">중요도 점수</td> 
      <td>처음에 Workfront에서 지정한 심각도 수준을 심각도에 대해 늘리거나 줄입니다.
      <p>각 심각도에 대한 중요도 번호는 고유해야 합니다. 가장 높은 숫자는 가장 높은 심각도 수준에 해당합니다.</p> <p>심각도를 저장한 후에는 이 번호를 편집할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>심각도의 색을 선택합니다.</p> 
      <p>심각도 색상은 문제 심각도별로 결과를 그룹화할 때 차트 보고서에 사용됩니다. 차트 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">보고서에 차트 추가</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 심각도</td> 
      <td>Workfront에서 새로 만든 모든 문제를 자동으로 선택할 심각도를 선택합니다.</p>
      <p>화장품은 Workfront의 문제에 대한 기본 심각도입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>해당 기능을 설명하는 심각도에 대한 설명을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">숨기기</td> 
      <td> 더 이상 필요하지 않은 심각도를 숨깁니다. 
      <p>숨겨진 심각도는 Workfront에 표시되지 않으므로 사용자가 문제에 대해 심각도를 선택할 수 없습니다.</p> 
      <p><b>중요 사항</b>: 더 이상 사용하지 않을 심각도를 삭제하는 대신 숨길 것을 권합니다. 이렇게 하면 모든 기록 데이터를 심각도와 함께 이미 완료된 객체에 보관하면서 나중에 심각도를 사용하지 못하도록 합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 심각도를 원하는 순서로 드래그하여 놓아 목록 순서를 변경합니다.

   그러면 문제에 대해 표시되는 순서가 변경됩니다. 변경 사항이 없습니다 **중요도** 번호.

1. **저장**&#x200B;을 클릭합니다.

문제를 사용하여 작업하는 동안 심각도를 사용하는 방법에 대한 자세한 내용은 [문제 심각도 업데이트](../../../manage-work/issues/issue-information/update-issue-severity.md).
