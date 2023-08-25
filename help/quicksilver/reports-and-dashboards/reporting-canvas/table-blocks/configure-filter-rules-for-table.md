---
title: 보고 캔버스에서 테이블 필터링
description: 보고 캔버스에서 테이블 필터링
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 2%

---


# 보고 캔버스에서 테이블 필터링

보고서에 테이블 블록을 추가한 후 필터를 설정하여 테이블에 표시되는 정보를 제한할 수 있습니다.

필터 규칙에는 3가지 구성 요소가 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">필드</td> 
   <td> <p>테이블을 필터링할 정보가 포함된 필드입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">연산자</td> 
   <td> <p>필터가 테이블에 포함되거나 제외되는 필드 값을 결정하는 방법입니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">값</td> 
   <td> <p>연산자에 따라 평가되는 선택한 필드 내의 값입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** Jane Doe가 소유한 프로젝트만 표시하도록 보고서의 결과를 제한하려면 필드 &quot;프로젝트 소유자&quot;, 연산자 &quot;같음&quot; 및 값 &quot;Jane Doe&quot;로 필터 규칙을 만들 수 있습니다.

또는 필드 &quot;프로젝트 소유자&quot;와 연산자 &quot;비어 있지 않음&quot;을 갖는 프로젝트 소유자가 할당된 프로젝트만 표시할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 Beta: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 테이블에 대한 필터 규칙 구성

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음&#x200B;**보고**.

1. 클릭 **새 보고서**.

   또는

   기존 보고서로 이동하여 **기타 메뉴** 아이콘 ![](assets/more-icon.png) 보고서 헤더에서 를 선택합니다. **편집**.

1. 새 테이블의 행을 그룹화하려면 테이블 블록을 캔버스로 드래그하거나 두 번 클릭합니다.

   또는

   기존 테이블의 행을 그룹화하려면 **편집** 아이콘 ![](assets/edit-icon.png) 테이블 머리글에서 사용할 수 있습니다.

1. 오른쪽 패널에서 테이블을 필터링할 필드를 찾은 다음 필터 섹션으로 드래그합니다.

   필터 규칙 세트가 선택한 필드의 이름으로 표시됩니다.

1. 드롭다운 메뉴에서 원하는 연산자를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>다음과 같음</strong> </td> 
      <td> <p>검색된 값의 정확한 일치만 반환합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>다음과 같지 않음</strong> </td> 
      <td> <p>검색된 값과 정확히 일치하지 않는 결과만 반환합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>비어 있음</strong> </td> 
      <td> <p>오브젝트에 대한 필드가 있지만 필드에 값이 아직 지정되지 않았습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>비어 있지 않음</strong> </td> 
      <td> <p>필터링 중인 필드가 존재하며 해당 필드에 값이 지정되었습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>다음보다 작음</strong> </td> 
      <td> <p>입력한 값을 포함하지 않고 입력한 값보다 작은 값을 갖는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작거나 같음</strong> </td> 
      <td> <p>입력한 값보다 작거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>다음보다 큼</strong> </td> 
      <td> <p>입력한 값을 포함하지 않고 입력한 값보다 큰 값이 있는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>다음보다 크거나 같음</strong> </td> 
      <td> <p>입력한 값보다 크거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사이</strong> </td> 
      <td> <p>2개의 필수 필드 값을 제공하고 입력한 값을 포함하여 두 필드 범위 내에서 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>다음을 포함함</strong> </td> 
      <td> <p>전체 텍스트 문자열에서 지정된 텍스트를 검색합니다.</p> <p>예를 들어 "Contains Inf"를 사용하면 "Infinity"와 같이 "Inf" 또는 "inf"가 포함된 모든 항목이 캡처됩니다.</p> <p>참고: Adobe Workfront은 각 필터 규칙에 대해 입력한 전체 단어 또는 구를 검색합니다. 예를 들어 이름에 "new project"라는 문구가 있는 필드를 검색하는 경우 Workfront은 이름에 "new" 또는 "project"만 있는 프로젝트 또는 "new main project"와 같이 그 사이에 추가 단어가 포함된 구문을 표시하지 않습니다. 필터는 이름에 "새 프로젝트"와 정확히 일치하는 구문이 있는 프로젝트만 찾습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>포함하지 않음</strong> </td> 
      <td> <p>지정된 텍스트가 누락된 항목을 필터링합니다.</p> <p>예를 들어 "inf를 포함하지 않음"은 이름에 "Inf" 또는 "inf"가 없는 필드를 반환합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 선택한 연산자에 따라 마지막 값을 입력하여 필터 규칙을 완료합니다.

   >[!NOTE]
   >
   >여기에 입력한 값은 다음과 같습니다 **아님** 대/소문자를 구분합니다.

1. (선택 사항) 규칙 세트에 다른 필터 규칙을 추가하려면 다음을 수행합니다.

   1. 다른 필드를 다음으로 드래그 **드롭하여 다른 규칙을 추가하세요** 필터 섹션의 다른 규칙 아래에 있는 영역입니다.
   1. 4~6단계를 반복합니다.
   1. 새 규칙의 왼쪽에 있는 연산자 드롭다운에서 를 선택합니다. **및** 또는 **또는**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>및</p> </td> 
         <td> <p>필터 규칙 또는 규칙 세트를 AND 연산자로 조인할 때 동일한 수준의 모든 규칙을 충족하도록 지정합니다.</p> <p>기본적으로 필터의 문은 AND 연산자로 연결됩니다.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>또는</p> </td> 
         <td> <p>OR 연산자로 필터 규칙 또는 규칙 세트를 조인할 때 원하는 것을 나타냅니다 <strong>최소</strong> 충족해야 할 해당 수준에서 하나의 규칙(또는 규칙 세트)이 있습니다.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >규칙 세트 내의 여러 규칙 또는 전체 규칙 세트를 함께 연결하는 동일한 레벨의 AND 및 OR 연산자는 항상 일치합니다. 예를 들어 규칙 세트 내의 두 규칙 간에 연산자를 변경하면 해당 규칙 세트의 다른 모든 연산자가 그에 일치하도록 자동으로 변경됩니다.

1. (조건부) 필터 규칙 세트를 추가하려면 다음을 수행합니다.

   1. 추가할 필드를 **규칙 세트 추가** 다른 필터 규칙 세트 아래의 영역입니다.
   1. 4~7단계를 반복합니다.
   1. 새 규칙 세트의 왼쪽에 있는 연산자 드롭다운에서 을 선택합니다. **및** 또는 **또는**. 이러한 연산자는 7단계에 나열된 연산자와 동일하게 작동하지만 세트 내의 개별 규칙이 아니라 전체 규칙 세트에 적용됩니다.****
