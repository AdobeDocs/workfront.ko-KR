---
content-type: release-notes
keywords: 메모,분기별,업데이트
navigation-topic: product-releases
title: 21.1 관리자 개선 사항
description: 이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 향상된 모든 관리자 기능을 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1 관리자 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.1 릴리스로 향상된 모든 관리자 기능을 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 프로덕션 환경에서 사용할 수 있습니다.

21.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.1 릴리스 개요](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 프로젝트 복사를 위한 새 액세스 수준 설정 소개

시스템 관리자로서, 플래너가 프로젝트를 사용하여 수행할 수 있는 작업을 보다 세밀하게 제어하기 위해, 프로젝트 복사 기능을 활성화하거나 비활성화할 수 있는 새로운 설정을 도입하여 액세스 수준의 프로젝트에 대한 편집 액세스를 보다 세밀하게 만들었습니다. 이 변경 전에 프로젝트 편집에 대한 사용자의 액세스를 활성화하면 자동으로 해당 프로젝트를 복사할 수 있는 액세스 권한이 부여되었습니다. 새 기능을 사용하면 새 복사 설정을 비활성화하여 복사할 수 있는 액세스 권한이 없어도 다른 사용자에게 프로젝트 편집 액세스 권한을 제공할 수 있습니다.

사용자가 이 변경 전에 액세스 수준에서 프로젝트 편집에 액세스할 수 있는 경우 이 기능이 릴리스될 때 자동으로 이 설정이 활성화됩니다.

계획 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

프로젝트 복사에 대한 자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md).

