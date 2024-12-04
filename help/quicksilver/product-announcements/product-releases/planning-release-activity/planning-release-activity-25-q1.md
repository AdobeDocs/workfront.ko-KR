---
content-type: release-notes
title: 25.1 릴리스에 대한 Adobe Workfront Planning 릴리스 활동
description: 2025년 1분기 Adobe Workfront Planning 제품 릴리스 활동입니다.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '1769'
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

이 문서에서는 2025년 1분기 릴리스 동안 Workfront Planning에 대해 릴리스되는 기능에 대해 설명합니다.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

2024년 8월 28일 일반 출시 이후 Adobe Workfront Planning에 대해 릴리스된 모든 기능 목록에 대해서는 [Adobe Workfront Planning 릴리스 활동: 문서 색인](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)을 참조하십시오.


## 기존 Workfront 필드를 Workfront Planning 레코드 유형으로 가져오기

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 레코드 종류에 필드를 추가할 때 기존 Workfront 사용자 지정 또는 네이티브 필드를 가져와 선택한 레코드 종류에 연결할 수 있는 옵션이 있습니다. 기존 필드를 가져오면 Workfront Planning에서 Workfront 필드의 사본이 만들어집니다. 복사된 필드는 원래 버전과 독립적입니다.

이 개선 이전에는 모든 필드를 수동으로 만들어 레코드 유형과 연결해야 했습니다.

현재 계산된 필드는 지원되지 않습니다.

자세한 내용은 [Adobe Workfront에서 필드 가져오기](/help/quicksilver/planning/fields/import-fields-from-workfront.md)를 참조하십시오.

## CSV 또는 Excel 파일을 가져와 레코드 유형, 레코드 및 필드 만들기

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 CSV 또는 Excel 파일을 가져와서 새 레코드 유형을 가져올 수 있습니다.

다음 정보를 가져옵니다.

* 시트나 파일의 이름을 레코드 유형 이름으로 가져옵니다.

* 모든 열의 첫 번째 행을 새 필드로 가져옵니다. 가져온 각 시트에는 최대 500개의 필드가 있을 수 있습니다.

* 각 행을 새 레코드로 가져옵니다. 각 시트에 최대 10,000개의 레코드가 있을 수 있습니다.

자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

## 수식에서 순환 참조 방지

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

자체 또는 공유 필드에 대한 순환 참조를 만들 수 있는 수식 필드를 편집하거나 만들 때 경고 메시지가 도입되었습니다. 자체 또는 해당 계산에서 참조되는 항목을 참조하는 공식 필드는 저장할 수 없습니다.

자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

## 연결 보기 페이지를 레코드의 페이지에 추가하여 테이블 보기에 연결된 레코드를 표시합니다.

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

레코드의 세부 정보 영역에 페이지를 추가하여 테이블 보기에 연결된 레코드를 표시할 수 있습니다. 연결된 레코드당 한 페이지를 추가할 수 있습니다.

추가된 페이지는 읽기 전용입니다.

자세한 내용은 [레코드 페이지 레이아웃 관리](/help/quicksilver/planning/records/manage-the-record-page.md)를 참조하십시오.

## 요청 영역의 제출됨 섹션에서 새 Workfront 및 계획 탭

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 Workfront의 요청 영역에 있는 제출됨 섹션에서 Workfront Planning 요청을 찾을 수 있습니다. 이제 제출됨 섹션에 다음 탭이 표시됩니다.

* Workfront: Workfront에서 제출된 요청을 표시합니다.
* Planning: Workfront Planning 요청 양식을 사용하여 제출된 요청을 표시합니다.

Workfront Planning 레코드 유형에 요청을 추가하려면 요청 양식에 대한 링크를 사용해야 합니다. Workfront의 요청 영역에서 Workfront Planning 요청을 제출하는 것은 나중에 사용할 수 있습니다.

요청 영역에서 계획 탭을 사용할 수 있으려면 먼저 조직이 Workfront Planning 패키지를 구매해야 합니다.

