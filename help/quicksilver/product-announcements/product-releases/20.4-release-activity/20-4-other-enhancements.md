---
title: 20.4 기타 개선 사항
description: 20.4 기타 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 기타 개선 사항

이 페이지에서는 미리보기 환경에 대한 20.4 릴리스의 기타 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 11월 9일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

20.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 [20.4 릴리스 개요](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md)를 참조하십시오.

## 관리자용 새로운 기능: Workfront 환경 전환 옵션을 사용할 수 있음

보다 효율적이고 편리한 환경을 위해 그룹 관리자와 Workfront 관리자는 이제 로그아웃할 필요 없이 Workfront의 모든 페이지에서 서로 다른 Workfront 환경 간을 빠르게 전환할 수 있습니다.

새 Workfront 경험에서 클래식으로 전환 옵션이 메인 메뉴에 나타납니다.

Workfront Classic에서 글로벌 탐색 막대의 오른쪽 상단 모서리에 있는 프로필 사진을 클릭하면 표시되는 메뉴에 새 경험으로 전환 옵션이 나타납니다.

이 기능은 이제 Workfront One의 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)에 포함되어 있습니다.

## Workfront Proof의 암호화 개선

Workfront 증명 애플리케이션의 Data-in-motion 암호화 강도를 개선하기 위해 몇 가지 사항을 변경하고 있습니다. 약한 TLS 암호는 2020년 11월 11일에 사용이 중단됩니다.

Workfront에 액세스할 때 지원되는 브라우저를 사용하고 있는지 확인하십시오. 지원되는 브라우저에 대한 자세한 내용은 [Adobe Workfront 브라우저 요구 사항](../../../workfront-basics/workfront-browser-requirements.md)을 참조하십시오.

## 3개의 이메일 템플릿에 대한 새로운 모양과 느낌

가독성과 전반적인 환경을 개선하기 위해 다음 이메일 템플릿에는 새로운 모양과 느낌이 있습니다.

* 새 작업 요청
* 귀하에게 할당된 종속 작업을 시작할 준비가 되었습니다.
* 전임 작업 완료 팀 이메일 알림

미리 보기 환경에서 테스트용 전자 메일을 사용하려면 [전자 메일 알림 수정](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)의 미리 보기에서 전자 메일 관리 섹션을 참조하십시오.

## 팀에 대한 새 이메일 알림

팀에 대해 다음과 같은 이메일 알림을 추가했습니다.

* 내 팀에 할당된 작업의 전임 작업이 완료됨: 작업 중 하나의 전임 작업이 완료로 표시되면 할당된 팀이 이메일 알림을 받습니다.
* 내 팀에 할당된 작업의 모든 전임 작업이 완료되었습니다. 할당된 팀이 완료 상태로 표시된 각 전임 작업에 대한 이메일 알림을 받습니다.

자세한 내용은 [알림: 나에게 할당된 작업에 대한 정보](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md)를 참조하세요.

## 관리자용 새로운 기능: 이메일 알림 개선 사항

이제 한 번의 클릭으로 설정에서 이벤트 이메일 알림을 활성화하거나 비활성화할 수 있습니다. 알림 이름 옆에 있는 On/Off 스위치를 클릭하면 됩니다.

또한 이제 최신 스타일을 사용하여 이메일 알림 영역에서 이벤트 알림을 구성하는 경험을 개선할 수 있습니다.

전자 메일 알림 구성에 대한 자세한 내용은 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

이 기능은 이제 Workfront One의 [전자 메일 및 인앱 알림 학습 경로](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0)에 포함되어 있습니다.

## 이벤트 구독 업데이트를 트리거하는 새 API 개체

두 개의 새 API 개체인 documentVersion 및 proofApproval이 만들어지고 문서의 버전이 지정되거나 승인될 때 이벤트 구독 업데이트를 트리거하도록 구성됩니다.

각 개체와 연결된 전체 필드 목록은 [이벤트 구독 리소스 필드](../../../wf-api/api/event-sub-resource-fields.md)를 참조하세요.
