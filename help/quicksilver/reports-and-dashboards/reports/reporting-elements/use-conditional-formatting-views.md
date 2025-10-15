---
product-area: reporting
navigation-topic: reporting-elements
title: 보기에서 조건부 서식 사용
description: Adobe Workfront의 다른 사용자와 보고서를 공유할 때 특정 정보를 더 쉽게 읽거나 눈에 띄도록 보고서 보기를 사용자 지정하는 것이 좋습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 3%

---

# 보기에서 조건부 서식 사용

<!-- Audited: 11/2024 -->

Adobe Workfront의 다른 사용자와 보고서를 공유할 때 특정 정보를 더 쉽게 읽거나 눈에 띄도록 보고서 보기를 사용자 지정하는 것이 좋습니다.

보고서 보기에 특수 또는 조건부 서식을 추가하여 보고서의 세부 정보 탭을 사용자 지정할 수 있습니다.

보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

보고서 보기에서 열 서식을 조건부로 지정하여 보고서 표시 방식에 영향을 주는 규칙을 설정할 수 있습니다. 이러한 조건 또는 규칙이 충족되면 특수 서식이 적용됩니다.

예를 들어 작업 완료율이 20% 미만인 경우 백분율을 굵게, 빨간색 텍스트 및 노란색 배경색으로 표시하여 필드를 강조 표시할 수 있습니다.

조건부 서식의 보기를 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* 열의 헤더를 변경합니다.
* 열 값을 사용자 지정된 텍스트 또는 이미지로 변경합니다.
* 글꼴 유형, 색상, 정렬 또는 배경색을 변경하여 필드 표시 형식을 지정합니다.

보고서 보기에서 수행한 변경 사항은 보고서의 세부 정보 탭에서만 적용됩니다. 이러한 변경 사항은 보고서의 요약, 매트릭스 또는 차트 탭에 영향을 주지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</strong></td> 
   <td> 
    <p>보고서 보기에 대한 표준 또는 계획</p>
    <p>목록 보기에 대한 기여자 또는 요청</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 편집</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
    <td> <p>보고서에서 보기를 만들거나 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 권한 관리</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

조건부 서식을 해당 보기에 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)를 참조하십시오.

## 조건부 서식의 보기 만들기

{{step1-to-reports}}

1. 조건부 서식이 지정된 보기를 만들 보고서 이름을 클릭합니다

   또는

   **새 보고서**&#x200B;를 클릭한 다음 개체 유형을 선택하여 새 보고서를 작성하십시오.

1. (조건부) 기존 보고서를 편집하는 경우 **보고서 동작**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. **열(보기)** 탭에서 기존 열을 클릭하여 선택하거나 **열 추가**&#x200B;를 클릭하여 열을 만듭니다.
1. Report Builder의 왼쪽 위 모서리에 있는 **이 열에 표시** 필드에서 새 열에 표시할 필드를 선택합니다.
1. **고급 옵션**&#x200B;을 클릭합니다.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>사용자 정의 열 레이블</strong></td> 
      <td> <p>열의 이름을 지정합니다.</p> <p>기존 열을 편집하는 경우 여기에서 이름을 지정하면 기존 열 이름이 변경됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>필드 형식</strong></td> 
      <td>열에 있는 값이 표시되는 형식을 선택합니다. 열 필드에 따라 날짜, 숫자 또는 통화가 표시되는 방식을 설정할 수 있습니다. 일부 열에는 이 옵션이 표시되지 않습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>대시보드에 있을 때 이 열 표시</strong></td> 
      <td>보고서를 대시보드에 배치할 때 열을 표시하려면 이 필드를 선택합니다. 이 열은 대시보드 외부의 보고서를 볼 때 항상 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **이 열에 대한 규칙 추가**&#x200B;를 클릭합니다.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. **When the:** 섹션에서 열에 대한 조건문을 설정합니다.

   예: &quot;작업 완료율이 50(대/소문자 구분)인 경우&quot;
