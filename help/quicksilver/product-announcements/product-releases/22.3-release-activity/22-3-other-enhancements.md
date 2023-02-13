---
title: 22.3 릴리스 일정 동안 기타 업데이트
description: 22.3 릴리스 일정 동안 기타 업데이트
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3 기타 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.3 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 7월 11일이 있는 프로덕션 환경에서 사용할 수 있었습니다. 22.3 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.3 릴리스 개요](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 업데이트된 작업표

작업표를 사용할 때 사용 환경을 개선하고 업데이트할 수 있도록 계속 노력하고 있습니다. 다음은 이 업데이트에 포함된 일부 기능입니다.

* 새로운 Workfront 경험에 어울리는 새로운 모습과 느낌입니다.

* 자동 저장 기능을 사용하여 기록된 시간과 시간 주석을 추가한 후 자동으로 저장합니다.

* 다른 개체 페이지와 일치하도록 보다 직관적인 페이지 레이아웃. 예를 들어 작업표에 왼쪽 패널을 추가했습니다. 이제 왼쪽 패널의 업데이트 섹션에 작업표 업데이트가 표시됩니다. 작업표 페이지에서 작업표를 삭제하고 작업표를 즐겨찾기 목록에 추가할 수도 있습니다.

* 작업표에 프로젝트, 작업 또는 문제를 검색하고 추가할 때 더 나은 환경을 제공합니다. Workfront의 다른 모든 목록에 있는 경험과 일치합니다.

* 작업 및 문제에 대해 작업표에서 메모를 추가하거나 정보를 업데이트할 수 있습니다.


현재 업데이트에서는 다음 기능도 더 이상 사용되지 않습니다.

* 업데이트에서 작업 만들기가 제거되었습니다. 이 기능은 다른 모든 개체의 업데이트 영역에서 2018.2 릴리스 이후 제거되었지만 작업표 업데이트 스트림에서 계속 사용할 수 있었습니다.

* 작업표에서 비용 추가 &quot;기본 설정이 설치 프로그램의 작업표 및 시간 기본 설정 영역에서 제거되었으며 더 이상 작업표에서 비용을 기록할 수 없습니다. 여전히 작업 및 프로젝트 페이지에서 비용을 기록할 수 있습니다.


자세한 내용은 다음 문서를 참조하십시오.

* [작업표 레이아웃 이해](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [작업표 및 시간 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 왼쪽 탐색 패널 개선 사항

Adobe Workfront의 왼쪽 탐색 패널에 여러 가지 기능이 개선되었습니다.

* 왼쪽 탐색 패널의 모양과 느낌을 색상 및 글꼴을 포함한 Adobe 디자인 표준으로 업데이트했습니다.

* 패널 하단에 있는 &quot;사용자 지정 섹션 추가&quot; 링크의 이름을 &quot;대시보드 추가&quot;로 변경하여 기능을 더 잘 설명했습니다.

## 사용자 지정 OAuth2 애플리케이션에서 자동 새로 고침 토큰 회전 사용

사용자 지정 OAuth2 응용 프로그램의 보안을 더 잘 제어할 수 있도록 새로 고침 토큰 회전을 활성화하는 옵션에 추가했습니다. 이 옵션을 활성화하면 새로 고침 토큰이 사용될 때마다 애플리케이션이 자동으로 새 새로 고침 토큰을 만들고 전송하며 이전 토큰을 비활성화합니다.

새로 고칠 때마다 애플리케이션이 새 새로 고침 토큰을 저장해야 합니다. Workfront은 이 새로 고침 토큰을 저장하지 않습니다.

이전에는 사용자 지정 OAuth2 애플리케이션 설정에 구성된 일정 시간 후에 토큰을 새로 고침했습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 단일 페이지 웹 애플리케이션용 사용자 지정 OAuth2 통합에서 PKCE 사용

이제 PKCE를 사용하여 사용자 지정 통합에서 단일 페이지 웹 응용 프로그램을 만들 수 있습니다. PKCE는 모바일 앱과 같은 응용 프로그램을 동적으로 새로 고치는 데 잘 작동하지만 모든 OAuth2 클라이언트에서 중요합니다. PKCE는 정적 클라이언트 암호 대신 동적으로 생성된 문자열을 사용하여 유출된 클라이언트 비밀의 위험을 제거합니다.

이전에는 사용자 정의 OAuth2 응용 프로그램에 사용할 수 있는 옵션이 사용자 이름과 암호 또는 클라이언트 암호를 사용했습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
