---
title: 필드 개요
description: 조직의 라이프사이클을 반영하는 새 필드를 Adobe Maestro에 추가할 수 있습니다. 필드는 레코드 유형의 속성입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# 필드 개요

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

조직의 라이프사이클을 반영하는 새 필드를 Adobe Maestro에 추가할 수 있습니다. 필드는 레코드 유형의 속성입니다.


## Maestro 필드에 대한 고려 사항

* 레코드 유형 페이지의 테이블 보기에서만 필드를 만들 수 있습니다. 필드는 표 보기에서 열로 표시됩니다. 레코드 유형과 연관된 모든 필드는 해당 유형의 각 레코드에 대한 세부 정보 페이지에도 표시됩니다.

  테이블 열(또는 레코드 필드) 관리에 대한 자세한 내용은 [표 보기 관리](../views/manage-the-table-view.md).

  필드 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [필드 편집](../fields/edit-fields.md)
   * [필드 삭제](../fields/delete-fields.md)

* 레코드 형식과 연결된 필드는 해당 형식의 모든 레코드와 연결할 수 있습니다. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 레코드 형식과 연결된 필드는 다른 레코드 형식에 추가할 수 없습니다. <!-- this will change when they open the Field library tab when creating a field-->

* 다음 방법으로 필드를 수동 또는 자동으로 만들 수 있습니다.

   * 수동:

      * 레코드 유형 페이지의 테이블 뷰에 열을 추가합니다. 테이블의 열은 레코드 유형과 연관된 필드입니다. 레코드의 세부 정보 페이지에 표시되는 필드와 동일합니다.

        레코드의 세부 정보 페이지에서 필드를 만들 수 없습니다.

        이 문서에서는 필드를 수동으로 만드는 방법을 설명합니다.

      * 레코드 유형을 연결하여 두 Maestro 레코드 유형 또는 다른 응용 프로그램의 레코드 유형과 객체 유형 간에 새로운 연결을 추가할 때 연결된 레코드 필드를 만들 수 있습니다.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Maestro 레코드 유형 연결에 대한 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

      * Excel 또는 CSV 파일을 사용하여 레코드 유형을 가져옵니다. 자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

   * 자동:

      * 레코드 유형을 만들 때마다 기본적으로 표시됩니다.

        다음은 각 새 작업 레코드 유형에 대해 기본적으로 생성되는 표준 필드입니다.

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

        다음은 각 새 분류 레코드 유형에 대해 기본적으로 생성되는 표준 필드입니다.

         * 이름 <!--will more be added? If not, consider rephrasing this bullet-->

      * 템플릿으로 작업 공간을 만들 때 템플릿에서 작업 영역을 만들 때 Maestro는 작동 기록 유형 및 분류법에 대한 필드를 만듭니다. 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).

* Workfront에서 Maestro 필드에 액세스할 수 없습니다.

* Workfront 레코드 유형을 Workfront 개체 유형과 연결하고 Workfront 개체에서 연결 또는 조회 필드를 추가하는 경우에만 Maestro에서 필드에 액세스할 수 있습니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

* 필드가 속한 작업 영역에 대한 관리 권한이 있는 경우 사용자 또는 다른 사용자가 만든 필드의 설정을 보고 업데이트할 수 있습니다.

* 하나의 레코드 유형에 대해 최대 500개의 필드가 있을 수 있습니다.

* 필드 이름은 최대 250자입니다.

* 작업 레코드 유형, 분류 또는 작업 영역을 삭제할 때 연결된 모든 필드와 필드 값도 삭제되므로 복구할 수 없습니다. <!-- this might change with a possible recycle bin solution?!-->
