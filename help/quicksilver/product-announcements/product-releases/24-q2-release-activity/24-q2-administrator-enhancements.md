---
title: 2024년 2분기 관리자 개선 사항
description: 2024년 2분기 관리자 개선 사항
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 2551089a20d3301ff1cf7dd633114dbb5235e959
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# 2024년 2분기 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 2024년 2분기 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2024년 2분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [2024년 2분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## 이제 새로운 패키지 유형에 JumpSeat 통합을 사용할 수 있습니다.

>[!NOTE]
>
>미리보기 릴리스: 2024년 2월 26일, 빠른 릴리스를 위한 프로덕션: 24.3 릴리스 포함(2024년 3월 14일), 모든 고객을 위한 프로덕션: 24.4(2024년 4월)

이제 새로운 패키지 유형(예: Select, Prime 또는 Ultimate) 중 하나를 사용하는 계정에서 기존 JumpSeat 통합을 사용할 수 있습니다. 통합을 활성화하려면 여전히 활성 JumpSeat 구독이 있어야 합니다.

JumpSeat 통합에 대한 자세한 내용은 [JumpSeat 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Workfront 기본 필드는 양식 디자이너 베타에서 사용할 수 있습니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 2월 29일, 빠른 릴리스를 위한 프로덕션: 24.3 릴리스 포함(2024년 3월 14일), 모든 고객을 위한 프로덕션: 24.4(2024년 4월)

이제 Workfront의 기본 필드를 사용하여 사용자 정의 양식에 추가할 수 있습니다. 이 새 필드 유형을 사용하면 사용자 정의 필드에서 기존 데이터를 다시 생성하지 않고도 데이터를 논리적으로 구성하고 사용자에게 제공할 수 있습니다.

사용자 정의 양식 필드 목록에서 네이티브 필드 를 선택하여 양식 디자이너에 필드를 추가한 후에는 해당 양식의 개체에 대한 네이티브 필드를 선택할 수 있습니다. 예를 들어 양식 디자이너 상단의 개체 유형 목록에 프로젝트가 표시되면 프로젝트에 대한 기본 필드는 선택할 수 있지만 작업에만 해당하는 필드는 선택할 수 없습니다.

사용자 정의 양식을 오브젝트에 첨부하면 필드가 오브젝트 데이터에서 채워집니다. 예를 들어 프로젝트에 첨부된 사용자 정의 양식의 설명 필드는 프로젝트 설명을 가져옵니다. (데이터가 없는 경우 필드에 &quot;N/A&quot;가 표시될 수 있습니다.)

사용자 정의 양식에 사용된 기본 필드는 디자이너의 필드 라이브러리에서 다시 사용할 수 있게 되며, 설정 > 사용자 정의 Forms > 필드 영역에도 표시되므로 해당 필드가 사용되는 양식을 확인할 수 있습니다.

이 기능은 기존 양식 빌더가 아닌 양식 디자이너 Beta에서만 사용할 수 있습니다.

이 기능에 대한 Experience League 문서는 3월 7일까지 업데이트됩니다.

## 이제 Adobe IMS로 마이그레이션한 조직에서 속성 매핑을 사용할 수 있습니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 2월 22일, 모든 고객의 프로덕션: 2024년 2월 22일

이제 Workfront 시스템 관리자는 Adobe IMS로 마이그레이션한 조직에 대한 사용자 속성 매핑을 설정할 수 있습니다. 이렇게 하면 사용자 정보를 조직의 SSO(Single Sign-On) 공급자에서 Workfront으로 전달할 수 있으므로 사용자의 데이터를 Workfront과 SSO 공급자 모두에 입력할 필요가 없습니다.

이전에는 Adobe IMS에 아직 온보딩되지 않은 조직에서만 이 기능을 사용할 수 있었습니다.

속성 매핑 구성에 대한 지침은 **Adobe 통합 경험의 사용자 속성 매핑** 이 문서에서 [사용자 속성 매핑 및 새 사용자 자동 프로비저닝](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## 이제 양식 디자이너 베타에서 건너뛰기 논리 및 표시 논리를 사용할 수 있습니다

>[!NOTE]
>
>미리보기 릴리스: 2024년 2월 8일, 빠른 릴리스를 위한 프로덕션: 24.2 릴리스 포함(2024년 2월 15일), 모든 고객을 위한 프로덕션: TBD

이제 양식 디자이너 베타에서 기존 표시 및 건너뛰기 논리를 편집하고 새 논리를 사용자 정의 양식에 추가할 수 있습니다. 사용하기 쉬운 논리 빌더를 사용하여 양식의 선택 사항을 기반으로 표시하거나 건너뛸 필드를 정의할 수 있습니다.

양식 디자이너 캔버스의 필드에 있는 아이콘은 해당 필드에 논리가 구성되었거나 필드가 다른 필드에 구성된 논리 규칙에 사용되었음을 나타냅니다.

자세한 내용은 [양식 디자이너를 사용하여 표시 논리 및 건너뛰기 논리 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).