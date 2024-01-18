---
title: 22.3 릴리스 일정 동안의 기타 업데이트
description: 22.3 릴리스 일정 동안의 기타 업데이트
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 기타 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.3 릴리스의 기타 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 7월 11일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다. 22.3 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [22.3 릴리스 개요](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 업데이트된 타임시트

타임시트로 작업할 때 환경을 계속 개선하고 업데이트하고 있습니다. 다음은 이 업데이트에 포함된 기능 중 일부입니다.

* 새로운 Workfront 경험에 어울리는 새로운 모양과 느낌입니다.

* 자동 저장 기능을 사용하면 기록된 시간과 시간 주석을 추가한 다음 자동으로 저장할 수 있습니다.

* 다른 오브젝트 페이지와 일치하도록 보다 직관적인 페이지 레이아웃. 예를 들어 타임시트에 왼쪽 패널을 추가했습니다. 이제 타임시트 업데이트가 왼쪽 패널의 업데이트 섹션에 표시됩니다. 타임시트 페이지에서 타임시트를 삭제하고 즐겨찾기 목록에 타임시트를 추가할 수도 있습니다.

* 타임시트에 프로젝트, 작업 또는 문제를 검색하고 추가할 때 더 나은 환경을 제공합니다. Workfront의 다른 모든 목록에 있는 경험과 일치합니다.

* 요약 패널은 작업 및 문제에 대해 타임시트에서 댓글을 추가하거나 정보를 업데이트하는 데 사용할 수 있습니다.


현재 업데이트에서는 다음 기능도 더 이상 사용되지 않습니다.

* 업데이트에서 작업 생성이 제거되었습니다. 이 기능은 다른 모든 개체의 업데이트 영역에서 2018.2 릴리스 이후 제거되었지만 타임시트 업데이트 스트림에서 계속 사용할 수 있습니다.

* &quot;타임시트에서 경비 추가. &quot;환경 설정이 설정의 타임시트 및 시간 환경 설정 영역에서 제거되었으며 타임시트의 경비를 더 이상 기록할 수 없습니다. 작업 및 프로젝트 페이지에서 비용을 기록할 수 있습니다.


자세한 내용은 다음 문서를 참조하십시오.

* [타임시트 레이아웃 이해](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [타임시트 및 시간 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 왼쪽 탐색 패널 개선 사항

Adobe Workfront의 왼쪽 탐색 패널에 몇 가지 개선 사항이 있습니다.

* 색상 및 글꼴을 포함한 Adobe 디자인 표준에 맞게 왼쪽 탐색 패널의 모양과 느낌이 업데이트되었습니다.

* 패널 하단의 &quot;사용자 정의 섹션 추가&quot; 링크의 이름이 해당 기능을 더 잘 설명하기 위해 &quot;대시보드 추가&quot;로 변경되었습니다.

## 사용자 지정 OAuth2 애플리케이션에서 자동 새로 고침 토큰 순환 사용

사용자 정의 OAuth2 애플리케이션의 보안을 보다 세밀하게 제어할 수 있도록 새로 고침 토큰 순환 사용 옵션이 추가되었습니다. 이 옵션을 활성화하면 새로 고침 토큰이 사용될 때마다 응용 프로그램에서 자동으로 새 새로 고침 토큰을 만들어 보내고 이전 새로 고침 토큰을 비활성화합니다.

애플리케이션은 매번 새로 고침 후 새 새로 고침 토큰을 저장해야 합니다. Workfront은 이 새로 고침 토큰을 저장하지 않습니다.

이전에는 새로 고침 토큰이 사용자 지정 OAuth2 애플리케이션 설정에 구성된 시간 설정 후 만료되었습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 단일 페이지 웹 애플리케이션에 대한 사용자 정의 OAuth2 통합에서 PKCE 사용

이제 PKCE를 사용하여 사용자 정의 통합에서 단일 페이지 웹 애플리케이션을 만들 수 있습니다. PKCE는 모바일 앱과 같이 동적으로 새로 고치는 애플리케이션에서 잘 작동하는 보안 인증 흐름이지만 모든 OAuth2 클라이언트에서 매우 중요합니다. PKCE에서는 정적 클라이언트 암호 대신 동적으로 생성된 문자열을 사용하므로 클라이언트 암호가 유출될 위험이 없습니다.

이전에는 사용자 정의 OAuth2 애플리케이션에 사용 가능한 옵션이 사용자 이름 및 암호 또는 클라이언트 암호를 사용했습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
