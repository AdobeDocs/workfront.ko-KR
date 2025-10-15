---
product-area: reporting
navigation-topic: text-mode-reporting
title: EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기
description: EXISTS 문을 사용하여 복잡한 텍스트 모드 필터를 만들 수 있습니다. 이 문서를 사용하려면 Adobe Workfront API 및 텍스트 모드 보고 인터페이스에 대한 철저한 이해가 필요합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2668'
ht-degree: 0%

---

# EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기

<!-- Audited: 01/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>이 문서를 사용하려면 Adobe Workfront API 및 텍스트 모드 보고 인터페이스에 대한 철저한 이해가 필요합니다. Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md)을 참조하세요.\
>텍스트 모드 사용에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

## Workfront의 개체 관계 개요

모든 개체는 Workfront 데이터베이스의 다른 개체에 연결됩니다.

객체의 계층 구조 및 상호 종속성을 이해하면 보고서에서 참조할 수 있는 객체를 찾는 데 도움이 됩니다.

Workfront에 있는 개체, 개체의 계층 구조 및 상호 종속성에 대한 자세한 내용은 [Adobe Workfront 개체 개요](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)를 참조하십시오.

필터를 작성할 때 표준 보고 인터페이스를 사용하여 최대 2개의 관계 수준 내에서 필터 개체에 연결된 다른 개체를 참조할 수 있습니다.

예를 들어 문제 필터에서 Portfolio ID를 참조하여 표준 인터페이스를 사용하여 특정 포트폴리오와 연결된 프로젝트의 문제만 표시할 수 있습니다. 이 경우 포트폴리오는 이슈와 2단계 떨어져 있습니다.

하지만 표준 인터페이스를 사용하여 문제 필터에서 Portfolio 소유자를 참조하여 소유자가 특정 사용자인 포트폴리오와 연결된 프로젝트의 문제만 표시할 수는 없습니다. 텍스트 모드를 사용하여 문제에서 3 단계 떨어진 Portfolio 소유자 이름 필드에 액세스해야 합니다.

