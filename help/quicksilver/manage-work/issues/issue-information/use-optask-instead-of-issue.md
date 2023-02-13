---
product-area: projects
navigation-topic: issue-information
title: 문제를 참조할 때 "opTask" 및 "issue"를 사용합니다
description: 문제 이름이 Adobe Workfront 데이터베이스에 opTask로 표시됩니다. 문제 필드 이름을 사용하여 문제를 참조해야 하는 경우가 있지만, 대부분의 경우 문제를 참조할 때 문제 대신 opTask 필드 이름을 사용해야 합니다.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# 문제를 참조할 때 &quot;opTask&quot; 및 &quot;issue&quot;를 사용합니다

문제 이름이 `opTask` ( Adobe Workfront 데이터베이스)를 참조하십시오. 하지만 `issue` 문제를 참조하는 필드 이름, 대부분의 경우 `opTask` 필드 이름 `issue` 문제를 참조할 때

Workfront 데이터베이스에 개체가 표시되는 방법에 대한 자세한 내용은 [API 탐색기](https://one.workfront.com/s/api-explorer).

## `opTask` 파일

를 사용하십시오 `opTask` 다음 컨텍스트에서 문제를 참조할 때 필드 이름입니다.

* 문제에 대한 텍스트 모드 사용자 지정 보고서를 만들고 보기, 필터, 그룹화 또는 프롬프트의 문제를 참조하려는 경우.

   보고서에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Kick-Start Data Importer 시트의 문제 필드를 업데이트할 때

   Kick-Start를 사용하여 Workfront에서 데이터를 가져오는 방법에 대한 자세한 내용은 [킥시작 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` 필드 이름

를 사용하십시오 `issue` 다음 컨텍스트에서 문제를 참조하는 필드 이름:

* 보고서에서 텍스트 모드를 사용하여 컬렉션에서 문제를 참조할 때.
* Workfront API를 사용하여 문제 컬렉션을 참조하는 경우.

컬렉션에 대한 보고에 대한 자세한 내용은 [보고서에서 컬렉션 참조](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://one.workfront.com/s/api-explorer" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
