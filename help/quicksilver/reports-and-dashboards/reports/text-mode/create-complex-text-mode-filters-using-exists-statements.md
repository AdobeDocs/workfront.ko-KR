---
product-area: reporting
navigation-topic: text-mode-reporting
title: EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기
description: EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# EXISTS 문을 사용하여 복잡한 텍스트 모드 필터 만들기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>이 문서를 사용하려면 Adobe Workfront API 및 텍스트 모드 보고 인터페이스에 대한 철저한 이해가 필요합니다. Workfront API에 대한 자세한 내용은 [API 기본 사항](../../../wf-api/general/api-basics.md).\
>텍스트 모드 사용에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Workfront의 개체 관계 개요

모든 개체는 Workfront 데이터베이스의 다른 개체에 연결됩니다.

개체의 계층 구조 및 상호 종속성을 이해하면 보고서에서 참조할 수 있는 개체를 찾을 수 있습니다.

Workfront에 있는 개체, 계층 및 상호 종속성에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

필터를 작성할 때 표준 보고 인터페이스를 사용하여 최대 2수준의 관계 내에서 필터 개체에 연결된 다른 개체를 참조할 수 있습니다.

예를 들어 문제 필터에서 Portfolio ID를 참조하여 표준 인터페이스를 사용하여 특정 포트폴리오와 연결된 프로젝트에 대한 문제만 표시할 수 있습니다. 이 경우 포트폴리오는 문제로부터 2수준 떨어져 있습니다.

그러나 표준 인터페이스를 사용하여 문제 필터에서 Portfolio 소유자를 참조하여 소유자가 특정 사용자인 포트폴리오와 연관된 프로젝트의 문제만 표시할 수 없습니다. 문제가 발생하는 3단계 떨어진 Portfolio 소유자 이름 필드에 액세스하려면 텍스트 모드를 사용해야 합니다.