![포트폴리오 소유자 아이콘에 문제](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Workfront의 전체 개체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

API 탐색기를 탐색하고 개체를 찾는 방법에 대한 자세한 내용은 [API 탐색기 사용](../../../wf-api/general/using-api-explorer.md)을 참조하십시오.

필터를 작성할 때 이러한 유형의 개체를 참조하려면 텍스트 모드 인터페이스에서 복잡한 문을 작성해야 합니다.

복합 필터 빌드에 대한 자세한 내용은 이 문서의 [EXISTS 문을 사용하는 복합 텍스트 모드 필터의 개요](#overview-of-complex-text-mode-filters-that-use-exists-statements) 섹션을 참조하십시오.

## EXISTS 문을 사용하는 복잡한 텍스트 모드 필터의 개요 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

객체 계층의 여러 수준에 걸쳐 있는 필터 또는 누락된 객체에 대한 필터를 생성할 때는 다음 사항을 고려하십시오.

* 필터 개체에 직접 연결되지 않은 개체를 참조하려면 복잡한 필터를 만들어야 합니다.
* 다음을 수행하려면 EXISTS 문을 사용해야 합니다.

   * 여러 수준에 걸쳐 있는 필터를 만듭니다.
   * 누락된 오브젝트를 찾는 필터를 만듭니다.\
     예를 들어 사용자 보고서를 작성할 때 특정 기간 동안 시간을 기록하지 않은 사용자를 필터링할 수 있습니다.

필터에 EXISTS 문을 사용할 때는 다음 규칙을 고려하십시오.

* EXISTS 필터에서 참조할 수 있는 세 가지 개체가 있습니다.

   * 필터의 개체(원본 개체)입니다.
   * 참조할 필드가 있는 개체(대상 개체)입니다.
   * 원본 개체와 대상 개체가 직접 연결되어 있지 않은 경우 원본 개체와 대상 개체를 연결하는 개체(연결 개체)입니다.

* EXISTS를 사용하는 필터에는 등호로 연결된 두 개의 개별 문이 포함되어 있습니다.

   * 등호 앞의 문은 참조하는 개체(연결 또는 대상 개체)를 참조합니다.
   * 등호 다음의 문은 참조하는 객체(원본 객체)를 참조합니다.

* 문을 연결하려면 연결 개체의 개체 코드를 사용해야 합니다.\
  API 탐색기에서 모든 개체의 개체 코드를 찾을 수 있습니다.\
  API 탐색기에 대한 자세한 내용은 [API 탐색기](../../../wf-api/general/api-explorer.md)를 참조하십시오.

* 원본 개체와 대상 개체가 직접 연결되어 연결 개체가 없을 경우 연결 개체 대신 대상 개체의 개체 코드를 사용할 수 있습니다.
* 동일한 개체(대상 개체)에서 여러 필드(대상 필드)를 참조할 수 있습니다. 이 경우 AND로 필드를 참조하는 줄을 연결해야 합니다.\
  대상 개체에 속한 둘 이상의 필드에 대한 필터링의 예는 이 문서의 [예 4: 여러 필드별 필터링: Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID별 작업](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) 섹션을 참조하십시오.

* EXISTS 문에 지원되는 유일한 한정자는 NOTEXISTS입니다.

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
     <p>표준</p>
     <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서의 필터 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>보고서에서 필터를 편집할 보고서에 대한 권한 관리</p> <p>편집할 필터에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 객체 계층의 여러 수준에 걸쳐 있는 복잡한 텍스트 모드 필터 만들기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

필터 개체가 있는 개체 계층의 여러 수준에 걸쳐 개체를 참조하는 필터를 빌드할 수 있습니다. 예를 들어 특정 Portfolio 소유자와 관련이 없는 프로젝트에 있는 문제에 대한 문제 필터를 빌드할 수 있습니다.

이 필터를 빌드하려면 항상 EXISTS 문과 텍스트 모드 인터페이스를 사용해야 합니다.

필터의 예는 이 문서의 [예 1: Portfolio 소유자 이름별 문제 필터링](#example-1-filter-for-issues-by-portfolio-owner-name) 섹션을 참조하십시오.

객체 계층의 여러 레벨에 걸쳐 적용되는 필터를 생성하려면 다음과 같이 하십시오.

1. 필터의 개체를 식별합니다. 이 객체를 원래 객체라고 합니다.\
   예를 들어, 문제

1. 필터링 기준으로 사용할 필드를 식별합니다. 이 객체를 Target 객체에 속한 Target 필드라고 합니다.\
   예를 들어 Portfolio(대상 개체)에 속하는 ownerID 필드(대상 필드)입니다.

1. (조건부) 원본 개체(Issue)와 대상 필드(ownerID)가 직접 연결되어 있지 않으면 세 번째 개체인 원본 개체와 대상 필드 사이를 연결하는 연결 개체(Project)를 찾아야 합니다. 연결 객체에는 원본 객체의 필드 또는 참조 탭(원본 객체에 표시된 연결 필드)에서 참조하는 하나 이상의 필드가 있어야 하며 대상 객체로의 연결 필드도 있어야 합니다. 연결 개체에 표시되는 대상 개체로의 연결 필드(또는 연결 개체에 표시되는 연결 필드)는 대상 필드와 일치해야 합니다.

   예를 들어, (프로젝트) ID(원래 오브젝트에 표시된 연결 필드)는 문제(원래 오브젝트)에서 참조됩니다. (Portfolio) ownerID(대상 오브젝트에 대한 필드 연결)가 프로젝트(연결 오브젝트)의 필드 탭에 표시됩니다. Portfolio ownerID 는 Target 개체 (Portfolio)의 필드입니다. 연결 개체의 연결 필드는 대상 필드와 일치합니다.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. API 탐색기를 사용하여 연결 개체(프로젝트)의 **개체 코드**&#x200B;를 식별합니다.\
   예를 들어 프로젝트의 개체 코드는 PROJ입니다.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 원본 개체에 대한 필터를 만듭니다.\
   예를 들어 문제 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 새 필터의 텍스트 모드 인터페이스에 다음 수식 예제를 붙여넣고 예제 텍스트를 올바른 개체 및 필드로 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   위에서 식별한 필드를 사용하는 예제는 이 문서의 [예 1: Portfolio 소유자 이름별로 문제 필터링](#example-1-filter-for-issues-by-portfolio-owner-name) 섹션을 참조하십시오.

1. **필터 저장**&#x200B;을 클릭합니다.

## 누락된 오브젝트에 대한 복잡한 텍스트 모드 필터 만들기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

누락된 개체를 참조하는 필터를 빌드할 수 있습니다. 예를 들어 Workfront에서 시간을 기록하지 않은 사용자를 표시하는 사용자 필터를 빌드할 수 있습니다.

이 필터를 빌드하려면 항상 *EXISTS* 문과 텍스트 모드 인터페이스를 사용해야 합니다.

누락된 오브젝트에 대한 필터의 예는 이 문서의 다음 섹션을 참조하십시오.

* [예제 2: 누락된 개체 필터링: 사용자 정의 양식에 표시되지 않는 사용자 정의 필드](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [예제 3: 누락된 개체 필터링: 특정 기간 동안 시간을 기록하지 않은 사용자](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

누락된 개체를 참조하는 필터를 만들려면 다음 작업을 수행하십시오.

1. 필터의 개체를 식별합니다. 이 객체를 원래 객체라고 합니다.\
   예: 매개변수 또는 사용자 정의 필드.

1. 필터링 기준으로 사용할 필드를 식별합니다. 이 객체를 Target 객체에 속한 Target 필드라고 합니다.\
   예를 들어 Category(대상 객체)에 속하는 categoryID 필드(대상 필드)입니다.

1. 원본 개체(매개 변수)와 대상 필드(categoryID)는 서로 직접 연결되어 있지 않으므로 세 번째 개체인 연결 개체(범주 매개 변수)를 찾아야 합니다. 연결 객체에는 원본 객체의 필드 또는 참조 탭(원본 객체에 표시된 연결 필드)에서 참조하는 하나 이상의 필드가 있어야 하며 대상 객체로의 연결 필드도 있어야 합니다. 연결 개체에 표시되는 대상 개체로의 연결 필드(또는 연결 개체에 표시되는 연결 필드)는 대상 필드와 일치해야 합니다.

   예를 들어, Parameter(원본 개체)에서 Category 매개 변수(원본 개체에 표시된 연결 필드)의 ID를 참조합니다. parameterID(대상 개체에 필드 연결)는 범주 매개 변수(개체 연결)의 필드 탭에 표시됩니다. 연결 객체에 표시되는 대상 객체에 대한 연결 필드는 대상 필드와 일치합니다.

1. API 탐색기를 사용하여 연결 개체(범주 매개 변수)의 **개체 코드**&#x200B;를 식별합니다.\
   예를 들어, 범주 매개변수에 대한 개체 코드는 CTGAA입니다.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 원본 개체에 대한 필터를 만듭니다.\
   예를 들어 매개 변수 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. (조건부) 누락된 오브젝트를 필터링하는 경우 다음 수식 예제를 새 필터의 텍스트 모드 인터페이스에 붙여넣고 예제 텍스트를 올바른 오브젝트 및 필드로 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   사용자 지정 Forms과 연결되지 않은 사용자 지정 필드에 대한 보고의 예를 보려면 이 문서의 [예 2: 누락된 개체에 대한 필터: 사용자 지정 양식에 표시되지 않는 사용자 지정 필드](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) 섹션을 참조하십시오.

1. **필터 저장**&#x200B;을 클릭합니다.

## 객체 계층의 여러 수준에 걸쳐 있는 텍스트 모드 필터의 예

다음 예를 사용하여 EXISTS 문을 사용하여 텍스트 모드 필터를 빌드합니다.

### 예제 1: Portfolio 소유자 이름별로 문제 필터링 {#example-1-filter-for-issues-by-portfolio-owner-name}

텍스트 모드 인터페이스를 사용하여 문제 목록에 대한 필터를 빌드하여 소유자가 특정 사용자인 포트폴리오와 연결된 프로젝트에 있는 문제만 표시할 수 있습니다.

Portfolio 소유자 이름별로 문제를 필터링하려면 다음을 수행하십시오.

1. 문제 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. **보고서에 대한 필터 규칙 설정** 영역에 다음 코드를 붙여넣어 위의 일반 코드를 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=PROJ
   EXISTS:A:ID=FIELD:projectID
   EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221
   ```

   >[!NOTE]
   >
   >* 원래 개체는 보고서의 개체입니다. 문제
   >* 대상 개체는 Portfolio입니다.
   >* 연결 개체는 프로젝트입니다.
   >* 대상 필드 및 대상 객체에 대한 연결 필드는 연결 객체에서 참조되는 ownerID입니다.
   >* 여기에서 연결 개체의 개체 코드는 PROJ입니다.
   >* 원래 오브젝트에 표시되는 연결 필드는 projectID이고 연결 필드는 ID입니다.

1. 마지막 문의 Target 필드(ownerID) 값을 환경의 사용자 ID로 바꿉니다.
1. **필터 저장**&#x200B;을 클릭합니다.

### 예제 2: 누락된 개체 필터링: 사용자 정의 양식에 표시되지 않는 사용자 정의 필드 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

텍스트 모드 인터페이스를 사용하여 사용자 지정 Forms(카테고리)와 연결되지 않은 사용자 지정 필드(매개 변수)를 보는 필터를 빌드할 수 있습니다. 이 필터는 다른 개체 Category Parameter를 통해 연결된 Categories에 매개 변수를 연결합니다. 두 필드가 서로 직접 연결되어 있지 않고 누락된 정보를 필터링하고 있으므로 EXISTS 문을 사용해야 합니다.

>[!IMPORTANT]
>
>매개 변수는 사용자 정의 양식에서 참조된 필드 라이브러리에 있는 필드입니다. 카테고리 매개 변수는 특정 양식에 나타나는 필드의 버전입니다. 예를 들어 동일한 필드가 5개의 양식에 나타나는 경우, Workfront 데이터베이스에 1개의 매개 변수와 5개의 범주 매개 변수가 있습니다.

사용자 정의 양식과 연결되지 않은 사용자 정의 필드를 필터링하려면 다음을 수행하십시오.

1. 매개 변수 또는 사용자 지정 필드 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. **보고서에 대한 필터 규칙 설정** 영역에 다음 코드를 붙여넣어 위의 일반 코드를 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=CTGYPA
   EXISTS:A:parameterID=FIELD:ID
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 원본 객체는 보고서의 객체인 매개 변수입니다.
   >* 대상 개체는 범주입니다.
   >* 연결 개체는 범주 매개 변수입니다.
   >* Linking 개체의 개체 코드는 CTGAA입니다.
   >* parameterID는 연결 개체 테이블과 대상 개체 테이블 모두에 있으므로 대상 개체에 대한 연결 필드는 parameterID입니다.
   >* 원래 오브젝트에 표시되는 연결 필드는 범주 매개 변수의 ID입니다.

1. **필터 저장**&#x200B;을 클릭합니다.

### 예제 3: 누락된 개체 필터링: 특정 기간 동안 시간을 기록하지 않은 사용자 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

텍스트 모드 인터페이스를 사용하여 특정 기간 동안 시간을 기록하지 않은 사용자를 보는 필터를 작성할 수 있습니다. 이 필터는 사용자를 서로 직접 연결된 시간에 연결합니다. 그러나 누락된 정보를 필터링하려면 EXISTS 문과 텍스트 모드 인터페이스를 사용해야 합니다.

지난 주 동안 시간을 기록하지 않은 사용자를 필터링하려면 다음을 수행하십시오.

1. 사용자 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. **보고서에 대한 필터 규칙 설정** 영역에 다음 코드를 붙여넣어 위의 일반 코드를 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=HOUR
   EXISTS:A:ownerID=FIELD:ID
   EXISTS:A:entryDate=$$TODAYb-1w
   EXISTS:A:entryDate_Range=$$TODAYe-1w
   EXISTS:A:entryDate_Mod=between
   EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 원본 객체는 보고서의 객체인 사용자입니다.
   >* 대상 객체는 시간입니다.
   >* 사용자 및 시간은 Workfront 데이터베이스에서 직접 연결되므로 이 예제에서는 연결 개체가 필요하지 않습니다.
   >* 연결 개체가 없으므로 대상 개체의 개체 코드 HOUR을 사용해야 합니다.
   >* 대상 객체에 대한 연결 필드는 원래 객체에 표시되는 ownerID입니다. 이 필드에는 연결 객체가 없습니다.
   >* 원래 객체에 표시되는 연결 필드는 대상 객체에 표시되는 ID(시간의)이며, 연결 객체가 없습니다.
   >* EXISTS:A:entryDate 문은 Target 개체(Hour)를 정의하고 일반 필터 문과 동일한 구문을 사용하는 필드를 나타냅니다. 이렇게 하면 특정 기간(이 경우 이전 주) 동안 시간을 기록하지 않은 사용자만 표시할 수 있습니다.
   >* NOTEXISTS 수정자는 보고서(사용자) 개체에 존재하지 않는 항목(시간)을 찾고 있음을 나타냅니다.

1. **필터 저장**&#x200B;을 클릭합니다.

### 예제 4: 여러 필드로 필터링: Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID별 작업 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

텍스트 모드 인터페이스를 사용하여 Target 개체에 두 개 이상의 필드를 참조하는 필터를 빌드할 수 있습니다. 이 경우 타겟 필드를 참조하는 필터 문은 AND로 연결해야 합니다.

예를 들어 작업 목록을 필터링하여 다음 기준을 충족하는 작업만 표시할 수 있습니다.

* 소유자가 특정 사용자인 포트폴리오와 연결된 프로젝트에 있습니다.
* 특정 정렬 스코어카드와 프로젝트가 연결되지 않은 포트폴리오와 연결된 프로젝트에 있습니다.

Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID로 작업을 필터링하려면 다음을 수행하십시오.

1. 작업 필터를 만듭니다.\
   필터 만들기에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)를 참조하세요.

1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **보고서에 대한 필터 규칙 설정** 영역에 다음 코드를 붙여넣습니다.

   ```
   EXISTS:A:$$OBJCODE=PROJ
   EXISTS:A:ID=FIELD:projectID
   EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f
   AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS
   AND:A:EXISTS:A:$$OBJCODE=PROJ
   AND:A:EXISTS:A:ID=FIELD:projectID
   AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad
   ```

   >[!NOTE]
   >
   >* 원래 개체는 필터의 개체입니다. 작업.
   >* 대상 개체는 Portfolio입니다.
   >* 첫 번째 대상 필드는 ownerID입니다.
   >* 두 번째 대상 필드는 정렬 스코어카드 ID입니다.
   >* 연결 개체는 프로젝트입니다.
   >* 연결 개체의 개체 코드는 PROJ입니다.
   >* 대상 오브젝트에 대한 연결 필드는 Portfolio의 ID입니다.
   >* 원래 오브젝트에 표시되는 연결 필드는 projectID입니다.
   >* ownerID를 환경의 사용자 ID로 바꿉니다.

1. **필터 저장**&#x200B;을 클릭합니다.