1. **다음과 같은 필드 표시:** 섹션에서 위에 정의된 조건이 충족될 때 이 필드의 모양을 지정합니다.

   다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>텍스트 색상</strong></td> 
      <td> <p>색상 선택기를 사용하여 텍스트가 표시되는 색상을 선택합니다.</p> <p><b>메모</b></p> <p> 필드에 하이퍼링크가 포함되어 있으면 텍스트 색상 선택이 이 필드에 적용되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 포맷</strong></td> 
      <td>텍스트를 굵게 표시할지 기울임체로 표시할지를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 정렬</strong></td> 
      <td>열 내에서 텍스트를 오른쪽, 가운데 또는 왼쪽으로 정렬할지 여부를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>배경</strong></td> 
      <td>색상 선택기를 사용하여 텍스트의 배경색을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>아이콘 표시</strong></td> 
      <td>이 열에 대한 실제 값 대신 아이콘을 표시하려면 16개의 아이콘 중에서 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 표시</strong></td> 
      <td> <p>이 열의 실제 값 대신 사용자 지정 레이블을 표시하려면 이 옵션을 선택합니다. 제공된 필드에 있는 값 대신 표시할 텍스트를 지정합니다.</p> <p><b>중요 사항</b></p> <p><strong>텍스트 표시</strong>를 선택하면 이 열의 텍스트를 인라인 편집할 수 없습니다.<br>또한 전임 작업 열에는 기본 제공 논리가 포함되어 있으므로 이 열의 값을 변경할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>전체 행에 적용</strong></td> 
      <td>선택한 열에만 설정을 적용하는 대신 전체 행에 설정을 적용하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **규칙 추가**&#x200B;를 클릭합니다.\
   동일한 열에 규칙을 추가하거나 다른 열에 규칙을 추가할 수 있습니다.

   규칙은 만들어진 순서대로 적용됩니다. 열 규칙이 동일한 셀의 행 규칙보다 우선하지만, 이러한 규칙은 결합되지만 서로 덮어쓰지는 않습니다.

   **예 1**

   먼저 프로젝트가 빌드 상태일 때 텍스트 색상이 자주색이고 굵게 표시되는 규칙을 만들 수 있습니다. 그런 다음 작업 이름이 비어 있지 않을 때 텍스트 색상이 빨간색이고 이탤릭체이며 배경색이 녹색이라는 두 번째 규칙을 만듭니다. 이 예제에서 다음 오류가 발생합니다.

   * 프로젝트 상태가 작성 중인 작업은 자주색 및 굵은 텍스트로 표시됩니다. 작업 이름이 비어 있지 않으면 작업도 녹색 배경이 표시됩니다.
   * 프로젝트 상태가 빌드가 아닌 다른 작업(작업 이름은 비어 있지 않음)은 녹색 배경과 함께 빨간색과 기울임꼴 텍스트로 표시됩니다.

   **예 2**

   프로젝트 계획 완료 일자 열에 전체 행에 영향을 주는 규칙을 생성하여 프로젝트가 취소될 경우(예: 프로젝트 상태가 정지일 경우) 배경을 회색으로 표시합니다. 그런 다음 프로젝트 계획 완료 일자가 오늘보다 적을 때(프로젝트가 늦어짐을 의미함) 배경이 빨간색으로 바뀌는 열 규칙을 만듭니다. 이 예에서는 취소된 프로젝트에 완료 일자가 늦은 경우 행의 다른 셀이 회색이더라도 해당 셀이 빨간색으로 나타납니다. 이 서식을 수정하려면:

   * 계획된 완료 일자에 대한 포맷을 편집하고 지연 프로젝트의 빨간색 배경에 대한 열 규칙을 삭제합니다.
   * 행 규칙과 동일한 형식의 열 규칙을 추가합니다(프로젝트 상태가 정지인 경우 회색 배경).
   * 지연 프로젝트의 빨간색 배경에 대한 열 규칙을 다시 추가합니다.
   * 규칙 및 보기를 저장할 때 빨간색 배경이 취소된 프로젝트에 적용되지 않습니다.

1. **저장**&#x200B;을 클릭합니다.
1. **저장 및 닫기**&#x200B;를 클릭합니다.\
   지정된 조건이 충족되는 경우 보고서에 형식 변경 사항이 표시됩니다.
