---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 향상된 분석에서 프로젝트 트리맵 시각화 보기
description: 프로젝트 트리맵 시각화는 규모에 있어 다른 작업 노력과 비교하여 특정 기간 동안 작업한 시간 또는 일을 보는 것입니다. 이렇게 하면 사람들이 프로젝트에 얼마나 많은 시간을 할애했는지 이해하는 데 도움이 됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 2%

---

# 향상된 분석에서 프로젝트 트리맵 시각화 보기

>[!IMPORTANT]
>
>향상된 Analytics가 5월 27일에 Workfront에서 제거되었습니다. Workfront Data Connect는 새로운 대체 솔루션이며 현재 사용하는 향상된 Analytics 시각화를 복제하는 데 사용할 수 있습니다. <br>자세한 내용은 [향상된 Analytics 사용 중단](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) 안내서를 참조하십시오.


<!-- Audited: 12/2023 -->

프로젝트 트리맵 시각화는 규모에 있어 다른 작업 노력과 비교하여 특정 기간 동안 작업한 시간 또는 일을 보는 것입니다. 이렇게 하면 사람들이 프로젝트에 얼마나 많은 시간을 할애했는지 이해하는 데 도움이 됩니다.

![프로젝트 트리맵](assets/project-treemap-350x126.png){width="700"}

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront 플랜</a></td> 
   <td> <p>비즈니스 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a></td> 
   <td>   <p>신규:</p> 
   <ul><li>밝은 색 이상</li></ul>
   <p>현재:</p>
   <ul><li>검토 이상</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 보기</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보기</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

향상된 Analytics를 사용하기 위한 전제 조건은 [향상된 Analytics 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 &quot;전제 조건&quot; 섹션을 참조하십시오.

## 프로젝트 트리맵 시각화 이해

프로젝트 트리맵 시각화의 상자는 프로젝트를 나타내며 상자의 크기는 서로 다른 프로젝트에서 소비한 시간의 비교를 보여 줍니다. 상자가 클수록 프로젝트에 더 많은 시간이 소요됩니다.

프로젝트 트리맵 시각화는 다음과 같이 구성됩니다.

* **더 작고 연한 파란색 상자**: 몇 시간 또는 며칠이 더 적은 프로젝트는 연한 파란색의 더 작은 상자로 표시됩니다.

  ![작은 상자](assets/project-treemap-smaller-box.png)

* **크고 짙은 파란색 상자**: 시간이 더 많은 프로젝트(일)는 어두운 파란색의 더 큰 상자로 표시됩니다.

  ![큰 상자](assets/project-treemap-larger-box-350x205.png)

* **Medium 크기, 파란색 상자**: 두 범주 사이에 있는 프로젝트는 어두운 파란색과 연한 파란색 사이에 파란색 음영이 있는 중간 크기 상자로 표시됩니다. 중간 크기의 상자에는 3가지 가능한 파란색 음영이 있습니다.

오른쪽의 범례는 각 파란색 음영에 대한 완료된 시간 분류를 보여 줍니다. 이 범례는 동적이며 데이터에 따라 업데이트됩니다.

![트리맵 시간 완료됨](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>프로젝트 트리맵 시각화를 계획된 시간이 아닌 기간별로 보고 있는 경우 이 범례는 각 파란색 음영에 대해 작업한 일의 분류를 표시합니다.\
>![트리맵 작업일](assets/project-treemap-days-worked.png)>

이 정보를 보면 다음과 같은 사항을 확인할 수 있습니다.

* 선택한 날짜 범위 동안 작업 중인 항목의 우선 순위
* 어떤 팀이 시간을 보내고 있습니까?
* 팀이 올바른 것에 집중한다면,
* 특정 프로젝트를 클릭할 때 해당 기간 동안 프로젝트 범위가 얼마나 변경되었는지 보여 줍니다.

이 시각화에 가장 적합한 데이터를 얻는 방법에 대해 알아보려면 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md)를 참조하십시오.

## 프로젝트 트리맵 시각화 보기

1. 주 메뉴 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon-16x12.png)을 클릭한 다음 **분석**&#x200B;을 선택합니다.
1. (선택 사항) 다른 날짜 범위를 사용하려면 날짜 범위 필터에서 새 시작 날짜와 종료 날짜를 선택합니다.

   ![날짜 범위 선택](assets/filters-select-date-range-350x344.png)

   날짜 범위 필터 사용에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

