---
title: 보고 캔버스에서 테이블 필터링
description: 보고 캔버스에서 테이블 필터링
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# 보고 캔버스에서 테이블 필터링

보고서에 테이블 블록을 추가하면 테이블에 표시되는 정보를 제한하는 필터를 설정할 수 있습니다.

필터 규칙에는 다음과 같은 3가지 구성 요소가 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">필드</td> 
   <td> <p>테이블을 필터링하려는 정보가 포함된 필드입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">연산자</td> 
   <td> <p>필터에 따라 테이블에 포함되거나 제외되는 필드 값이 결정됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">값</td> 
   <td> <p>선택한 필드 내의 값이 연산자에 따라 평가됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

**예:** Jane Doe가 소유한 프로젝트만 표시하도록 보고서의 결과를 제한하려는 경우, &quot;프로젝트 소유자&quot;, &quot;같음&quot; 연산자 및 &quot;Jane Doe&quot; 값이 있는 필터 규칙을 만들 수 있습니다.

또는 &quot;프로젝트 소유자&quot; 필드와 &quot;비어 있지 않음&quot; 연산자가 있는 할당된 프로젝트 소유자만 표시할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 베타: 개요](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 테이블에 대한 필터 규칙 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고&#x200B;**보고**.

1. 클릭 **새 보고서**.

   또는

   기존 보고서로 이동하여 **추가 메뉴** 아이콘 ![](assets/more-icon.png) 보고서 헤더에서 **편집**.

1. 새 테이블의 행을 그룹화하려면 테이블 블록을 캔버스로 드래그하거나 두 번 클릭합니다.

   또는

   기존 테이블의 행을 그룹화하려면 **편집** 아이콘 ![](assets/edit-icon.png) 테이블 헤더에서 을 참조하십시오.

1. 오른쪽 패널에서 테이블을 필터링할 필드를 찾은 다음 필터 섹션으로 드래그합니다.

   필터 규칙 세트가 선택한 필드의 이름과 함께 표시됩니다.

1. 드롭다운 메뉴에서 원하는 연산자를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>같음</strong> </td> 
      <td> <p>이렇게 하면 검색된 값과 정확히 일치하는 항목만 반환됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>같지 않음</strong> </td> 
      <td> <p>검색된 값과 정확히 일치하지 않는 결과만 반환합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>비어 있음</strong> </td> 
      <td> <p>객체에 대한 필드가 있지만 필드에 값이 아직 지정되지 않았습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>비어 있지 않음</strong> </td> 
      <td> <p>필터링하는 필드가 존재하며 값이 제공되었습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>보다 작음</strong> </td> 
      <td> <p>입력한 값을 포함하지 않고 입력한 값보다 작은 값을 가진 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작거나 같음</strong> </td> 
      <td> <p>입력한 값보다 작거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>보다 큼</strong> </td> 
      <td> <p>입력한 값을 포함하지 않고 입력한 값보다 큰 값을 가진 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>크거나 같음</strong> </td> 
      <td> <p>입력한 값보다 크거나 같은 값이 있는 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사이</strong> </td> 
      <td> <p>두 개의 필수 필드 값을 제공하고 입력한 값을 포함하여 두 필드 범위 내의 모든 결과를 검색합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>포함:</strong> </td> 
      <td> <p>전체 텍스트 문자열 전체에서 지정된 텍스트를 검색합니다.</p> <p>예를 들어, "Contains Inf"를 사용하면 "Infinity"와 같이 "Inf" 또는 "inf"가 포함된 모든 것을 캡처합니다.</p> <p>참고: Adobe Workfront은 각 필터 규칙에 대해 입력하는 전체 단어 또는 구를 검색합니다. 예를 들어 이름이 "새 프로젝트"인 필드를 검색하는 경우, Workfront은 이름에 "new" 또는 "project"만 있는 프로젝트를 표시하지 않거나 "새 기본 프로젝트"와 같이 사이에 추가 단어가 포함된 구문을 표시하지 않습니다. 이 필터는 이름에 "새 프로젝트" 구문을 정확히 사용하는 프로젝트만 찾습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>포함하지 않음</strong> </td> 
      <td> <p>지정된 텍스트가 누락된 항목을 필터링합니다.</p> <p>예를 들어 "inf 포함하지 않음"은 해당 이름에 "Inf" 또는 "inf"가 없는 필드를 반환합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 선택한 연산자에 따라 필터 규칙을 완성할 마지막 값을 입력합니다.

   >[!NOTE]
   >
   >여기에 입력한 값은 다음과 같습니다 **not** 대/소문자를 구분합니다.

1. (선택 사항) 규칙 세트에 다른 필터 규칙을 추가하려면 다음을 수행합니다.

   1. 다른 필드를 **다른 규칙을 추가하려면 을 드롭합니다.** 영역에서 다른 규칙 아래의 필터 섹션을 참조하십시오.
   1. 4-6단계를 반복합니다.
   1. 새 규칙의 왼쪽에 있는 연산자 드롭다운에서 를 선택합니다. **및** 또는 **또는**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>및</p> </td> 
         <td> <p>필터 규칙이나 규칙 세트를 AND 연산자로 조인할 때 동일한 수준의 모든 규칙을 충족하도록 지정합니다.</p> <p>기본적으로 필터의 문은 AND 연산자로 연결됩니다.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>또는</p> </td> 
         <td> <p>필터 규칙이나 규칙 세트를 OR 연산자로 조인할 때 원하는 것을 나타냅니다 <strong>적어도</strong> 충족할 해당 레벨에서 하나의 규칙 또는 규칙 세트.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >규칙 세트 내의 여러 규칙 또는 전체 규칙 세트를 함께 연결하는 동일한 수준의 AND 및 OR 연산자는 항상 일치합니다. 예를 들어, 규칙 세트 내의 두 규칙 간에 연산자를 변경하면, 해당 규칙 세트의 다른 모든 연산자가 자동으로 변경되며,

1. (조건부) 필터 규칙 세트를 더 추가하려면 다음을 수행합니다.

   1. 추가할 필드를 **규칙 세트 추가** 다른 필터 규칙 세트 아래의 영역입니다.
   1. 4-7단계를 반복합니다.
   1. 새 규칙 세트의 왼쪽에 있는 연산자 드롭다운에서 를 선택합니다 **및** 또는 **또는**. 이러한 연산자는 7단계에 나열된 연산자와 동일하게 작동하지만 집합 내의 개별 규칙과 반대로 전체 규칙 세트에 적용됩니다.****
