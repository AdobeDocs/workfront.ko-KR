---
title: 사용자 지정 양식 개선 사항
description: 22.2 릴리스에서 사용자 지정 양식을 관리하기 위해 다음과 같은 중요한 사항이 개선되었습니다.
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 사용자 지정 양식 개선 사항

22.2 릴리스에서 사용자 지정 양식을 관리하기 위해 다음과 같은 중요한 사항이 개선되었습니다.

## 자산 위젯 추가

사용자 지정 양식에 이미지를 포함할 수 있습니다. 이를 통해 보다 인터랙티브하고 시각적인 방식으로 사용자 지정 양식 사용자와 통신할 수 있습니다. 추가 위젯 유형이 곧 제공될 예정입니다.

![](assets/image-in-custom-form.png)

위젯이 포함된 사용자 지정 양식이 개체에 첨부된 경우 개체를 사용하여 작업하는 사용자는 다음 영역에서 위젯을 볼 수 있습니다.

* 개체의 세부 정보 영역(예: 프로젝트의 경우 프로젝트 세부 정보 영역)&#x200B;입니다

   ![](assets/see-image-details-page.png)

* 개체의 편집 상자에 새 Adobe Workfront 경험 모양과 느낌(예: 프로젝트 편집 및 작업 편집 상자)이 &#x200B; 있습니다

   ![](assets/image-see-in-edit.png)

현재 사용자는 다음 영역에서 위젯을 볼 수 &#x200B; 없습니다.

* 목록 및 보고서
* 홈 및 요약
* 개체의 편집 상자에 새 Adobe Workfront 경험 모양과 느낌(예: 비용 편집 상자)이 없는 경우
* Workfront &#x200B; 모바일 앱

