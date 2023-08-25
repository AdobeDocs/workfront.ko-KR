---
title: 보고 캔버스에서 파이 시각화 구성
description: 보고 캔버스에서 파이 시각화 구성
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---


# 보고 캔버스에서 파이 시각화 구성

파이 시각화를 사용하면 상대적인 비율을 나타내는 쐐기를 사용하여 원형 그래픽에 중요한 정보를 강조 표시하여 데이터에 대한 스토리를 빠르게 전달할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 Beta: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 파이 시각화 구성

>[!TIP]
>
>보고서에서 블록을 빌드하고 편집할 때 모든 변경 사항이 자동으로 저장됩니다.

1. 를 사용하여 시각화 블록을 추가하는 것부터 시작하십시오. **파이** 에 설명된 대로 보고서에 대한 시각화 유형 [보고 캔버스에서 시각화 블록 추가 또는 편집](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. 시각화 편집 아이콘 을 클릭합니다 ![](assets/edit-icon.png) 시각화의 오른쪽 상단 모서리에서 다음 중 하나를 수행합니다.

   1. 다음에서 **설정** 탭:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">시각화 유형</td>
         <td><p>다른 유형의 시각화로 전환합니다. 이렇게 하면 메뉴의 후속 옵션이 변경될 수 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">고정</td>
         <td>개별 웨지를 나타낼 데이터를 선택합니다.</td>
        </tr>
        <tr>
         <td role="rowheader">값</td>
         <td><p>왼쪽 드롭다운 메뉴에서 각 쐐기에 표시할 값을 선택합니다.</p><p>오른쪽 드롭다운 메뉴에서 표시에서 해당 값을 계산하는 방법을 선택합니다.</p>
          <ul>
           <li><p><b>카운트</b>: 값의 수</p></li>
           <li><p><b>합계</b>: 모든 값의 합계 </p></li>
           <li><p><b>평균</b>: 모든 값의 평균</p></li>
           <li><p><b>최소</b>: 가장 낮은 값만</p></li>
           <li><p><b>최대</b>: 가장 높은 값만</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. 다음에서 **데이터** 탭:

      | 데이터 소스(드롭다운 메뉴) | 시각화의 데이터 소스를 보고서 캔버스의 다른 테이블로 변경합니다. |
      |---|---|
      | 데이터 소스 표시 | 보고서 캔버스에 시각화에 대한 소스 테이블을 표시하려면 이 옵션을 활성화하고, 숨기는 옵션을 비활성화합니다. |

      {style="table-layout:auto"}

<!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 시각화 설정 메뉴 외부의 아무 곳이나 클릭하여 닫습니다.
