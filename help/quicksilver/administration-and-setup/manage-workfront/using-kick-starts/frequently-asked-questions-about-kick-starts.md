---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: 킥스타트, 킥스타트, 킥스타트, 킥스타트
navigation-topic: use-kick-starts
title: 킥스타트에 대한 FAQ
description: 킥스타트를 사용하여 Workfront 데이터 가져오기 및 내보내기에 대한 FAQ에 대한 답변을 찾을 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 킥스타트에 대한 FAQ

킥스타트에 대한 FAQ는 다음과 같습니다.

## 킥스타트 파일을 가져오려고 할 때 이 오류가 발생하는 이유는 무엇입니까: &quot;파일은 올바르지만 아무것도 가져오지 않았습니다.&quot;

### 답변

다음 세 가지 중 하나가 킥스타트 파일에서 누락될 수 있습니다.

1. 가져올 모든 항목에 대해 **isNew** 열을 **TRUE**(으)로 설정해야 합니다. 킥스타트를 사용해야 새 데이터를 가져올 수 있으므로 **isNew**&#x200B;은(는) **TRUE**&#x200B;이어야 합니다. 킥스타트를 통해 기존 데이터를 수정할 수 없습니다. 스프레드시트에 **isNew = FALSE**&#x200B;인 다른 행이 있을 수 있지만 이러한 행은 가져오지 않습니다.

1. 데이터 헤더&#x200B;이 시작되기 전에 파일에 빈 행이 하나 있어야 합니다.
1. &#x200B; Excel 시트의 이름은 정확해야 합니다.

킥스타트를 사용하여 작업할 때 먼저 킥스타트 템플릿을 다운로드하고 수동으로 올바른 데이터로 채운 다음 다시 Adobe Workfront으로 가져오는 것이 좋습니다.

킥스타트를 사용하여 Workfront에서 데이터를 올바르게 가져오는 방법에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)를 참조하십시오.

## 킥스타트 파일을 사용하여 시간을 Workfront으로 가져오려고 할 때 이 오류가 발생하는 이유는 무엇입니까: &quot;기본 키 값이 &quot;null&quot;인 사용자를 찾을 수 없습니까?&quot;

### 답변

오류는 시간과 연결된 사용자의 GUID를 참조합니다.

해결 방법:

1. **Hours** 개체에 대해서만 빈 킥스타트 템플릿을 내보냅니다.\
   빈 킥스타트 파일 내보내기에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)에서 &quot;킥스타트 템플릿 내보내기&quot;를 참조하십시오.

1. 원본 킥스타트에서 데이터를 수동으로 복사하여 빈 파일에 붙여넣습니다.\
   각 열에 대해 이 작업을 수행합니다.
1. 새 파일을 다시 가져오십시오.\
   킥스타트를 성공적으로 가져왔습니다.

## 킥스타트 가져오기에서 사용자 프로필에 국가 필드가 채워지지 않는 이유는 무엇입니까?

### 문제

필드 **setCountry**&#x200B;로 User Kick-Start를 가져올 때 해당 데이터가 사용자 프로필의 국가로 전달되지 않습니다.

### 답변

사용자가 UUM(Unified User Management) 또는 IMS(Adobe Identity Management System)에 대해 활성화된 경우 **국가** 필드에는 국가 코드 값(예: US, GB, IN)만 허용됩니다. 가져오기 전에 킥스타트 템플릿의 **setCountry** 필드에서 국가 코드 값을 사용하고 있는지 확인하십시오.

킥스타트를 사용하여 Workfront에서 데이터를 올바르게 가져오는 방법에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)를 참조하십시오.
