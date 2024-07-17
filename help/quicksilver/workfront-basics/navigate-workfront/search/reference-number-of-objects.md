---
content-type: reference
navigation-topic: search
title: 참조 개체 수 사용
description: ' [!DNL Adobe Workfront]에서 항목은 개체로 식별됩니다. 개체는 데이터베이스와 일치하며 데이터와 항목의 상관 관계를 지정하는 데 사용됩니다. 참조 번호는 다른 유사한 두 객체(예: 동일한 이름을 가진 작업)를 구별하는 데 유용합니다. 참조 번호를 검색하여 보고서에 포함할 수 있습니다.'
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 참조 개체 수 사용

[!DNL Adobe Workfront]에서 항목이 개체로 식별됩니다. 개체는 데이터베이스와 일치하며 데이터와 항목의 상관 관계를 지정하는 데 사용됩니다.

Workfront은 객체를 생성할 때 다음 각 객체에 고유 참조 번호를 자동으로 지정합니다.

* 프로젝트
* 작업
* 문제
* 문서

참조 번호는 다른 유사한 두 객체(예: 동일한 이름을 가진 작업)를 구별하는 데 유용합니다. 참조 번호를 검색하여 보고서에 포함할 수 있습니다.

>[!IMPORTANT]
>
>* [!DNL Workfront]은(는) 모든 고객 및 모든 개체에 참조 번호를 계속 할당합니다. 예를 들어, 작업을 만들 때 [!DNL Workfront]에서 작업의 참조 번호를 할당할 수 00005. 다른 고객이 다음에 프로젝트를 만들 경우 해당 프로젝트는 사용 가능한 다음 참조 번호(예: 00006)를 받을 수 있습니다. 다음에 문제를 만들면 문제에 참조 번호 00007 등이 표시될 수 있습니다.
>* [!DNL Workfront]에 있는 개체의 참조 번호 시퀀스를 제어할 수 없습니다. 그 순서는 항상 우리 데이터베이스에 의해 통제된다.
>



## 오브젝트의 참조 번호 보기

작업 및 문제에 대한 참조 번호는 기본적으로 표시됩니다. 다른 형식의 개체에 대한 참조 번호를 표시하도록 [!DNL Workfront]을(를) 쉽게 구성할 수도 있습니다.

* [작업 및 문제에 대한 참조 번호 보기](#view-reference-numbers-for-tasks-and-issues)
* [다른 개체에 대한 참조 번호 보기](#view-reference-numbers-for-other-objects)
* [보고서에서 참조 번호 보기](#view-reference-numbers-in-reports)

### 작업 및 문제에 대한 참조 번호 보기

작업 또는 문제를 볼 때 기본적으로 참조 번호가 표시됩니다.  참조 번호를 보려면 왼쪽 패널에서 **[!UICONTROL 작업 세부 정보]** 또는 **[!UICONTROL 문제 세부 정보]**&#x200B;를 클릭한 다음 개요에서 **[!UICONTROL 기본 정보]** 섹션을 찾습니다.

![](assets/reference-number-nwe-350x184.png)

### 다른 개체에 대한 참조 번호 보기

개체의 참조 번호를 보려면 사용자 지정 보기를 만들거나 기존 보기를 수정하고 [!UICONTROL 참조 번호] 필드를 보기의 열에 추가할 수 있습니다. 예를 들어 [!UICONTROL 프로젝트] 보기를 수정하여 모든 프로젝트에 대한 참조 번호를 표시할 수 있습니다.

보기를 만들거나 수정하는 방법에 대한 자세한 내용은 [보기 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

### 보고서에서 참조 번호 보기

보고서에 [!UICONTROL 참조 번호] 열을 추가하여 보고서에 있는 개체의 참조 번호를 표시할 수 있습니다.

보고서에 열을 추가하는 방법에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

## 참조 번호로 개체 검색

[!DNL Workfront]을(를) 사용하면 참조 번호로 개체를 검색할 수 있습니다.

**[!UICONTROL 검색]** 필드에 개체의 참조 번호를 입력한 다음 **[!UICONTROL Enter]**&#x200B;를 누릅니다.

Workfront 검색에 대한 자세한 내용은 [검색 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)을 참조하십시오.
