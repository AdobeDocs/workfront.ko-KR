---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 타임시트의 작업 주 시작일 수정
description: 내 타임시트에 있는 주의 시작 일자가 내 타임시트 프로필에 구성된 주의 시작 일자와 일치하지 않습니다.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 타임시트의 작업 주 시작일 수정

## 문제

내 타임시트의 시작 요일이 내 타임시트 프로필에 구성된 주의 시작 요일과 일치하지 않습니다([타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)에 설명된 대로).

## 솔루션

Adobe Workfront의 타임시트 시작 일자는 브라우저의 언어 및 로케일 설정을 사용하여 요일을 결정합니다. 따라서 브라우저에 대한 언어 및 로케일 설정을 업데이트해야 합니다. 

예를 들어 브라우저 언어가 영어로 설정되고 로케일이 미국으로 설정되면 주가 일요일에 시작됩니다. 또는 브라우저 언어가 영어로 설정되고 로케일이 영국으로 설정된 경우 시작일은 월요일입니다.

이 설정은 시스템의 팝업 달력에서 요일의 시작일에도 영향을 줍니다.

로케일 변경은 리소스 그리드(또는 리소스 그리드 보기)의 요일에 영향을 주지 않습니다. 그 주는 항상 일요일에 시작한다.

다음은 Workfront에서 지원되는 다양한 브라우저에 대한 언어 및 로케일 설정을 변경하는 지침입니다.

* **Chrome:** Chrome 브라우저에 다음 링크 `chrome://settings/languages`을(를) 복사하여 붙여 넣은 다음 언어로 이동하십시오.
* **Firefox:**다음 링크를 복사하여 Firefox 브라우저에 붙여 넣은 다음 `about:preferences#content` 언어로 이동합니다.
* **IE 11:** 도구 -> 인터넷 옵션 -> 일반 -> 언어
* **Safari:** 죄송합니다. Safari에서는 전체 운영 체제 언어를 변경하지 않고 웹 탐색 언어를 변경할 수 없습니다. Chrome 또는 Firefox와 같은 다른 브라우저를 설치하는 것이 더 쉬울 수 있습니다.

 
