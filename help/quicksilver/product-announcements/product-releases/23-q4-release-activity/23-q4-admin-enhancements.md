---
title: 2023년 4분기 관리자 개선 사항
description: 2023년 4분기 관리자 개선 사항
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
TQID: https://experienceleague.adobe.com/6-hscCn7M4UgFBhZVCsugo-ulyuFVc4nyBKKVNN3ZiM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 0%

---

# 2023년 4분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2023년 4분기 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 23.10 릴리스를 통해 사용할 수 있습니다.

2023년 4분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2023년 4분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)를 참조하십시오.

## 기존 라이선스 모델 고객이 사용할 수 있는 증명 및 문서 결정

새로운 Adobe Workfront 라이선스 모델로 전환되지 않은 이전 고객은 이제 단일 보고서에서 사용자당 월별 증명/문서 결정 수가 포함된 데이터를 볼 수 있습니다. 이 데이터는 사용자 의사 결정 보고서를 실행할 때 사용할 수 있습니다.

자세한 내용은 [Adobe Workfront의 개체 이해](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 및 [모든 사용자에 대한 증명 및 문서 결정 횟수 보기](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md)를 참조하십시오.

## 이제 사용자 정의 양식의 계산된 필드에서 $$USER 와일드카드를 사용할 수 있습니다.

이제 새 양식 디자이너의 계산된 사용자 지정 필드 및 외부 조회 필드에서 `$$USER` 와일드카드를 사용할 수 있습니다. 계산에서 `$$USER`을(를) 참조하면 현재 사용자의 ID가 추가됩니다. 와일드카드를 다른 필드와 함께 사용할 수도 있습니다. 예를 들어 `$$USER.{name}`은(는) 현재 사용자의 이름을 추가합니다.

계산된 필드에 대한 자세한 내용은 [양식 디자이너를 사용하여 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

## 외부 API의 값 옵션을 사용자 정의 양식에 추가

이제 사용자 지정 양식 디자이너에서 새 필드 형식 **외부 조회**&#x200B;를 사용할 수 있습니다. 외부 시스템에 데이터가 저장된 경우 이 필드 유형을 사용하면 외부 API에서 옵션을 로드하고 사용자 정의 양식의 다른 필드 값을 기준으로 필터링할 수 있습니다.

양식이 오브젝트에 추가되면 API에서 반환된 값이 드롭다운 필드에 나타나고 사용자가 선택할 수 있습니다.

>[!NOTE]
>
>기존 양식 빌더에서는 새 **외부 조회** 필드 유형을 사용할 수 없습니다.

자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
