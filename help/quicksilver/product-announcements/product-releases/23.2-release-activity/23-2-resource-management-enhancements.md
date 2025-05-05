---
title: 23.2 향상된 리소스 관리 기능
description: 23.2 향상된 리소스 관리 기능
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2 향상된 리소스 관리 기능

이 페이지에서는 미리보기 환경에 대한 23.2 릴리스의 모든 리소스 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 23.2 릴리스를 통해 제공될 예정입니다.

23.2 릴리스 주기 동안 현재 사용 가능한 모든 변경 사항 목록을 보려면 [23.2 릴리스 개요](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md)를 참조하십시오.

## 작업 시간 필드를 도입하여 사용자 용량을 정확하게 계산

>[!NOTE]
>
>미리보기 릴리스: 2023년 2월 16일, 프로덕션 계획 릴리스: 2023년 3월 2일

리소스 관리자가 사용자의 가용성을 정확하게 계산하고 사용자가 실제 프로젝트 관련 작업에 투입하는 시간을 고려할 수 있도록 Adobe Workfront에 작업 시간 개념을 도입하고 있습니다.

프로필을 만들거나 편집할 때 모든 사용자에 대한 작업 시간 필드의 값을 정의할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

작업 시간 필드는 사용자가 간접비를 포함하지 않고 실제 작업에 사용할 수 있는 FTE(Full Time Equivalent) 시간의 백분율을 나타냅니다. Work Time은 0과 1 사이의 값을 가진 10진수여야 합니다. 예를 들어, 실제 작업에 대한 20% 가용성은 0.2입니다.

필드의 기본값은 1이며, 사용자가 전체 FTE를 실제 프로젝트 관련 작업에 사용함을 나타냅니다.

이 업데이트의 결과로, Workfront은 리소스 관리 환경 설정 영역에서 선택한 항목에 따라 아래 공식을 사용하여 사용자의 가용성을 계산합니다.

* 기본 일정:
* 사용자 수용작업량 = [(일정 시간 - 일정 예외) * FTE - 휴무] * 작업 시간
* 사용자 일정:
* 사용자 능력 = (스케줄 시간 - 스케줄 예외 - 휴무) * 작업 시간.

자세한 내용은 [리소스 관리 구성]기본 설정(/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)을 참조하세요.

[이 기능의 비디오 데모 보기](https://video.tv.adobe.com/v/3415608/){target=_blank}
