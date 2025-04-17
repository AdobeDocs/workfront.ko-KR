---
title: 연결된 레코드 개요
description: 레코드 종류 간에 연결을 만든 후에는 개별 레코드를 서로 연결할 수 있습니다. 이 문서에서는 Adobe Workfront Planning에서 레코드를 연결할 때 고려해야 하는 고려 사항에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 연결된 레코드 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

{{planning-important-intro}}

Adobe Workfront Planning 레코드를 서로 연결하거나 다른 응용 프로그램의 객체에 연결할 수 있습니다.

이 문서에서는 Adobe Workfront Planning에서 레코드를 연결할 때 고려해야 하는 고려 사항에 대해 설명합니다.

레코드를 서로 연결하거나 다른 개체에 연결하는 방법에 대한 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하십시오.


## 레코드 연결에 대한 고려 사항

* 레코드 유형을 연결하면 연결된 레코드 유형이 연결된 레코드 유형의 테이블 및 해당 레코드 페이지에서 연결된 레코드 필드로 표시됩니다.
* 연결된 레코드 필드에서 연결된 레코드와 개체 유형의 레코드와 개체를 찾아보고 추가할 수 있습니다.
* 연결 중인 레코드 유형의 테이블에 연결된 레코드 유형의 필드(조회 필드)를 추가할 수 있습니다.

  또한 연결할 레코드 유형의 테이블에서 연결할 레코드 유형의 필드(조회 필드)를 추가할 수도 있습니다.

  예를 들어 Campaign의 레코드 유형에서 제품의 레코드 유형을 연결하는 경우 캠페인에 대한 제품 필드와 제품에 대한 캠페인 필드를 표시할 수 있습니다.
* 연결 중인 레코드의 조회 필드 값은 수동으로 업데이트할 수 없습니다.

  조회 필드의 값은 원래 레코드나 개체에서 업데이트된 후 자동으로 연결되는 Workfront Planning 레코드를 채웁니다.

* 작업 영역 <span class="preview">에 대한 Workfront 계획 및 보기 이상의 사용 권한과 레코드 종류</span>에 대한 액세스 권한이 있는 모든 사용자는 레코드 간 또는 레코드와 다른 응용 프로그램의 개체 간에 사용자가 연결한 내용을 볼 수 있습니다. 연결하려는 응용 프로그램의 사용 권한에 관계없이 연결된 레코드와 개체를 볼 수 있습니다.
* 작업 영역 <span class="preview">과(와) 연결된 레코드가 있는 레코드 종류</span>에 대한 관리 권한이 있는 경우 다른 사용자의 연결을 보고 편집할 수 있습니다.
* 레코드 유형을 연결할 때 선택한 연결 유형에 따라 하나의 레코드를 다른 응용 프로그램에서 하나 또는 여러 개체에 연결할 수 있습니다. 자세한 내용은 문서 [연결된 레코드 형식 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)의 &quot;연결 형식&quot; 섹션을 참조하십시오.

## 레코드를 연결할 수 있는 영역

다음 영역에서 다른 레코드 또는 다른 응용 프로그램의 개체에 레코드를 연결할 수 있습니다.

* Workfront Planning의 레코드를 Planning 레코드의 다음 영역에서 Workfront 객체 또는 Experience Manager Assets 객체에 연결할 수 있습니다.

   * Planning에 있는 레코드 유형의 테이블 뷰에 있는 연결된 레코드 필드.
   * 세부 정보 탭의 연결된 레코드 필드에 있는 레코드의 미리 보기 또는 페이지입니다.
   * 연결 탭의 레코드 미리 보기 또는 페이지입니다.
   * 연결된 레코드의 연결 보기 탭에 있는 레코드의 페이지

* Workfront의 다음 영역에서 Workfront 개체를 Workfront Planning 레코드에 연결할 수 있습니다.

   * Workfront 개체의 계획 섹션입니다.
   * Workfront 오브젝트의 사용자 정의 양식에 대한 Planning 연결 필드.

  자세한 내용은 [Workfront 개체에서 레코드 연결 관리](/help/quicksilver/planning/records/manage-records-in-planning-section.md)를 참조하십시오.
