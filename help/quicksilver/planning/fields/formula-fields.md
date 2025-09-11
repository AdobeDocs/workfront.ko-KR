---
title: 공식 필드 개요
description: Adobe Workfront Planning에서 함수 및 기존 필드를 사용하여 새 사용자 정의 값을 계산하는 공식 필드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: d7af8c5888147e847b4e239b629373b4b72541f7
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 4%

---

# 공식 필드 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

기존 필드를 참조하고 수식 유형 필드에서 연결하여 Adobe Workfront Planning에서 사용자 정의 필드를 만들 수 있습니다.

공식 필드는 레코드 유형의 다른 필드에 있는 기존 값과 기존 값을 계산하는 방법을 나타내는 함수를 사용하여 새 값을 생성합니다.

자세한 내용은 문서 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)의 &quot;수식&quot; 섹션을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 제품</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류 </a>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr>

</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 공식 필드에 대한 고려 사항

* 공식 필드는 동일한 레코드 유형에 속하는 필드를 참조합니다.
* 다른 레코드 종류를 수식 필드를 만드는 레코드 종류에 연결하는 경우에만 다른 레코드 종류의 필드를 참조할 수 있습니다.
* 수식에서 연결된 레코드 종류 또는 조회 필드를 참조하는 것은 연결된 레코드 종류에 대한 사용 권한에 따라 다릅니다. 레코드 종류를 볼 수 있는 권한이 없으면 수식에서 해당 필드를 참조할 수 없습니다.
* 수식 필드를 저장한 후에는 수식 필드의 필드 유형을 변경할 수 없습니다.
* 배합표 필드를 저장한 후 배합표 필드의 계산을 갱신할 수 있으며, 계산 결과는 동일한 유형의 모든 레코드에 대해 자동으로 갱신됩니다.
* 수식에서 참조하는 필드가 Workfront Planning 인터페이스에 표시되는 대로 추가해야 합니다.
* 레코드 유형의 표 보기 또는 레코드 세부 정보 페이지에 표시되는 필드만 참조할 수 있습니다.
* 다음 형식 옵션 중에서 선택하여 공식 계산 값에 대한 형식을 정의할 수 있습니다.

   * 텍스트
   * 숫자
   * 비율
   * 통화
   * 태그
   * Date

  자세한 내용은 문서 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)의 &quot;수식&quot; 섹션을 참조하십시오.
* 새 수식에서 수식 필드를 참조할 수 있습니다. 공식 필드에서 참조되는 필드에서 값이 업데이트되면 해당 필드를 참조하는 모든 후속 필드 또는 해당 필드가 포함된 공식 필드가 자동으로 업데이트됩니다.

<div class="preview">

* 수식 필드 또는 수식 필드에 영향을 줄 수 있는 필드를 업데이트하면 경고가 변경 사항의 영향을 알려줍니다. 경고는 다음과 같은 경우에 표시됩니다.

   * 수식 필드를 업데이트할 때(이름 및 설명 변경 제외) 해당 필드에 종속 수식 또는 조회 필드가 있는 경우. 경고는 이러한 종속 필드를 나열하고 계속 진행할지 여부를 묻습니다.

   * 공식 표현식에서 또는 조회 필드로 사용되는 필드를 삭제할 때. 경고는 종속 수식 및 조회 필드를 나열하고 삭제를 계속할 것인지 여부를 묻습니다.

</div>



<div class="preview">

## 공식 필드의 제한 사항

* 하나의 레코드 유형에 최대 20개의 공식 필드를 추가할 수 있습니다.

  연결된 레코드 유형에서 추가된 수식 조회 필드는 이 제한에 포함되지 않습니다.

* 공식 표현식은 50,000자를 초과할 수 없습니다.

* 다음과 같은 경우 수식 필드가 `#ERROR!`(으)로 표시될 수 있습니다.
   * 수식에 사용된 필드가 삭제되는 경우.
   * 집계된 조회 필드에 사용된 필드가 `#ERROR!`(으)로 표시되는 경우.

     예를 들어 집계된 조회 수식 필드가 포함된 조회 필드를 표시하는 경우 참조된 수식 필드 중 하나가 `#ERROR!`(으)로 표시됩니다.
   * 수식 값을 선택한 형식으로 표시할 수 없는 경우입니다.

     예를들어 수식 필드의 형식으로 [숫자]를 선택하고 수식에 사용된 필드가 숫자가 아닌 텍스트 값만 표시하는 텍스트 필드인 경우 텍스트를 숫자로 구문 분석할 수 없으므로 수식 결과는 `#ERROR!`으로 표시됩니다.

</div>

## 지원되는 공식

Adobe Workfront Planning 공식 필드는 Workfront 계산된 필드의 대부분의 표현식을 지원합니다.

>[!NOTE]
>
>다음 Workfront 표현식은 Workfront Planning 공식 필드에서 지원되지 않습니다.
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* 전환
>* 형식

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Workfront 식의 전체 목록을 보려면 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

또한 Workfront Planning 공식 필드에 대해 다음 표현식을 지원합니다. 다음 표현식은 Workfront 표현식에 지원되지 않습니다.

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>표현식</th> 
   <th>설명 및 예제</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>구분 기호로 연결된 문자열을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>ARRAYJOIN(구분 기호,배열)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>고유한 값이 있는 배열을 반환합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>ARRAYUNIQUE(배열)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>레코드의 ID를 반환합니다. 각 레코드에는 고유한 ID가 있습니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>제공된 JSONPath로 JSON의 데이터를 반환합니다. JSONPath가 JSON에 존재하지 않으면 빈 결과가 반환됩니다. </p> <p>표현식의 형식은 다음과 같습니다.
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>날짜 및 시간의 시간대를 특정 시간대로 설정합니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>1년의 주 수를 반환합니다. 선택적으로 주가 시작되는 요일을 지정할 수 있습니다(일요일은 1, 월요일은 2 사용). 생략하면 기본적으로 주가 일요일에 시작됩니다.</p> <p>표현식의 형식은 다음과 같습니다.

<code>WEEKOFYEAR(date,2)</code>
또는
<code>WEEKOFYEAR(일자)</code>
</p>
   </td></tr>

</table>