사용자 지정 양식에 위젯을 추가하는 방법에 대한 자세한 내용은 [사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 사용자 지정 양식을 여러 개체 유형과 연결

여러 객체 유형을 새로운 사용자 정의 양식과 연결할 수 있습니다.

![](assets/new-custom-form-object-types.png)

또는 기존 사용자 지정 양식:

![](assets/add-object-type-existing-form.png)

이를 통해 프로젝트, 작업, 문제 및 사용자 지정 양식에 대해 지원되는 다른 유형의 개체에 사용할 단일 사용자 지정 양식을 만들 수 있습니다.

이 기능은 사용자 지정 양식과 해당 데이터를 변환된 개체로 가져올 수 있으므로 문제 또는 작업을 변환할 때 특히 유용합니다. 더 이상 다양한 개체 유형에 대해 동일한 사용자 지정 양식의 정확한 사본을 만들고 유지 관리할 필요가 없으며, 사용자 지정 양식을 프로젝트에 수동으로 추가합니다.

>[!INFO]
>
>**예:**
>
>누군가 내부 IT 요청(문제)을 제출하고 첨부된 사용자 지정 양식에 필요한 세부 정보를 제공합니다.
>
>작업을 수행할 사용자를 위해 문제를 프로젝트로 변환합니다.
>
>제출자의 세부 사항이 포함된 사용자 지정 양식은 Issue 및 Project 개체 유형과 모두 연결되어 있으므로 사용자 지정 양식과 이러한 모든 세부 정보가 변환 중에 프로젝트에 전달됩니다.

>[!NOTE]
>
>변환이 수행되면 사용자 지정 양식이 변환하려는 개체 유형과 이미 연결되어 있어야 합니다.

자산 위젯을 사용자 지정 양식에 추가하는 방법에 대한 지침은 [사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

다중 개체 사용자 지정 양식을 만들거나 편집할 때 다음 사항을 고려하십시오.

* [섹션 브레이크에 대한 권한 옵션](#permission-options-for-section-breaks)
* [계산된 사용자 지정 필드 호환성](#calculated-custom-field-compatibility)
* [사용자 정의 양식에서 객체 유형을 삭제하는 것에 대한 주의](#caution-about-deleting-an-object-type-from-a-custom-form)

### 섹션 브레이크에 대한 권한 옵션

[문제], [작업], [프로젝트] 및 [사용자] 객체 유형에 사용할 수 있는 섹션 브레이크 권한 옵션 집합에는 다른 모든 객체 유형에 대한 권한 옵션 집합보다 한 가지 더 많은 권한 옵션이 있습니다. 제한된 편집.

![](assets/section-break-permissions-limited-edit.png)

다른 모든 객체 유형(Portfolio, 문서, 프로그램, 비용, 회사, 이터레이션, 청구 레코드 및 그룹)에 사용할 수 있는 섹션 브레이크 권한 집합에는 제한된 편집이 포함되지 않습니다.

![](assets/section-break-permissions-no-limited-edit.png)

이 두 그룹의 객체 유형과 연관된 사용자 지정 양식에서는 모든 객체 유형에 대해 작동하는 공통 섹션 나누기 권한 집합을 사용합니다. 특히, 이 공통 집합에서는 [제한된 편집] 권한 옵션을 사용하지 않고 [제한된 편집] 권한 옵션의 [편집] 권한 옵션으로 대체합니다. 편집 옵션은 모든 객체 유형과 호환됩니다.

사용자 지정 양식에 이미 있는 다른 개체 유형과 다른 사용 권한 옵션을 사용하는 개체 유형을 연결하면 메시지에 표시되고 공통 사용 권한 옵션 집합으로 전환할 수 있는 사용 권한 옵션이 양식에 사용됩니다. 이 변경 사항은 섹션 브레이크 아래에 있지 않더라도 모든 필드에 적용됩니다.

자세한 내용은 [사용자 지정 양식에 섹션 브레이크 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### 계산된 사용자 지정 필드 호환성

다중 개체 사용자 지정 양식에서 계산된 필드가 양식의 모든 관련 개체 유형(예: 여러 개체 유형에 사용할 수 있는 {name}, {description} 및 {entryDate})에 사용할 수 있는 필드를 참조하는 경우 어떤 개체에 연결하든 데이터가 올바르게 계산됩니다.

예를 들어 프로젝트 및 문제에 대한 다중 개체 양식이 있고 {name} 식이 들어 있는 계산된 필드를 추가한 경우 양식을 프로젝트에 추가할 때 필드에 프로젝트 이름이 표시되고, 양식을 작업에 추가할 작업 이름이 표시됩니다.

그러나 양식의 계산된 필드가 양식의 모든 개체 유형과 호환되지 않는 필드를 참조하는 경우 메시지를 통해 조정을 수행합니다.

>[!INFO]
>
>**예:** 작업 개체 유형과 연결된 사용자 지정 양식에서는 기본 제공 필드 지정 대상: 양식을 작업에 첨부할 때마다 담당 주 할당자의 이름을 표시할 수 있도록 이름을 지정합니다.
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>나중에 사용자 지정 양식에 프로젝트 개체 유형을 추가합니다. 경고 메시지는 프로젝트 개체 유형이 계산된 사용자 지정 필드와 호환되지 않음을 알려줍니다. 지정된 대상 필드를 프로젝트에 사용할 수 없기 때문입니다.

이 경우 다음 중 하나를 수행할 수 있습니다.

* 사용자 지정 양식에서 호환되지 않는 두 항목 중 하나(개체 유형 또는 참조된 필드)를 제거합니다.
* 두 항목을 모두 유지하고 와일드카드 필터 변수를 사용하십시오 `$$OBJCODE` 를 IF 표현식의 조건으로 사용하여 In Charge 필드의 두 가지 다른 버전을 만듭니다. 따라서 양식이 첨부된 객체 유형에 관계없이 필드가 성공적으로 작동할 수 있습니다.

   Assigned To가 내장된 것은 아니지만 위의 예를 사용합니다. 프로젝트에 대한 이름 필드에 기본적으로 제공되는 소유자 필드가 있습니다. 수동으로 변경하지 않는 한 프로젝트를 생성한 사람의 이름으로 자동으로 채워집니다. 따라서 사용자 지정 담당자 필드에서 `$$OBJCODE` 사용자 지정 양식이 프로젝트에 첨부된 경우 소유자 필드를 참조하고 지정 대상: 양식에 작업이 첨부된 경우 이름 필드:

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  필드 이름 앞에 객체 유형을 추가하면 해당 객체 상위 객체가 참조되므로 사용할 수 없습니다 `{project}.{name}` 프로젝트에 사용할 수 있지만 작업에 사용할 수 있습니다.

사용자 지정 양식에 계산된 사용자 지정 필드를 추가하는 방법에 대한 지침은 [사용자 지정 양식에 계산된 데이터 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

와 같은 변수에 대한 자세한 정보 `$$OBJCODE`를 참조하십시오. [와일드카드 필터 변수](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### 사용자 정의 양식에서 객체 유형을 삭제하는 것에 대한 주의

언제든지 사용자 지정 양식에서 객체 유형을 삭제할 수 있지만, 이러한 작업은 신중하게 수행해야 합니다. 사용자가 삭제하려는 유형의 개체에 사용자 지정 양식을 이미 첨부하고 해당 개체에 데이터를 추가한 경우 해당 데이터는 양식에서 해당 개체 유형을 삭제할 때 영구적으로 삭제됩니다.

또한 사용자 지정 양식을 사용하는 사용자에게 삭제한 것을 알리는 알림 시스템이 없습니다.

자세한 내용은 [시스템에서 사용자 지정 필드 또는 위젯 삭제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
