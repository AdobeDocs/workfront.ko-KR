---
title: 2026년 2분기 보고 개선 사항
description: 2026년 2분기 보고 개선 사항
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 8bcea5cec9f68deacc5f89ca7703303a1b00769f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---

# 2026년 2분기 보고 개선 사항

이 페이지에서는 미리보기 환경에 대한 2026년 2분기 릴리스의 보고 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2026년 2분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2026년 2분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)를 참조하십시오.

## 보고서를 작성할 때 표시되는 사용자 정의 필드 레이블

>[!NOTE]
>
>미리 보기: 2026년 2월 26일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

이제 사용자 지정 필드 레이블이 보고서 작성 도구의 필드 이름과 개체 앞에 표시되므로 필드를 더 쉽게 찾을 수 있습니다. 목록에서 필터, 보기 및 그룹화를 정의할 때도 필드 레이블이 표시됩니다.

사용자 정의 필드 레이블은 시스템 인터페이스용이며, 필드 이름은 API 및 백엔드 스토리지 용도로 자주 사용되며, 필드를 찾을 때 그다지 유용하지 않을 수 있습니다.

자세한 내용은 [사용자 지정 보고서 만들기](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

<!--

## Shareable Report Folders

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now organize and share reports using shareable report folders. This new feature helps teams that manage large volumes of reports maintain scalable and consistent access control:

* **Create organized folder structures**: System administrators can create top-level folders, and users with manage access can create subfolders up to 4 levels deep.
* **Granular permission controls**: Share folders with two permission levels:
   * View: Users can open reports and share folders
   * Manage: Users can edit folder details, add/remove items, and automatically receive manage access to all reports within the folder
* **Inherited permissions**: Permissions cascade from parent folders to all subfolders and reports within the folder tree
* **Enhanced list experience**: When you enable sharable folders, you will have access to the enhanced list experience. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


For more information, see [Use shareable report folders](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

-->

## 캔버스 대시보드의 차트 그룹화에 대한 날짜 레이블이 개선됨

>[!NOTE]
>
>미리 보기: 2026년 2월 26일
>프로덕션 빠른 릴리스: 2026년 3월 12일
>모두를 위한 프로덕션: 2026년 4월 16일

데이터를 날짜별로 그룹화하는 차트에 이제 더 명확하고 읽기 쉬운 날짜 레이블이 표시됩니다. 이 업데이트를 통해 날짜 레이블은 선택한 그룹화 기준 옵션(예: 일, 주, 월 또는 년)에 따라 동적으로 조정되므로 차트를 쉽게 읽고 해석할 수 있습니다.

<table> <tbody> <tr> <td>Day</td> <td>전체 날짜를 표시합니다. 예: 2026/3/12</td> </tr> <tr> <td>주</td> <td>서식이 지정된 주 시작 날짜를 표시합니다. 예, 2026년 3월 8일</td> </tr> <tr> <td>Month</td> <td>월과 연도를 표시합니다. 예제 2026년 3월</td> </tr> <tr> <td>Year</td> <td>연도만 표시합니다. 예: 2026</td> </tr> </tbody> </table>

이전에는 차트 그룹화에 선택한 기간의 시작 일자가 항상 숫자 형식으로 표시되었습니다.


