---
title: 보고 캔버스에서 막대 시각화 구성
description: 보고 캔버스에서 막대 시각화 구성
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# 보고 캔버스에서 막대 시각화 구성

막대 시각화는 가로 막대를 사용하여 중요한 정보를 강조 표시하여 데이터에 대한 스토리를 빠르게 전달하는 데 도움이 됩니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 베타: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)를 참조하십시오.

## 막대 시각화 구성

>[!NOTE]
>
>보고서에서 블록을 빌드하고 편집할 때 모든 변경 사항이 자동으로 저장됩니다.

1. [보고 캔버스에서 시각화 블록 추가 또는 편집](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md)에 설명된 대로 **막대** 시각화 유형을 사용하는 시각화 블록을 보고서에 추가합니다.

1. 시각화의 오른쪽 상단에 있는 시각화 편집 아이콘 ![](assets/edit-icon.png)을(를) 클릭한 후 다음 중 하나를 수행합니다.

   1. **설정** 탭에서:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">시각화 유형</td>
         <td><p>다른 유형의 시각화로 전환합니다. 이렇게 하면 메뉴의 후속 옵션이 변경될 수 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">세로 축</td>
         <td><p>막대 시각화의 세로 왼쪽 가장자리 또는 Y축을 따라 나타낼 데이터를 선택합니다. 시각화는 가로 축의 각 항목에 따라 이 축의 항목을 비교합니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">가로축</td>
         <td><p>왼쪽 드롭다운 메뉴에서 가로 또는 X축을 따라 표시할 데이터를 선택합니다. 이 축의 항목은 해당 값을 기준으로 비교 막대로 표시됩니다.</p><p>오른쪽 드롭다운 메뉴에서 시각화가 가로 축을 따라 값을 계산하고 표시할 방법을 선택합니다.</p>
          <ul>
           <li><p><b>Count</b>: 값의 수</p></li>
           <li><p><b>합계</b>: 모든 값의 합계 </p></li>
           <li><p><b>평균</b>: 모든 값의 평균</p></li>
           <li><p><b>최소</b>: 가장 낮은 값만</p></li>
           <li><p><b>최대값</b>: 가장 높은 값만</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ 값 추가</td>
         <td>가로 축을 따라 추적할 다른 필드를 추가합니다.</td>
        </tr>
       </tbody>
      </table>

   1. **데이터** 탭에서:

      | 데이터 소스(드롭다운 메뉴) | 시각화의 데이터 소스를 보고서 캔버스의 다른 테이블로 변경합니다. |
      |---|---|
      | 데이터 Source 표시 | 보고서 캔버스에 시각화에 대한 소스 테이블을 표시하려면 이 옵션을 활성화하고, 숨기는 옵션을 비활성화합니다. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 시각화 설정 메뉴 외부의 아무 곳이나 클릭하여 닫습니다.
