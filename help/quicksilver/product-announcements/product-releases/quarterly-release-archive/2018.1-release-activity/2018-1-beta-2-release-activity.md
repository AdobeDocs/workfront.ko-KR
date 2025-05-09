---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2 릴리스 활동
description: 이 페이지에서는 2018.1 Beta 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 12월 14일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 3월에 사용할 수 있습니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# 2018.1 Beta 2 릴리스 활동

이 페이지에서는 2018.1 Beta 2 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 12월 14일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2018년 3월에 사용할 수 있습니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2018.1의 모든 변경 사항 목록은 다음을 참조하십시오.  [2018.1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 2 릴리스에는 Workfront 관리자와 기타 사용자 모두를 위한 개선 사항이 포함되어 있습니다.

관리자용 **1&rbrace;**

* [사용자 및 레이아웃 템플릿을 위한 그룹 관리](#group-administration-for-users-and-layout-templates)

**모든 사용자용**

* [시스템 전체 와이드스크린 디스플레이](#system-wide-widescreen-display)
* [간트 차트에서 타임라인 스냅숏 크기 조정](#resize-timeline-snapshot-on-the-gantt-chart)
* 비즈니스 사례의 [대화형 리소스 플래너](#interactive-resource-planner-in-the-business-case)
* [리소스 플래너의 시각화 - 사용자 할당 차트](#visualization-in-the-resource-planner-user-allocation-chart)
* [홈 영역의 개선 사항](#improvements-in-the-home-area)
* [새 증명 뷰어 개선 사항](#new-proofing-viewer-improvements) 

## 사용자 및 레이아웃 템플릿을 위한 그룹 관리 {#group-administration-for-users-and-layout-templates}

이제 Workfront에서 그룹 관리자를 지정할 수 있습니다. 그룹 소유자 필드의 이름이 그룹 관리자로 변경되었으며 그룹 관리자로 지정된 사용자에게는 자신이 관리하는 그룹의 사용자 및 레이아웃 템플릿을 관리할 수 있는 추가 권한이 있습니다.

* [그룹 관리자의 사용자 관리](#user-management-by-group-administrator)
* [그룹 관리자별 레이아웃 템플릿 관리](#layout-template-management-by-group-administrators)

### 그룹 관리자별 사용자 관리 {#user-management-by-group-administrator}

**그룹 관리자**&#x200B;의 새로운 개념을 소개합니다. 이를 지원하기 위해 **그룹 소유자** 필드의 이름이 **그룹 관리자**(으)로 변경되었으며 그룹 관리자로 지정된 사용자에게는 사용자 및 그룹을 관리할 수 있는 추가 권한이 있습니다.

그룹 관리자는 그룹 소유자가 이전에 사용자를 관리해야 했던 권한 외에도 그룹 관리자로 설정된 그룹 내에서 사용자를 관리할 때 다음과 같은 추가 액세스 권한을 갖습니다.

* 자신이 관리하는 그룹에 속한 다른 사용자로 로그인합니다.
* 자신이 관리하는 그룹에 속한 다른 사용자의 암호를 재설정합니다.
* 해당 그룹에서 관리하는 레이아웃 템플릿을 만듭니다. 

이 변경 이전에는 Workfront 관리자만 이러한 기능을 수행할 수 있었습니다.

그룹 관리자에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)의 &quot;그룹 관리자 이해&quot; 섹션을 참조하십시오.

### 그룹 관리자별 레이아웃 템플릿 관리 {#layout-template-management-by-group-administrators}

레이아웃 템플릿과 연결할 수 있는 **관리 액세스 권한이 있는 그룹**&#x200B;의 새로운 개념을 소개합니다.

이 그룹에서 그룹 관리자로 지정된 사용자는 해당 레이아웃 템플릿을 관리하고 새 레이아웃 템플릿을 만들 수 있는 액세스 권한을 가집니다. 여기서 관리하는 그룹은 템플릿의 관리 그룹입니다. 

이 변경 이전에는 Workfront 관리자만 레이아웃 템플릿을 만들 수 있었습니다.

레이아웃 템플릿 만들기에 대한 자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

## 시스템 와이드스크린 디스플레이 {#system-wide-widescreen-display}

이제 Workfront에 페이지를 표시하면 전체 브라우저 창이 자동으로 채워지고 화면 크기에 맞게 조정됩니다.

이 변경 이전에는 다음 오브젝트와 관련된 페이지만 와이드스크린으로 표시되었습니다.

* 프로젝트
* 작업
* 문제
* 보고서
* 대시보드
* 캘린더

## 간트 차트에서 타임라인 스냅샷 크기 조정 {#resize-timeline-snapshot-on-the-gantt-chart}

이제 타임라인 스냅샷을 확장하여 간트 차트에 전체 프로젝트를 표시할 수 있습니다.

이 기능이 향상되기 전에는 타임라인 스냅샷에서 특정 지점을 선택하여 간트 차트에서 해당 지점으로 이동할 수 있었습니다.

간트 차트에 정보가 표시되는 방식을 구성하는 방법에 대한 자세한 내용은 [간트 차트에 정보가 표시되는 방식 구성](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)을 참조하십시오.

## 비즈니스 사례의 대화형 리소스 플래너 {#interactive-resource-planner-in-the-business-case}

이제 리소스 관리자는 비즈니스 사례의 리소스 예산 섹션에서 리소스 풀을 추가할 수 있습니다. 프로젝트 수준 리소스 플래너를 사용하여 프로젝트 리소스의 예산을 책정할 수도 있습니다. 프로젝트에 대한 리소스의 예산을 책정하는 경우 프로젝트의 예산 인건비가 생성됩니다.

이 변경 이전에는 프로젝트가 글로벌 리소스 플래너의 리소스에 대해 예산이 책정된 경우 비즈니스 사례에서 리소스 예산 책정 정보를 볼 수 있었습니다.

비즈니스 사례에서 프로젝트 리소스 예산 책정을 완료하는 방법에 대한 자세한 내용은 [비즈니스 사례의 리소스 예산](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)을 참조하십시오.

## 리소스 플래너 - 사용자 할당 차트의 시각화 {#visualization-in-the-resource-planner-user-allocation-chart}

이제 리소스 플래너의 차트에 가용성에 대한 모든 사용자의 전체 계획된 할당을 표시할 수 있습니다. 리소스 플래너에서 **사용자별 보기**&#x200B;를 선택하면 차트를 사용할 수 있습니다.

이 차트에는 다음 정보가 표시됩니다.

* 모든 사용자에 대해 초과 할당이 없는 가용성 %
* 모든 사용자의 초과 할당(%)
* 모든 사용자의 과소 활용(%)
* 이 기간 동안 최소 한 명의 사용자에게 초과 할당이 있습니다.

이 변경 이전에는 테이블 형식으로만 개별 사용자의 할당 및 가용성을 볼 수 있었습니다.

리소스 플래너의 사용자 할당 차트에 대한 자세한 내용은 [리소스 플래너 개요](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)를 참조하십시오.

## 홈 영역의 개선 사항 {#improvements-in-the-home-area}

이제 홈 영역에서 다음을 포함하여 다양한 개선 사항을 사용할 수 있습니다.

* 향상된 디자인

   * 이제 오른쪽 패널이 더 커져 작업 및 문제 정보를 위한 더 많은 공간이 제공됩니다.
   * 이제 왼쪽 패널에서 선택하면 지연 항목이 더 밝은 빨간색 음영으로 표시됩니다.
   * 이제 왼쪽 패널과 오른쪽 패널 간의 관계를 더 쉽게 볼 수 있습니다. 왼쪽 패널에서 선택한 문서는 오른쪽 패널을 가리킵니다.

* 선택한 항목에 대한 기본 필드가 표시됩니다. 

  기본 필드에 대한 자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

* 요청에 대해 &quot;처리 중&quot;을 클릭하면 문제와 관련된 필드가 오른쪽 패널에 표시됩니다.

  홈 영역의 요청에 대한 작업에 대한 자세한 내용은 [홈 영역의 작업 및 팀 요청 관리](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)에서 [홈 영역의 작업 및 팀 요청 관리](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)를 참조하십시오.

* 왼쪽 패널의 작업 항목에서 사용자 아바타를 가리켜 사용자의 이름을 봅니다.
* 왼쪽 패널의 &quot;지연&quot; 영역을 확장하여 모든 지연 항목을 표시합니다(이 영역이 축소되면 처음 5개 항목만 표시됨).
* 항목을 완료로 표시하면 다른 항목을 선택할 때까지 항목이 왼쪽 패널에 유지됩니다.\
  완료된 항목을 표시하는 방법에 대한 자세한 내용은 [홈 영역의 작업 목록에 항목 표시](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)의 [홈 영역의 작업 목록에 항목 표시](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)를 참조하십시오.

새 홈 영역 사용에 대한 자세한 정보와 내 작업과 홈 간의 기능 차이를 설명하는 정보는 [홈 영역 사용](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)을 참조하십시오.

## 새 증명 뷰어 개선 사항  {#new-proofing-viewer-improvements}

* [향상된 레이아웃 및 디자인](#improved-layout-and-design)
* [댓글 번호로 댓글 검색](#search-comments-by-comment-number)
* [태그 표시기 옆에 있는 주석을 편집하는 옵션](#option-to-edit-comment-next-to-the-markup-indicator)
* [모든 댓글을 읽은 상태로 표시](#mark-all-comments-as-read)
* [왼쪽 메뉴 개선 사항](#left-menu-improvements)

### 향상된 레이아웃 및 디자인 {#improved-layout-and-design}

증명 뷰어의 모양과 느낌이 업데이트되었습니다. 다음  증명 뷰어의 다음 영역이 업데이트되었습니다.

* 썸네일 영역

  축소판 영역 사용에 대한 자세한 내용은에서 를 참조하십시오.

* 댓글 영역\
  설명 영역에 대한 자세한 내용은 를 참조하십시오.
* 왼쪽 메뉴 영역

### 댓글 번호로 댓글 검색 {#search-comments-by-comment-number}

이제 증명 뷰어에서 주석 목록을 검색할 때 검색 필드에 주석 번호를 입력할 수 있습니다. 그런 다음 주석 목록이 필터링되어 검색한 주석이 표시됩니다. 

자세한 내용은에서 를 참조하십시오.

### 마크업 표시기 옆에 있는 주석 편집 옵션 {#option-to-edit-comment-next-to-the-markup-indicator}

이제 기존 주석을 보다 쉽게 편집할 수 있습니다. 증명에서 주석 표시기를 클릭하면 풍선 옆에 편집 아이콘이 표시됩니다. 

이 변경 이전에는 주석 영역에서 편집 아이콘을 클릭해야 했습니다.  

자세한 내용은 를 참조하십시오.

### 모든 주석을 읽은 상태로 표시 {#mark-all-comments-as-read}

이제 증명 뷰어에서 문서를 볼 때 모든 주석을 읽음으로 표시할 수 있습니다.

### 왼쪽 메뉴 개선 사항 {#left-menu-improvements}

증명 뷰어 왼쪽의 메뉴에는 다음과 같은 개선 사항이 포함되어 있습니다.

* 업데이트된 모양 및 느낌
* 메뉴 상단에 있는 아이콘을 클릭하여 메뉴를 표시하거나 숨깁니다.

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* 메뉴 위로 마우스를 가져가면 메뉴가 자동으로 확장되어 아이콘과 함께 레이블을 볼 수 있습니다. (또는 축소된 보기에서 메뉴를 항상 유지하려면 옵션을 활성화합니다.)
