---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: 비즈니스 규칙 만들기 및 편집
description: 비즈니스 규칙을 사용하면 Workfront 객체에 검증을 적용하고 특정 조건이 충족될 때 사용자가 객체를 생성, 편집 또는 삭제하지 못하도록 할 수 있습니다. 비즈니스 규칙을 사용하면 데이터 무결성을 손상시킬 수 있는 작업을 방지하여 데이터 품질과 운영 효율성을 향상시킬 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: f9c2c7192254a0d0c04056bc4c193eb35d4116b5
workflow-type: tm+mt
source-wordcount: '1820'
ht-degree: 4%

---

# 비즈니스 규칙 만들기 및 편집

비즈니스 규칙을 사용하면 Workfront 객체에 검증을 적용하고 특정 조건이 충족될 때 사용자가 객체를 생성, 편집 또는 삭제하지 못하도록 할 수 있습니다. 비즈니스 규칙 유효성 검사는 데이터 무결성을 손상시킬 수 있는 작업을 방지하여 데이터 품질과 운영 효율성을 개선하는 데 도움이 됩니다.

Workflow Ultimate 패키지가 있는 조직은 특정 조건이 충족될 때 작성, 편집 또는 수정된 오브젝트에 대한 작업을 자동화하도록 비즈니스 규칙을 구성할 수도 있습니다. 사용 가능한 작업에는 오브젝트 공유 또는 오브젝트에 사용자 정의 양식 첨부 등이 포함됩니다.


단일 비즈니스 규칙은 하나의 객체에만 할당할 수 있습니다. 예를 들어 특정 조건에서 프로젝트를 편집하지 않는 비즈니스 규칙을 만드는 경우 동일한 규칙을 작업에 적용할 수 없습니다. 작업에 대해 동일한 조건으로 별도의 비즈니스 규칙을 만들어야 합니다.

사용자가 오브젝트와 상호 작용할 때 액세스 수준 및 오브젝트 공유는 비즈니스 규칙보다 우선 순위가 높습니다. 예를 들어, 사용자에게 프로젝트 편집을 허용하지 않는 액세스 수준 또는 권한이 있는 경우, 이러한 권한은 특정 조건에서 프로젝트 편집을 허용하는 비즈니스 규칙보다 우선합니다.

객체에 둘 이상의 비즈니스 규칙이 적용되면 모든 규칙이 준수되지만 특정 순서로 적용되지 않습니다. 예를 들어 두 가지 비즈니스 규칙이 있습니다. 하나는 2월의 경비 만들기를 제한합니다. 두 번째는 프로젝트 상태가 완료일 때 프로젝트를 편집할 수 없도록 합니다. 사용자가 6월에 완료된 프로젝트에 경비를 추가하려고 하면 두 번째 규칙을 트리거했기 때문에 경비를 추가할 수 없습니다.

비즈니스 규칙은 API와 Workfront 인터페이스를 통해 개체를 만들고, 편집하고, 삭제하는 데 적용됩니다.

>[!NOTE]
>
>비즈니스 규칙은 특정 작업을 차단하므로 항상 샌드박스 또는 미리보기 환경에서 비즈니스 규칙을 먼저 구성하고 철저하게 테스트한 후 프로덕션에서 활성화해야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront 패키지
   </td>
   <td> <p>비즈니스 규칙 유효성 검사:<ul><li><p>Ultimate</p></li><li>
    <p>워크플로 얼티밋</p></li></ul></p><p>비즈니스 규칙 자동화:<ul><li>
    <p>워크플로 얼티밋</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>표준</td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr>  
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 비즈니스 규칙 시나리오

