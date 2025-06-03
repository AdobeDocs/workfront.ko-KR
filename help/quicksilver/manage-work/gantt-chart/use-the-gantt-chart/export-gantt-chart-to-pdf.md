---
navigation-topic: use-the-gantt-chart
title: 간트 차트를 PDF으로 내보내기
description: 간트 차트를 PDF으로 내보낼 수 있습니다. 이후에 인쇄하거나 이메일에 첨부하여 다른 사용자와 공유할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 1%

---

# PDF으로 [!UICONTROL 간트 차트] 내보내기

<!--Audited: 5/2025-->

[!UICONTROL 간트 차트]를 PDF으로 내보낼 수 있습니다. 이후에 인쇄하거나 이메일에 첨부하여 다른 사용자와 공유할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 라이선스</td> 
   <td> <p>새로 만들기:[!UICONTROL Light] 이상</p>
   <p>현재:[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 보기] 이상 액세스</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상 액세스 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!UICONTROL 간트 차트] 내보내기

1. [간트 차트 시작](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)에 설명된 대로 PDF으로 내보낼 [!UICONTROL 간트 차트]에 액세스합니다.
1. 내보낼 적절한 정보를 표시하도록 [!UICONTROL 간트 차트]를 구성합니다.

   >[!NOTE]
   >
   >프로젝트 목록에서 [!UICONTROL 간트 차트]를 내보내는 경우 PDF 파일에는 각 프로젝트의 작업이 아닌 목록의 프로젝트만 포함됩니다. 작업 목록을 내보내려면 연결된 프로젝트에서 내보내거나 작업 보고서를 작성하고 보고서 결과를 [!UICONTROL 간트 보기]에 표시하면 됩니다.

   다음 정보 중 하나를 구성합니다.

   * [!UICONTROL 간트 차트] 위에 있는 **필터**, **보기** 및 **그룹화** 아이콘을 클릭하고 [!UICONTROL 간트 차트]의 항목 목록에 적용된 기존 필터, 보기 또는 그룹화를 추가하거나 편집합니다.

     목록 보기에서 선택한 모든 필터 및 그룹화는 [!UICONTROL 간트 차트]를 볼 때 유지됩니다. 보기는 첫 페이지의 [!UICONTROL 간트 차트] 옆에 표시되는 목록 내에서만 내보낸 [!UICONTROL 간트 차트]에 반영됩니다. [!UICONTROL 간트 차트] 자체에는 보기가 표시되지 않습니다.

     >[!TIP]
     >
     >[!UICONTROL 간트 차트]에 더 많은 공간을 허용하려면 가능한 한 적은 수의 열이 포함된 보기를 적용하세요.

   * 계획된 일자가 아닌 예상 일자를 보려면 **예상 일자로 전환** 옵션을 선택하십시오. 기본적으로 계획된 일자가 표시됩니다.

   * 간트 차트의 오른쪽 위 모서리에 있는 **설정** 아이콘 ![설정 아이콘](assets/settings-icon.png)을 클릭하고 보려는 정보를 선택합니다. 선택하면 이 정보가 내보낸 Gantt PDF 파일에 포함됩니다.

     다음 옵션 중에서 선택합니다.

      * 실제 일자
      * 할당
      * 기준선
      * 커밋 일자
      * % 완료
      * 중요 경로
      * 마일스톤 다이아몬드
      * 마일스톤 라인
      * 전임 작업
      * 진행 상태
      * (조건부) 계획된 일자
      * (조건부) 예상 일자

     자세한 내용은   [정보가 [!UICONTROL 간트 차트에 표시되는 방식을 구성합니다]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > [!UICONTROL 간트 차트]을(를) PDF으로 내보낼 때 [!UICONTROL 간트 차트]에 할당이 표시되지 않습니다. 내보내면 할당이 목록 보기에만 표시됩니다.

   * [!UICONTROL 간트 차트]에 표시되는 기간입니다. 내보내기 파일에 표시되는 방식은 이후 단계에서 **[!UICONTROL 표시되는 항목]** 또는 **[!UICONTROL 여러 페이지]**&#x200B;를 선택했는지 여부에 따라 달라집니다.

     자세한 내용은 [간트 차트에서 정보 보기](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)를 참조하십시오.



1. (선택 사항) 내보낸 PDF의 특정 작업만 포함하려면 포함할 작업을 선택합니다. 작업을 선택하지 않으면 내보낸 PDF에 모든 작업이 포함됩니다.

   예를 들어 50개의 작업이 포함된 프로젝트에 대한 [!UICONTROL 간트 차트]를 보고 있지만 내보낸 [!UICONTROL 간트 차트]에 10개의 작업만 표시하려면 표시할 10개의 작업을 선택합니다.

1. 간트 차트의 오른쪽 위 모서리에 있는 프린터 아이콘 ![프린터 아이콘](assets/printer-icon.png)을 클릭합니다.
**[!UICONTROL PDF으로 내보내기]** 대화 상자가 표시됩니다.

   ![PDF으로 내보내기 대화 상자](assets/exported-gantt-ui-350x225.png)

1. **내보내기** 섹션에서 다음 옵션 중 하나를 선택하여 표시된 것만 내보내는지 아니면 전체 [!UICONTROL 간트 차트]를 내보낼지 지정합니다.

   * **[!UICONTROL 표시되는 항목]:** 최대 500개의 항목을 내보내기 전에 화면에 표시되는 모든 작업(하위 작업 포함)을 내보냅니다. (**[!UICONTROL 미리 보기]** 섹션에 표시되는 내용이 아닙니다. **미리 보기** 섹션에는 샘플 데이터만 포함됩니다.)

     상위 작업이 축소되고 하위 작업이 표시되지 않는 경우에도 하위 작업이 내보낸 PDF에 포함됩니다. 상위 작업만 포함하려면 포함하려는 상위 작업을 선택하고 하위 작업은 선택하지 않은 상태로 두십시오.

     >[!TIP]
     >
     >[간트 차트에서 정보 보기[!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)에 설명된 대로 확대/축소 또는 슬라이더 도구를 사용하여 [!UICONTROL 간트 차트]의 일부만 표시할 수 있습니다. 내보낼 페이지를 더 많이 표시하려면 더 세분화된 옵션을 선택하고, 내보낼 페이지를 더 적게 표시하려면 더 세분화된 옵션을 선택합니다.


   * **[!UICONTROL 여러 페이지]:** 현재 화면에 표시되지 않는 항목을 포함하여 전체 [!UICONTROL 간트 차트]&#x200B;(최대 500개 항목)를 내보냅니다.

     >[!NOTE]
     >
     >* 500개 이상의 항목을 포함하는 [!UICONTROL 간트 차트]를 내보내려면 [!UICONTROL 간트 차트]를 보기 전에 목록에 필터를 적용하여 500개 이하의 항목 또는 250페이지가 표시되도록 하십시오. 필터를 적용하는 방법에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하십시오.
     >
     >
     >* 다음과 같은 경우에는 전체 간트 차트를 내보낼 수 없습니다.
     >   
     >   * 250페이지를 초과하는 경우.
     >   * 항목이 500개가 넘는 경우.


1. PDF을 PDF으로 내보낸 후 인쇄할 경우 **[!UICONTROL 페이지 크기]** 드롭다운 메뉴에서 인쇄할 용지 크기를 선택합니다.
다음 옵션 중에서 선택할 수 있습니다.

   * **[!UICONTROL 편지]**
   * **[!UICONTROL 법률]**
   * **[!UICONTROL 원장]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]**(일부 언어에서만 사용 가능)
   * **[!UICONTROL A4]**
1. **[!UICONTROL 페이지 방향]** 섹션에서 PDF을 가로 방향으로 내보내거나 세로 방향으로 내보내기를 선택합니다.
1. 내보낸 PDF에 범례를 포함하려면 **[!UICONTROL 범례 표시]**&#x200B;를 선택합니다.
1. **[!UICONTROL 내보내기]**&#x200B;를 클릭합니다. pdf가 만들어지고 컴퓨터로 다운로드됩니다.

   내보낸 파일의 맨 아래에 있는 범례는 [!UICONTROL 간트 차트]에서 활성화했으며 작업 목록에서 사용할 수 있는 옵션만 설명합니다. 예를 들어 마일스톤은 마일스톤과 연관된 작업이 하나 이상 있는 경우에만 범례에 표시됩니다.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
