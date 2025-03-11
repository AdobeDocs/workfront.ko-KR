---
title: 필드 개요
description: 조직의 라이프사이클을 반영하는 새 필드를 Adobe Workfront Planning에 추가할 수 있습니다. 필드는 레코드 유형의 속성입니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 2%

---


# 필드 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

조직의 라이프사이클을 반영하는 새 필드를 Adobe Workfront Planning에 추가할 수 있습니다. 필드는 레코드 유형의 속성입니다.


## Adobe Workfront Planning 필드에 대한 고려 사항

* 레코드 유형 페이지의 테이블 보기에서만 필드를 만들 수 있습니다. 필드는 표 보기에서 열로 표시됩니다. 레코드 유형과 연관된 모든 필드도 레코드 페이지에 표시됩니다.

  테이블 열 또는 레코드 필드 관리에 대한 자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md)를 참조하십시오.

  필드 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [필드 설정 편집](/help/quicksilver/planning/fields/edit-fields.md)
   * [필드 삭제](/help/quicksilver/planning/fields/delete-fields.md)

* 레코드 형식과 연결된 필드는 해당 형식의 모든 레코드와 연결할 수 있습니다. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 레코드 형식과 연결된 필드는 다른 레코드 형식에 추가할 수 없습니다. <!-- this will change when they open the Field library tab when creating a field-->

* 다음 방법으로 필드를 수동 또는 자동으로 만들 수 있습니다.

   * 수동:

      * 레코드 유형 페이지의 테이블 보기에서 열을 추가할 때 테이블의 열은 레코드 유형과 연관된 필드입니다. 레코드 페이지에 표시되는 필드와 동일합니다.

        레코드의 페이지에서 필드를 만들 수 없습니다.

      * 레코드 유형을 연결하는 경우. 두 레코드 형식 또는 다른 응용 프로그램의 레코드 형식과 개체 형식 간에 새 연결을 추가할 때 연결된 레코드 필드를 만들 수 있습니다.

        레코드 종류 연결에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

      * Workfront에서 기존 필드를 가져오는 경우.

        자세한 내용은 [Adobe Workfront에서 필드 가져오기](/help/quicksilver/planning/fields/import-fields-from-workfront.md)를 참조하십시오.


   * 자동:

      * 레코드 유형을 만들 때:

         * 이름
         * 설명
         * 시작 일자
         * 종료 일자
         * 상태. 레코드 상태의 기본값은 다음과 같습니다.
            * 개발
            * 계획됨
            * 활성
            * 완료됨
            * 보류 중

        값을 더 추가하거나 기존 값의 이름을 변경할 수 있습니다.

      * 템플릿으로 작업 공간을 만들 때

        자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

      * Excel 또는 CSV 파일을 사용하여 레코드 유형을 가져오는 경우.

        자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

* Workfront Planning 필드는 Workfront에서 액세스할 수 없습니다.

* Workfront 필드는 레코드 유형을 Workfront 개체 유형과 연결하고 Workfront 개체에서 연결 또는 조회 필드를 추가하는 경우에만 Workfront Planning에서 액세스할 수 있습니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

* 필드가 속한 작업 영역 <!--<span class="preview">and record type</span>-->에 대한 관리 권한이 있는 경우 사용자 또는 다른 사용자가 만든 필드의 설정을 보고 업데이트할 수 있습니다.

* 하나의 레코드 유형에 대해 최대 500개의 필드가 있을 수 있습니다.

* 필드 이름은 최대 250자입니다.

* 레코드 종류 또는 작업 영역을 삭제하면 레코드 종류 또는 작업 영역과 관련된 모든 필드와 필드 값도 삭제되며 복구할 수 없습니다. <!-- this might change with a possible recycle bin solution?!-->
