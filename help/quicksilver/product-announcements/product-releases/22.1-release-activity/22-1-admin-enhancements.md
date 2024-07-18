---
title: 22.1 관리자 개선 사항
description: 22.1 관리자 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# 22.1 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.1 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 1월 17일이 있는 주.

22.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.1 릴리스 개요](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)를 참조하십시오.

## 업데이트 영역에 기록된 문서 다운로드

사용자가 Workfront에 저장하는 문서의 다운로드를 추적할 수 있도록 이제 누군가 문서를 다운로드할 때 시스템에서 업데이트 영역에 문서에 대한 항목을 기록합니다.

>[!NOTE]
>
>새로 업로드한 문서에 대한 미리 보기에서 이 기능을 테스트하는 것이 좋습니다.

Workfront이 개체에 자동 업데이트를 기록하는 방법에 대한 자세한 내용은 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)를 참조하십시오.

## 액세스 수준을 사용하여 팀에 액세스 권한 부여

액세스 수준 영역의 새 섹션에서는 팀에 대한 사용자의 액세스를 관리하기 위한 보다 세부적인 제어 기능을 제공합니다. 이제 팀을 만들고, 편집하고, 볼 수 있는 사용자를 결정할 수 있습니다.

따라서 팀에 대한 사용자의 기존 액세스 권한은 변경되지 않습니다.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## 이제 블루프린트에서 그룹 매핑을 사용할 수 있습니다.

이제 일부 블루프린트에 그룹이 포함되어 있습니다. 이 그룹은 블루프린트를 설치하기 전에 사용자 지정할 수 있습니다. 블루프린트의 그룹을 Workfront 인스턴스의 기존 그룹에 매핑하거나 필요한 경우 새 그룹을 만들 수 있습니다.

자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md)을 참조하세요.

## 사용자 지정 Forms 영역의 스타일 업데이트

사용자 지정 Forms 영역에는 새 Workfront 경험의 다른 많은 영역과 일치하는 새로운 모양과 느낌이 있습니다.

## 계산된 사용자 정의 필드를 만들기 위한 많은 개선 사항

이제 새 계산 편집기에서 다음과 같은 추가 기능을 사용하여 계산된 사용자 정의 필드를 훨씬 쉽게 만들 수 있습니다.

* 설명, 사용 방법의 예, 도움말 문서의 추가 정보에 대한 링크 등 계산에 있는 모든 표현식에 마우스를 가져다 대면 해당 표현식에 대한 정보를 표시할 수 있습니다.
* 추가하는 각 표현식은 유형에 따라 색상으로 구분됩니다. 이렇게 하면 표현식을 더 쉽게 찾고 표현식을 즉시 인식할 수 있습니다.
* 행 번호는 긴 계산에서 함수를 식별하고 참조하는 데 도움이 됩니다.
* 표현식 또는 필드 이름을 입력할 때 원하는 항목을 선택할 수 있도록 사용 가능한 항목 목록이 표시됩니다. 그리고 여는 괄호를 입력하면 닫는 괄호가 자동으로 추가됩니다.
* 계산 편집기를 종료하지 않고 기존 객체를 사용하여 계산 결과를 미리 볼 수 있습니다.

또한 계산된 사용자 정의 필드에 대한 사용자 정의 가능한 &quot;지침&quot; 가리키기 텍스트에서 필드의 수식을 표시하거나 숨길 수 있습니다. 이 기능은 사용자 정의 양식을 작성할 사용자에게 해당 정보가 필요하지 않다고 생각되는 경우 유용합니다.

## 상태 및 회사에 대한 감사 로그 정보 보기

이제 설정의 감사 로그 영역에서 상태 및 회사와 관련된 정보를 보고 문제를 보다 쉽게 해결할 수 있습니다.

For example:

* 이름을 바꾸거나, 잠기거나, 상태를 숨긴 사람과 언제 숨겼는지 파악할 수 있습니다.
* 회사에서 일부 구성원 또는 작업 역할을 삭제한 사람과 제거 시기를 확인할 수 있습니다.