![issue_to_portfolio_owner_stream_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Workfront의 전체 개체 목록은 [API 탐색기](../../../wf-api/general/api-explorer.md).

API 탐색기를 탐색하고 개체를 찾는 방법에 대한 자세한 내용은 [API 탐색기 사용](../../../wf-api/general/using-api-explorer.md).

필터를 작성할 때는 이러한 유형의 개체를 참조할 수 있도록 텍스트 모드 인터페이스에서 복잡한 문을 작성해야 합니다.

복잡한 필터 빌드에 대한 자세한 내용은 [EXISTS 문을 사용하는 복잡한 텍스트 모드 필터 개요](#overview-of-complex-text-mode-filters-that-use-exists-statements) 섹션을 참조하십시오.

## EXISTS 문을 사용하는 복잡한 텍스트 모드 필터 개요 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

개체 계층 구조에서 여러 수준에 걸쳐 있는 필터를 만들거나 누락된 개체에 대해 필터를 만들 때 다음 사항을 고려하십시오.

* 필터 개체에 직접 연결되지 않은 개체를 참조하려면 복잡한 필터를 만들어야 합니다.
* 다음을 수행하려면 EXISTS 문을 사용해야 합니다.

   * 여러 수준에 걸쳐 필터를 만듭니다.
   * 누락된 개체를 찾는 필터를 만듭니다.\
      예를 들어 사용자 보고서를 작성할 때 특정 기간 동안 로그인이 되지 않은 사용자를 기준으로 필터링할 수 있습니다.

필터에서 EXISTS 문을 사용할 때는 다음 규칙을 고려하십시오.

* EXISTS 필터에서 참조할 수 있는 개체가 세 개 있습니다.

   * 필터의 개체(원본 개체)입니다.
   * 참조할 필드가 있는 개체(Target 개체)입니다.
   * 원본 객체와 Target 객체를 연결하는 객체(객체 연결)

* EXISTS를 사용하는 필터에는 등호 기호로 연결된 두 개의 별도 문이 포함되어 있습니다.

   * 등호 앞의 문은 참조하는 개체(연결 또는 Target 개체)를 참조합니다.
   * 등호 다음에 나오는 문은 참조하는 개체(원본 개체)를 참조합니다.

* 연결 개체의 개체 코드를 사용하여 문을 연결해야 합니다.\
   API 탐색기에서 모든 개체의 개체 코드를 찾을 수 있습니다.\
   API 탐색기에 대한 자세한 내용은 [API 탐색기](https://one.workfront.com/s/api-explorer).

* 원본 및 Target 개체가 서로 직접 연결되어 연결 개체가 없는 경우 연결 개체 대신 Target 개체의 개체 코드를 사용할 수 있습니다.
* 동일한 개체(Target 개체)에 여러 필드(Target 필드)를 참조할 수 있습니다. 이 경우 필드를 참조하는 줄을 AND로 연결해야 합니다.\
   Target 객체에 속한 두 개 이상의 필드에 대한 필터링 예는 를 참조하십시오. [예제 4: 여러 필드로 필터링: Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID별 작업](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) 섹션에 자세히 설명되어 있습니다.

* EXISTS 문에 대해 지원되는 유일한 수정자는 NOEXISTS입니다.

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
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 필터를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리를 통해 보고서의 필터를 편집합니다</p> <p>필터에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 개체 계층 구조에서 여러 수준에 걸쳐 있는 복잡한 텍스트 모드 필터를 만듭니다

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

필터 객체가 있는 객체 계층의 여러 레벨에서 객체를 참조하는 필터를 작성할 수 있습니다. 예를 들어 특정 Portfolio 소유자와 연관되지 않은 프로젝트에 있는 문제에 대한 문제 필터를 작성할 수 있습니다.

이 필터를 빌드하려면 항상 EXISTS 문과 텍스트 모드 인터페이스를 사용해야 합니다.

필터의 예는 를 참조하십시오. [예제 1: Portfolio 소유자 이름별로 문제를 필터링합니다.](#example-1-filter-for-issues-by-portfolio-owner-name) 섹션에 자세히 설명되어 있습니다.

객체 계층 구조에서 여러 수준에 걸쳐 있는 필터를 생성하려면 다음을 수행합니다.

1. 필터의 개체를 식별합니다. 이 개체를 원래 개체로 참조합니다.\
   예, 문제.
1. 필터링할 필드를 식별합니다. 이 개체를 Target 개체에 속하는 Target 필드로 참조합니다.\
   예를 들어 Portfolio(Target 개체)에 속하는 ownerID 필드(Target 필드)입니다.
1. (조건부) 원본 개체(문제)와 Target 필드(ownerID)가 서로 직접 연결되어 있지 않으면 세 번째 개체(Linking 개체)가 연결되어 있는 것을 찾아야 합니다. 연결 객체에는 원본 객체의 필드 또는 참조 탭(원본 객체에 표시된 연결 필드)에서 참조되는 필드가 하나 이상 있어야 하며, 연결 객체의 필드 또는 참조 탭에 표시되는 Target 객체에 연결 필드가 있어야 합니다. 연결 개체(또는 연결 개체에 표시된 연결 필드)에 표시되는 Target 개체에 대한 연결 필드는 Target 필드와 일치해야 합니다.\
   예를 들어 (프로젝트) ID(원본 개체에 표시된 연결 필드)가 문제(원본 개체)에서 참조됩니다. (Portfolio) ownerID(Target 개체에 필드 연결)가 프로젝트(개체 연결)의 필드 탭에 표시됩니다. Portfolio ownerID는 Target 개체(Portfolio)의 필드이기도 합니다. 연결 개체의 연결 필드가 Target 필드와 일치합니다.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. API 탐색기를 사용하여 **개체 코드** 연결 개체(프로젝트)에 대한 액세스 권한 섹션을 참조하십시오.\
   예를 들어 프로젝트에 대한 개체 코드는 PROJ입니다.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 원본 개체에 대한 필터를 만듭니다.\
   예를 들어 문제 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. 다음 수식 예제를 새 필터의 텍스트 모드 인터페이스에 붙여넣고 제안된 텍스트를 올바른 개체 및 필드로 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   위에서 식별한 필드를 사용하는 예제는 [예제 1: Portfolio 소유자 이름별로 문제를 필터링합니다.](#example-1-filter-for-issues-by-portfolio-owner-name) 섹션에 자세히 설명되어 있습니다.

1. 클릭 **필터 저장**.

## 누락된 객체에 대해 복잡한 텍스트 모드 필터 만들기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

누락된 개체를 참조하는 필터를 작성할 수 있습니다. 예를 들어 Workfront에서 로그인하지 않은 사용자를 보여주는 사용자 필터를 작성할 수 있습니다.

항상 를 사용해야 합니다 *존재함* 문 및 이 필터를 빌드할 텍스트 모드 인터페이스입니다.

누락된 객체에 대한 필터의 예는 이 문서에서 다음 섹션을 참조하십시오.

* [예제 2: 누락된 개체에 대해 필터링: 사용자 지정 양식에 표시되지 않는 사용자 지정 필드](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [예제 3: 누락된 개체에 대해 필터링: 특정 기간 동안 시간을 기록하지 않은 사용자](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

누락된 개체를 참조하는 필터를 만들려면

1. 필터의 개체를 식별합니다. 이 개체를 원래 개체로 참조합니다.\
   예를 들어 매개 변수 또는 사용자 지정 필드가 있습니다.
1. 필터링할 필드를 식별합니다. 이 개체를 Target 개체에 속하는 Target 필드로 참조합니다.\
   예를 들어 카테고리(Target 개체)에 속하는 categoryID 필드(Target 필드)가 있습니다.
1. 원본 개체(매개 변수)와 Target 필드(categoryID)가 직접 연결되어 있지 않으므로 세 번째 개체(Linking 개체)가 연결되어 있는 범주 매개 변수를 찾아야 합니다. 연결 객체에는 원본 객체의 필드 또는 참조 탭(원본 객체에 표시된 연결 필드)에서 참조되는 필드가 하나 이상 있어야 하며, 연결 객체의 필드 또는 참조 탭에 표시되는 Target 객체에 연결 필드가 있어야 합니다. 연결 개체(또는 연결 개체에 표시된 연결 필드)에 표시되는 Target 개체에 대한 연결 필드는 Target 필드와 일치해야 합니다.\
   예를 들어, Category Parameter(원본 개체에 표시된 Linking Field)의 ID는 Parameter(Original Object)에서 참조됩니다. parameterID(Target 개체에 필드 연결)는 카테고리 매개 변수(연결 개체)의 필드 탭에 표시됩니다. 연결 개체에 표시되는 Target 개체에 연결 필드는 Target 필드와 일치합니다.
1. API 탐색기를 사용하여 **개체 코드** 연결 개체(카테고리 매개 변수)의 를 참조하십시오.\
   예를 들어, 카테고리 매개 변수의 개체 코드는 CTGYPA입니다.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 원본 개체에 대한 필터를 만듭니다.\
   예를 들어 매개 변수 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. (조건부) 누락된 개체를 필터링하려면 다음 공식 예제를 새 필터의 텍스트 모드 인터페이스에 붙여 넣고 제안된 텍스트를 올바른 개체 및 필드로 바꿉니다.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   사용자 지정 Forms과 연관되지 않은 사용자 지정 필드에 대한 보고의 예는 를 참조하십시오. [예제 2: 누락된 개체에 대해 필터링: 사용자 지정 양식에 표시되지 않는 사용자 지정 필드](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) 섹션에 자세히 설명되어 있습니다.

1. 클릭 **필터 저장**.

## 개체 계층 구조에서 여러 수준에 걸쳐 있는 텍스트 모드 필터의 예

* [예제 1: Portfolio 소유자 이름별로 문제를 필터링합니다.](#example-1-filter-for-issues-by-portfolio-owner-name)
* [예제 2: 누락된 개체에 대해 필터링: 사용자 지정 양식에 표시되지 않는 사용자 지정 필드](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [예제 3: 누락된 개체에 대해 필터링: 특정 기간 동안 시간을 기록하지 않은 사용자](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [예제 4: 여러 필드로 필터링: Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID별 작업](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### 예제 1: Portfolio 소유자 이름별로 문제를 필터링합니다. {#example-1-filter-for-issues-by-portfolio-owner-name}

텍스트 모드 인터페이스를 사용하여 문제 목록에 대한 필터를 작성하여 소유자가 특정 사용자인 포트폴리오와 연결된 프로젝트에 있는 문제만 표시할 수 있습니다.

Portfolio 소유자 이름별로 문제를 필터링하려면

1. 문제 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. 다음 코드를 **보고서에 대한 필터 규칙 설정** 위의 일반 코드를 바꿀 영역:

   <pre>존재함:A:$$OBJCODE=PROJ<br>존재함:A:ID=FIELD:projectID<br>존재함:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* Original Object 는 보고서의 객체입니다. 문제
   >* Target 개체가 Portfolio입니다.
   >* 연결 개체는 프로젝트입니다.
   >* Target 필드 및 연결 필드가 연결 개체에서 참조되는 Target 개체에 대해서는 ownerID입니다.
   >* 여기에 있는 연결 개체의 개체 코드는 PROJ입니다.
   >* 원본 개체에 표시되는 연결 필드는 projectID이고 연결 필드는 ID입니다.


1. 마지막 문에 있는 Target 필드(ownerID)의 값을 환경의 사용자 ID로 바꿉니다.
1. 클릭 **필터 저장**.

### 예제 2: 누락된 개체에 대해 필터링: 사용자 지정 양식에 표시되지 않는 사용자 지정 필드 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

텍스트 모드 인터페이스를 사용하여 필터를 작성하여 사용자 지정 Forms(카테고리)와 연결되지 않은 사용자 지정 필드(매개 변수)를 볼 수 있습니다. 이 필터는 다른 개체, Category 매개 변수를 통해 연결된 범주에 매개 변수를 연결합니다. 두 필드가 서로 직접 연결되어 있지 않으므로 누락된 정보를 필터링하려면 EXISTS 문을 사용해야 합니다.

>[!IMPORTANT]
>
>매개 변수는 사용자 지정 양식에서 참조되는 필드 라이브러리에 있는 필드입니다. 카테고리 매개 변수는 특정 양식에 나타나는 필드의 버전입니다. 예를 들어 동일한 필드가 5개의 양식에 나타나면 Workfront 데이터베이스에 1개의 매개 변수와 5개의 카테고리 매개 변수가 있습니다.

사용자 지정 양식과 연관되지 않은 사용자 지정 필드를 필터링하려면 다음을 수행하십시오.

1. 매개 변수 또는 사용자 지정 필드 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 다음 코드를 **보고서에 대한 필터 규칙 설정** 위의 일반 코드를 바꿀 영역:

   <pre>존재함:A:$$OBJCODE=CTGYPA<br>존재함:A:parameterID=FIELD:ID<br>존재함:A:$$EXISTSMOD=NOEXISTS</pre>

   >[!NOTE]
   >
   >* Original Object 는 보고서의 객체입니다. 매개 변수.
   >* Target 객체는 카테고리입니다.
   >* 연결 개체는 카테고리 매개 변수입니다.
   >* 연결 개체의 개체 코드는 CTGYPA입니다.
   >* 매개 변수 ID가 연결 개체 테이블과 Target 개체 테이블 모두에 있으므로 Target 개체에 연결 필드는 parameterID입니다.
   >* 원본 개체에 표시되는 연결 필드는 카테고리 매개 변수의 ID입니다.


1. 클릭 **필터 저장**.

### 예제 3: 누락된 개체에 대해 필터링: 특정 기간 동안 시간을 기록하지 않은 사용자 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

텍스트 모드 인터페이스를 사용하여 특정 기간 동안 시간을 기록하지 않은 사용자를 보는 필터를 작성할 수 있습니다. 이 필터는 사용자가 시간에 연결되며 서로 직접 연결됩니다. 그러나 누락된 정보를 필터링하려면 EXISTS 문과 텍스트 모드 인터페이스를 사용해야 합니다.information

지난 주 동안 시간을 기록하지 않은 사용자를 필터링하려면 다음을 수행하십시오.

1. 사용자 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. 다음 일반 코드를 참조하십시오.

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 다음 코드를 **보고서에 대한 필터 규칙 설정** 위의 일반 코드를 바꿀 영역:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* Original Object 는 보고서의 객체입니다. 사용자.
   >* Target 개체는 Hour입니다.
   >* 사용자 및 시간이 Workfront 데이터베이스에 직접 연결되므로 이 예제에서는 연결 개체가 필요하지 않습니다.
   >* 연결 개체가 없으므로 Target 개체의 개체 코드를 사용해야 합니다. 시간
   >* Target 객체에 연결 필드는 원래 객체에 표시되는 ownerID입니다. 연결 개체가 없습니다.)
   >* 원본 개체에 표시되는 연결 필드는 Target 개체에 표시되는 ID(시간 기준)입니다. 연결 개체가 없습니다.)
   >* 존재함:A:entryDate 문은 Target 개체(시간)를 정의하고 일반 필터 문과 동일한 구문을 사용하는 필드를 참조합니다. 따라서 특정 기간(이 경우 이전 주) 동안 시간을 기록하지 않은 사용자만 표시할 수 있습니다.
   >* NOEXISTS 수정자는 보고서 객체(사용자)에 대해 존재하지 않는 항목(시간)을 찾고 있음을 나타냅니다.


1. 클릭 **필터 저장**.

### 예제 4: 여러 필드로 필터링: Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID별 작업 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

텍스트 모드 인터페이스를 사용하여 Target 개체에서 두 개 이상의 필드를 참조하는 필터를 작성할 수 있습니다. 이 경우 Target 필드를 참조하는 필터 문은 AND로 연결해야 합니다.

예를 들어 다음 기준을 충족하는 작업만 표시하도록 작업 목록을 필터링할 수 있습니다.

* 소유자가 특정 사용자인 포트폴리오와 연결된 프로젝트에 있습니다.
* 프로젝트가 특정 정렬 스코어카드와 연결되지 않은 포트폴리오와 연결된 프로젝트에 있습니다.

Portfolio 소유자 이름 및 Portfolio 정렬 스코어카드 ID로 작업을 필터링하려면:

1. 작업 필터를 만듭니다.\
   필터 만들기에 대한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 클릭 **텍스트 모드로 전환**.
1. 다음 코드를 **보고서에 대한 필터 규칙 설정** 영역:
   <pre>존재함:A:$$OBJCODE=PROJ<br>존재함:A:ID=FIELD:projectID<br>존재함:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>및:A:존재함:A:$$EXISTSMOD=NOEXISTS<br>및:A:존재함:A:$$OBJCODE=PROJ<br>및:A:존재함:A:ID=FIELD:projectID<br>및:A:존재함:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* Original Object 는 필터의 객체입니다. 작업.
   >* Target 개체가 Portfolio입니다.
   >* 첫 번째 Target 필드는 ownerID입니다.
   >* 두 번째 Target 필드는 정렬 스코어카드 ID입니다.
   >* 연결 개체는 프로젝트입니다.
   >* 연결 개체의 개체 코드는 PROJ입니다.
   >* Target 개체에 연결 필드는 Portfolio의 ID입니다.
   >* 원본 개체에 표시되는 연결 필드는 projectID입니다.
   >* ownerID를 환경의 사용자 ID로 바꿉니다.


1. 클릭 **필터 저장**.
