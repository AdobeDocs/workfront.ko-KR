---
title: 사용자 지정 Forms 및 필드에 논리 규칙 추가
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 논리 규칙을 사용하면 양식의 필드를 추가로 사용자 지정할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 49f26e963647f5015955396489bfe537bbac0918
workflow-type: tm+mt
source-wordcount: '3544'
ht-degree: 0%

---

# 사용자 정의 양식 및 필드에 논리 규칙 추가

논리 규칙을 사용하면 양식의 필드를 추가로 사용자 지정할 수 있습니다.

예를 들어, 사용자가 필드 또는 섹션을 작성할 때 선택하는 내용에 따라 사용자 정의 양식의 필드나 섹션을 표시하거나 건너뛸 수 있습니다.

>[!NOTE]
>
>논리는 한 양식 내에서만 적용되며 다른 양식의 선택 사항을 기반으로 할 수 없습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td> <p>고급 표시, 기본값, 조건부 서식 또는 편집 논리 적용: 워크플로우 Prime 이상</p>
         <p>다른 모든 논리 유형(모든 Workfront 또는 워크플로 패키지)을 적용하려면</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 논리 표시기 아이콘

사용자 정의 양식에는 필드에 논리가 적용되는 시기를 나타내는 아이콘이 표시됩니다.

다른 필드 논리 형식에 대한 아이콘을 표시하거나 숨기려면 양식 디자이너 헤더에서 **논리 표시**&#x200B;를 클릭하십시오.

| 아이콘 | 정의 |
| --- | --- |
| ![대상 필드에 대한 디스플레이 논리](assets/display-logic-bottom-right.png) | 필드는 표시 논리가 적용되는 대상 필드입니다. 양식에서 특정 항목을 선택하면 이 필드가 표시됩니다. |
| ![참조 필드에 대한 논리 아이콘 표시](assets/display-logic-bottom-left.png) | 필드는 표시 논리의 참조 필드입니다. 이 필드의 특정 선택 또는 값은 대상 필드를 표시합니다. |
| ![대상 필드에 대한 건너뛰기 논리](assets/skip-logic-bottom-right.png) | 필드는 건너뛰기 논리가 적용되는 대상 필드입니다. 이 필드의 특정 선택 또는 값은 다른 필드를 건너뛰고 참조 필드로 바로 이동합니다. |
| ![참조 필드의 건너뛰기 논리 아이콘](assets/skip-logic-bottom-left.png) | 필드는 건너뛰기 논리의 참조 필드입니다. 대상 필드에서 특정 항목을 선택하면 양식이 이 필드로 건너뛰고 그 사이의 필드는 숨겨집니다. |
| ![대상 필드에 대한 유효성 검사 논리](assets/validation-logic-icon.png) | 필드는 유효성 검사 논리가 적용되는 대상 필드입니다. 참조 필드의 특정 선택 또는 값은 유효성 검사 실패 여부를 결정합니다. 대상 필드와 참조 필드는 유효성 검사 논리에 대해 동일할 수 있습니다. |
| ![참조 필드에 대한 유효성 검사 논리](assets/validation-logic-reference-field.png) | 필드는 유효성 검사 논리의 참조 필드입니다. 이 필드의 특정 선택 또는 값은 대상 필드에서 유효성 검사가 실패하는지 여부를 결정합니다. 대상 필드와 참조 필드는 유효성 검사 논리에 대해 동일할 수 있습니다. |
| ![대상 필드의 기본값 논리](assets/default-value-logic-icon.png) | 필드는 기본값 논리가 적용되는 대상 필드입니다. 참조 필드의 특정 선택 또는 값이 기본값을 결정합니다. 타겟 필드와 참조 필드는 기본값 논리에 대해 동일할 수 있습니다. |
| ![참조 필드의 기본값 논리](assets/default-value-logic-reference-field.png) | 필드는 기본값 논리의 참조 필드입니다. 이 필드의 특정 선택 또는 값이 대상 필드의 기본값을 결정합니다. 타겟 필드와 참조 필드는 기본값 논리에 대해 동일할 수 있습니다. |
| ![대상 필드에 대한 서식 논리](assets/formatting-logic-icon.png) | 필드는 서식 논리가 적용되는 대상 필드입니다. 참조 필드의 특정 선택 항목이나 값에 따라 서식이 결정됩니다. 대상 필드 및 참조 필드는 서식 지정 논리에 대해 동일할 수 있습니다. |
| ![참조 필드에 대한 서식 논리](assets/formatting-logic-reference-field.png) | 필드는 서식 논리의 참조 필드입니다. 이 필드의 특정 선택 또는 값이 대상 필드의 형식을 결정합니다. 대상 필드 및 참조 필드는 서식 지정 논리에 대해 동일할 수 있습니다. |
| ![대상 필드에 대한 편집 논리](assets/editability-logic-icon.png) | 필드는 편집 가능성 논리가 적용되는 대상 필드입니다. 정의된 조건이 충족되는 경우 필드를 편집할 수 있거나 읽기 전용으로 사용할 수 있습니다. 대상 필드 및 참조 필드는 편집 가능 논리에 대해 동일할 수 있습니다. |
| ![참조 필드에 대한 편집 논리](assets/editability-logic-reference-field.png) | 필드는 편집 논리의 참조 필드입니다. 이 필드에서 정의된 조건이 충족되면 대상 필드에 논리가 적용됩니다. 대상 필드 및 참조 필드는 편집 가능 논리에 대해 동일할 수 있습니다. |