1. (조건부) 프로젝트 데이터 세트를 제한해야 하는 경우 사용할 필터를 선택하고 적용합니다.

   향상된 분석에서 필터를 추가하는 방법에 대한 자세한 내용은 [향상된 분석에서 필터 적용](../enhanced-analytics/use-enhanced-analytics-filters.md)을 참조하십시오.

   필터를 추가하면 최대 50개의 프로젝트에 대한 데이터가 표시되고 페이지를 떠나거나 Workfront에서 로그아웃한 후에도 필터가 활성 상태로 유지됩니다.

1. (선택 사항) 프로젝트 정렬 방법을 변경하려면 프로젝트 트리맵 시각화의 오른쪽 상단에 있는 **정렬 기준** 메뉴를 클릭한 다음, 새 정렬 옵션을 선택하십시오.

   * **A - Z**
   * **Z - A**
   * **계획된 완료 일자**
   * **계획된 시작 일자**

   페이지의 다른 모든 시각화는 정렬 선택 사항과 일치하도록 업데이트됩니다.

1. (조건부) 데이터 세트에 50개가 넘는 프로젝트가 있는 경우 시각화의 왼쪽 하단 모서리에 있는 화살표를 사용하여 50개의 프로젝트 그룹 중 하나에서 다음 그룹으로 이동합니다.

   페이지의 다른 모든 시각화는 페이지 선택 사항과 일치하도록 업데이트됩니다.

   ![페이지 매김](assets/pagination-350x118.png)

1. (선택 사항) 보기를 **계획된 시간**&#x200B;에서 **지속 시간**(으)로 변경합니다.

   계획된 시간이 기본적으로 선택됩니다.

1. 프로젝트 상태를 확인하고 총 계획된 시간, 총 완료된 시간 및 일별 프로젝트에 소요된 평균 시간을 확인하려면 프로젝트 위로 마우스를 가져갑니다.

   ![트리맵 프로젝트 세부 정보](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >**duration** 보기를 선택한 경우 다음 기간 세부 정보가 표시됩니다.
   >
   >* **계획된 일정**: 프로젝트를 완료하는 데 계획된 일 수입니다.
   >* **근무일**: 맨 위에서 선택한 날짜 범위 내에 완료된 각 작업의 계획된 기간을 하루의 시간 수로 나눈 값입니다.
   >   
   >![트리맵 기간](assets/duration-treemap-350x159.png)
   >
   >기간에 대한 자세한 내용은 [향상된 분석 개요](../enhanced-analytics/enhanced-analytics-overview.md)의 &quot;기간 보기&quot; 섹션을 참조하십시오.

1. (선택 사항) 시각화 데이터를 내보내려면 시각화의 오른쪽 상단에 있는 **내보내기 아이콘** ![내보내기 아이콘](assets/export.png)을 클릭한 다음 내보내기 형식을 선택합니다.

   * **차트(PNG)**
   * **데이터 테이블(XSLX)**

1. 번다운 및 진행 중인 작업 시각화를 열어 작업과 시간(또는 일)이 프로젝트 크기에 어떻게 기여했는지에 대한 심도 있는 insight을 얻으려면 프로젝트를 클릭하십시오.

번다운 시각화에 대한 자세한 내용은 [향상된 분석에서 번다운 시각화 보기](../enhanced-analytics/burndown-overview.md)를 참조하십시오. 진행 중인 작업 시각화에 대한 자세한 내용은 [향상된 분석에서 진행 중인 작업 시각화 보기](../enhanced-analytics/tasks-in-flight-overview.md)를 참조하십시오.

