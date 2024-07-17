---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 1 릴리스 활동
description: 이 페이지에서는 2017.3 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 8월 9일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 2017.3 Beta 1 릴리스 활동

이 페이지에서는 2017.3 릴리스의 미리보기 환경에서 가장 최근에 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 8월 9일에 미리보기 환경에서 사용할 수 있습니다. 프로덕션 환경에서는 2017년 11월 초에 제공될 예정입니다.

>[!IMPORTANT]
>
> 이 페이지에 설명된 기능은 프로덕션 환경에서 사용하기 전에 변경될 수 있습니다.

2017.3의 모든 변경 사항 목록은 다음을 참조하십시오.  [2017.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 Beta 1 릴리스에는 Workfront 관리자와 기타 사용자를 위한 개선 사항이 포함되어 있습니다.

**관리자용:**

* [시간이 기록될 때 작업 및 문제가 삭제되지 않도록 방지](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [설정 영역에서 &quot;조기 액세스&quot; 설정 제거](#removal-of-the-early-access-setting-from-the-setup-area)
* [Workfront 기본 이메일 주소 변경](#workfront-default-email-address-change)

**모든 사용자의 경우:**

* [리소스 예약 개선](#resource-scheduling-improvements)
* [와이드스크린 디스플레이](#widescreen-display)
* [보고서 및 목록의 열 크기 조정 및 순서 바꾸기](#resize-and-reorder-columns-in-reports-and-lists)
* 작업 및 문제를 복사할 때 [사용자 지정 데이터 지우기](#clear-custom-data-option-when-copying-tasks-and-issues)
* [템플릿에서 직접 프로젝트 만들기](#create-a-project-directly-from-a-template)
* [구독한 개체에 대한 인앱 알림](#in-app-notification-for-subscribed-objects)
* [@Tagging은(는) 현재 미리 보기 환경에서 사용할 수 없습니다](#tagging-currently-not-available-in-the-preview-environment)
* [프로젝트에 대한 활용성 보고서에 사용자 할당 정보 포함](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## 리소스 예약 개선 사항 {#resource-scheduling-improvements}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

리소스 관리자로 팀, 프로젝트 또는 여러 프로젝트에 대한 리소스를 예약할 때 다음과 같은 리소스 일정 조정 개선 사항을 사용할 수 있습니다.

* [전체 화면 모드로 예약 영역 보기](#view-scheduling-area-in-full-screen-mode)
* [리소스 일정 영역을 볼 수 있는 추가 날짜 범위 옵션](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [예약 타임라인에서 예상 일자 보기](#view-projected-dates-on-the-scheduling-timeline)

### 전체 화면 모드로 예약 영역 보기 {#view-scheduling-area-in-full-screen-mode}

전체 화면 모드에서 예약 타임라인을 볼 수 있으므로 단일 보기에서 자세한 정보를 볼 수 있습니다. 

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

### 리소스 일정 영역을 보기 위한 추가 날짜 범위 옵션 {#more-date-range-options-for-viewing-the-resource-scheduling-area}

예약 타임라인을 볼 때 다음과 같은 추가 날짜 범위 옵션을 볼 수 있습니다.

* 하루 보기
* 4주 보기
* 6주 보기

이 변경 이전에는 1주, 2주 또는 3주 보기에서만 예약 타임라인을 볼 수 있었습니다. 이러한 날짜 범위는 새 날짜 범위 외에도 계속 사용할 수 있습니다.

단일 보기에서 예약 타임라인을 볼 때 사용자 할당(일일 총 시간 포함)을 표시할 수 없습니다.

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

### 예약 타임라인에서 예상 일자 보기 {#view-projected-dates-on-the-scheduling-timeline}

이제 작업 및 문제에 대한 계획된 일자 대신 예상 일자를 표시하도록 예약 타임라인을 구성할 수 있습니다. 

이 변경 이전에는 예약 타임라인의 작업 및 문제에 계획된 일자만 표시되었습니다.

예약 타임라인에서 예상 일자를 조회할 때 사용자 할당(일일 총 시간 포함)을 표시할 수 없습니다.

자세한 내용은 &quot;리소스 예약 시작&quot;을 참조하십시오.

## 와이드스크린 디스플레이 {#widescreen-display}

Workfront에 다음 개체 중 하나를 표시하면 전체 브라우저 창이 자동으로 채워집니다.

* 프로젝트
* 작업
* 문제
* 보고서
* 대시보드
* 캘린더

이 변경 이전에는 표시된 영역의 양쪽에 두 개의 흰색 사이드바가 있었습니다. 이제 와이드스크린 보기가 화면 및 브라우저 창의 너비에 맞게 동적으로 조정됩니다.

## 보고서와 목록의 열 크기 조정 및 순서 바꾸기 {#resize-and-reorder-columns-in-reports-and-lists}

이제 보고서를 편집하지 않고도 보고서나 목록의 열을 재배열하고 크기를 조정할 수 있습니다. (이 기능은 올해 초 조기 액세스 환경의 사용 중지와 함께 제거되었습니다. 현재 다시 도입되고 있습니다.)

대시보드 목록은 새 데이터 그리드 구조로 다시 디자인되었으므로 이 기능은 대시보드 목록 또는 보고서에 사용할 수 없습니다. 이 릴리스에서는 다른 모든 목록에서도 이 기능을 사용할 수 있습니다.

열 크기 조정 및 순서 변경에 대한 자세한 내용은 [열 너비 및 순서 수정](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)을 참조하십시오.

## 작업 및 문제를 복사할 때 사용자 지정 데이터 지우기 옵션 {#clear-custom-data-option-when-copying-tasks-and-issues}

이제 작업 또는 문제를 복사할 때 사용자 지정 데이터를 지우는 옵션을 선택할 수 있습니다. 작업 또는 문제의 사용자 정의 데이터를 지우도록 선택하면 양식이 새 항목에 복사되지만 양식의 사용자 정의 데이터는 복사되지 않습니다. 사용자 정의 데이터 지우기는 항목에 첨부된 문서에 첨부된 사용자 정의 양식 또는 작업의 비용에 첨부된 사용자 정의 양식에도 영향을 줍니다.

이 변경 이전에는 작업 또는 문제를 복사할 때 사용자 정의 양식에 포함된 사용자 정의 데이터도 새 항목에 복사되었습니다. 

작업 복사에 대한 자세한 내용은 [작업 복사 및 복제](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)를 참조하십시오.

문제 복사에 대한 자세한 내용은 [문제 복사](../../../../manage-work/issues/manage-issues/copy-issues.md)를 참조하십시오.

## 템플릿에서 바로 프로젝트 만들기 {#create-a-project-directly-from-a-template}

이제 템플릿 수준의 템플릿에서 프로젝트를 만들 수 있습니다.

이 변경 이전에는 **템플릿의 새 프로젝트** 옵션을 사용하여 Workfront의 프로젝트 영역에 있는 프로젝트 탭에서만 템플릿에서 프로젝트를 만들 수 있었습니다.

템플릿으로 프로젝트를 만드는 방법에 대한 자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](../../../../manage-work/projects/create-projects/create-project-from-template.md)를 참조하십시오.

## 시간이 기록될 때 작업 및 문제가 삭제되지 않도록 방지 {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

이제 시간이 기록된 작업 및 문제의 삭제를 허용하거나 방지하도록 Workfront을 구성할 수 있습니다.

이 변경 전에 시간이 기록된 작업 또는 문제를 삭제하면 타임시트 및 시간 환경 설정에 따라 시간이 작업 또는 문제와 함께 삭제되거나 프로젝트로 이동되었습니다.

작업 삭제에 대한 자세한 내용은 [작업 삭제](../../../../manage-work/tasks/manage-tasks/delete-tasks.md)를 참조하십시오.

문제 삭제에 대한 자세한 내용은 [문제 삭제](../../../../manage-work/issues/manage-issues/delete-issues.md)를 참조하십시오.

작업 및 문제 삭제를 위해 시스템 설정을 사용하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

## 설정 영역에서 &quot;조기 액세스&quot; 설정 제거 {#removal-of-the-early-access-setting-from-the-setup-area}

Workfront 관리자가 조기 액세스 환경에 참여할 사용자를 등록할 수 있도록 허용한 설정을 제거하고 있습니다. 이 기능은 2016년 말부터 더 이상 사용되지 않습니다. 2017년에는 조기 액세스에 새로운 기능이 출시되지 않았으며, 해당 환경에 남아 있던 모든 기능이 프로덕션으로 이동되었습니다.

이 변경 이전에는 액세스할 수 있는 새로운 기능이 없었지만 Workfront 관리자는 여전히 조기 액세스 환경에 사용자를 추가할 수 있었습니다.

## Workfront 기본 이메일 주소 변경 {#workfront-default-email-address-change}

Workfront 발신 메일의 기본 전자 메일 주소가 [noreply@attask.com](mailto:noreply@attask.com)에서 [noreply@my.workfront.com](mailto:noreply@workfront.com)(으)로 변경되었습니다.

현재 Workfront에서 보낸 이메일을 필터링하는 경우 새 기본 주소를 반영하도록 필터를 변경해야 합니다. 

기본 주소 변경은 구성된 Workfront 이메일 주소에 영향을 주지 않습니다. 

자세한 내용은 를 참조하십시오.

## 구독한 오브젝트에 대한 인앱 알림 {#in-app-notification-for-subscribed-objects}

사용자가 구독한 프로젝트, 작업 및 문제에 대해 댓글을 달면 이제 인앱 알림을 받게 됩니다. 구독 인앱 알림에 대한 자세한 내용은 [인앱 알림 보기 및 관리](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)를 참조하세요.

Workfront 관리자가 활성화한 기능에 따라 구독한 항목에 대한 이메일 알림을 받을 수도 있습니다. [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md)에 설명된 대로 구독 전자 메일의 링크를 통해 항목에서 구독을 쉽게 취소할 수 있습니다.

이 변경 이전에는 항상 구독한 항목에 대한 이메일 알림을 받았으며 인앱 알림을 받는 옵션이 없었습니다.

구독 이메일을 비활성화할 수 있지만 구독한 항목에 대한 인앱 알림을 비활성화할 수 없습니다. 자세한 내용은 [시스템의 모든 사용자에 대한 이벤트 알림 구성](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

항목 구독에 대한 자세한 내용은 [Adobe Workfront에서 항목 구독](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)을 참조하세요.

## @Tagging은 현재 미리보기 환경에서 사용할 수 없음 {#tagging-currently-not-available-in-the-preview-environment}

리치 텍스트 형식 기능을 업데이트 스트림으로 가져오려고 하면 일시적으로 @ 기호를 사용하여 미리보기 환경의 다음 개체에 대한 업데이트 스트림에서 다른 사용자를 태그 지정할 수 없습니다.

* 프로젝트
* 작업
* 문제
* 타임시트

**이 업데이트에 다른 사용자 포함** 아이콘을 클릭하여 다른 사용자를 태그 지정할 수 있습니다.

자세한 내용은 [업데이트에 다른 사용자 태그 지정](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.

## 프로젝트에 대한 활용성 보고서에 사용자 할당 정보 포함 {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>리소스 예약 도구는 23.1 릴리스에서 더 이상 사용되지 않으며 Workfront에서 제거되었습니다. 업무 균형자를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 [업무 균형자 개요](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)를 참조하십시오.

이제 프로젝트의 활용성 보고서에서 작업 기간 동안 계획된 시간이 다시 할당되었는지 여부를 고려합니다. &quot;예약 영역의 사용자 할당 관리&quot;에 설명된 대로 시간에 대한 사용자 할당이 수정되면 활용성 보고서에서 선택한 날짜에 작업의 일부만 포함된 경우 활용성 보고서의 데이터에 영향을 줄 수 있습니다.

자세한 내용은 [리소스 사용률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)를 참조하십시오.
