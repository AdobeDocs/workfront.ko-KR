---
content-type: reference
navigation-topic: search
title: 개체 참조 번호 사용
description: in [!DNL Adobe Workfront], 항목은 개체로 식별됩니다. 객체는 데이터베이스와 일치하며 데이터와 항목을 상호 연결하는 데 사용됩니다. 참조 번호는 같은 이름의 작업과 같이 서로 유사한 두 개체를 구별할 때 유용합니다. 참조 번호를 검색하고 보고서에 포함할 수 있습니다.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 개체 참조 번호 사용

in [!DNL Adobe Workfront], 항목은 개체로 식별됩니다. 객체는 데이터베이스와 일치하며 데이터와 항목을 상호 연결하는 데 사용됩니다.

Workfront은 개체를 만들 때 다음 개체 각각에 고유한 참조 번호를 자동으로 할당합니다.

* 프로젝트
* 작업
* 문제
* 문서

참조 번호는 같은 이름의 작업과 같이 서로 유사한 두 개체를 구별할 때 유용합니다. 참조 번호를 검색하고 보고서에 포함할 수 있습니다.

>[!IMPORTANT]
>
>* [!DNL Workfront] 모든 고객 및 모든 객체에 항상 참조 번호를 할당합니다. 예를 들어 작업을 만들 때 [!DNL Workfront] 참조 번호 00005을 할당할 수 있습니다. 다른 고객이 다음 프로젝트를 만들면 프로젝트에서 사용할 수 있는 다음 참조 번호를 받게 됩니다(예: 00006). 다음에 문제를 만들면 문제를 해결하기 위해 참조 번호 00007 등을 받게 됩니다.
>* 의 객체에 대한 참조 번호 시퀀스를 제어할 수 없습니다 [!DNL Workfront]. 시퀀스는 항상 데이터베이스에 의해 제어됩니다.
>




## 개체의 참조 번호 보기

작업 및 문제에 대해서는 기본적으로 참조 번호가 표시됩니다. 쉽게 구성할 수도 있습니다 [!DNL Workfront] 다른 유형의 객체에 대한 참조 번호를 표시하려면

* [작업 및 문제에 대한 참조 번호 보기](#view-reference-numbers-for-tasks-and-issues)
* [다른 객체에 대한 참조 번호 보기](#view-reference-numbers-for-other-objects)
* [보고서에서 참조 번호 보기](#view-reference-numbers-in-reports)

### 작업 및 문제에 대한 참조 번호 보기

작업이나 문제를 볼 때 기본적으로 참조 번호가 표시됩니다.  참조 번호를 보려면 **[!UICONTROL 작업 세부 사항]** 또는 **[!UICONTROL 문제 세부 정보]** 왼쪽 패널에서 **[!UICONTROL 기본 정보]** 섹션에 자세히 설명되어 있습니다.

![](assets/reference-number-nwe-350x184.png)

### 다른 객체에 대한 참조 번호 보기

객체에 대한 참조 번호를 보려면 사용자 정의 뷰를 생성하거나 기존 뷰를 수정하고 [!UICONTROL 참조 번호] 필드를 보기의 열에 추가합니다. 예를 들어 [!UICONTROL 프로젝트] 를 클릭하여 모든 프로젝트에 대한 참조 번호를 표시합니다.

보기를 만들거나 수정하는 방법에 대한 자세한 내용은 [의 보기 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 보고서에서 참조 번호 보기

를 추가하여 보고서에 개체의 참조 번호를 표시할 수 있습니다 [!UICONTROL 참조 번호] 열을 보고서에 추가합니다.

보고서에 열을 추가하는 방법에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 참조 번호로 개체 검색

[!DNL Workfront] 참조 번호로 객체를 검색할 수 있습니다.

개체의 참조 번호를 **[!UICONTROL 검색]** field 를 누른 다음 **[!UICONTROL Enter 키]**.

Workfront에서 검색하는 방법에 대한 자세한 내용은 [검색 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