감사 로그 정보를 보는 방법에 대한 자세한 내용은 [감사 로그 보기 및 내보내기](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)를 참조하십시오.

## 블루프린트 회사 매핑 및 기타 개선 사항

이제 다음 블루프린트 개선 사항을 사용할 수 있습니다.

* 이제 일부 블루프린트에 회사가 포함되어 있으며, 블루프린트를 설치하기 전에 사용자 지정할 수 있습니다. 블루프린트의 회사를 Workfront 인스턴스의 기존 회사에 매핑하거나 필요한 경우 새 회사를 만들 수 있습니다.
* 이제 새로운 블루프린트 유형인 조직 구조를 사용할 수 있습니다. 일부 블루프린트에는 여러 유형의 요소(예: 프로젝트 템플릿 및 조직 구조)가 포함되어 있습니다. 카탈로그 페이지에서 블루프린트 유형별로 필터링할 수 있습니다.
* 구성 페이지의 &quot;설치 환경 설정&quot; 및 &quot;템플릿 소유권&quot; 섹션은 단순성을 위해 &quot;템플릿 환경 설정&quot;으로 결합되었습니다.

자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md)을 참조하세요.

## 회사 멤버십을 보다 쉽게 관리

회사 영역에서 업데이트된 도구 모음을 사용하여 기존 Workfront 사용자를 회사에 추가하고 회사 구성원을 쉽게 제거할 수 있습니다.

이전에는 이러한 작업을 회사 편집 상자에서만 사용할 수 있었습니다.

업데이트된 도구 모음에는 멤버의 사용자 프로필 정보를 편집하고 시스템에서 이를 비활성화하는 것과 같이 이전 도구 모음에서 사용할 수 있었던 모든 작업이 포함되어 있습니다.

자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)를 참조하십시오.

## 새 계산된 필드 창에서 표현식 및 필드 선택

사용자 정의 양식에서 계산된 필드를 더 쉽게 만들 수 있도록 계속 노력하고 있습니다. 이제 최대화 를 클릭하여 새 계산 편집기를 열면 필요한 표현식과 필드를 찾아 선택할 수 있습니다.

## 그룹은 자신의 타임시트 및 시간 환경 설정을 구성할 수 있습니다.

>[!NOTE]
>
>이 기능은 처음에는 21.4 릴리스의 일부로 클러스터 4의 고객에 대해서만 단계별 롤아웃의 일부로 제공되었습니다. 이 기능은 2021년 11월 8일에 프로덕션의 나머지 모든 클러스터에 사용할 수 있습니다.

대규모 조직의 경우, 일부 그룹은 시스템 수준에서 관리자가 구성한 환경 설정을 상속하지 않고 고유 워크플로우에 맞게 타임시트 및 시간 환경 설정을 독립적으로 구성해야 할 수 있습니다. 이제 Workfront 관리자는 시스템의 모든 그룹에 대한 타임시트 및 시간 기본 설정을 잠금 해제하여 직접 구성할 수 있습니다.

이 기능은 프로젝트 환경 설정 및 작업 및 문제 환경 설정에 대해서도 최근에 추가되었습니다.

Workfront 관리자가 타임시트 및 시간 환경 설정을 잠금 해제하는 방법에 대한 자세한 내용은 문서 [타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)의 [그룹에 대한 타임시트 및 시간 환경 설정 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 섹션을 참조하십시오.

그룹 관리자가 잠금 해제된 작업 및 문제 환경 설정을 그룹에 대해 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)을 참조하십시오.

## 그룹에 대해 잠금 해제하거나 다시 잠글 여러 알림 선택

이제 그룹에 대한 이메일 알림을 잠금 해제하거나 다시 잠그는 것이 더 빠르고 쉽습니다. 이제 여러 알림을 선택하고 선택 내용이 올바른지 확인한 다음 도구 모음에 표시되는 새로운 잠금 해제 또는 잠금 버튼을 클릭할 수 있습니다.