[논리 아이콘](assets/custom-form-logic-icon-samples.png)

표시 및 건너뛰기 논리에만 해당하는 경우 필드 설정에서 기존 논리 규칙을 표시할 필드를 선택합니다.

![논리 규칙](assets/form-designer-view-only-logic.png)

## 디스플레이 논리 및 건너뛰기 논리 사용에 대한 고려 사항

* 사용자 지정 필드, 위젯 또는 섹션 구분에 표시 논리를 추가하려면 적어도 하나의 다중 선택 필드(라디오 버튼, 드롭다운 또는 확인란)를 양식에서 그 앞에 배치해야 합니다.
사용자 정의 양식의 사용자 정의 필드 및 위젯에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
* 위젯 또는 섹션 구분에 건너뛰기 논리를 추가할 수 없습니다. 다중 선택 필드(라디오 단추, 드롭다운 또는 확인란)에만 추가할 수 있습니다.
* 다중 옵션 필드의 선택 사항을 표시하거나 숨기려면 표시 또는 건너뛰기 논리를 적용할 수 없습니다. 예를 들어 다른 필드의 표시 또는 건너뛰기 논리에 따라 드롭다운, 확인란 그룹 또는 라디오 버튼 필드에 대해 표시되는 선택 사항을 제한할 수 없습니다.
* 사용자 정의 필드에 대해 다음 내용이 모두 참인 경우 표시 논리와 건너뛰기 논리를 모두 사용자 정의 필드에 추가할 수 있습니다.

   * 객관식 필드(라디오 버튼, 드롭다운 또는 확인란)입니다
   * 앞에 다중 선택 필드가 옵니다.
   * 뒤에 다른 사용자 지정 필드가 옵니다.

* 표시 논리나 건너뛰기 논리를 사용하여 양식을 복사할 경우 해당 논리는 새 사용자 정의 양식에 복사됩니다.
* 개체를 일괄 편집할 때 생략되거나 숨겨진 필드를 포함하여 모든 사용자 정의 필드가 [개체 편집] 상자에 표시됩니다.
* 사용자 정의 양식에 대한 표시 논리 규칙을 만들 때는 다음 사항에 유의하십시오.

   * 표시 논리 문에 포함되지 않은 사용자 정의 필드는 기본적으로 사용자 정의 양식에 표시됩니다.
   * 다중 필드 표시 논리 문을 만들 수 있습니다.
   * 섹션 구분 아래의 모든 필드에 표시 논리가 적용되어 있고 논리의 결과로 해당 필드가 모두 숨겨져 있는 경우 사용자 정의 양식에서 전체 섹션이 숨겨집니다.

## 사용자 정의 양식에 표시 논리 추가

표시 논리는 사용자가 다중 선택 필드에서 특정 값을 선택할 때 양식에 표시되는 사용자 정의 필드를 정의합니다. 값이 선택될 때만 표시되는 대상 필드에 논리가 추가됩니다.

