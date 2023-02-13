---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 작업표의 작업주 시작 날짜를 정합니다.
description: 내 작업표의 주 시작일이 내 작업표 프로필에 구성된 주의 시작일과 일치하지 않습니다.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 작업표의 작업주 시작 날짜를 정합니다.

## 문제

내 작업표의 주 시작일이 내 작업표 프로필에 구성된 주의 시작일과 일치하지 않습니다(에 설명된 대로). [작업표 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).)

## 솔루션

Adobe Workfront의 작업표 시작 날짜에는 브라우저의 언어 및 로케일 설정을 사용하여 요일을 결정합니다. 따라서 브라우저의 언어 및 로케일 설정을 업데이트해야 합니다. 

예를 들어 브라우저 언어가 영어로 설정되어 있고 로케일이 미국으로 설정되어 있으면 주가 일요일에 시작됩니다. 또는 브라우저 언어가 영어로 설정되고 영국으로 설정된 로케일이 월요일입니다.

이 설정은 시스템 전체의 팝업 달력에 있는 주의 시작일에도 영향을 줍니다.

로케일 변경은 리소스 그리드(또는 리소스 그리드 보기)에서 주의 시작일에 영향을 주지 않습니다. 주일은 항상 일요일에 시작됩니다.

다음은 Workfront에서 지원하는 다양한 브라우저의 언어 및 로케일 설정을 변경하는 지침입니다.

* **Chrome:** 다음 링크를 복사하여 Chrome 브라우저에 붙여넣습니다. `chrome://settings/languages` 그런 다음 언어로 이동합니다.
* **Firefox:**다음 링크를 복사하여 Firefox 브라우저에 붙여넣습니다. `about:preferences#content` 그런 다음 언어로 이동합니다.
* **IE 11:** 도구 -> 인터넷 옵션 -> 일반 -> 언어
* **Safari:** 안타깝게도 Safari에서는 전체 운영 체제 언어를 변경하지 않고 웹 탐색 언어를 변경할 수 없습니다. Chrome이나 Firefox와 같은 다른 브라우저를 설치하는 것이 더 쉽습니다.

 
