---
product-area: reporting
navigation-topic: text-mode-reporting
title: 조건부 서식의 필드 비교
description: 조건부 서식을 사용하여 한 보기에서 두 개의 다른 필드를 비교하고 필드 간에 특정 기준이 충족될 때 강조 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 조건부 서식의 필드 비교

조건부 서식을 사용하여 한 보기에서 두 개의 다른 필드를 비교하고 필드 간에 특정 기준이 충족될 때 강조 표시할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서의 보기를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 보기를 편집합니다</p> <p>보기에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 예: 실제 시작 일자와 계획 시작 일자 비교

예를 들어 작업의 실제 시작 날짜가 계획 시작 날짜 이후인 경우 조건부 서식을 사용하여 계획 시작 날짜 열을 강조 표시할 수 있습니다.

조건부 서식을 사용하여 작업의 계획 시작 날짜와 실제 시작 날짜를 비교하려면

1. 작업 보기 또는 보고서로 이동합니다.
1. (조건부) 보고서 작업을 하는 경우&#x200B;**열(보기)** 탭에서 조건부 서식을 지정할 열의 헤더를 클릭하여 선택합니다.\
   예를 들어, **실제 시작 날짜** 열(계획 시작 일자 및 실제 시작 일자 필드를 비교하여 조건부 서식을 추가하려면)

1. 클릭 **고급 옵션**&#x200B;를 클릭한 다음 추가 를 클릭합니다 **이 열에 대한 규칙**.

1. 빌더에 있는 기존 값을 사용하여 비교 기준을 입력하고 조건부 서식을 지정합니다.\
   예를 들어 실제 시작 날짜가 계획 시작 날짜보다 이전( 또는 이상)인 작업을 강조 표시하려고 합니다. 보다 큼 수정자를 선택하고 일자 필드에서 실제 일자를 선택합니다.\
     ![](assets/cond-format-1-350x84.png)

1. (선택 사항) 선택 **전체 행에 적용** 서식을 전체 행에 적용하려면
1. 클릭 **규칙 추가**, 그런 다음 **완료**.

1. 을(를) 선택합니다 **실제 시작 날짜** 열을 누른 다음 **텍스트 모드로 전환**.

1. **텍스트를 편집하려면 클릭하십시오.** 그런 다음 다음 텍스트 줄을 추가합니다.

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   이 예제에서는 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Workfront 기본 필드를 비교하는 경우 필드 이름에 카멜 사례 구문을 사용합니다. 사용자 지정 필드를 비교하는 경우 **DE:필드의 실제 이름** 이름 필드에 대해 첫 번째 필드와 비교할 수 있습니다.\
   >예를 들어 **실제 시작 날짜** 사용자 지정 필드에 **배달 날짜**&#x200B;를 채울 때 텍스트 모드 코드에 다음 문을 추가합니다.
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 다음을 확인합니다. `righttext` 코드 줄은 `rightmethod` 코드 줄.

   ![](assets/cond-format-2-350x171.png)

1. **저장**&#x200B;을 클릭합니다.
1. 클릭 **저장 + 닫기**.

   열에는 기준에 맞는 필드가 강조 표시됩니다.
