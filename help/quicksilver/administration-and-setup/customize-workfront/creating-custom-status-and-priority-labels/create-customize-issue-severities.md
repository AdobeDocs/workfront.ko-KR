---
title: 문제 심각도 만들기 또는 사용자 지정
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 사용자는 심각도를 사용하여 문제의 심각도를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도를 사용자 정의하거나 사용자에 대한 새 심각도를 만들 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 4a7362ae663b73ce48f049556145b4de3e6a6ac9
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 3%

---

# 문제 심각도 만들기 또는 사용자 정의

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

사용자는 심각도를 사용하여 문제의 심각도를 정의할 수 있습니다. Adobe Workfront에 있는 5개의 기본 심각도를 사용자 정의하거나 사용자에 대한 새 심각도를 만들 수 있습니다.

>[!NOTE]
>
>작업 및 프로젝트에 심각도가 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td>
     <p>새로운 기능: 표준</p>
     <p>또는</p>
     <p>현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기본 제공 문제 심각도

Workfront에는 5개의 내장된 문제 심각도가 있습니다.

* 표시용
* 혼란 야기
* 해결 방법이 있는 버그
* 해결 방법이 없는 버그
* 치명적인 오류

이러한 심각도에 대해 다음을 편집할 수 있습니다.

* 이름
* 색상

  [문제 심각도]별로 결과를 그룹화할 경우 심각도의 색상은 차트 보고서에 유지됩니다. 차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오.

* 기본 심각도는 무엇입니까?

  기본 심각도에 대한 자세한 내용은 이 문서에서 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity)을 참조하십시오.

* 설명
* Workfront에 심각도가 숨겨져 있는지 여부

  심각도 숨기기에 대한 자세한 내용은 이 문서에서 [문제 심각도 만들기 또는 편집](#create-or-edit-an-issue-severity)을 참조하십시오.

* 심각도 삭제

  이 작업을 수행하는 경우 대체 심각도를 선택해야 합니다.

## 문제 심각도 만들기 또는 편집 {#create-or-edit-an-issue-severity}

Workfront 관리자는 사용자의 요구 사항에 맞게 문제 심각도를 만들고 편집할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **프로젝트 환경 설정** > **심각도**&#x200B;를 클릭합니다.

1. 새 심각도를 만드는 경우 테이블 하단에 있는 <span class="preview">**새 행**&#x200B;을 클릭하거나</span>, **새 심각도를 추가**&#x200B;하세요.
1. 새 심각도에 대해 다음 옵션을 구성하거나 기존 심각도를 편집합니다.

   * **심각도 이름**: 심각도의 이름을 입력하십시오.
   * **중요도**: 심각도에 대해 원래 Workfront에서 할당한 심각도의 수준을 높이거나 낮춥니다.

     각 심각도의 중요도 번호는 고유해야 합니다. 가장 높은 숫자는 가장 높은 수준의 심각도에 해당합니다.

     심각도를 저장한 후에는 이 숫자를 편집할 수 없습니다.

   * **색상**: 심각도의 색상을 선택하십시오.

     심각도의 색상은 문제 심각도별로 결과를 그룹화할 때 차트 보고서에 사용됩니다. 차트 보고서에 대한 자세한 내용은 [보고서에 차트 추가](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)를 참조하십시오.

   * **기본 심각도**: 새로 만든 모든 문제에 Workfront을 자동으로 적용할 심각도를 선택하십시오.

     **Cosmetic**&#x200B;은(는) Workfront 문제에 대한 기본 심각도입니다.

     숨겨진 심각도를 기본값으로 설정할 수 없습니다.

     <div class="preview">

     기본 심각도는 ![기본 심각도 아이콘](assets/default-icon.png) 아이콘으로 표시됩니다. 새 기본값을 선택하려면 다음 중 하나를 수행합니다.

      * 심각도 이름 옆에 있는 확인란을 선택하고 화면 하단의 작업 표시줄에서 **기본값으로 설정**&#x200B;을 선택합니다.
      * 심각도 이름 위로 마우스를 가져간 후 표시되는 **자세히** 메뉴를 클릭합니다. **기본값으로 설정**&#x200B;을 선택합니다.

        새 기본 심각도는 아이콘으로 레이블이 지정됩니다.

     </div>

   * **설명**: 기능을 설명하기 위해 심각도에 대한 설명을 입력하십시오.
   * <span class="preview">**선택 항목 숨기기**</span> 또는 **숨기기**: <span class="preview">더 이상 필요하지 않은 심각도를 숨기려면 **예**</span>&#x200B;를 선택하거나 확인란을 선택하십시오.

     숨겨진 심각도는 Workfront의 어디에도 표시되지 않으므로 사용자가 문제에 대해 심각도를 선택할 수 없습니다.

     >[!IMPORTANT]
     >
     >더 이상 사용하지 않을 심각도를 삭제하는 대신 숨기는 것이 좋습니다. 이렇게 하면 심각도가 이미 완료된 객체에 대한 모든 내역 데이터를 유지하면서 나중에 사람들이 심각도를 사용하지 못하도록 할 수 있습니다.

1. (선택 사항) 심각도를 원하는 순서로 드래그 앤 드롭하여 목록 순서를 변경합니다.

   그러면 문제에 대해 표시되는 순서가 변경됩니다. **중요도** 번호는 변경되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.

문제를 처리하는 동안 심각도를 사용하는 방법에 대한 자세한 내용은 [문제 심각도 업데이트](../../../manage-work/issues/issue-information/update-issue-severity.md)를 참조하십시오.