이전에는 알림을 한 번에 하나씩 잠금 해제했다가 다시 잠가야 했습니다. Workfront에는 현재 95개의 알림이 있으므로 전체 또는 많은 알림에 대해 수행해야 하는 경우 시간이 다소 걸렸습니다.

자세한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)을 참조하세요.

## 그룹 관리자의 경우: 그룹을 삭제할 때 보다 쉽게 대체 그룹을 선택할 수 있습니다.

그룹을 삭제할 때 [그룹 삭제] 상자의 두 가지 개선 사항을 사용하면 삭제된 그룹의 사용자, 작업 항목 및 하위 그룹을 유지할 대체 그룹을 쉽게 선택할 수 있습니다.

* 그룹의 이름을 입력하여 빠르게 찾을 수 있습니다. 이전에는 입력할 수 없는 드롭다운 목록만 있었습니다. 목록을 스크롤하여 원하는 그룹을 찾아야 하므로 그룹이 많은 조직에서는 문제가 발생했습니다. 또한 드롭다운 목록에는 항목 제한이 있으므로 원하는 그룹이 표시되지 않았을 수 있습니다.
* 새 정보 아이콘을 사용하여 원하는 대체 그룹을 선택할 수 있습니다. 아이콘 위로 마우스를 가져가면 그룹 계층 구조 및 해당 관리자의 이름과 같은 그룹에 대한 정보가 나열된 도구 설명이 표시됩니다.

자세한 내용은 [그룹 삭제](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)를 참조하세요.

## 계산된 필드를 생성할 더 큰 영역

이제 사용자 정의 양식에서 복잡한 계산된 필드를 더 쉽게 작성할 수 있습니다. 계산을 빌드하기 위한 큰 편집 창을 열려면 새로 만든 최대화 단추를 누릅니다. 작업을 마쳤으면 최소화를 클릭하여 사용자 정의 양식에서 작업을 계속합니다.

## 그룹에 사용자 정의 양식 추가

이제 사용자 정의 양식이 Group 개체에 대해 지원됩니다. 이를 통해 조직의 그룹은 특정 요구 사항과 워크플로에 맞는 정보를 보다 쉽게 캡처하고 공유할 수 있습니다. 사용자는 다른 Workfront 개체에 대해 수행할 수 있는 것처럼 그룹에 대해 다음을 수행할 수 있습니다.

* 사용자 정의 양식 만들기
* 사용자 정의 양식 첨부
* 사용자 정의 양식 데이터 저장
* 사용자 정의 양식 제거
* 목록에서 사용자 정의 데이터를 편집하고, 새 Workfront 경험의 그룹 페이지에서 를 편집합니다

사용자 정의 양식에 대한 자세한 내용은 [사용자 정의 양식](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)을 참조하세요.

## OAuth2 앱을 만들어 Workfront과 애플리케이션 통합

이제 Workfront을 Workfront에서 기본 제공 통합을 제공하지 않는 다른 애플리케이션과 통합할 수 있습니다. 통합하려는 애플리케이션에 대한 OAuth2 앱을 생성하면 데이터가 보안 업계 표준 OAuth2 인증 프로토콜에 의해 보호된다는 사실을 알면서도 해당 애플리케이션이 Workfront에 액세스하도록 할 수 있습니다.

이전에는 내장된 통합, Workfront Fusion 또는 Workfront API를 통해서만 다른 애플리케이션과 통합할 수 있었습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md)를 참조하십시오.

## 회사 영역의 인터페이스 텍스트 개선 사항

설정 의 회사 영역에서 새 확인 메시지와 약간의 단어 변경을 통해 회사 멤버십을 보다 쉽게 관리할 수 있습니다. 예를 들어 왼쪽 패널의 섹션 이름 &quot;People&quot;은 이제 &quot;회사 구성원&quot;입니다.

회사 멤버십 관리에 대한 자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)를 참조하십시오.