이 기능은 이제 [새로운 Workfront 환경의 관리자 기본 사항, 1부: 사용자 조직](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One에서 학습 경로.

## 개체의 사용자 지정 양식에서 다중 선택 드롭다운 필드에서 모든 항목을 선택합니다

>[!NOTE]
>
>현재 새 요청을 제출할 때는 이 기능을 사용할 수 없습니다.

개체의 세부 정보 페이지에서 사용자 지정 양식의 다중 선택 드롭다운 필드를 채우는 경우 사용 가능한 옵션을 모두 선택해야 하는 경우 모두 선택을 클릭할 수 있습니다.

사용자 지정 양식에서 데이터 편집에 대한 자세한 내용은 [사용자 지정 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 개체의 모든 사용자 지정 양식 필드 다시 계산

이제 계산된 사용자 지정 필드의 모든 데이터가 개체에 대해 최신 상태인지 확인하는 것이 더 쉽습니다. 새 표현식 다시 계산 메뉴 옵션을 사용하면 이러한 필드의 데이터를 모두 빠르게 다시 계산할 수 있습니다.

이 기능은 개체의 계산된 사용자 지정 필드에서 참조하는 다른 개체의 데이터를 편집한 후에 특히 유용합니다.

이전에는 사용자가 계산된 사용자 지정 필드의 모든 데이터가 최신 상태인지 확인하기 위해 해결 방법을 사용해야 했습니다. 예를 들어, 벌크 편집에 사용할 수 있는 다시 계산 옵션을 사용하기 위해 개체를 다른 개체와 함께 편집했습니다.

자세한 내용은 [사용자 지정 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 그룹 관리자에 대한 작업 잠금 해제 및 문제 환경 설정

>[!NOTE]
>
>2021년 6월 24일까지, 이 기능은 그룹에 대한 프로젝트 환경 설정을 잠금 해제할 수 있는 고객에게만 단계별 롤아웃을 통해 사용할 수 있었습니다. 이제 모든 고객이 이용할 수 있습니다.

이제 Adobe Workfront 관리자는 개별 작업 및 문제 환경 설정을 잠금 해제하여 그룹 관리자에게 더 많은 자율성을 제공할 수 있습니다. 기본 설정이 잠금 해제되면 그룹 관리자는 해당 그룹이 각 그룹의 고유한 요구 사항과 내부 프로세스를 제공하도록 구성할 수 있습니다.

자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

이 기능은 이제 [새로운 Workfront 환경의 관리자 기본 사항, 2부: 프로젝트 설정](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) Workfront One에서 학습 경로.

## 포트폴리오 및 프로그램에 대한 액세스 수준 설정을 별도로 구성

이제 액세스 수준 설정을 별도로 구성할 수 있으므로 포트폴리오와 프로그램에 대한 사용자 액세스를 관리하는 것이 더 쉽습니다.

이전에는 포트폴리오와 프로그램에 대한 액세스 수준 설정이 결합되었습니다. 즉, 포트폴리오에 대해 동일한 방식으로 프로그램을 구성하지 않으면 프로그램에 대한 액세스 설정을 구성할 수 없으며 이는 반대로 적용된 것입니다.

액세스 수준 구성에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

프로그램 및 포트폴리오에 대해 구성할 수 있는 액세스 설정에 대한 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

이 기능은 이제 [새로운 Workfront 환경의 관리자 기본 사항, 1부: 사용자 조직](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One에서 학습 경로.

## 사용자 지정 양식에서 정보를 편집할 때 시리즈의 모든 확인란을 선택합니다

>[!NOTE]
>
>현재 새 요청을 제출할 때는 이 기능을 사용할 수 없습니다.

개체의 세부 정보 페이지에서 확인란이 포함된 사용자 지정 양식 필드를 입력할 때 사용 가능한 모든 확인란을 선택해야 하는 경우 모두 선택 을 클릭할 수 있습니다.

이 옵션은 필드에 2개 이상의 확인란이 포함된 경우에만 표시됩니다.

자세한 내용은 [사용자 지정 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Workfront 이메일 허용 목록에 추가하다 구성

이제 데이터 보안을 향상하기 위해 이메일 도메인을 사용하여 다음을 수행할 수 허용 목록에 추가하다 있습니다.

* Workfront에 저장된 보고서나 문서가 포함된 경우 Workfront 이메일이 이동할 수 있는 위치를 제어합니다
* 제어 이메일 도메인은 사용자가 사용자 프로필에 지정할 수 있는 이메일 주소에 포함될 수 있습니다

예를 들어 위험 발생 시 고객을 나열하는 보고서와 같은 중요한 데이터를 보호하려는 경우 내부 이메일 도메인 또는 도메인만 이메일 도메인에 포함할 수 허용 목록에 추가하다 있습니다. 그렇게 하면 사용자가 해당 보고서(또는 다른 Workfront 보고서)를 외부 이메일 주소로 보낼 수 없습니다.

자세한 내용은 섹션을 참조하십시오 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) 기사 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 하위 그룹에 대한 그룹 관리자 할당

조직 수준이 독립적으로 운영되도록 하기 위해 Adobe에서는 하위 그룹에 그룹 관리자를 할당할 수 있는 기능을 추가했습니다. 이제 하위 그룹 관리를 올바른 사람에게 위임하고 있는지 확인할 수 있습니다.

이전에는 최상위 그룹만 그룹 관리자를 가질 수 있었고 그러한 관리자는 최상위 그룹 아래에 있는 모든 하위 그룹을 관리했습니다.

자세한 내용은 섹션을 참조하십시오 [하위 그룹의 그룹 관리자](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) 기사 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

이 기능은 이제 [새로운 Workfront 환경의 관리자 기본 사항, 1부: 사용자 조직](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One에서 학습 경로.

## 그룹에 대한 이벤트 알림 구성

>[!NOTE]
>
>그룹에 대한 프로젝트 환경 설정을 잠금 해제할 수 있는 고객에게만 단계별 롤아웃을 통해 제공됩니다. 여기에는 클러스터 4와 6의 모든 고객과 다른 클러스터의 적은 수의 고객이 포함됩니다. 이 메모는 더 많은 클러스터에서 기능을 사용할 수 있게 되면 업데이트됩니다.

이제 Workfront 관리자는 최상위 그룹에 대한 이벤트 알림을 구성할 수 있으므로 그룹 관리자에게 더 많은 자율성을 제공할 수 있습니다. 하위 그룹은 상위 상위 상위 그룹에서 이벤트 알림 구성을 상속합니다.

이전에는 시스템 수준에서 Workfront 관리자만 이벤트 알림을 구성할 수 있었습니다. 즉, 모든 그룹이 동일한 이벤트 알림 세트를 사용해야 했습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [모든 그룹에 대한 이벤트 알림 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

이 기능은 이제 [새로운 Workfront 환경의 관리자 기본 사항, 1부: 사용자 조직](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront One에서 학습 경로.

이 기능은 이제 [새로운 Workfront 환경의 이메일 및 인앱 알림](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) Workfront One에서 학습 경로.

## 그룹 영역에서 그룹 프로젝트 및 승인 프로세스를 사용하여 작업

그룹 관리자라면 이제 그룹 영역에 프로젝트 및 승인 프로세스가 나열되므로 그룹의 프로젝트를 보고 작업할 수 있습니다. 그룹의 주 페이지에서 다음을 수행할 수 있습니다.

* 왼쪽 메뉴에서 프로젝트 를 클릭하여 그룹의 프로젝트를 확인하고 그룹에 대해 새 프로젝트를 만듭니다. 선택한 프로젝트가 사용자와 공유된 경우 도구 모음의 버튼을 사용하여 프로젝트를 편집, 내보내기, 복사 또는 삭제할 수 있습니다.

   자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* 왼쪽 메뉴에서 승인 을 클릭하여 그룹과 연관된 모든 승인 프로세스를 확인하고 관리합니다.

   자세한 내용은 [그룹 수준 승인 프로세스](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Workfront 관리자도 이 기능을 사용할 수 있습니다.

## 그룹에 사용 및 할당된 라이선스 수 보기

이제 라이센스가 얼마나 잘 배포되는지 확인하기 위해 한 그룹에서 사용되는 라이선스 수와 그 아래의 하위 그룹 수를 볼 수 있습니다.

최상위 그룹을 관리하는 경우 그룹(및 해당 하위 그룹)에 사용되는 라이선스 수와 그룹에 할당된 최대 라이선스 수를 모두 볼 수 있습니다.

자세한 내용은 [새 Adobe Workfront 경험에서 그룹에 할당되고 사용되는 라이선스 수를 봅니다](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

