---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 미리 보기 4
description: 이 페이지에서는 R1.4 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 2월 15일에 미리보기 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# R1 미리 보기 4

이 페이지에서는 R1.4 릴리스의 미리보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 2월 15일에 미리보기 환경에서 사용할 수 있습니다.

R1의 모든 변경 사항 목록은 다음을 참조하십시오. [Workfront R1 릴리스](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## 업데이트된 프로젝트, 작업 및 문제 승인

이제 프로젝트, 작업 및 문제 승인에 대한 승인 프로세스를 만들 때 다음과 같은 개선 사항 및 변경 사항을 사용할 수 있습니다. 

* 이제 승인 &quot;단계&quot;를 승인 &quot;단계&quot;라고 합니다.
* 단계당 여러 유형의 승인자를 포함합니다.\
  여기에는 사용자, 팀 및 작업 역할이 포함됩니다.\
  이 변경 이전에는 동일한 유형의 승인자만 여러 명 포함할 수 있었습니다. 예를 들어 여러 작업 역할을 포함할 수 있지만 작업 역할과 팀은 포함할 수 없습니다.

* 기존 글로벌 승인 프로세스 수정과 관련된 다음과 같은 기존 제한 사항이 제거되었습니다.

   * 수정된 승인 프로세스는 승인 프로세스가 아직 시작되지 않았거나 승인 프로세스가 수정되지 않은 시스템 전체의 객체에만 반영됩니다. 승인 프로세스가 이미 시작되었거나 승인 프로세스가 수정된 오브젝트는 변경 내용으로 업데이트되지 않습니다.
   * 승인이 시작되는 시기를 결정하는 상태는 수정할 수 없습니다.

* 모양과 느낌이 업데이트되었습니다.

승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

이제 승인 프로세스를 프로젝트, 작업 또는 문제와 연결할 때 다음과 같은 개선 사항 및 변경 사항을 사용할 수 있습니다.

* 모양과 느낌이 업데이트되었습니다.
* 승인 다이어그램이 승인 탭에 표시되어 이전, 현재 및 향후 승인 단계를 시각적으로 표시합니다.

승인을 프로젝트, 작업 및 문제와 연관시키는 방법에 대한 자세한 내용은 [신규 또는 기존 승인 프로세스를 작업과 연결](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 프로젝트 페이지에서 직접 프로젝트 상태 변경

프로젝트 상태를 변경하기 위해 더 이상 프로젝트를 편집할 필요가 없습니다. 이제 프로젝트의 기본 페이지에서 직접 프로젝트의 상태를 변경할 수 있습니다.

자세한 내용은 [프로젝트 상태 변경](../../../../manage-work/projects/manage-projects/change-project-status.md).

## 사용자 비활성화 예약

이제 미래의 날짜에 비활성화되도록 사용자를 예약할 수 있습니다.

이 개선 이전에는 사용자를 수동으로만 즉시 비활성화할 수 있었습니다.

사용자를 비활성화하도록 예약하는 것은 다양한 시나리오에서 유용할 수 있습니다. 예를 들어 Workfront에서 임시로 고용된 사용자를 만드는 경우 계약이 종료될 때 비활성화되도록 설정할 수 있습니다.

이 기능은 사용자를 일괄 편집할 때도 사용할 수 있습니다. 

비활성화 일정을 예약하는 방법에 대한 자세한 내용은 [사용자 비활성화 또는 재활성화](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) 및 [사용자 추가](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## &quot;필요한 작업&quot;에 대한 새로운 이메일 다이제스트 옵션

이제 알림 설정의 &quot;필요한 작업&quot; 영역에서 일별 요약 전달 옵션을 사용할 수 있습니다.

자세한 내용은 [이메일 알림 수정](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

이 기능을 테스트하려면 계정과 연결된 이메일 주소를 업데이트해야 합니다. 이는 미리보기 샌드박스가 모든 사용자의 이메일 주소를 지우므로 필요합니다.

## 휴지통 개선: 업데이트 스트림에 기록되고 이메일 알림 수신

삭제된 프로젝트, 작업 및 문제를 복원할 때 다음과 같은 개선 사항이 추가되었습니다.

* 이제 개체를 복원한 후 이메일 알림을 받게 됩니다.\
  이제 Workfront 관리자는 이전에 삭제된 프로젝트, 작업 또는 문제를 복원한 후 이메일 알림을 받게 됩니다. 이메일 알림은 복원 프로세스의 상태를 알려줍니다.\
  Workfront에서 개체를 복원하는 방법에 대한 자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 개체가 복원되면 개체의 삭제 및 복원이 개체 자체의 업데이트 스트림과 부모 개체의 업데이트 스트림에 기록됩니다.\
  이전에는 상위 개체의 업데이트 스트림에 삭제만 기록되었습니다.\
  예를 들어 작업이 복원되면 프로젝트 및 작업 자체의 업데이트 스트림에 작업이 복원되었음을 나타내는 메시지가 추가됩니다. (삭제 및 복원은 하위 작업에 기록되지 않습니다. 하위 작업의 삭제 및 복원에 대한 정보는 상위 작업에서만 사용할 수 있습니다.)\
  자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## 그룹 구성원 관리를 위한 업데이트된 대화 상자

보다 쉽고 사용자 친화적인 환경을 제공하는 그룹 및 하위 그룹 관리를 위한 새로운 인터페이스가 있습니다.

이제 그룹 소유자 필드와 그룹 구성원 필드가 아래에 나열된 그룹 구성원 목록과 함께 단일 필드로 결합됩니다. 또한 그룹 구성원 목록을 필터링하고 그룹 구성원이 소유자인지 또는 구성원인지를 변경할 수 있습니다. 

그룹에 하위 그룹을 추가하고 사용자를 그룹의 구성원 또는 그룹 소유자로 지정하는 방법에 대한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 및 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## 모바일 앱에서 텍스트 복사

모바일 앱에 표시되는 모든 개체의 다음 필드에 있는 텍스트를 복사할 수 있습니다.

* 이름
* 설명
* 참조 번호
* 댓글

이 기능은 2월 13일이 있는 주에 iOS 및 Android 앱 스토어 모두에 출시될 예정입니다.