>[!NOTE]
>
>이 절차에서는 표시 논리의 기본 모드를 설명합니다. 고급 디스플레이 논리도 사용할 수 있습니다. 자세한 내용은 이 문서에서 [사용자 정의 양식에 고급 표시 논리 추가](#add-advanced-display-logic-to-a-custom-form)를 참조하십시오.

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다. 하나 이상의 객관식 필드(라디오 버튼, 드롭다운 또는 확인란)를 표시할 대상 필드 앞에 배치해야 합니다.
1. 대상 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **표시** 탭을 선택합니다.
1. **표시 규칙 추가**&#x200B;를 클릭합니다.

   ![디스플레이 논리 빌더](assets/simple-display-logic1.png)

1. 아래 단계에 따라 빌더에 논리 구문을 만듭니다.

   1. 첫 번째 옵션은 정의 필드를 선택하는 것입니다. 대상을 표시하는 선택 값이 있는 필드입니다. 객관식 필드여야 합니다.
   1. 두 번째 옵션은 선택 값을 선택하는 것입니다. 해당 필드에 이미 정의된 값만 사용할 수 있습니다.
   1. 세 번째 옵션은 **선택됨** 또는 **선택되지 않음**&#x200B;입니다. **선택됨**&#x200B;을(를) 선택하면 값을 선택할 때 대상 필드가 표시됩니다. **선택되지 않음**&#x200B;을 선택하면 정의 필드에서 다른 값을 선택하면 대상 필드가 표시됩니다.
   1. **And** 규칙을 논리 문에 추가하려면 방금 만든 규칙 바로 아래에 있는 **규칙 추가**&#x200B;를 클릭합니다. 동일한 프롬프트에 따라 규칙을 빌드합니다. 대상 필드를 표시하려면 And 규칙이 모두 충족되어야 합니다.

      ![디스플레이 논리 빌더](assets/simple-display-logic2.png)

   1. 논리 문에 **Or** 규칙을 추가하려면 논리 빌더 아래쪽의 **규칙 추가**&#x200B;를 클릭하십시오. 그런 다음 Or 영역 내에서 **규칙 추가**&#x200B;를 클릭하고 같은 프롬프트에 따라 규칙을 만듭니다. 하나 이상의 규칙이 충족되면 대상 필드가 표시됩니다.

1. 논리 문 작성을 마치면 **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

## 사용자 정의 양식에 고급 표시 논리 추가

사용자 정의 양식 필드에 대한 고급 표시 논리를 사용하면 공식을 사용하여 복잡한 논리를 작성할 수 있습니다. 이 논리는 한 줄 텍스트, 단락, 서식이 있는 텍스트, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 다중 선택 외부 조회, 기본 필드 참조, 자동 완성, 계산된 날짜, 확인란 그룹 및 라디오 버튼과 같은 필드 유형에 적용할 수 있습니다.

>[!NOTE]
>
>이 절차에서는 표시 논리의 고급 모드에 대해 설명합니다. 기본 디스플레이 논리도 사용할 수 있습니다. 자세한 내용은 이 문서에서 [사용자 정의 양식에 표시 논리 추가](#add-display-logic-to-a-custom-form)를 참조하십시오.

### 예

고급 표시 논리를 사용하여 사용자 역할에 따라 사용자 정의 양식 섹션의 가시성을 제어하고 다른 필드의 상태에 따라 필드의 가시성을 제어할 수 있습니다.

양식의 기본 섹션에는 논리가 적용되지 않으므로 모든 사용자가 항상 볼 수 있습니다.

다음 조건을 사용하면 리소스 관리자의 작업 역할이 있는 사용자가 양식을 볼 때만 리소스 필수 섹션이 표시됩니다.

```IF($$USER.{roleID}="123abc", true)```

```123abc```은(는) 리소스 관리자의 역할 ID를 나타냅니다.

역할에 대해 ![양식 섹션 표시됨](assets/advanced-display-on-form1.png)

다른 역할 ID를 가진 동일한 조건이 프로젝트 재무 KPI 섹션에 적용되어 재무 관리자 역할만 섹션을 볼 수 있도록 정의합니다.

다음 조건을 사용하면 프로젝트가 완료될 때만 판매된 KPI 필드가 표시됩니다. 이 논리는 양식 섹션 대신 필드에 직접 적용됩니다. 필드가 있는 섹션에 이미 정의되어 있으므로 필드를 볼 수 있는 역할을 지정할 필요가 없습니다.

```IF({status}="CPL", true)```

![필드가 전체 프로젝트에 표시됨](assets/advanced-display-on-form2.png)

### 고급 표시 논리 정의

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다.
1. 논리를 적용할 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **표시** 탭을 선택합니다.
1. **고급 모드**&#x200B;를 켭니다.

   단순 표시 논리 모드를 지원하지 않는 필드 유형의 경우 이 옵션이 자동으로 켜질 수 있습니다.

   ![표시 논리에 대한 고급 모드](assets/advanced-display-logic-blank-editor.png)

1. 편집기에서 표시 조건을 작성합니다.

   계산 및 식에 대한 자세한 내용은 [양식에 계산 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

   >[!NOTE]
   >
   >고급 표시 논리는 양식 디자이너 미리 보기 모드에서 지원되지 않습니다.

## 사용자 정의 양식에 건너뛰기 논리 추가

건너뛰기 논리는 사용자가 다중 선택 필드에서 특정 값을 선택할 때 건너뛰는 사용자 정의 양식 필드를 정의합니다. 건너뛴 필드는 양식에서 숨겨집니다. 로직은 건너뛴 필드가 아니라 선택한 정의 필드에 적용됩니다.

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다. 건너뛰기 논리를 위한 정의 필드는 다중 선택 필드(라디오 단추, 드롭다운 또는 확인란)여야 합니다.
1. 정의 필드를 선택하고 화면 왼쪽 하단에서 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **건너뛰기** 탭을 선택합니다.
1. **건너뛰기 규칙 추가**&#x200B;를 클릭합니다.

   ![논리 빌더 건너뛰기](assets/skip-logic1.png)

1. 아래 단계에 따라 빌더에 논리 구문을 만듭니다.

   1. 정의 필드가 빌더에 표시됩니다. 건너뛰기 논리를 적용하기 위해 선택한 필드입니다.
   1. 첫 번째 옵션은 선택 값을 선택하는 것입니다. 필드에 이미 정의된 값만 사용할 수 있습니다.
   1. 두 번째 옵션은 **선택됨** 또는 **선택되지 않음**&#x200B;입니다. **선택됨**&#x200B;을(를) 선택하면 값을 선택할 때 대상 필드가 표시되고 그 사이의 필드는 건너뜁니다. **선택되지 않음**&#x200B;을 선택하면 정의 필드에서 다른 값을 선택할 때 대상 필드가 표시되고 그 사이의 필드는 건너뜁니다.
   1. 세 번째 옵션은 타겟 필드이거나 건너뛸 위치입니다. 필드 이름 또는 **양식의 끝**&#x200B;을(를) 선택하십시오. 옵션을 선택하기 전에 먼저 &quot;empty&quot;라는 단어를 클릭해야 할 수 있습니다.

      ![논리 빌더 건너뛰기](assets/skip-logic2.png)

   1. 논리 문에 **Or** 규칙을 추가하려면 논리 빌더 아래쪽의 **규칙 추가**&#x200B;를 클릭하십시오. 그런 다음 동일한 프롬프트에 따라 옵션을 선택하여 규칙을 빌드합니다. **Or** 규칙 하나가 충족되면 대상 필드가 표시됩니다.

1. 논리 문 작성을 마치면 **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

## 사용자 정의 양식에 기본값 논리 추가

기본값 논리를 사용하면 공식을 사용하여 사용자 정의 양식 필드에 대한 기본값을 구성할 수 있습니다. 정의된 조건이 충족되면 기본값이 표시됩니다. 기본값은 개체 내의 다른 필드를 참조하는 정적 값 또는 동적 값일 수 있습니다. 기본값은 다른 필드를 참조할 수 있지만 양식의 다른 필드가 변경되어도 변경되지 않습니다.

한 줄 텍스트, 단락, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 다중 선택 외부 조회 등의 필드 유형에 고급 기본값 로직을 적용할 수 있습니다. 기본 필드 참조, 자동 완성, 확인란 그룹 및 라디오 단추.

>[!TIP]
>
>사용자 정의 양식이 오브젝트에 첨부된 경우 기본값은 사용자 정의 필드에 한 번만 적용됩니다. 기본값 공식이 다른 필드의 값에 따라 달라지는 경우 사용자 정의 양식을 첨부할 때 다른 필드의 값이 이미 존재해야 합니다.

>[!NOTE]
>
>양식 디자이너의 표준 기본값 논리는 여전히 존재합니다. 두 유형이 동일한 필드에 적용되는 경우 고급 논리가 우선합니다. 표준 기본값 논리에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkbox-groups-and-drop-downs)에서 [라디오 단추, 확인란 그룹 및 드롭다운 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### 예

다음 공식을 사용하여 논리가 적용되는 다중 선택 드롭다운 필드는 프로젝트 상태가 계획인 경우 프로젝트 설명에서 기본값을 가져옵니다.

```
IF({status} = 'PLN', ARRAY({description}, ','))
```

사용자 정의 양식이 프로젝트에 첨부되고 프로젝트 상태가 계획이면 프로젝트 설명 필드 값이 다중 선택 필드의 기본값으로 사용됩니다. 다중 선택 필드이므로 값이 설명과 일치하면 둘 이상의 값을 가져올 수 있습니다. 설명 값이 다중 선택 값 옵션과 일치하지 않으면 다중 선택 필드에 기본값이 없으며 사용자가 드롭다운에서 값을 선택할 수 있습니다.

### 기본값 논리 정의

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다.
1. 논리를 적용할 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **기본값** 탭을 선택합니다.

   ![기본 값 논리 작성기](assets/default-value-blank-editor.png)

1. 편집기에서 기본값 조건을 빌드합니다.

   계산 및 식에 대한 자세한 내용은 [양식에 계산 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

   >[!NOTE]
   >
   >양식 디자이너 미리 보기 모드에서는 기본값 논리가 지원되지 않습니다.

## 사용자 정의 양식에 유효성 검사 논리 추가

유효성 검사 논리는 공식을 사용하여 작성되며, 논리를 필요한 만큼 단순하거나 복잡하게 만들 수 있습니다. 유효성 검사는 다른 필드의 값 또는 객체의 상태를 기반으로 할 수 있으며, 유효성 검사가 실패하는 경우에 대한 오류 메시지를 제공할 수 있습니다.

사용자가 사용자 정의 양식을 작성할 때 논리가 적용된 필드가 정의된 유효성 검사 조건을 충족하면 필드가 강조 표시되고 오류 메시지가 표시됩니다.

한 줄 텍스트, 단락, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 다중 선택 외부 조회, 자동 완성, 날짜, 확인란 그룹 및 라디오 버튼과 같은 필드 유형에 유효성 검사 논리를 적용할 수 있습니다.

### 예

다음 조건을 사용하면 사용자가 메시지를 트리거하는 값을 입력할 때 예산 필드가 필드 아래에 메시지를 표시합니다. 예를 들어 입력한 값이 음수이면 첫 번째 메시지가 표시됩니다. 예산 값을 입력하기 전에 프로젝트 상태를 현재로 변경하려고 하면 두 번째 메시지가 표시됩니다.

```
IF({DE:Budget Field} < 0,
     "Budget cannot be negative",
     IF({DE:Budget Field} == 0 && {status} == "CUR", "Budget must be specified before moving to Current status")
)
```

또 다른 간단한 예는 전화 번호 필드가 유효하려면 특정 자릿수를 포함해야 한다는 것입니다.

다른 필드를 기반으로 한 유효성 검사의 추가 예는 회의실 크기(소규모, 중간 또는 대규모)에 대한 필드와 회의 참석자의 수에 대한 별도의 필드입니다. 각 룸 크기에 대한 인원은 유효성 검사 공식에 기록됩니다. 사용자가 입력한 참석자 수가 선택한 회의실에 비해 너무 많은 경우 오류 메시지가 표시됩니다.

유효성 검사 논리의 추가 예제는 [사용자 지정 양식의 고급 논리 예제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/advanced-logic-examples.md)를 참조하십시오.

### 유효성 검사 논리 정의

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다.
1. 논리를 적용할 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **유효성 검사** 탭을 선택합니다.

   ![유효성 검사 논리 빌더](assets/validation-logic-blank-editor.png)

1. 유효성 검사를 충족하지 않을 때 표시할 오류 메시지를 포함하여 편집기에서 유효성 검사 조건을 작성합니다.

   계산 및 식에 대한 자세한 내용은 [양식에 계산 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

   >[!NOTE]
   >
   >유효성 검사 논리는 양식 디자이너 미리 보기 모드에서 지원되지 않습니다.

## 사용자 정의 양식에 서식 논리 추가

서식 논리는 정의된 조건을 충족하면 필드 값을 강조 표시합니다. 적용된 서식은 여러 필드에서 한 번에 작동합니다.

한 줄 텍스트, 단락, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 다중 선택 외부 조회, 자동 완성, 계산, 날짜, 확인란 그룹 및 라디오 버튼과 같은 필드 유형에 서식 로직을 적용할 수 있습니다.

사용자 정의 양식에 적용되는 서식은 목록 및 보고서에 적용되는 서식과 별개입니다. 보고서 서식에 대한 자세한 내용은 [보기에서 조건부 서식 사용](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)을 참조하십시오.

### 예

다음 조건을 사용하면 사용자가 1000 이상의 값을 입력할 때 예산 필드가 빨간색으로 표시됩니다. 사용자가 500 이상의 값을 입력하면 필드가 노란색으로 표시됩니다.

서식에 대한 마우스 오버 정의를 추가하려면 사용자 정의 양식의 지침 필드를 사용합니다. 예를 들어 예산 필드에 &quot;합리적인 범위 내에서 예산을 입력하십시오. 값이 500이 넘으면 경고 알림이며 1000이 넘으면 너무 높은 것으로 간주됩니다.&quot;

```
IF(
     {DE:Budget Field} >=1000,
     FORMAT($$NEGATIVE),
     IF({DE:Budget Field} >= 500, FORMAT($$NOTICE))
)
```

### 서식 논리 정의

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다.
1. 논리를 적용할 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **서식** 탭을 선택합니다.

   ![서식 논리 빌더](assets/formatting-logic-blank-editor.png)

1. 편집기에서 서식 조건을 작성합니다.

   필드당 최대 5개의 서식 규칙을 추가할 수 있습니다.

   필드 강조 표시 색상 옵션은 다음과 같습니다.

   * `$$POSITIVE (green)`
   * `$$INFORMATIVE (blue)`
   * `$$NEGATIVE (red)`
   * `$$NOTICE (orange)`

   텍스트 서식 옵션은 다음과 같습니다.

   * `$$BOLD`
   * `$$ITALIC`
   * `$$UNDERLINE`

   최대 3개의 추가 텍스트 서식 옵션과 함께 기능당 하나의 색상 옵션만 사용할 수 있습니다. 색상 옵션을 지정하지 않으면 시스템의 기본 색상이 적용됩니다.

   계산 및 식에 대한 자세한 내용은 [양식에 계산 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

   >[!NOTE]
   >
   >양식 디자이너 미리 보기 모드에서는 서식 논리가 지원되지 않습니다.

## 사용자 정의 양식에 편집 논리 추가

편집 논리는 사용자 정의 양식 필드를 편집할 수 있는지 또는 읽기 전용인지 여부를 결정합니다. 이 논리는 공식을 사용하여 작성되며 필드가 정의된 조건을 충족하면 편집 가능 또는 읽기 전용으로 설정할 수 있습니다.

한 줄 텍스트, 단락, 서식이 있는 텍스트, 단일 선택 드롭다운, 다중 선택 드롭다운, 외부 조회, 다중 선택 외부 조회, 자동 완성, 날짜, 확인란 그룹 및 라디오 버튼과 같은 필드 유형에 편집 논리를 적용할 수 있습니다.

### 예

다음 수식을 사용하면 논리가 적용된 필드는 Radio라는 다른 필드에서 Enabled 선택 사항이 선택된 경우에만 편집할 수 있습니다.

```
IF({DE:Radio} = "Enabled", true)
```

다음 공식을 사용하면 설명 필드가 비어 있을 때만 편집할 수 있습니다. 값을 입력하면 읽기 전용이 됩니다.

```
IF(ISBLANK({DE:Description}), true)
```

다음 공식을 사용하면 리소스 관리자의 작업 역할이 있는 사용자가 양식을 볼 때만 논리가 적용된 필드를 편집할 수 있습니다.

```
IF($$USER.{role}.{name}="Resource Manager", true)
```

### 편집 논리 정의

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 새 사용자 정의 양식을 만들거나 기존 양식을 엽니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
1. 필요에 따라 양식에 필드를 추가합니다.
1. 논리를 적용할 필드를 선택하고 **논리 추가**&#x200B;를 클릭합니다.
1. 논리 빌더에서 **편집 가능성** 탭을 선택합니다.

   ![편집 가능 논리 빌더](assets/editability-blank-editor.png)

1. 편집기에서 편집 조건을 작성합니다.

   계산 및 식에 대한 자세한 내용은 [양식에 계산 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) 및 [계산된 데이터 식의 개요](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)를 참조하십시오.

1. **적용**&#x200B;을 클릭합니다.

   논리가 적용되고 논리 아이콘이 양식 디자이너의 대상 필드 및 참조 필드에 추가됩니다.

   >[!NOTE]
   >
   >양식 디자이너 미리 보기 모드에서는 편집 가능 논리가 지원되지 않습니다.
