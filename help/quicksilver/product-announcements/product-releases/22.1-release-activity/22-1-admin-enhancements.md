---
title: 22.1 관리자 개선 사항
description: 22.1 관리자 개선 사항
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 22.1 관리자 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.1 릴리스로 향상된 모든 관리자 기능을 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 1월 17일이 있는 주.

22.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.1 릴리스 개요](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 업데이트 영역에 기록된 문서 다운로드

사용자가 Workfront에 저장하는 문서의 다운로드를 추적할 수 있도록 하기 위해, 이제 시스템에서 사용자가 문서를 다운로드할 때 업데이트 영역에 항목을 기록합니다.

>[!NOTE]
>
>새로 업로드한 문서의 미리 보기에서 이 기능을 테스트하는 것이 좋습니다.

Workfront이 개체에 자동 업데이트를 기록하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [시스템 추적 업데이트](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## 액세스 수준을 사용하여 팀에 액세스 권한 부여

액세스 수준 영역의 새 섹션에서는 팀에 대한 사용자의 액세스를 관리하기 위한 보다 세부적인 컨트롤을 제공합니다. 이제 팀을 만들고, 편집하고, 볼 수 있는 사람을 결정할 수 있습니다.

이렇게 해도 팀에 대한 사용자의 기존 액세스 권한은 변경되지 않습니다.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## 이제 블루프린트에서 그룹 매핑을 사용할 수 있습니다.

이제 일부 블루프린트를 설치하기 전에 사용자 지정할 수 있는 그룹이 포함되어 있습니다. 블루프린트의 그룹을 Workfront 인스턴스의 기존 그룹에 매핑하거나, 필요한 경우 새 그룹을 만들 수 있습니다.

자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md).

## 사용자 지정 Forms 영역의 스타일 지정 업데이트

사용자 지정 Forms 영역에는 새로운 Workfront 경험의 다른 많은 영역과 함께 새로운 모양과 느낌이 있습니다.

사용자 지정 양식 만들기에 대한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 계산된 사용자 지정 필드를 만들기 위한 여러 가지 개선 사항

이제 새 계산 편집기에서 이러한 추가 기능을 사용하면 계산된 사용자 지정 필드를 훨씬 쉽게 만들 수 있습니다.

* 계산의 모든 표현식을 마우스로 가리키면 설명, 사용 가능한 방법의 예 및 도움말 문서의 추가 정보에 대한 링크를 비롯하여 해당 식에 대한 정보를 표시할 수 있습니다.
* 추가하는 각 표현식은 유형에 따라 색상으로 구분됩니다. 이를 통해 표현식을 쉽게 찾아 해당 유형을 즉시 인식할 수 있습니다.
* 라인 번호는 긴 계산에서 함수를 식별하고 참조하는 데 도움이 됩니다.
* 표현식이나 필드 이름을 입력하기 시작하면 원하는 항목을 선택할 수 있도록 사용 가능한 항목 목록이 표시됩니다. 그리고 여는 괄호를 입력하면 닫는 괄호가 자동으로 추가됩니다.
* 계산 편집기를 종료하지 않고 기존 개체를 사용하여 계산 결과를 미리 볼 수 있습니다.

또한 사용자 지정 가능한 &quot;지침&quot;에서 계산된 사용자 지정 필드에 대한 텍스트를 마우스로 가리키면 필드의 수식을 표시하거나 숨길 수 있습니다. 이 기능은 사용자 지정 양식을 작성할 사용자에게 해당 정보가 필요하지 않을 경우 유용합니다.

계산된 사용자 지정 필드 만들기에 대한 자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 상태 및 회사에 대한 감사 로그 정보 보기

이제 설정의 감사 로그 영역에서 상태 및 회사와 관련된 인시던트 문제를 보다 쉽게 해결할 수 있습니다.

For example:

* 이름을 바꾸거나, 잠기거나, 상태를 숨긴 사람과, 그런 사람을 언제 발견했는지 알 수 있습니다.
* 회사에서 일부 구성원 또는 Job 역할을 제거한 사람과 제거한 시기를 확인할 수 있습니다.

감사 로그 정보 보기에 대한 자세한 내용은 [감사 로그 보기 및 내보내기](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprint 회사 매핑 및 기타 개선 사항

이제 다음과 같은 Blueprint 개선 사항을 사용할 수 있습니다.

* 이제 일부 블루프린트를 설치하기 전에 사용자 지정할 수 있는 회사가 포함되어 있습니다. 블루프린트의 회사를 Workfront 인스턴스의 기존 회사에 매핑하거나, 필요한 경우 새 회사를 만들 수 있습니다.
* 이제 새 블루프린트 유형인 조직 구조를 사용할 수 있습니다. 일부 블루프린트는 여러 유형의 요소(예: 프로젝트 템플릿 및 조직 구조)를 포함합니다. 카탈로그 페이지에서 블루프린트 유형별로 필터링할 수 있습니다.
* 구성 페이지의 &quot;설치 환경 설정&quot; 및 &quot;템플릿 소유권&quot; 섹션이 단순함을 위해 &quot;템플릿 환경 설정&quot;에 결합되었습니다.

자세한 내용은 [블루프린트 구성](../../../administration-and-setup/blueprints/configure-template-package.md).

## 회사 멤버십을 보다 쉽게 관리

회사 영역에서 업데이트된 도구 모음을 사용하면 기존 Workfront 사용자를 회사에 쉽게 추가하고 회사 구성원을 제거할 수 있습니다.

이전에는 이러한 작업을 회사 편집 박스에서만 사용할 수 있었습니다.

업데이트된 도구 모음에는 구성원의 사용자 프로필 정보 편집 및 시스템에서 비활성화와 같이 이전 도구 모음에서 사용할 수 있었던 모든 작업이 포함되어 있습니다.

자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 새 계산된 필드 창에서 표현식 및 필드를 선택합니다

사용자 지정 양식에서 계산된 필드를 더 쉽게 만들 수 있도록 계속 노력하고 있습니다. 이제 최대화 를 클릭하여 새 계산 편집기를 열면 필요한 표현식과 필드를 찾아 선택할 수 있습니다.

자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 그룹은 작업표와 시간 기본 설정을 직접 구성할 수 있습니다

>[!NOTE]
>
>이 기능은 처음에 21.4 릴리스의 일부로 클러스터 4의 고객에게만 단계적 롤아웃을 통해 사용할 수 있었습니다. 이 기능은 2021년 11월 8일에 프로덕션에 있는 나머지 모든 클러스터에 사용할 수 있습니다.

대규모 조직에서는 시스템 수준에서 관리자가 구성한 환경 설정을 상속하지 않고 작업표와 시간 환경 설정을 고유한 워크플로우에 맞게 독립적으로 구성해야 할 수도 있습니다. 이제 Workfront 관리자는 시스템의 모든 그룹에 대한 작업표와 시간 기본 설정을 잠금 해제할 수 있으므로 직접 구성할 수 있습니다.

이 기능은 프로젝트 환경 설정, 작업 및 문제 환경 설정에 대해서도 최근에 추가되었습니다.

Workfront 관리자가 작업표 및 시간 기본 설정을 잠금 해제하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [그룹에 대한 작업표 및 시간 환경 설정 잠금 해제](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 기사 [작업표 및 시간 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

그룹 관리자가 잠금 해제된 작업 및 그룹에 대한 문제 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 작업표 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## 그룹의 잠금을 해제하거나 다시 잠글 여러 개의 알림을 선택합니다

이제 그룹의 이메일 알림을 더 빠르고 쉽게 잠금 해제하거나 다시 잠글 수 있습니다. 이제 여러 알림을 선택하고 선택 항목을 확인하여 올바른지 확인한 다음, 도구 모음에 표시되는 새 잠금 해제 또는 잠금 단추를 클릭할 수 있습니다.

이전에는 알림을 한 번에 한 번씩 잠금 해제와 다시 잠가야 했습니다. Workfront에는 현재 95개의 알림이 있으므로 전체 또는 많은 알림을 처리하는 데 시간이 걸립니다.

자세한 내용은 [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## 그룹 관리자의 경우: 그룹을 삭제할 때 교체 그룹을 쉽게 선택

그룹을 삭제할 때 [그룹 삭제] 상자에서 두 가지 향상된 기능을 통해 삭제된 그룹의 사용자, 작업 항목 및 하위 그룹을 보존할 대체 그룹을 쉽게 선택할 수 있습니다.

* 그룹 이름을 입력하여 빠르게 찾을 수 있습니다. 이전에는 입력할 수 없는 드롭다운 목록만 있었습니다. 원하는 그룹을 찾기 위해 목록을 스크롤해야 했기 때문에 많은 그룹이 있는 조직에는 문제가 되었습니다. 또한 드롭다운 목록에 항목 제한이 있으므로 원하는 그룹이 표시되지 않을 수 있습니다.
* 새 정보 아이콘을 사용하여 원하는 교체 그룹을 선택할 수 있습니다. 아이콘 위로 마우스를 이동하면 해당 그룹 위에 있는 그룹 계층 구조 및 해당 관리자 이름과 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.

자세한 내용은 [그룹 삭제](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## 계산된 필드를 만들기 위한 더 큰 영역

이제 사용자 지정 양식으로 복잡한 계산된 필드를 작성하는 것이 더 쉽습니다. 새 최대화 단추를 눌러 계산을 작성할 큰 편집 창을 엽니다. 완료되면 최소화를 클릭하여 사용자 지정 양식 작업을 계속합니다.

자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 그룹에 사용자 지정 양식 추가

이제 사용자 지정 양식이 그룹 개체에 대해 지원됩니다. 이를 통해 조직의 그룹이 특정 요구 사항과 워크플로우를 충족하는 정보를 쉽게 캡처하고 공유할 수 있습니다. 사용자는 다른 Workfront 객체에 대해 수행할 수 있는 것처럼 그룹에 대해 다음을 수행할 수 있습니다.

* 사용자 지정 양식 만들기
* 사용자 지정 양식 첨부
* 사용자 지정 양식 데이터 저장
* 사용자 지정 양식 제거
* 목록 및 새 Workfront 경험의 그룹 페이지에서 사용자 지정 데이터를 편집합니다

사용자 지정 양식에 대한 자세한 내용은 [사용자 지정 양식](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## OAuth2 앱을 만들어 Workfront과 애플리케이션 통합

이제 Workfront에서 내장된 통합을 제공하지 않는 다른 애플리케이션과 Workfront을 통합할 수 있습니다. 통합할 애플리케이션용 OAuth2 앱을 만들면 해당 애플리케이션에서 Workfront에 액세스할 수 있도록 허용하지만, 데이터는 업계 표준의 보안 OAuth2 인증 프로토콜로 보호됩니다.

이전에는 통합, Workfront Fusion 또는 Workfront API를 통해서만 다른 애플리케이션과 통합할 수 있었습니다.

자세한 내용은 [Workfront 통합을 위한 OAuth2 애플리케이션 만들기](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 회사 영역의 인터페이스 텍스트 개선 사항

설정의 회사 영역에서 새 확인 메시지와 약간의 문구 변경 사항을 통해 회사 멤버십을 보다 쉽게 관리할 수 있습니다. 예를 들어 왼쪽 패널의 섹션 이름 &quot;사람&quot;이 이제 &quot;회사 구성원&quot;이 됩니다.

회사 멤버십 관리에 대한 자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
