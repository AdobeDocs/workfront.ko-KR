---
title: 문제 심각도 만들기 또는 사용자 지정
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 사용자는 심각도를 사용하여 문제의 심각도를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도를 사용자 정의하거나 사용자에 대한 새 심각도를 만들 수 있습니다.
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

사용자는 심각도를 사용하여 문제의 심각도를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도를 사용자 정의하거나 사용자에 대한 새 심각도를 만들 수 있습니다.

>[!NOTE]
>
>작업 및 프로젝트에 심각도가 없습니다.

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

## 기본 제공 문제 심각도

Workfront에는 5개의 내장된 문제 심각도가 있습니다.

* 표시용
* 혼란 야기
* 해결 방법이 있는 버그
* 해결 방법이 없는 버그
* 치명적인 오류

<p>이러한 심각도에 대해 다음을 편집할 수 있습니다.</p>

* 이름
* 색상

  [문제 심각도]별로 결과를 그룹화할 경우 심각도의 색상은 차트 보고서에 유지됩니다. 차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오.

* 기본 심각도는 무엇입니까?

  기본 심각도에 대한 자세한 내용은 이 문서에서 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity)을 참조하십시오.
* 설명
* Workfront에 심각도가 숨겨져 있는지 여부

  심각도 숨기기에 대한 자세한 내용은 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity")을 참조하세요.

* 심각도 삭제

  이 작업을 수행하는 경우 대체 심각도를 선택해야 합니다.

## 문제 심각도 만들기 또는 편집 {#create-or-edit-an-issue-severity}

Workfront 관리자는 사용자의 요구 사항에 맞게 문제 심각도를 만들고 편집할 수 있습니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **심각도**&#x200B;를 클릭합니다.

1. 새 심각도를 만드는 경우 **새 심각도 추가**&#x200B;를 클릭합니다.
1. 새 심각도에 대해 다음 옵션을 구성하거나 기존 심각도를 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">심각도 이름</td> 
      <td>심각도 이름 입력</td> 
     </tr> 
     <tr> 
      <td role="rowheader">중요도 점수</td> 
      <td>심각도에 대해 원래 Workfront에서 할당한 심각도 수준을 높이거나 낮춥니다.
      <p>각 심각도의 중요도 번호는 고유해야 합니다. 가장 높은 숫자는 가장 높은 수준의 심각도에 해당합니다.</p> <p>심각도를 저장한 후에는 이 숫자를 편집할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">색상</td> 
      <td> <p>심각도의 색상을 선택합니다.</p> 
      <p>심각도의 색상은 문제 심각도별로 결과를 그룹화할 때 차트 보고서에 사용됩니다. 차트 보고서에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">보고서에 차트 추가</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 심각도</td> 
      <td>새로 생성된 모든 문제를 Workfront에서 자동으로 선택할 심각도를 선택합니다.</p>
      <p>코스메틱은 Workfront 문제에 대한 기본 심각도입니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>심각도에 대한 설명을 입력하여 해당 기능을 설명합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">숨기기</td> 
      <td> 더 이상 필요하지 않은 심각도를 숨깁니다. 
      <p>숨겨진 심각도는 Workfront의 어디에도 표시되지 않으므로 사용자가 문제에 대해 심각도를 선택할 수 없습니다.</p> 
      <p><b>중요</b>: 더 이상 사용하지 않을 심각도를 삭제하지 말고 숨기는 것이 좋습니다. 이렇게 하면 심각도가 이미 완료된 객체에 대한 모든 내역 데이터를 유지하면서 나중에 사람들이 심각도를 사용하지 못하도록 할 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 심각도를 원하는 순서로 드래그 앤 드롭하여 목록 순서를 변경합니다.

   그러면 문제에 대해 표시되는 순서가 변경됩니다. **중요도** 번호는 변경되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.

문제를 처리하는 동안 심각도를 사용하는 방법에 대한 자세한 내용은 [문제 심각도 업데이트](../../../manage-work/issues/issue-information/update-issue-severity.md)를 참조하십시오.
