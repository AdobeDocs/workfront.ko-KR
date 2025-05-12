---
title: 사용자 지정 Forms의 고급 논리 예
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 이 문서에서는 사용자 지정 필드에 대한 고급 논리를 작성하는 데 사용되는 표현식의 예를 제공합니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 01eeed1f73c47b79344ca60f3f6d866452cad140
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 사용자 정의 양식의 고급 논리 예

논리 규칙을 사용하면 사용자 정의 양식의 필드를 추가로 사용자 정의할 수 있습니다.

이 문서에서는 사용자 지정 필드에 대한 고급 논리를 작성하는 데 사용되는 표현식의 예를 제공합니다.

사용자 정의 양식에 논리를 추가하는 방법에 대한 자세한 내용은 [사용자 정의 양식 및 필드에 논리 규칙 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront 플랜 </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>사용자 정의 양식에 대한 관리 액세스 </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 유효성 검사 논리 예

유효성 검사 논리는 공식을 사용하여 작성되며, 논리를 필요한 만큼 단순하거나 복잡하게 만들 수 있습니다. 유효성 검사는 다른 필드의 값 또는 객체의 상태를 기반으로 할 수 있으며, 유효성 검사가 실패하는 경우에 대한 오류 메시지를 제공할 수 있습니다.

사용자가 사용자 정의 양식을 작성할 때 논리가 적용된 필드가 정의된 유효성 검사 조건을 충족하면 필드가 강조 표시되고 오류 메시지가 표시됩니다.

한 줄 텍스트, 단락, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 자동 완성, 날짜, 확인란 그룹 및 라디오 버튼과 같은 필드 유형에 유효성 검사 논리를 적용할 수 있습니다.

### 프로젝트 소유자만 &quot;Rush&quot; SLA을 선택할 수 있음

이 예에서 단일 선택 드롭다운 필드에는 SLA of Standard(14일, 우선순위 - 7일, 돌입 - 2일)에 대한 선택 사항이 있습니다.

유효성 검사 표현식:

```
IF({ownerID}!=$$USER&&{DE:DV - Dropdown - Control Dates}="2",CONCAT("Only ",{owner}.{name}," may select X Rush"))
```

프로젝트 소유자(시스템 관리자 포함)가 아닌 사용자가 **X Rush**&#x200B;을(를) 선택하려고 하면 오류가 표시됩니다.

![프로젝트 소유자인 Claire Stevens만 X Rush를 선택할 수 있습니다](assets/sla-xrush.png)

### 이전 필드의 선택에 따른 날짜 유효성 검사

SLA 예제를 계속 진행하여 이전 드롭다운 필드의 설정을 기반으로 유효성이 검사되는 날짜 필드를 추가할 수 있습니다.

유효성 검사 표현식:

```
IF({DE:DV - Date - Dropdown SLA}<ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates}),CONCAT("Earliest: ",ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates})))
```

허용된 날짜 이전의 날짜를 선택하면 메시지에 선택할 수 있는 가장 빠른 날짜가 표시됩니다.

![선택한 날짜는 3월 28일이지만 사용 가능한 날짜가 4월 3일](assets/date-validation-based-on-previous-choice.png)입니다.

### 재정의할 옵션이 있는 최소 문자 수

이 예제에서 최소 문자 수는 텍스트 필드에 적용되며 문자 수는 표시됩니다. 또한 별도의 확인란이 설정되어 문자 수에 대한 유효성 검사를 비활성화합니다.

유효성 검사 표현식:

```
IF({DE:DV - Override}!="Disable Validation"&&LEN({DE:DV - Text - Min Length})<"7",CONCAT(LEN({DE:DV - Text - Min Length})," characters / ",("7"-LEN({DE:DV - Text - Min Length}))," remaining"))
```

확인란을 선택하여 유효성 검사 시행을 재정의할 수 있습니다.

![유효성 검사를 사용하지 않도록 설정하는 확인란](assets/disable-validation-checkbox.png)

실행 중인 문자 수가 텍스트 필드에 포함됩니다.

![문자 개수 5개 사용 가능, 2개 남음](assets/running-character-count.png)

### 소유자만 편집할 수 있도록 필드 잠금

이 예제에서 필드는 프로젝트 소유자만 편집할 수 있습니다. 시스템 관리자라도 필드를 편집할 수 없습니다.

유효성 검사 표현식:

```
IF({ownerID}!=$$USER,IF(ISBLANK({ownerID}),"Project Owner will provide this.",CONCAT("Only ",{owner}.{name}," can edit this.")))
```

프로젝트 소유자가 아닌 사용자가 필드를 입력하려고 하면 프로젝트 소유자만 필드를 편집할 수 있다는 메시지가 표시됩니다.

![Claire Stevens만 이 필드를 편집할 수 있습니다](assets/only-project-owner-can-edit.png)

### 자동 완성 다른 필드 값을 기준으로 값을 허용하거나 거부합니다.

이 예제에서 자동 완성 필드는 양식의 다른 필드에 입력한 값을 기반으로 값을 동적으로 허용하거나 거부합니다.

유효성 검사 표현식:

```
IF({DE:DV - Text - Budget}>"10000",
   IF({DE:DV - TA User - by Budget}.{role}!="Director","Requires Director Approver")
)
```

예산 필드의 값이 $10,000 이상인 경우 자동 완성 구성에서 활성화된 역할 필터가 없더라도 자동 완성 기능에서 디렉터 역할이 있는 사용자만 선택할 수 있습니다.

![예산 금액에 디렉터 승인이 필요합니다](assets/budget-director.png)

### 입력 날짜로부터 10일 미만의 값 허용 안 함

이 예제에서는 입력 날짜로부터 10일 후의 값만 검증이 허용됩니다. 검증을 재정의하는 옵션(별도의 확인란 필드)도 공식에 포함되어 있으며 날짜 필드를 비워둘 수 있습니다.

유효성 검사 표현식:

```
IF({DE:DV - Override}!="Disable Validation"&&ISBLANK({DE:DV - Date - Deadline})!="true"&&{DE:DV - Date - Deadline}<ADDDAYS({entryDate},"10"),CONCAT("Earliest: ",ADDDAYS({entryDate},"10")))
```

입력 날짜로부터 10일 미만의 값이 유효성 검사를 트리거합니다.

![선택한 날짜는 3월 28일이지만 사용 가능한 가장 빠른 날짜는 4월 4일입니다](assets/earliest-deadline-date.png)

빈 값은 유효성 검사 메시지를 트리거하지 않습니다.

![날짜의 빈 값](assets/blank-date-allowed.png)

### 다중 선택 필드에 정확한/최소/최대 선택 적용

이 예에서 확인란 그룹과 같은 다중 선택 필드는 사용자가 특정 수의 옵션을 선택해야 합니다.

유효성 검사 표현식(정확히 두 개 선택):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick exactly 2},","))!="2","Pick Exactly 2 Options")
```

유효성 검사 표현식(최소 두 개 이상 선택):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick at least 2},","))<"2","Pick at least 2 choices")
```

유효성 검사 표현식(2개 이하로 선택):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick no more than 2},","))>"2","Pick no more than 2 choices")
```

올바른 수의 옵션을 선택하지 않으면 유효성 검사 오류가 표시됩니다.

![유효성 검사 오류 예](assets/min-max-selections.png)
