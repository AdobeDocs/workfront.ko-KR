---
title: 보고 캔버스에서 테이블 열 구성
description: 보고 캔버스에서 테이블 열 구성
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 2%

---


# 보고 캔버스에서 테이블 열 구성

테이블의 열을 표시하도록 구성할 수 있습니다. 열의 다음 측면을 수정할 수 있습니다.

* 이름
* 정렬
* 권한 편집
* 가리킨 텍스트
* 집계
* 조건부 서식

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 Beta: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 테이블의 열 수정

1. 기존 보고서로 이동하여 **기타 메뉴** 아이콘 ![](assets/more-icon.png) 보고서 헤더에서 를 선택합니다. **편집**.
1. 보고서의 표 머리글에서 **편집** 아이콘 ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >표를 만들었지만 아직 필드를 추가하지 않은 경우에는 표 중앙에 있는 편집 단추를 클릭하십시오.

1. (선택 사항) 테이블에서 열을 추가, 위치 변경 또는 삭제합니다. 테이블에서 필드를 편집하는 방법에 대한 자세한 내용은 [보고 캔버스에서 테이블 블록 추가 또는 편집](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | 새 열 추가 | 테이블에 열을 추가하려면 을(를) 클릭하고 **필드** 패널을 배치하려는 테이블의 페이지 오른쪽에 배치하거나 필드를 더블 클릭하여 맨 오른쪽 열로 추가합니다. |
   |---|---|
   | 열 이동 | 테이블의 열 순서를 재배열하려면 열 이름을 클릭하고 새 위치로 끕니다. |
   | 열 삭제 | 테이블에서 열을 삭제하려면 삭제할 열을 클릭한 다음 열 이름의 오른쪽에 있는 x를 클릭합니다. |

   {style="table-layout:auto"}

1. 열을 구성하려면 테이블의 헤더 행에서 수정할 열의 이름을 클릭한 다음 오른쪽 패널에서 다음 탭 중 하나를 누릅니다.

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">데이터 탭</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">다음을 기준으로 집계</td>
      <td><p> 열에 있는 정보를 집계(헤더에서 요약)하려면 <strong>다음을 기준으로 집계</strong> 드롭다운 메뉴. 사용 가능한 옵션은 열에 포함된 데이터 유형에 따라 다릅니다.</p><p>테이블에서 그룹을 사용하는 경우 집계된 값이 열 이름 옆에 표시되지 않고 열 이름 위의 그룹 행에 표시됩니다.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">필드 형식</td>
      <td><p>열에 텍스트가 아닌 날짜, 백분율, 통화 또는 시간 데이터가 포함된 경우에만 사용할 수 있습니다. 에서 데이터에 사용할 형식을 선택합니다. <b>필드 형식</b> 드롭다운. 예를 들어 열의 숫자 뒤에 퍼센트 기호를 표시하거나 날짜가 표시되는 방식을 변경할 수 있습니다.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">필드는 편집 가능합니다.</td>
      <td><span>활성화 <strong>필드는 편집할 수 있습니다.</strong> 표를 보는 사용자가 열의 이름을 편집할 수 있도록 하려면 을 선택합니다.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>정렬</strong></td>
      <td><p>기본적으로 테이블은 가장 왼쪽 열의 데이터에 따라 오름차순으로 정렬됩니다. 대신 선택한 열을 기준으로 정렬하려면 옆에 있는 아래쪽 화살표를 클릭합니다. <strong>정렬</strong>을 클릭한 다음 확인란을 클릭합니다 <b>이 열을 기준으로 정렬</b>. 그런 다음 을(를) 선택할 수 있습니다 <strong>정렬</strong> 방향(오름차순 또는 내림차순 값) 및 <strong>정렬 순서</strong> (테이블의 다른 정렬 열과 비교한 이 열의 상대적 정렬 우선 순위).</p><p>이 프로세스를 반복하여 테이블을 5개의 다른 열로 정렬할 수 있습니다. 각 열에 올바른 열이 있는지 확인합니다 <strong>정렬 순서</strong> 정렬하기 위해 선택한 새 열을 기준으로 합니다.</p><p>참고: 테이블을 정렬하기 위해 선택된 열을 삭제하고 다른 열도 정렬하기 위해 선택된 경우 해당 열을 사용하여 내림차순으로 테이블을 정렬합니다. 정렬을 위해 선택한 다른 열이 없는 경우 테이블은 기본값으로 돌아갑니다. 첫 번째 열을 기준으로 정렬합니다.</p><p>테이블을 정렬할 열을 지정하면 테이블 정렬 시 해당 열의 상대적 우선 순위를 나타내는 숫자(테이블이 먼저 1, 2로 정렬됨)와 정렬 방향이 오름차순인지 내림차순인지를 나타내는 화살표가 열 이름 옆에 작은 상자가 표시됩니다. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">스타일 탭</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 정의 열 레이블</strong> </td> 
      <td>열에 대한 새 표시 이름을 입력합니다(100자 제한).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">가리킨 텍스트 표시</td> 
      <td> <p>누군가가 열 이름 위로 마우스를 가져갈 때 설명 텍스트를 표시할지 여부를 결정합니다.</p> <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">가리킨 텍스트</td> 
      <td>(다음 경우에만 사용 가능) <strong>가리킨 텍스트 표시</strong> 이(가) 활성화되었습니다. 열 이름 위에 마우스 포인터를 놓으면 표시되는 설명 텍스트를 사용자 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>조건부 서식</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>추가 <img src="assets/add-rule.png">, 편집 <img src="assets/edit-icon.png">, 또는 삭제 <img src="assets/delete.png"> 값이 사용자가 지정한 기준을 만족할 때 열에서 셀 서식을 지정하는 규칙입니다.</p> <p>예를 들어 "프로젝트 상태" 필드의 값이 "작성 중"인 경우 해당 필드의 글꼴을 굵게 자주색으로 변경하는 규칙을 만들 수 있습니다.</p> <p>또는 <b>아이콘 표시</b> "현재" 상태인 열의 모든 항목에 녹색 플래그 아이콘을 추가합니다.</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>참고: 다음을 사용하는 경우 <strong>아이콘 표시</strong>다른 서식 지정 옵션은 사용할 수 없습니다.</p> <p>다음을 선택할 수 있습니다. <strong>전체 행에 적용</strong> 서식 지정이 규칙 조건을 충족하는 셀의 전체 행에 영향을 미치도록 하려면 다음을 수행합니다. 예를 들어 "기한" 열의 날짜 셀뿐만 아니라 해당 날짜가 발생하는 전체 행에 노란색 배경색을 적용하여 특정 날짜 이후에 만료되는 프로젝트를 강조 표시할 수 있습니다.</p> <p>팁: 규칙에 서식 옵션을 추가하면 결과 셀 서식이 <strong>미리 보기</strong> 패널 하단에서.</p> </li> 
        <li value="2">규칙을 추가하고 나면 <strong>저장</strong>.</li> 
        <li value="3"> <p>(선택 사항) <b>+ 규칙 추가</b> 를 클릭하여 동일한 열에 규칙을 추가합니다.</p> <p>테이블의 여러 조건부 서식 규칙은 다음 순서로 적용됩니다.</p> 
         <ul> 
          <li> <p>전체 행에 적용되는 규칙은 먼저 각 열에 대해 왼쪽에서 오른쪽으로 평가한 다음 열 내에서 위에서 아래로 평가합니다.</p> <p>참고: 행 서식은 다른 열 규칙의 조건을 충족하더라도 해당 행의 셀에 대한 다른 조건부 서식을 재정의합니다.</p> </li> 
          <li> <p>다른 규칙은 열의 오른쪽 패널에 나열되므로 위에서 아래로 평가됩니다. 드래그할 수 있습니다. <img src="assets/drag-object-icon.png"> 순서를 변경하기 위해 해당 패널에 규칙을 저장했습니다.</p> <p>참고: 셀의 서식은 첫 번째 조건을 기준으로 지정되며, 다른 조건을 만족하더라도 더 이상 서식이 지정되지 않습니다.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음을 클릭합니다. **돌아가기** 화면 왼쪽 상단 모서리에 있는 화살표를 클릭하여 보고서로 돌아갑니다.
