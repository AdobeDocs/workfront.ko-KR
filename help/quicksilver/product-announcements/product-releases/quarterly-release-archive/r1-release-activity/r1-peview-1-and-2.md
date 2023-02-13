---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 미리 보기 1 및 2
description: 이 페이지에서는 R1.1 및 R1.2 릴리스와 함께 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 1월 19일 미리 보기 환경에서 사용할 수 있게 되었습니다.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1 미리 보기 1 및 2

이 페이지에서는 R1.1 및 R1.2 릴리스와 함께 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 1월 19일 미리 보기 환경에서 사용할 수 있게 되었습니다.

R1에서 수행한 모든 변경 사항 목록은 [R1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 휴지통에서 프로젝트, 작업 및 문제 복원 

이제 Workfront 관리자는 지난 30일 이내에 삭제된 프로젝트, 작업 및 문제를 복원할 수 있습니다. 문서 및 사용자 지정 데이터를 포함하여 프로젝트, 작업 또는 문제와 관련된 모든 정보가 복원됩니다.

프로젝트, 작업 또는 삭제된 문제에 대해 기록되는 시간(시)을 구성하는 데에도 새 옵션을 사용할 수 있습니다. 자세한 내용은 [객체를 삭제하고 복원할 때 시간에 영향을 구성](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Workfront에서 개체 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

최근에 복원된 프로젝트, 작업 및 문제를 보는 방법에 대한 자세한 내용은 [복원된 항목 보기](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## 승인 다이어그램은 이전, 현재 및 향후 승인 단계를 시각적으로 표시합니다.

이제 프로젝트, 작업 또는 문제에 대한 승인이 보류되면 다이어그램이 표시됩니다. 승인 다이어그램은 승인 프로세스의 현재 단계(보류 중)를 보여주며, 승인 탭으로 이동하지 않고도 이전 및 향후 승인 단계를 빠르게 볼 수 있습니다.

이 변경 전에 승인 단계에 대한 정보는 프로젝트, 작업 또는 문제 내의 승인 탭에서만 사용할 수 있었고 다이어그램 보기가 아닌 목록 보기에서만 표시되었습니다. (이 정보는 승인 탭에서 계속 사용할 수 있으며 변경되지 않습니다.)

프로젝트에서 승인 정보는 프로젝트 제목 옆에 있는 헤더에 표시됩니다. 작업 및 문제에 대해 승인 정보가 오른쪽 패널에 표시됩니다.

자세한 내용은 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## 승인 보류 중인 업데이트할 객체를 구성합니다.

이제 프로젝트, 작업 또는 문제가 승인 보류 중이면 사용자가 다음을 수행할 수 있는지를 구성할 수 있습니다.

* 승인 보류 중인 프로젝트, 작업 또는 문제의 사용자 지정 양식을 편집합니다.\
   승인 보류 시 편집할 프로젝트, 작업 및 문제를 구성하는 방법에 대한 자세한 내용은 [전역 승인 설정 구성](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 승인 보류 중인 프로젝트에 문제를 추가합니다.\
   프로젝트가 승인 보류 중일 때 사용자가 문제를 추가할 수 있도록 프로젝트를 구성하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 승인 보류 중인 프로젝트 내의 작업 및 문제를 편집합니다.\
   프로젝트가 승인 보류 중일 때 사용자가 작업 및 문제를 편집할 수 있도록 프로젝트를 구성하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

이 변경 전에 승인 보류 중인 프로젝트, 작업 및 문제를 편집할 수 없습니다. 또한 승인이 보류 중인 프로젝트에 문제를 추가할 수 없으며 승인이 보류 중인 프로젝트 내에서 작업 및 문제를 편집할 수 없습니다.

## 그룹에 레이아웃 템플릿 할당

이제 레이아웃 템플릿을 그룹에 할당할 수 있습니다.

이 변경 전에 사용자, 팀 및 작업 역할에 레이아웃 템플릿을 할당할 수 있습니다. 그룹에 레이아웃 템플릿을 할당하면 레이아웃 템플릿 할당 우선 순위가 가장 낮습니다. 

자세한 내용은 &quot;레이아웃 템플릿 만들기 및 관리&quot;를 참조하십시오.

## 벌크 편집 사용자 알림 변경

사용자 이메일 알림 설정을 일괄적으로 편집하는 것과 관련하여 기능이 변경되었습니다. 알림 이메일 설정을 편집할 여러 사용자를 선택하면 선택한 모든 사용자에 대해 업데이트할 특정 알림만 변경됩니다. 사용자와 사용자가 다르더라도 선택한 모든 사용자에 대해 변경되지 않은 모든 이메일 알림 설정은 동일하게 유지됩니다. 

이 변경 전에 선택한 전자 메일 알림 설정이 저장되었으며 변경 내용을 저장할 때 변경되지 않은 다른 모든 알림 설정이 선택 취소되었습니다. 

자세한 내용은 의 &quot;사용자 알림 설정 일괄적으로 수정&quot;을 참조하십시오. [고유한 이벤트 알림 활성화 또는 비활성화](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 여러 이메일 알림의 모양과 느낌을 업데이트했습니다

다음 이메일 알림의 모양과 느낌은 새 UI로 업데이트되었습니다.

* 문제 지정
* 날짜 변경 커밋
* 내가 진행 중인 프로젝트가 활성화됩니다.
* 이해관계자에 대한 승인 결정
* 작업 종속 항목에 대한 이전 작업 완료
* 승인 보류 중(프로젝트, 작업, 문제)
* 프로젝트, 작업, 문제에 대한 상태 변경

미리 보기 샌드박스는 모든 사용자의 이메일 주소를 지우므로 이 기능을 테스트할 수 있도록 계정과 연결된 이메일 주소를 업데이트해야 합니다.    이메일 알림에 대한 자세한 내용은 [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## 여러 알림 영역에 대한 새 이메일 다이제스트 옵션

다음 알림 영역에는 &quot;일별 다이제스트&quot; 옵션이 추가되었습니다.

* 내 프로젝트 정보
* 내가 후원하는 프로젝트 정보
* 승인 정보
* 나에게 할당된 작업 정보
* 커뮤니케이션

자세한 내용은 [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md).  미리 보기 샌드박스는 모든 사용자의 이메일 주소를 지우므로 이 기능을 테스트할 수 있도록 계정과 연결된 이메일 주소를 업데이트해야 합니다. 

## 그룹 공개 만들기

이제 그룹을 공개하면 그룹 소유자가 아닌 사용자에게 해당 그룹을 추가할 수 있습니다. 사용자를 편집하려면 사용자 관리 액세스 권한이 있어야 합니다.

그룹을 공개하기 위한 자세한 내용은 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) 섹션 [그룹 만들기](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 모바일 앱에서 개체의 URL 공유 

이제 Workfront 모바일 앱에서 다음 개체에서 URL을 공유할 수 있습니다.

* 프로젝트
* 작업
* 문제
* 타임시트
* 문서

다음 응용 프로그램에서 개체의 URL을 공유할 수 있습니다.

* 문자 메시지
* 이메일
* 스토리지 드라이브(예: iCloud 드라이브)
* 다른 설치된 애플리케이션(예: 참고, Facebook)
* 객체에 대한 링크를 클립보드에 복사하여 다른 애플리케이션에 나중에 붙여넣을 수 있습니다. 

## 설정의 문맥에 따른 도움말

설정 메뉴 아래의 모든 영역이 영역의 오른쪽 상단 모서리에 있는 도움말 아이콘으로 업데이트되었습니다. 이 아이콘은 해당 영역에 대한 도움말 사이트 문서에 대한 링크를 제공합니다. 설정 영역 내의 일부 섹션도 도움말 아이콘으로 업데이트되었습니다. 

## 보다 정확한 비용 비율 추가

이제 비용 유형을 생성할 때 정확한 비용 비율을 추가할 수 있습니다. 비용 비율은 소수점 뒤에 최대 4자를 포함할 수 있습니다(예: 1.0375). 즉, 이 비율을 사용하는 모든 필드는 더 정확할 수 있습니다.

이 변경 전에 비용 비율은 소수점 뒤에 최대 2자까지 포함할 수 있습니다(예: 1.03).

비용 비율 생성에 대한 자세한 내용은 [사용자 지정 비용 유형 만들기](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 미리 보기 1 및 2 릴리스 웨비나 기록

이 웨비나는 2017년 1월 19일에 Workfront 릴리스 준비 팀에서 제공합니다. 이 웨비나는 2017년 릴리스 변경 사항에 초점을 맞췄으며 미리 보기에서 테스트하는 데 사용할 수 있는 새로운 기능을 다룹니다.
