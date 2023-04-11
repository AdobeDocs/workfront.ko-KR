---
product-area: reporting
navigation-topic: reporting-elements
title: 보기에서 조건부 서식 사용
description: 보고서를 Adobe Workfront의 다른 사용자와 공유할 때 보고서 보기를 사용자 지정하여 특정 정보를 보다 쉽게 읽거나 두드러지게 만드는 것이 좋습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 2%

---

# 보기에서 조건부 서식 사용

보고서를 Adobe Workfront의 다른 사용자와 공유할 때 보고서 보기를 사용자 지정하여 특정 정보를 보다 쉽게 읽거나 두드러지게 만드는 것이 좋습니다.

보고서 보기에 특수 또는 조건부 서식을 추가하여 보고서의 세부 사항 탭을 사용자 지정할 수 있습니다.

보고서를 편집하고 보기에 특수 서식을 추가하려면 보고서에 대한 관리 권한이 있어야 합니다.

보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

보고서 보기에서 조건부 열 서식을 지정하면 보고서 표시 방식에 영향을 주는 규칙을 설정할 수 있습니다. 이러한 조건 또는 규칙이 충족되면 특수 서식이 적용됩니다.

예를 들어 작업 완료율이 20% 미만인 경우 백분율 번호를 굵게, 빨간색, 노란색 배경색으로 표시하여 필드를 강조 표시할 수 있습니다.

조건부 서식 보기를 사용하면 다음 작업을 수행할 수 있습니다.

* 열의 헤더를 변경합니다.
* 열 값을 사용자 지정된 텍스트 또는 이미지로 변경합니다.
* 글꼴 유형, 색상, 정렬 또는 배경색을 변경하여 필드 표시 형식을 지정합니다.

보고서 보기에서 변경한 사항은 보고서의 세부 사항 탭에서만 적용됩니다. 이러한 변경 사항은 보고서의 요약, 매트릭스 또는 차트 탭에 영향을 주지 않습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 보기를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서에서 보기를 만들거나 편집합니다</p> <p>보기에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

조건부 서식을 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 조건부 서식 보기 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **보고서**.

1. 조건부 서식 보기를 만들 보고서의 이름을 클릭합니다.

   또는

   클릭 **보고서 작업**&#x200B;를 클릭한 다음 **편집**.

1. (조건부) 보고서를 편집한 경우 기존 열을 선택하거나 새 열을 만듭니다.
1. 클릭 **고급 옵션**.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>사용자 정의 열 레이블</strong></td> 
      <td> <p>열 이름을 지정합니다.</p> <p>기존 열을 편집하는 경우 여기에서 이름을 지정하면 기존 열 이름이 변경됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>필드 형식</strong></td> 
      <td>열의 값이 표시되는 형식을 선택합니다. 열 필드가 무엇인지에 따라, 날짜, 숫자 또는 통화 표시 방식을 설정할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>대시보드에 있을 때 이 열 표시</strong></td> 
      <td>보고서가 대시보드에 배치될 때 열을 표시하려면 이 필드를 선택합니다. 대시보드 외부에서 보고서를 보면 항상 열이 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **이 열에 대한 규칙 추가**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 에서 **설정:** 섹션에서 열에 대한 조건 문을 설정합니다. 예: 작업 완료 비율이 50인 경우(대/소문자 구분)
1. 에서 **다음과 같은 필드를 표시합니다.** 섹션에서 위에 정의된 조건이 충족될 경우 이 필드의 모양을 지정합니다.

   다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>텍스트 색상</strong></td> 
      <td> <p>텍스트가 표시되는 색상을 선택합니다. 8가지 색상이 있습니다</p> <p>참고: 필드에 하이퍼링크가 포함되어 있으면 텍스트 색상 선택이 이 필드에 적용되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 포맷</strong></td> 
      <td>텍스트를 굵게 또는 기울임체로 표시할지 여부를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 정렬</strong></td> 
      <td>텍스트를 열 내의 오른쪽, 가운데 또는 왼쪽에 맞춥니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>백그라운드</strong></td> 
      <td>텍스트의 배경색을 선택합니다. 8가지 색상이 있습니다</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>아이콘 표시</strong></td> 
      <td>이 열에 대한 실제 값 대신 아이콘을 표시하려면 16개의 아이콘 중 하나를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 표시</strong></td> 
      <td> <p>실제 값 대신 이 열에 대한 사용자 지정 레이블을 표시하려면 이 옵션을 선택합니다. 제공된 필드에 값 대신 표시할 텍스트를 지정합니다.</p> <p>중요 사항: 선택 <strong>텍스트 표시</strong> 이 열의 텍스트를 인라인 편집할 수 없도록 합니다.<br>또한 기본 제공 로직이 포함되어 있으므로 선행 행 열의 값을 변경할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>전체 행에 적용</strong></td> 
      <td>선택한 열에만 설정을 적용하지 않고 전체 행에 설정을 적용하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **규칙 추가**.\
   동일한 열에 규칙을 추가하거나 다른 열에 규칙을 추가할 수 있습니다.

   규칙은 만든 순서대로 적용됩니다. 열 규칙이 동일한 셀의 행 규칙보다 우선하지만 서로 결합되지만 덮어쓰지 않습니다.

   예제 1: 먼저 프로젝트 상태가 작성 중일 때 텍스트 색상이 보라색이고 굵게 표시되는 규칙을 만들 수 있습니다. 그런 다음 작업 이름이 비어 있지 않은 경우 텍스트 색상이 빨간색과 기울임꼴, 배경색이 녹색이라는 두 번째 규칙을 만듭니다. 이 예에서는 다음 경우가 발생합니다.

   * 프로젝트 상태가 작성 중인 작업은 자주색 및 굵은 텍스트로 표시됩니다. 작업 이름이 비어 있지 않으면 작업의 배경도 녹색으로 표시됩니다.
   * 프로젝트 상태가 작성 이외의 작업(및 작업 이름이 비어 있지 않음)인 작업은 녹색 배경이 있는 빨간색 기울임꼴 텍스트로 표시됩니다.

   예제 2: 프로젝트 계획 완료 일자에 전체 행에 영향을 주는 규칙을 생성하고, 프로젝트가 취소된 경우 백그라운드로 전환됩니다(상태 = &quot;중단&quot;). 그런 다음 프로젝트 계획 완료 일자가 오늘보다 작으면 백그라운드를 빨간색으로 변경하는 열 규칙을 만듭니다(즉, 프로젝트가 지연되었음을 의미합니다.). 이 예에서 취소된 프로젝트에 지연 완료 날짜가 있는 경우 행의 다른 셀이 회색으로 표시되더라도 해당 셀이 빨간색으로 표시됩니다. 이 서식을 수정하려면 다음을 수행합니다.

   * 계획 완료 일자에 대한 포맷을 편집하고 지연 프로젝트에서 빨간색 배경에 대한 열 규칙을 삭제합니다.
   * 행 규칙과 동일한 서식을 사용하는 열 규칙을 추가합니다(프로젝트 상태 = &quot;Dead&quot;일 때 회색 배경).
   * 지연 프로젝트에서 빨간색 배경에 대해 열 규칙을 다시 추가합니다.
   * 규칙과 보기를 저장하면 빨간색 배경이 취소된 프로젝트에 적용되지 않습니다.


1. 클릭 **완료**.
1. 클릭 **저장 + 닫기**.\
   보고서에서 사용자는 지정된 조건이 충족되는 경우 포맷의 변경 사항을 확인할 수 있습니다.
