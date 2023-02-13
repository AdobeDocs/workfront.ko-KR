---
title: 20.4 기타 개선 사항
description: 20.4 기타 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4 기타 개선 사항

이 페이지에서는 미리 보기 환경에 대한 20.4 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 11월 9일이 있는 프로덕션 환경에서 사용할 수 있습니다.

20.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [20.4 릴리스 개요](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 관리자를 위한 새로운 기능: Workfront 환경 전환 옵션 사용 가능

보다 효율적이고 편리한 경험을 위해 그룹 관리자와 Workfront 관리자는 이제 로그아웃하지 않고도 Workfront의 모든 페이지에서 다양한 Workfront 환경을 빠르게 전환할 수 있습니다.

새 Workfront 경험의 기본 메뉴에 Switch to Classic 옵션이 나타납니다.

Workfront Classic에서 새 경험으로 전환 옵션이 전역 탐색 막대의 오른쪽 상단 모서리에 있는 프로필 사진을 클릭하면 표시되는 메뉴에 표시됩니다.

이 기능은 이제 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## Workfront 증명을 위한 향상된 암호화

Adobe는 Workfront Proofing 응용 프로그램의 데이터 인-모션 암호화 강도를 개선하기 위해 몇 가지 변경 작업을 수행하고 있습니다. 약한 TLS 메시지는 2020년 11월 11일에 더 이상 사용되지 않습니다.

Workfront에 액세스할 때 지원되는 브라우저를 사용하고 있는지 확인하십시오. 지원되는 브라우저에 대한 자세한 내용은 [Adobe Workfront 브라우저 요구 사항](../../../workfront-basics/workfront-browser-requirements.md).

## 3개의 이메일 템플릿에 대한 새로운 모양 및 느낌

가독성과 전체 경험을 향상시키기 위해 다음 이메일 템플릿에는 새로운 모양과 느낌이 있습니다.

* 새 작업 요청
* 할당된 종속 작업을 시작할 준비가 되었습니다.
* 이전 작업이 완료된 팀 이메일 알림

미리 보기 환경에서 테스트 목적으로 이메일을 활성화하려면 미리 보기에서 이메일 관리 섹션을 참조하십시오. [고유한 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 팀을 위한 새로운 이메일 알림

팀을 위해 다음과 같은 이메일 알림을 추가했습니다.

* 팀에 할당된 작업의 이전 작업이 완료되었습니다. 지정된 팀은 해당 작업 중 이전 작업이 완료됨으로 표시되면 전자 메일 알림을 받습니다.
* 팀에 할당된 작업의 모든 선행 작업이 완료되었습니다. 할당된 팀이 완료된 것으로 표시된 각 전임자에 대한 이메일 알림을 수신합니다.

자세한 내용은 [알림: 나에게 할당된 작업 정보](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 관리자를 위한 새로운 기능: 향상된 이메일 알림

이제 한 번의 클릭으로 설정에서 이벤트 이메일 알림을 활성화하거나 비활성화할 수 있습니다. 알림 이름 옆에 있는 켜기/끄기 스위치를 클릭하면 됩니다.

또한 최신 스타일링을 통해 이제 이메일 알림 영역에서 이벤트 알림을 구성하는 경험이 개선되었습니다.

이메일 알림 구성에 대한 자세한 내용은 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

이 기능은 이제 [이메일 및 인앱 알림 학습 경로](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) Workfront One.

## 이벤트 구독 업데이트를 트리거하는 새 API 개체

두 개의 새 API 개체 documentVersion 및 proofApproval이 생성되었으며 문서의 버전이 지정되거나 승인될 때 이벤트 구독 업데이트를 트리거하도록 구성되었습니다.

각 개체와 연결된 필드의 전체 목록이 필요하면 [이벤트 구독 리소스 필드](../../../wf-api/api/event-sub-resource-fields.md).
