---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect 사용 지표 보기
description: Workfront Data Connect 지표 탭을 사용하여 월별 컴퓨팅 사용 시간과 수행된 쿼리 수에 따라 조직의 사용 지표를 볼 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: 7764e512a3fb30a89e6645a4d8544a5fcffee231
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# [!DNL Workfront Data Connect] 사용 지표 보기

[!DNL Workfront Data Connect] [!UICONTROL 지표] 탭을 사용하여 사용한 계산 시간과 수행한 쿼리 수에 따라 조직의 사용 지표를 볼 수 있습니다. 조직에서는 라이선스 유형 및 Data Connect 추가 기능 구매에 따라 사용할 수 있는 월별 컴퓨팅 시간이 제한됩니다. [!UICONTROL 지표] 탭에는 사용된 항목과 관련하여 사용 가능한 월별 계산 시간에 대한 정보가 표시됩니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용 지표 및 사용 가능한 계산 시간 보기

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 [!UICONTROL **설정**]&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 [!UICONTROL **시스템**] > [!UICONTROL **데이터 액세스**]&#x200B;를 클릭합니다.

1. [!UICONTROL **지표**] 탭을 클릭합니다. 사용 지표는 **사용량 계산** 그래프에 표시되고, 수행된 쿼리 수는 **쿼리 개수** 그래프에 표시됩니다.

   ![Data Connect 사용 지표](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (선택 사항) [!UICONTROL **보기 선택**] 드롭다운 메뉴를 사용하여 두 그래프에 포함된 정보의 시간 범위를 변경할 수 있습니다.

1. (선택 사항) **사용량 계산** 그래프 위의 확인란을 사용하여 표시하거나 숨길 수 있습니다.
   * [!UICONTROL **일별 계산 시간**] - 조직에서 일별로 사용하는 계산 시간입니다.
   * [!UICONTROL **월별 누적 계산 시간**] - 조직에서 한 달에 사용한 총 계산 시간 수입니다. 매달 0으로 재설정됩니다.
   * [!UICONTROL **월별 계산 시간 허용 한도**] - 라이선스 및/또는 추가 기능 구매를 기준으로 조직에서 사용할 수 있는 계산 시간.
