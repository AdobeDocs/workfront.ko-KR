---
product-area: projects
navigation-topic: issue-information
title: 문제를 참조할 때 "opTask" 및 "issue" 사용
description: 문제의 이름이 Adobe Workfront 데이터베이스에 opTask로 표시됩니다. 문제를 참조할 때 문제 필드 이름을 사용해야 하는 경우가 있지만, 대부분의 경우 문제를 참조할 때 문제 대신 opTask 필드 이름을 사용해야 합니다.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 문제를 참조할 때 &quot;opTask&quot; 및 &quot;issue&quot; 사용

문제의 이름이 Adobe Workfront 데이터베이스에 `opTask`(으)로 나타납니다. 문제를 참조하는 데 `issue` 필드 이름을 사용해야 하는 경우가 있지만, 대부분의 경우 문제를 참조할 때 `opTask` 대신 `issue` 필드 이름을 사용해야 합니다.

개체가 Workfront 데이터베이스에 나타나는 방식에 대한 자세한 내용은 [API 탐색기](https://developer.adobe.com/workfront/api-explorer/)를 참조하십시오.

## `opTask` 필드 이름

다음 컨텍스트에서 문제를 참조할 때 `opTask` 필드 이름을 사용하십시오.

* 문제에 대한 텍스트 모드 사용자 지정 보고서를 만들 때 보기, 필터, 그룹화 또는 프롬프트에서 문제를 참조하려고 합니다.

  보고서에서 텍스트 모드를 사용하는 방법에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)를 참조하십시오.

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* 킥스타트 데이터 가져오기 시트의 문제 필드를 업데이트할 때.

  킥스타트를 사용하여 Workfront에서 데이터를 가져오는 방법에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)를 참조하십시오.

## `issue` 필드 이름

다음 컨텍스트에서 문제를 참조하려면 `issue` 필드 이름을 사용하십시오.

* 보고서에서 텍스트 모드를 사용하여 컬렉션의 문제를 참조할 때.
* Workfront API를 사용하여 문제 컬렉션을 참조하는 경우.

컬렉션에 대한 보고에 대한 자세한 내용은 [보고서의 컬렉션 참조](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)를 참조하세요.

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
