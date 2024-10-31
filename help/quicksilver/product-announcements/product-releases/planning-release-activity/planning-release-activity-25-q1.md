---
content-type: release-notes
title: 25.1 릴리스에 대한 Adobe Workfront Planning 릴리스 활동
description: 2025년 1분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: f30bed961b339e20c0693a8b5e485f872375b688
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Adobe Workfront Planning의 2025년 1분기 릴리스 활동

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새 서비스인 Adobe Workfront Planning을 참조합니다.
>
>Workfront Planning 기능에 액세스하고 사용하려면 Workfront 계획 외에 Workfront Planning 계획을 구매해야 합니다.
>
>Workfront Planning에 액세스하기 위한 전체 요구 사항 목록은 [액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.
>Workfront Planning에 대한 개요는 [Adobe Workfront Planning 개요](/help/quicksilver/planning/general/planning-overview.md)를 참조하십시오.
>

이 문서에서는 2025년 1분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

2024년 8월 28일 일반 출시 이후 Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록에 대해서는 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.

## 이제 연결 필드가 요청 양식에서 지원됩니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 31일, 빠른 릴리스를 위한 프로덕션: 24.11 릴리스(2024년 11월 14일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 Workfront Planning 레코드에 대해 연결된 필드를 레코드 유형 요청 양식에 추가할 수 있습니다.

요청 양식에 Workfront 개체에 대한 연결 조회 필드 또는 연결된 필드를 추가할 수 없습니다.

이 개선 이전에는 이러한 유형의 필드를 Workfront Planning의 요청 양식에 추가할 수 없었습니다.

자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 다른 레코드에 이미 연결된 레코드를 연결할 때 연결 경고

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 31일, 빠른 릴리스를 위한 프로덕션: 24.11 릴리스(2024년 11월 14일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

다른 곳에 이미 연결되어 있고 일대다 또는 일대다 연결 유형을 통해 연결된 레코드 유형에 속하는 레코드를 연결하려고 하면 레코드가 이미 연결되어 있다는 경고가 표시됩니다. 연결을 사용하여 앞으로 이동하겠다고 확인하면 선택한 레코드가 원래 레코드에서 제거되고 현재 편집 중인 레코드에 추가됩니다.

연결 유형에 대한 자세한 내용은 [연결된 레코드 유형 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하십시오.

## 레코드의 세부 정보 페이지에 있는 필드에 대한 설명이 있는 새 정보 아이콘

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 30일, 빠른 릴리스를 위한 프로덕션: 24.11 릴리스(2024년 11월 14일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

레코드 페이지의 필드 이름 오른쪽에 정보 아이콘을 추가했습니다. 설명이 있는 경우 정보 아이콘을 클릭하면 필드에 대한 설명이 표시됩니다. 이 개선 이전에는 필드 이름을 마우스로 가리키면 필드에 대한 설명이 표시되었습니다.

자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

## Planning 연결에 대한 새 Workfront 필드 유형

>[!NOTE]
>
>미리보기 릴리스: 2024년 10월 24일, 빠른 릴리스를 위한 프로덕션: 24.11 릴리스(2024년 11월 14일), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

Workfront 개체를 Workfront Planning 레코드에 계속 브리징하기 위해 Workfront 사용자 정의 양식에 Planning 연결이라는 새 필드 유형을 추가했습니다. 이제 Workfront 사용자 정의 양식 및 궁극적으로 Workfront 개체에 이 필드 유형을 추가하여 다음을 수행할 수 있습니다.

* Workfront 개체에 연결된 레코드를 사용자 정의 양식으로 표시합니다.

* Workfront 객체에서 Workfront Planning 레코드를 연결하고 연결을 해제합니다.

모든 객체 유형의 양식에 새 필드를 추가할 수 있습니다. 그러나 Portfolio, 프로그램, 프로젝트, 회사, 그룹 같은 Workfront Planning 레코드 유형에서 연결할 수 있는 Workfront 개체에 첨부된 양식에서만 필드의 정보를 편집할 수 있습니다.

Workfront 객체에 대한 Planning 연결 필드를 일괄적으로 편집할 수는 없습니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

[이 기능의 비디오 데모 보기](https://video.tv.adobe.com/v/3435633/){target=_blank}
