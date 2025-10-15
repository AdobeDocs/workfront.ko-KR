---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 타임시트의 작업 주 시작일 수정
description: 내 타임시트의 그 주의 시작 일자가 내 예상 주간 시작 일자와 일치하지 않습니다.
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 타임시트의 작업 주 시작일 수정

<!--Audited: 5/2025-->

## 문제

내 타임시트의 그 주의 시작 일자가 내 예상 주간 시작 일자와 일치하지 않습니다.

일반적으로 이 문제는 타임시트 프로필에 할당되지 않고 타임시트가 수동으로 생성된 경우에 발생합니다.


## 솔루션

[타임시트 프로필 만들기, 편집 및 할당](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)에 설명된 대로 Workfront 관리자는 타임시트 프로필을 만들고 모든 사람을 프로필에 할당해야 합니다. Workfront 관리자는 타임시트의 시작 날짜를 예상 주별 시작 날짜가 아닌 다른 날로 정의할 수 있습니다. 타임시트에 대한 타임시트 프로필의 시작 날짜를 확인하려면 해당 파트너와 상의하십시오.

타임시트를 수동으로 만든 경우 타임시트의 시작 요일은 문서 [내 설정 구성](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)에 설명된 대로 사용자 프로필의 전자 메일 로케일 설정을 사용합니다.

예를 들어 이메일 로케일이 영어(미국)로 설정되면 타임시트의 주가 일요일에 시작됩니다. 또는 이메일 로케일이 영어(영국)로 설정되어 있으면 타임시트의 주가 월요일에 시작됩니다.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