* [비즈니스 규칙 유효성 검사 시나리오](#scenarios-for-business-rule-validation)
* [비즈니스 규칙 자동화를 위한 시나리오](#scenarios-for-business-rule-automation)

### 비즈니스 규칙 유효성 검사 시나리오

비즈니스 규칙 유효성 검사 형식은 &quot;정의된 조건이 충족되는 경우 사용자가 오브젝트에 대한 작업을 수행할 수 없게 되며 메시지가 표시됩니다.&quot;입니다.

비즈니스 규칙의 속성 및 기타 함수 구문은 사용자 정의 양식의 계산된 필드 구문과 동일합니다. 구문에 대한 자세한 내용은 [양식 디자이너를 사용하여 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

IF 문에 대한 자세한 내용은 계산된 사용자 지정 필드의 [&quot;IF&quot; 문 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) 및 [조건 연산자](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)를 참조하십시오.

사용자 기반 와일드카드에 대한 자세한 내용은 [사용자 기반 와일드카드를 사용하여 보고서 일반화](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)를 참조하십시오.

날짜 기반 와일드카드에 대한 자세한 내용은 [날짜 기반 와일드카드를 사용하여 보고서 일반화](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)를 참조하십시오.

API 와일드카드는 비즈니스 규칙에서도 사용할 수 있습니다. `$$ISAPI`을(를) 사용하여 API에서만 규칙을 트리거합니다. `!$$ISAPI`을(를) 사용하여 사용자 인터페이스에서만 규칙을 적용하고 사용자가 API를 통해 규칙을 무시할 수 있도록 합니다.

* 예를 들어 이 규칙은 사용자가 API를 통해 완료된 프로젝트를 편집할 수 없도록 합니다. 와일드카드가 사용되지 않은 경우 규칙은 사용자 인터페이스와 API 모두에서 작업을 차단합니다.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

`$$BEFORE_STATE` 및 `$$AFTER_STATE` 와일드카드는 편집 전후에 개체의 필드 값에 액세스하는 데 표현식에 사용됩니다.

* 이러한 와일드카드는 모두 편집 트리거에 사용할 수 있습니다. 편집 트리거의 기본 상태(식에 상태가 포함되지 않은 경우)는 `$$AFTER_STATE`입니다.
* before 상태가 존재하지 않으므로 개체 만들기 트리거에서 `$$AFTER_STATE`만 허용합니다.
* after 상태가 존재하지 않으므로 개체 삭제 트리거에서는 `$$BEFORE_STATE`만 허용합니다.

몇 가지 간단한 비즈니스 규칙 시나리오는 다음과 같습니다.

* 2월 마지막 주 중에는 새 경비를 추가할 수 없습니다. 이 공식은 다음과 같이 명시될 수 있습니다.

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* 완료 상태인 프로젝트의 프로젝트 이름은 편집할 수 없습니다. 이 공식은 다음과 같이 명시될 수 있습니다.

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

시스템은 트리거당 개체당 하나의 비즈니스 규칙을 허용합니다. 예를 들어 문제에 대해 하나의 편집 트리거 규칙이 허용됩니다. 그러나 중첩된 IF 문이 있는 수식에 여러 규칙을 포함할 수 있습니다.

중첩된 IF 문이 있는 시나리오는 다음과 같습니다.

사용자는 완료된 프로젝트를 편집할 수 없으며 3월에 계획된 완료 일자가 있는 프로젝트를 편집할 수 없습니다. 이 공식은 다음과 같이 명시될 수 있습니다.

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

### 비즈니스 규칙에서 현지화 사용

조직에서 사용자 정의 현지화를 사용하는 경우 비즈니스 규칙에서 비즈니스 규칙 메시지의 번역을 활성화해야 합니다. 번역이 활성화되어 있지 않을 경우, 메시지 텍스트가 로컬라이제이션 목록에 있고 사용자의 브라우저가 적절한 언어로 설정되어 있더라도 메시지는 영어로 독자에게 표시됩니다.

규칙을 구성할 때 메시지 앞에 TRANSLATE라는 단어를 삽입하고 메시지를 괄호로 묶습니다.

>[!BEGINSHADEBOX]

예:

이 예제에서는 &quot;완료된 프로젝트를 편집할 수 없습니다&quot;라는 메시지가 설정의 현지화 영역에 포함되어 있고 사용자의 브라우저가 현지화된 언어로 설정되어 있다고 가정합니다.

* `IF({status} = "CPL", "You cannot edit completed projects.") `
메시지가 영어로 표시됩니다.
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
메시지가 현지화된 언어로 표시됩니다.

>[!ENDSHADEBOX]

사용자 지정 지역화에 대한 자세한 내용은 [사용자 지정 지역화 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md)을 참조하십시오.

## 비즈니스 규칙 자동화를 위한 시나리오

>[!NOTE]
>
>비즈니스 규칙 자동화를 사용하려면 조직에 Workflow Ultimate 패키지가 있어야 합니다.

비즈니스 규칙 자동화의 형식은 &quot;정의된 조건이 충족되면 선택한 자동화가 트리거됩니다&quot;입니다.

비즈니스 규칙 자동화 수식은 오류 메시지가 필요하지 않습니다

프로젝트가 생성될 때와 같이 선택한 객체와 작업이 발생할 때마다 자동화가 실행되도록 하려면 다음 공식을 사용합니다.

```
IF(true, true)
```

해당 프로젝트가 승인된 경우에만 프로젝트를 공유하려면 다음과 같은 공식을 사용합니다.

```
IF({status} = "APR", true)
```

[비즈니스 규칙 유효성 검사를 위한 시나리오](#scenarios-for-business-rule-validation) 섹션에 설명된 대로 비즈니스 규칙 작업에 와일드카드를 사용할 수 있습니다.


## 새 비즈니스 규칙 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 **비즈니스 규칙**&#x200B;을 클릭합니다.
1. **새 비즈니스 규칙**&#x200B;을 클릭합니다.

1. 규칙 빌더 대화 상자에서 비즈니스 규칙의 **이름**&#x200B;을(를) 입력하십시오.
1. **활성 상태임** 필드에서 규칙을 저장할 때 규칙을 활성화해야 하는지 여부를 선택합니다.

   **아니요**&#x200B;를 선택하면 규칙이 비활성 상태로 저장되며 나중에 활성화할 수 있습니다.

1. (선택 사항) 비즈니스 규칙의 **설명**&#x200B;과(와) 비즈니스 규칙을 적용할 때 수행할 작업을 입력합니다.


1. 비즈니스 규칙을 할당할 객체 유형을 선택합니다.

   ![개체 선택](assets/object-for-business-rule4.png)

   다음 객체에 비즈니스 규칙을 적용할 수 있습니다.

   * 프로젝트
   * 작업
   * 문제 / 요청
   * 포트폴리오
   * 문서
   * 프로그램
   * 경비
   * 회사
   * 반복
   * 청구 기록
   * 그룹
   * 비노동 리소스
   * 위험
   * 요율 카드
   * 할당
   * 사용자
   * 역할
   * 시간
   * 템플릿
   * 휴무
   * 리소스 풀
   * 작업 역할
   * 비노동 리소스 카테고리
   * 리소스 풀
   * 휴무
   * 시간
   * 직원 채용 플랜
   * 템플릿
   * 직원 채용 플랜 리소스
   <!--
   * <span class="preview">Team</span>
   -->

1. 비즈니스 규칙에 대한 **트리거**&#x200B;를 선택하십시오. 옵션은 다음과 같습니다.

   * **생성됨** 사용자가 개체를 만들려고 할 때 규칙이 적용됩니다.
   * **편집됨** 사용자가 개체를 편집하려고 할 때 규칙이 적용됩니다.
   * **삭제됨** 사용자가 개체를 삭제하려고 할 때 규칙이 적용됩니다.

1. 비즈니스 규칙 대화 상자의 중앙에 있는 공식 편집기에서 공식을 작성합니다.

   비즈니스 규칙의 형식은 &quot;정의된 조건이 충족되는 경우 사용자가 오브젝트에 대한 작업을 수행할 수 없게 되며 메시지가 표시됩니다.&quot;입니다.

   공식 영역에서 작성하는 비즈니스 규칙의 일부는 조건이며, 조건이 충족될 때 Workfront에 표시되는 메시지입니다.

   * &quot;객체&quot;는 비즈니스 규칙을 생성할 때 선택한 객체 유형입니다. 대화 상자의 머리글에 표시됩니다.
   * &quot;작업&quot;은 규칙에 대해 선택한 트리거입니다(객체 만들기, 편집 또는 삭제).
   * 개체와 작업이 이미 정의되어 있으므로 수식에 포함하지 않습니다.
   * 사용자 지정 오류 메시지는 규칙이 유효성 검사를 위한 경우에만 포함되며 비즈니스 규칙을 트리거할 때 사용자에게 표시됩니다. 무엇이 잘못되었는지, 어떻게 문제를 수정해야 하는지에 대한 명확한 지침을 제공해야 한다.

     오류 메시지에 정적 URL을 포함하여 설명서 또는 기타 유용한 페이지에 연결하여 규칙의 제한 사항 내에서 사용자가 작업을 수정하는 방법을 안내할 수 있습니다.

     이 예에서 &quot;자세히 알아보기&quot;는 URL에 연결됩니다. `"You are not allowed to add a new project in November.[Learn more](http://url)"` URL은 괄호로 묶어야 하지만 대괄호로 묶인 링크 텍스트는 필요하지 않습니다. 전체 URL을 표시할 수 있으며 클릭할 수 있는 링크가 됩니다.

   ![비즈니스 규칙 추가 대화 상자](assets/add-business-rule-new.png)

   이 예제는 프로젝트에 대한 비즈니스 규칙입니다. 현재 월이 11월인 경우 사용자는 새 프로젝트를 만들 수 없으며 이 메시지가 표시됩니다.

   비즈니스 규칙의 자세한 예는 이 문서에서 [비즈니스 규칙에 대한 시나리오](#scenarios-for-business-rules)를 참조하십시오.

1. (선택 사항) 규칙 작성을 지원하려면 오른쪽 패널의 **식** 및 **필드** 수식을 사용합니다.

   사용 가능한 항목 목록의 범위를 좁히려면 표현식 또는 필드를 검색합니다.

   사용 가능한 필드 목록은 비즈니스 규칙의 개체 유형과 관련된 필드로 제한됩니다.

1. (조건부) 작업을 확인하는 경우, 조직이 Workfront Ultimate 패키지에 있는 경우, 그 다음 영역에서 **개체 유효성 검사**&#x200B;를 선택합니다.

   다른 패키지의 경우 이 옵션을 미리 선택합니다.

1. (조건부) 다른 작업을 자동화하려면 작업을 선택합니다.

   이러한 작업에 대한 자세한 내용은 이 문서의 [비즈니스 규칙 자동화 옵션](#business-rule-automation-options) 섹션을 참조하십시오.

   >[!NOTE]
   >
   >유효성 검사 외에 작업을 사용하려면 조직이 Workflow Ultimate 패키지에 있어야 합니다. 이러한 다른 옵션이 표시되지 않으면 조직이 Workflow Ultimate 패키지에 없는 것입니다.

1. 비즈니스 규칙 작성을 마치면 **저장**&#x200B;을 클릭합니다.

>[!NOTE]
>
>비즈니스 규칙을 추가한 후에는 연결된 개체를 추가, 편집 또는 삭제하여 비즈니스 규칙을 테스트하여 규칙이 제대로 적용되었는지 확인해야 합니다.

### 비즈니스 규칙 자동화 옵션

>[!NOTE]
>
>유효성 검사 외에 작업을 사용하려면 조직이 Workflow Ultimate 패키지에 있어야 합니다. 이러한 다른 옵션이 표시되지 않으면 조직이 Workflow Ultimate 패키지에 없는 것입니다.

비즈니스 규칙이 트리거될 때 이러한 작업을 자동화하도록 설정할 수 있습니다. 사용 가능한 작업은 선택한 객체 유형에 따라 다릅니다.

| 자동화 | 추가 구성 |
|---|---|
| 사용자 정의 양식 첨부 | 추가할 사용자 정의 양식 선택 |
| 오브젝트 공유 | 개체를 공유할 사람, 역할, 그룹, 회사 또는 액세스 수준을 선택합니다. |

## 비즈니스 규칙 활성화

비즈니스 규칙이 비활성 상태이면 비즈니스 규칙 목록의 활성 상태 필드에 False가 표시됩니다. 목록 보기에서 규칙의 상태를 업데이트할 수 없습니다.

비즈니스 규칙을 활성화하려면 다음을 수행합니다.

1. 규칙 목록에서 비즈니스 규칙을 선택하고 편집 아이콘을 클릭합니다.
1. 비즈니스 규칙 대화 상자에서 **활성 상태임**&#x200B;에 대해 **예**&#x200B;를 선택합니다.
1. **저장**&#x200B;을 클릭합니다.
