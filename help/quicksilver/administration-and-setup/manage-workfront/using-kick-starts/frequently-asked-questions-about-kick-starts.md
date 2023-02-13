---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kicstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 킥시작에 대한 FAQ
description: Kick-Starts를 사용하여 Workfront 데이터 가져오기 및 내보내기에 대한 FAQ 답변을 찾습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 킥시작에 대한 FAQ

다음은 킥스타트에 대한 FAQ입니다.

## 킥시작 파일을 가져오려고 할 때 이 오류가 표시되는 이유는 무엇입니까? &quot;파일이 올바르지만 가져오지 못했습니다.&quot;

### 답변

다음 세 가지 중 하나가 킥시작 파일에서 누락될 수 있습니다.

1. 다음 **isNew** 열은 로 설정되어야 합니다. **TRUE** 가져옵니다. **isNew** 반드시 **TRUE** 왜냐하면 킥스타트를 사용해야만 새 데이터를 가져올 수 있기 때문입니다. 킥스타트를 통해 기존 데이터를 수정할 수 없습니다. 스프레드시트에서 **isNew = FALSE** 그러나 이러한 행은 가져올 수 없습니다.

1. 데이터&#x200B;의 헤더를 시작하기 전에 파일에 빈 행이 한 개 있어야 합니다.
1. Excel 시트&#x200B;에 올바른 이름이 있어야 합니다.

킥스타트 작업 시 먼저 킥스타트 템플릿을 다운로드하고 수동으로 올바른 데이터로 채우고 Adobe Workfront으로 다시 가져오는 것이 좋습니다.

Kick-Starts를 사용하여 Workfront에서 데이터를 올바르게 가져오는 방법에 대한 자세한 내용은 [킥시작 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## 킥시작 파일을 사용하여 Workfront으로 시간을 가져오려고 할 때 이 오류가 표시되는 이유는 무엇입니까? &quot;기본 키 값이 &quot;null&quot;인 사용자를 찾을 수 없습니까?&quot;

### 답변

오류는 시간과 관련된 사용자의 GUID를 참조합니다.

이 문제를 해결하려면

1. 에 대해 빈 킥시작 템플릿을 내보냅니다. **시간** 객체에만 해당됩니다.\
   빈 킥스타트 파일 내보내기에 대한 자세한 내용은 의 &quot;킥스타트 템플릿 내보내기&quot;를 참조하십시오  [킥시작 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. 원래 킥스타트에서 데이터를 수동으로 복사하여 빈 파일에 붙여넣습니다.\
   각 열에 대해 이 작업을 수행합니다.
1. 새 파일을 다시 가져오십시오.\
   킥스타트를 가져왔습니다.

## Kick-Start 가져오기에서 사용자 프로필에 국가 필드를 채우지 않는 이유는 무엇입니까?

### 문제

사용자 킥을 가져올 때(필드로 시작) **setCountry**&#x200B;로 설정되면 해당 데이터가 사용자 프로필의 국가로 전송되지 않습니다.

### 답변

사용자가 UUM(Unified User Management) 또는 IMS(Analysis Workspace System)에 대해 활성화되어 있으면 **국가** 필드는 국가 코드 값(예: 미국, GB, IN)만 허용합니다. 다음 사항을 확인합니다. **setCountry** kick-Start 템플릿의 필드는 가져오기 전에 국가 코드 값을 사용합니다.

Kick-Starts를 사용하여 Workfront에서 데이터를 올바르게 가져오는 방법에 대한 자세한 내용은 [킥시작 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
