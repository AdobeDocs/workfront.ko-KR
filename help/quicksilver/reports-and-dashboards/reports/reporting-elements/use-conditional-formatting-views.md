---
product-area: reporting
navigation-topic: reporting-elements
title: 보기에서 조건부 서식 사용
description: Adobe Workfront의 다른 사용자와 보고서를 공유할 때 특정 정보를 더 쉽게 읽거나 눈에 띄도록 보고서 보기를 사용자 지정하는 것이 좋습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# 보기에서 조건부 서식 사용

Adobe Workfront의 다른 사용자와 보고서를 공유할 때 특정 정보를 더 쉽게 읽거나 눈에 띄도록 보고서 보기를 사용자 지정하는 것이 좋습니다.

보고서 보기에 특수 또는 조건부 서식을 추가하여 보고서의 세부 정보 탭을 사용자 지정할 수 있습니다.

보고서를 편집하고 보기에 특별한 서식을 추가하려면 보고서에 대한 관리 권한이 있어야 합니다.

보고서 만들기에 대한 자세한 내용은 문서 를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

보고서 보기에서 열 서식을 조건부로 지정하여 보고서 표시 방식에 영향을 주는 규칙을 설정할 수 있습니다. 이러한 조건 또는 규칙이 충족되면 특수 서식이 적용됩니다.

예를 들어 작업 완료율이 20% 미만인 경우 백분율을 굵게, 빨간색 텍스트 및 노란색 배경색으로 표시하여 필드를 강조 표시할 수 있습니다.

조건부 서식의 보기를 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* 열의 헤더를 변경합니다.
* 열 값을 사용자 지정된 텍스트 또는 이미지로 변경합니다.
* 글꼴 유형, 색상, 정렬 또는 배경색을 변경하여 필드 표시 형식을 지정합니다.

보고서 보기에서 수행한 변경 사항은 보고서의 세부 정보 탭에서만 적용됩니다. 이러한 변경 사항은 보고서의 요약, 매트릭스 또는 차트 탭에 영향을 주지 않습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>요청 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에서 보기를 만들거나 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

조건부 서식을 추가하기 전에 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 조건부 서식의 보기 만들기

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **보고서**.

1. 조건부 서식이 지정된 보기를 만들 보고서 이름을 클릭합니다.

   또는

   클릭 **보고서 작업**&#x200B;을 클릭한 다음 을 클릭합니다 **편집**.

1. (조건부) 보고서를 편집한 경우 기존 열을 선택하거나 새 열을 만듭니다.
1. 클릭 **고급 옵션**.

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
      <td>열에 있는 값이 표시되는 형식을 선택합니다. 열 필드에 따라 날짜, 숫자 또는 통화가 표시되는 방식을 설정할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>대시보드에 있을 때 이 열 표시</strong></td> 
      <td>보고서를 대시보드에 배치할 때 열을 표시하려면 이 필드를 선택합니다. 이 열은 대시보드 외부의 보고서를 볼 때 항상 표시됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **이 열에 대한 규칙 추가**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 다음에서 **다음의 경우:** 섹션에서 열에 대한 조건문을 설정합니다. 예를 들어 작업 완료율이 50(대/소문자 구분)인 경우입니다.
1. 다음에서 **다음과 같이 필드를 표시합니다.** 섹션은 위에 정의된 조건이 충족될 때 이 필드의 모양을 지정합니다.

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
      <td>텍스트를 굵게 표시할지 기울임체로 표시할지를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 정렬</strong></td> 
      <td>열 내에서 텍스트를 오른쪽, 가운데 또는 왼쪽으로 정렬할지 여부를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>백그라운드</strong></td> 
      <td>텍스트 배경색을 선택합니다. 8가지 색상이 있습니다</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>아이콘 표시</strong></td> 
      <td>이 열에 대한 실제 값 대신 아이콘을 표시하려면 16개의 아이콘 중에서 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>텍스트 표시</strong></td> 
      <td> <p>이 열의 실제 값 대신 사용자 지정 레이블을 표시하려면 이 옵션을 선택합니다. 제공된 필드에 있는 값 대신 표시할 텍스트를 지정합니다.</p> <p>중요: 선택 <strong>텍스트 표시</strong> 이 열의 텍스트를 인라인 편집하는 기능을 비활성화합니다.<br>또한 [전임 작업] 열에는 기본 제공 논리가 포함되어 있으므로 이 열의 값을 변경할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>전체 행에 적용</strong></td> 
      <td>선택한 열에만 설정을 적용하는 대신 전체 행에 설정을 적용하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **규칙 추가**.\
   동일한 열에 규칙을 추가하거나 다른 열에 규칙을 추가할 수 있습니다.

   규칙은 만들어진 순서대로 적용됩니다. 열 규칙이 동일한 셀의 행 규칙보다 우선하지만, 이러한 규칙은 결합되지만 서로 덮어쓰지는 않습니다.

   예 1: 먼저 프로젝트 상태가 건물일 때 텍스트 색상이 자주색이고 굵은 글꼴인 규칙을 만들 수 있습니다. 그런 다음 작업 이름이 비어 있지 않고 텍스트 색상이 빨간색이며 기울임꼴이고 배경색이 녹색인 두 번째 규칙을 만듭니다. 이 예제에서 다음 오류가 발생합니다.

   * 프로젝트 상태가 작성 중인 작업은 자주색 및 굵은 텍스트로 표시됩니다. 작업 이름이 비어 있지 않으면 작업도 녹색 배경이 표시됩니다.
   * 프로젝트 상태가 빌드가 아닌 다른 작업(작업 이름은 비어 있지 않음)은 녹색 배경과 함께 빨간색과 기울임꼴 텍스트로 표시됩니다.

   예 2: 프로젝트 계획 완료 일자에 프로젝트가 취소될 경우 배경이 회색으로 바뀌는 전체 행에 영향을 주는 규칙을 만듭니다(상태 = &quot;중단&quot;). 그런 다음 프로젝트 계획 완료 일자가 오늘보다 적은 경우(프로젝트가 늦어짐을 의미함) 배경을 빨간색으로 바꾸는 열 규칙을 만듭니다. 이 예에서는 취소된 프로젝트에 완료 일자가 늦은 경우 행의 다른 셀이 회색이더라도 해당 셀이 빨간색으로 나타납니다. 이 서식을 수정하려면:

   * 계획된 완료 일자에 대한 포맷을 편집하고 지연 프로젝트의 빨간색 배경에 대한 열 규칙을 삭제합니다.
   * 행 규칙과 동일한 형식의 열 규칙을 추가합니다(프로젝트 상태가 &quot;중단&quot;일 때 회색 배경).
   * 지연 프로젝트의 빨간색 배경에 대한 열 규칙을 다시 추가합니다.
   * 규칙 및 보기를 저장할 때 빨간색 배경이 취소된 프로젝트에 적용되지 않습니다.


1. 클릭 **완료**.
1. 클릭 **저장 + 닫기**.\
   지정된 조건이 충족되는 경우 보고서에 형식 변경 사항이 표시됩니다.
