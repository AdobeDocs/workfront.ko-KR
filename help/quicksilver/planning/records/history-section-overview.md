---
title: 내역 섹션 개요
description: Adobe Workfront Planning에서 레코드의 오른쪽 패널에서 레코드와 시스템에 의해 기록되는 변경 사항을 검토할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 3%

---

# 내역 섹션 개요

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.

레코드의 오른쪽 패널에는 다음 섹션이 표시됩니다.

* **댓글**: 사용자가 레코드에 추가하는 댓글 및 답글을 표시합니다. Workfront Planning 레코드에서 주석 관리에 대한 자세한 내용은 [레코드 주석 관리](/help/quicksilver/planning/records/manage-record-comments.md).
* **기록**: 사용자가 레코드 필드에 적용한 시스템 기록 변경 사항을 표시합니다.

## 레코드의 내역 섹션 찾기

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 기록 유형이 카드에 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.
레코드 유형 페이지가 열리고 해당 유형의 모든 레코드가 표시됩니다.

1. 다음에서 표 보기 선택 **보기** 드롭다운 메뉴.
1. 테이블 보기에서 레코드 이름을 클릭합니다.

   레코드 페이지가 열립니다. 주석(Comments) 영역은 기본적으로 오른쪽 패널에 열립니다.
1. 다음을 클릭합니다. **내역 표시** 아이콘 ![](assets/show-history-icon.png). 레코드의 필드에 대한 모든 변경 사항은 가장 최근 것부터 시작하여 오른쪽 패널에 표시됩니다.
1. (선택 사항) **내역 숨기기** 아이콘 ![](assets/hide-history-icon.png) 오른쪽 패널을 닫습니다.

## 작업 내역 섹션에 대한 고려 사항

레코드 페이지의 오른쪽 패널에 있는 기록 섹션에서 레코드 필드에 대한 변경 사항을 검토할 수 있습니다.

![](assets/history-area-in-comments.png)

* Workfront Planning은 내역 섹션에 다음 정보를 기록합니다.

   * 모든 필드 변경 사항

   * 값이 변경될 때 필드의 이전 값과 새 값. 이전 값은 취소선 형식으로 표시됩니다.

   * 변경한 사용자의 전체 이름

   * 변경이 발생한 날짜 및 시간 기록.

* 다음 유형의 필드에는 항상 이전 값(취소선 형식)과 새 값이 표시됩니다.

   * 텍스트
   * 단락
   * 통화
   * 일자
   * 숫자
   * 백분율
   * 단일 선택

* 다음 유형의 필드에는 여러 값 중 하나 이상이 제거된 경우에만 이전 값이 취소선 형식으로 표시됩니다.

   * 다중 선택
   * 연결된 레코드 필드
   * 사용자

  변경 사항이 필드에 값을 추가하기만 하면 이전 값은 표시되지 않고 새 필드 값만 표시됩니다.

* 확인란 유형 필드에는 이전 값이 취소선 형식으로 표시되지 않습니다. 필드를 편집하면 변경한 시점의 현재 상태만 표시됩니다.

  Workfront Planning 필드에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md).

* 다음 유형의 필드에 대한 변경 사항은 기록 섹션에 표시되지 않습니다.

   * 연결된(조회) 필드
   * 공식
   * 제작자
   * 만든 날짜
   * 마지막 수정자
   * 마지막 수정일

* 시스템에서 필드를 제거하면 해당 필드에 대한 업데이트가 기록 섹션에 남아 있습니다. 레코드의 내역 섹션에 필드가 제거되었다는 표시가 없습니다.
