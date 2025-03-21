---
product-area: reporting
navigation-topic: text-mode-reporting
title: 조건부 서식의 필드 비교
description: 조건부 서식을 사용하여 보기에서 두 개의 서로 다른 필드를 비교하고 필드 간에 특정 기준이 충족될 때 해당 필드를 강조 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# 조건부 서식의 필드 비교

<!-- Audited: 1/2025 -->

조건부 서식을 사용하여 보기에서 두 개의 서로 다른 필드를 비교하고 필드 간에 특정 기준이 충족될 때 해당 필드를 강조 표시할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>플랜</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서의 보기를 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 예: 실제 시작 일자와 계획된 시작 일자 비교

예를 들어 작업의 실제 시작 일자가 계획된 시작 일자 이후인 경우 조건부 서식을 사용하여 계획된 시작 일자 열을 강조 표시할 수 있습니다.

조건부 서식을 사용하여 작업의 계획된 시작 일자와 실제 시작 일자를 비교하려면

1. 작업 보기 또는 보고서로 이동합니다.
1. (조건부) 보고서를 사용하는 경우 보고서 편집기의 **열(보기)** 탭에서 조건부 서식을 지정할 열의 헤더를 클릭하여 선택합니다.\
   예를 들어 계획된 시작 날짜와 실제 시작 날짜 필드를 비교하여 조건부 서식을 추가하려면 **실제 시작 날짜** 열을 선택합니다.

1. **고급 옵션**&#x200B;을 클릭한 다음 이 열에 대한 **규칙 추가**&#x200B;를 클릭합니다.

1. 빌더에 있는 기존 값을 사용하여 비교 기준을 입력하고 조건부 서식을 지정합니다.\
   예를 들어, 실제 시작 일자가 계획된 시작 일자보다 늦거나 큰 작업을 강조 표시하려고 합니다. 보다 큼 수정자를 선택하고 날짜 필드에서 실제 날짜를 선택합니다.

   ![실제 시작 날짜에 대한 조건부 서식](assets/cond-format-1-350x84.png)

1. (선택 사항) 전체 행에 서식을 적용하려면 **전체 행에 적용**&#x200B;을 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

1. **실제 시작 날짜** 열을 선택한 다음 **텍스트 모드로 전환**&#x200B;을 클릭합니다.

1. **텍스트 모드 편집**&#x200B;을 클릭한 후 다음 텍스트 행을 추가합니다.

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   이 예제에서는

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Workfront 네이티브 필드를 비교하는 경우 필드 이름에 카멜 대/소문자 구문을 사용하십시오. 사용자 지정 필드를 비교하는 경우 첫 번째 필드와 비교하는 이름 필드에 **DE:실제 필드 이름**&#x200B;을(를) 사용하십시오.\
   >예를 들어 **실제 시작 날짜**&#x200B;를 **배달 날짜**(으)로 레이블이 지정된 사용자 지정 필드와 비교하는 경우 텍스트 모드 코드에 다음 문을 추가하십시오.
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. `righttext` 코드 줄이 `rightmethod` 코드 줄의 문과 일치하는지 확인하십시오.

   ![조건부 서식](assets/cond-format-2-350x171.png)

1. **저장**&#x200B;을 클릭합니다.
1. **저장 및 닫기**&#x200B;를 클릭합니다.

   열에는 기준에 맞는 필드가 강조 표시됩니다.
