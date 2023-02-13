---
content-type: release-notes
keywords: 메모,분기별,업데이트,릴리스
navigation-topic: 2021-2-release-activity
title: 21.2 기타 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 21.2 릴리스 개요를 참조하십시오.
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2 기타 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.2 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 5월 10일이 있는 프로덕션 환경에서 사용할 수 있습니다. 21.2 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.2 릴리스 개요](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 우리는 이제 공식적으로 Adobe Workfront에 있습니다

Workfront은 Adobe Workfront으로 브랜드를 변경했습니다.

Adobe Workfront 애플리케이션 및 고객 관련 웹 사이트에서 가장 두드러진 영역이 이제 업데이트됩니다. 다른 지역은 곧 업데이트될 예정입니다.

**업데이트된 영역**

* 로그인 화면, 위쪽 탐색, 교정
* 레이아웃 템플릿 UI, 기본 메뉴, 사용자 지정 Forms 내보내기(새 Adobe Workfront 경험에서만 사용 가능)
* Workfront 모바일 앱(iOS 및 Android)

곧 업데이트되는 영역

* 데스크탑 및 모바일용 언어 교정 앱
* 목록 및 보고서에 대한 PDF 내보내기
* 브라우저 탭의 favicon 아이콘

**나중에 업데이트되는 영역**

* 이메일 알림

## 전자 허용 목록에 추가하다 메일 유효성 검사

>[!NOTE]
>
>새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이메일를 사용하는 경우 허용 목록에 추가하다, 이제 새 사용자 이메일 주소와 업데이트된 사용자 이메일 주소의 유효성이 허용 목록에 추가하다 확인됩니다. 새 사용자를 추가하거나 기존 사용자를 편집하고에 이메일 도메인이 아닌 이메일 도메인을 입력하면 사용자가 이메일 메시지를 허용 목록에 추가하다 받지 못함을 알리는 메시지가 표시됩니다. 여전히 사용자 프로필을 저장할 수 있지만, 사용자가 이메일을 허용 목록에 추가하다 받을 수 있도록 도메인에 도메인을 추가해야 합니다.

자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 개체 헤더의 새로운 모양 및 느낌

>[!NOTE]
>
>이 기능은 2020년 3월 10일에 프로덕션 환경에 릴리스되었습니다.
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

이제 각 개체 헤더에는 정보 계층 구조를 강화하고 사용자가 표시되는 페이지를 보다 명확하게 이해할 수 있도록 하기 위해 다음을 포함합니다.

* 각 객체 유형에 대한 보다 현대적인 컬러풀한 아이콘
* 개체 이름 위에 나열된 개체 유형
* 업데이트된 글꼴 스타일 및 텍스트 크기
* 기타 부분 스타일 변경 사항

이전에는 개체 제목 오른쪽에 개체 이름이 표시된 아이콘과 배지가 없었습니다.

Enhanced Analytics, Resource Management 등과 같은 새로운 Workfront 환경에서 영역의 페이지 헤더도 이러한 업데이트된 모양과 느낌을 갖습니다.

새 Workfront 환경의 새 개체 헤더에 대해 자세히 알려면 다음을 참조하십시오 [새 개체 머리글](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## 개체 상태 검색 응답에 대한 업데이트

이제 Workfront은 개체 상태를 새로운 방식으로 저장합니다.

이러한 변경 사항은 상태 검색 요청이 수행되는 방식에 영향을 주지 않습니다. 그러나 개체 상태 검색이 포함된 API 요청은 불완전한 그룹 상태 목록을 반환합니다.

자세한 내용은 [핵심 API 변경 사항: 상태 검색 응답](../../../wf-api/api/api-changes-search.md) .

## 이벤트 구독 페이로드가 ID로 끝나는 모든 필드를 포함하도록 업데이트되었습니다

이제 모든 이벤트 구독 페이로드에는 &quot;ID&quot;로 끝나는 모든 필드가 포함됩니다.

각 객체에는 ID로 끝나는 고유한 관련 필드 세트가 포함된 고유한 관련 필드 세트가 있습니다. 즉, 각 페이로드에는 ID로 끝나는 해당 개체의 모든 연결된 필드가 포함되어 있지만 각 개체에는 ID로 끝나는 다른 필드 세트가 있습니다.

## Blueprint Beta를 이제 미리 보기에서 사용할 수 있습니다.

>[!NOTE]
>
>이 기능은 올해 말 21.3 릴리스까지 프로덕션 환경에서 일반적으로 사용할 수 없습니다. 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

Blueprint는 기본 구성 요소를 제공하여 사용자 성장에 따라 성장하는 작업 관리 시스템을 만드는 데 도움이 됩니다. 시스템 관리자는 Blueprint 카탈로그를 탐색하고 사용 가능한 프로젝트 템플릿을 설치할 수 있습니다.

자세한 내용은 [블루프린트](../../../administration-and-setup/blueprints/blueprints.md).
