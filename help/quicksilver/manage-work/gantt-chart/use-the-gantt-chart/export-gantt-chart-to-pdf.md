---
navigation-topic: use-the-gantt-chart
title: 간트 차트를 PDF으로 내보내기
description: 간트 차트를 PDF으로 내보낼 수 있습니다.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 내보내기 [!UICONTROL 간트 차트] 대상 PDF

을(를) 내보낼 수 있습니다 [!UICONTROL 간트 차트] PDF.

내보내기 후 [!UICONTROL 간트 차트] PDF을 위해 전자 메일을 인쇄 또는 첨부하여 다른 사용자와 공유할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 따르려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 계획*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 보기] 이상 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상 액세스 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 내보내기 [!UICONTROL 간트 차트]

1. 액세스 [!UICONTROL 간트 차트] 에 설명된 대로 PDF으로 내보낼 수 있습니다 [시작하기 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 다음을 구성했는지 확인합니다. [!UICONTROL 간트 차트] 내보내기 전에 적절한 정보를 표시합니다.

   >[!NOTE]
   >
   >를 내보내는 경우 [!UICONTROL 간트 차트] 프로젝트 목록에서 PDF 파일에는 각 프로젝트의 작업이 아닌 목록의 프로젝트만 포함되어 있습니다. 작업 목록을 내보내려면 작업 목록과 연관된 프로젝트에서 내보내거나 작업 보고서를 작성하여 보고서의 결과를 [!UICONTROL 간트 보기].

   다음 정보를 구성할 수 있습니다.

   * 작업 목록에서 원하는 대로 필터, 보기 및 그룹화. 목록 보기에서 선택한 모든 필터 및 그룹화는 [!UICONTROL 간트 차트]. 보기는 내보내기에 반영됩니다. [!UICONTROL 간트 차트] 다음 옆에 표시되는 목록 내에서만 [!UICONTROL 간트 차트] 첫 페이지에요. 보기가 다음에 표시되지 않음 [!UICONTROL 간트 차트] 그 자체.

     >[!TIP]
     >
     >을(를) 위한 더 많은 공간을 허용하려면 [!UICONTROL 간트 차트] 가능한 한 적은 열을 포함하는 보기를 적용합니다.

   * 의 구성 옵션 [!UICONTROL 간트 차트]. 예를 들어 마일스톤, 날짜, [!UICONTROL 기준선], 또는 [!UICONTROL 완료율] 다음에 표시 [!UICONTROL 간트 차트].

     자세한 내용은   [에 정보가 표시되는 방식 구성 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > 할당은에 표시되지 않습니다. [!UICONTROL 간트 차트] 다음과 같은 경우 [!UICONTROL 간트 차트] 은(는) PDF으로 내보냅니다. 다음의 경우 [!UICONTROL 간트 차트] 을 PDF으로 내보내면 목록 보기에만 할당이 표시됩니다.

   * 다음에 표시되는 기간 [!UICONTROL 간트 차트].\

     자세한 내용은 [에서 정보 보기 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     내보내기 파일에 기간이 표시되는 방식은 선택 여부에 따라 다릅니다 **[!UICONTROL 내가 보는 항목]** 또는 **[!UICONTROL 여러 페이지]** 을 참조하십시오.

1. (선택 사항) 내보낸 PDF에 특정 작업만 포함하려면 포함할 작업을 선택합니다.

   작업을 선택하지 않으면 내보낸 PDF에 모든 작업이 포함됩니다.

   예를 들어 다음을 보는 경우 [!UICONTROL 간트 차트] 50개의 작업이 들어 있지만 내보낸 작업에는 10개의 작업만 표시하려는 프로젝트의 경우 [!UICONTROL 간트 차트]표시할 10개의 작업을 선택합니다.

1. 프린터 아이콘을 클릭합니다.\
   다음 **[!UICONTROL PDF으로 내보내기]** 대화 상자가 표시됩니다.\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 표시된 내용만 내보낼지 전체 내보낼지 선택 [!UICONTROL 간트 차트]:

   * **[!UICONTROL 내가 보는 항목]:** 최대 500개의 항목을 내보내기 전에 화면에 표시되는 모든 작업(하위 작업 포함)을 내보냅니다. (이것이 다음에 표시되는 항목이 아닙니다.) **[!UICONTROL 미리 보기]** 섹션; [!UICONTROL 미리 보기] 섹션에는 샘플 데이터만 포함됩니다.)

     상위 작업이 축소되고 하위 작업이 표시되지 않는 경우에도 하위 작업이 내보낸 PDF에 포함됩니다. 상위 작업만 포함하려면 포함하려는 상위 작업을 선택하고 하위 작업은 선택하지 않은 상태로 두십시오.

     다음을 사용할 수 있습니다. **[!UICONTROL 확대/축소]** 드롭다운 메뉴 또는 슬라이더 도구를 사용하여 [!UICONTROL 간트 차트]에 설명된 대로 [에서 정보 보기 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 여러 페이지]:** 전체 내보내기 [!UICONTROL 간트 차트], 최대 500개 항목이 현재 화면에 표시되지 않습니다.\

     다음을 사용할 수 있습니다. **[!UICONTROL 확대/축소]** 드롭다운 메뉴 또는 슬라이더 도구를 사용하여 각 페이지에 표시되는 정보의 양을 결정합니다( 설명 참조) [에 정보가 표시되는 방식 구성 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 내보낼 페이지를 더 많이 표시하려면 더 세분화된 옵션을 선택하고, 내보낼 페이지를 더 적게 표시하려면 더 세분화된 옵션을 선택합니다.

     >[!NOTE]
     >
     >를 내보내야 하는 경우 [!UICONTROL 간트 차트] 500개가 넘는 항목을 포함하는 경우 [!UICONTROL 간트 차트] 따라서 500개 이하의 항목 또는 250개 페이지가 표시됩니다. 필터를 적용하는 방법에 대한 자세한 내용은 다음을 참조하십시오.  [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >다음과 같은 경우에는 전체 간트 차트를 내보낼 수 없습니다.
     >
     >   
     >   
     >   * 250페이지를 초과하는 경우
     >   * 항목이 500개를 초과하는 경우




1. PDF으로 내보낸 후 PDF을 인쇄하는 경우에서 **[!UICONTROL 페이지 크기]** 드롭다운 메뉴에서 인쇄할 용지 크기를 선택합니다.\
   다음을 선택할 수 있습니다. **[!UICONTROL 레터]**, **[!UICONTROL 리걸]**, **[!UICONTROL 원장]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (일부 언어에서만 사용 가능) 또는 **[!UICONTROL A4]**.
1. 다음에서 **[!UICONTROL 페이지 방향]** 섹션에서 PDF을 가로 방향으로 내보내거나 세로 방향으로 내보낼지 선택합니다.
1. 선택 **[!UICONTROL 범례 표시]** 내보낸 PDF에 범례를 포함하려는 경우.
1. 클릭 **[!UICONTROL 내보내기]**.

   의 pdf [!UICONTROL 간트 차트] 이 만들어지고 컴퓨터에 다운로드됩니다.

   내보낸 파일의 아래쪽에 범례가 있습니다. 에서 활성화한 옵션만 설명합니다. [!UICONTROL 간트 차트] 작업 목록에서 사용할 수 있습니다.

   예를 들어 마일스톤은 마일스톤과 연관된 작업이 하나 이상 있는 경우에만 범례에 표시됩니다.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