자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## 이제 요청 양식에서 추가 필드 유형을 지원합니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 Workfront Planning의 레코드 유형 요청 양식에 다음 필드 유형을 추가할 수 있습니다.

* 사용자
* Workfront 연결

이 개선 이전에는 이러한 유형의 필드를 Workfront Planning의 요청 양식에 추가할 수 없었습니다.

자세한 내용은 Adobe Workfront Planning에서 요청 양식 만들기 및 관리(/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 특정 필드 유형이 포함된 요청 양식의 공개 공유 제한

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 27일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스 포함(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스 포함(2025년 1월)

양식에 다음 필드 유형이 포함되어 있으면 더 이상 요청 양식을 공개적으로 공유할 수 없습니다.

* 공식
* Workfront 및 AEM Assets 연결
* 조회 필드
* 사용자

자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.


## 주별 달력 보기에 레코드 표시

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 26일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스 포함(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스 포함(2025년 1월)

이제 주별로 달력 보기에 레코드를 표시할 수 있습니다. 이 개선 이전에는 달력만 월별 보기를 표시할 수 있었습니다.

자세한 내용은 [일정 보기 관리](/help/quicksilver/planning/views/manage-the-calendar-view.md)를 참조하세요.

## 삭제된 레코드 복원

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 22일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

레코드가 삭제되면 이제 30일 동안 최근에 삭제된 저장소로 임시로 이동됩니다. 레코드 유형의 페이지에서 최근에 삭제된 BIN에 액세스할 수 있으며 여기에는 특정 유형의 레코드만 포함됩니다.

Workspace 관리자는 삭제된 후 최대 30일 동안 휴지통에서 레코드를 복원할 수 있습니다. 연결된 레코드 및 해당 필드 정보도 복원됩니다.

이 개선 이전에는 삭제된 레코드를 복원할 수 없었습니다.

자세한 내용은 [삭제된 레코드 복원](/help/quicksilver/planning/records/records-information.md)을 참조하세요.

## 레코드 세부 정보 영역에서 사용할 수 있는 Adobe AI Assistant

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 21일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

작업을 보다 쉽게 수행할 수 있도록 레코드의 세부 사항 미리 보기 또는 레코드 페이지에 Adobe AI Assistant를 추가했습니다. 레코드 페이지 내의 AI Assistant를 사용하여 레코드에 대한 정보를 업데이트할 수 있습니다.

자세한 내용은 [Adobe Workfront Planning AI Assistant 개요](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)를 참조하십시오.

## 기록 페이지에 썸네일 및 표지 이미지를 추가할 때의 새로운 경험

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 20일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스 포함(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스 포함(2025년 1월)

레코드의 미리 보기 또는 페이지를 열고 레코드에 축소판이나 표지 이미지가 없는 경우 이제 헤더에서 레코드 이름 위의 영역을 마우스로 가리켜야 레코드에 표지 및 축소판 이미지를 추가하는 옵션을 볼 수 있습니다. 이 개선 이전에는 축소판 및 표지에 대한 빈 자리 표시자 이미지가 레코드 이름 위에 표시되었습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [레코드에 표지 이미지 추가](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [레코드에 썸네일 이미지 추가](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## 테이블 보기의 백분율 유형 필드에 대한 새 표시 유형

>[!NOTE]
>
>미리보기 릴리스: 2024년 11월 7일, 빠른 릴리스를 위한 프로덕션: 24.12 릴리스(2024년 12월), 분기별 릴리스의 프로덕션: 25.1 릴리스(2025년 1월)

이제 다음 선택 사항 중에서 선택하여 테이블 보기에서 백분율 유형 필드가 표시되는 방식을 변경할 수 있습니다.

* 숫자
* 막대
* 원형

이 표시 유형은 테이블 보기에서만 지원됩니다.

이 개선 이전에는 백분율 값을 숫자로만 표시할 수 있었습니다.

자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

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
