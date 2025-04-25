---
content-type: release-notes
keywords: 메모,분기별,업데이트
navigation-topic: product-releases
title: 21.1 관리자 개선 사항
description: 이 페이지에서는 미리보기 환경에 대한 21.1 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1 관리자 개선 사항

이 페이지에서는 미리보기 환경에 대한 21.1 릴리스의 모든 관리자 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 2월 15일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

21.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록은 [21.1 릴리스 개요](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)를 참조하십시오.

## 프로젝트 복사를 위한 새로운 액세스 수준 설정 도입

시스템 관리자로서 플래너가 프로젝트로 수행할 수 있는 작업을 보다 세밀하게 제어할 수 있도록 프로젝트 복사 기능을 활성화하거나 비활성화할 수 있는 새로운 설정을 도입하여 액세스 수준의 프로젝트에 대한 편집 액세스 권한을 보다 세밀하게 설정했습니다. 이 변경 이전에는 프로젝트 편집에 대한 사용자 액세스 권한을 활성화하면 프로젝트 복사 권한이 자동으로 부여되었습니다. 새 기능을 사용하면 새 복사 설정을 비활성화하여 복사할 수 있는 액세스 권한이 없는 사용자가 프로젝트를 편집할 수 있는 액세스 권한을 부여할 수 있습니다.

이 변경 전에 사용자가 액세스 수준에서 프로젝트 편집에 액세스할 수 있었던 경우 이 기능이 릴리스되면 자동으로 이 설정이 활성화됩니다.

플랜 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

프로젝트 복사에 대한 자세한 내용은 [프로젝트 복사](../../../manage-work/projects/manage-projects/copy-project.md)를 참조하십시오.

이제 이 기능은 새 Workfront 환경의 [관리자 기본 사항, Workfront One의 1부: 사용자 조직](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) 학습 경로에 포함되어 있습니다.

## 오브젝트의 사용자 정의 양식에서 다중 선택 드롭다운 필드의 모든 항목을 선택합니다

>[!NOTE]
>
>새 요청을 제출할 때는 이 기능을 현재 사용할 수 없습니다.

객체에 대한 세부 정보 페이지에서 사용자 정의 양식의 다중 선택 드롭다운 필드를 입력할 때 사용 가능한 모든 옵션을 선택해야 하는 경우 모두 선택 을 클릭할 수 있습니다.

사용자 정의 양식에서 데이터를 편집하는 방법에 대한 자세한 내용은 [사용자 정의 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)을 참조하십시오.

## 오브젝트에 대한 모든 사용자 정의 양식 필드 다시 계산

이제 계산된 사용자 정의 필드의 모든 데이터가 오브젝트에 대해 최신 상태인지 확인하는 것이 더 쉽습니다. 새로운 표현식 다시 계산 메뉴 옵션을 사용하면 이러한 필드의 모든 데이터를 빠르게 다시 계산할 수 있습니다.

이 기능은 특히 개체의 계산된 사용자 지정 필드에서 참조하는 다른 개체의 데이터를 편집한 경우에 유용합니다.

이전에는 사용자가 계산된 사용자 정의 필드의 모든 데이터가 최신 상태인지 확인하기 위해 해결 방법을 사용해야 했습니다. 예를 들어, 벌크 편집에 사용할 수 있는 재계산 옵션을 사용하기 위해 다른 객체와 함께 객체를 편집했습니다.

자세한 내용은 [사용자 정의 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)을 참조하십시오.

## 그룹 관리자에 대한 작업 및 문제 환경 설정 잠금 해제

>[!NOTE]
>
>2021년 6월 24일까지 그룹에 대한 프로젝트 환경 설정을 잠금 해제하는 기능을 가진 고객에 대해서만 단계별 롤아웃의 일부로 사용할 수 있습니다. 이제 모든 고객이 이용할 수 있습니다.

이제 Adobe Workfront 관리자는 개별 작업 및 문제 환경 설정을 잠금 해제하여 그룹 관리자에게 보다 많은 자율성을 부여할 수 있습니다. 환경 설정이 잠금 해제되면 그룹 관리자는 각 그룹의 고유한 요구 사항 및 내부 프로세스를 제공하도록 그룹에 대해 환경 설정을 구성할 수 있습니다.

자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

이 기능은 이제 Workfront One의 새로운 Workfront 경험 2부: 프로젝트 설정](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)에서 [관리자 기본 사항에 포함되어 있습니다.

## 포트폴리오와 프로그램에 대한 액세스 수준 설정을 개별적으로 구성

이제 포트폴리오와 프로그램의 액세스 수준 설정을 별도로 구성할 수 있으므로 포트폴리오와 프로그램에 대한 사용자 액세스를 보다 쉽게 관리할 수 있습니다.

이전에는 포트폴리오와 프로그램에 대한 액세스 수준 설정이 결합되었습니다. 즉, 포트폴리오에 대해 동일한 방식으로 프로그램을 구성하지 않으면 프로그램에 대한 액세스 설정을 구성할 수 없으며, 반대의 경우도 마찬가지였습니다.

액세스 수준 구성에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

프로그램 및 포트폴리오에 대해 구성할 수 있는 액세스 설정에 대한 자세한 내용은 [각 개체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)를 참조하십시오.

이제 이 기능은 새 Workfront 환경의 [관리자 기본 사항, Workfront One의 1부: 사용자 조직](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) 학습 경로에 포함되어 있습니다.

## 사용자 정의 양식에서 정보를 편집할 때 일련의 확인란을 모두 선택합니다

>[!NOTE]
>
>새 요청을 제출할 때는 이 기능을 현재 사용할 수 없습니다.

개체에 대한 세부 정보 페이지에서 확인란이 포함된 사용자 정의 양식 필드를 채울 때 사용 가능한 확인란을 모두 선택해야 하는 경우 모두 선택을 클릭할 수 있습니다.

이 옵션은 필드에 확인란이 2개 이상 있는 경우에만 표시됩니다.

자세한 내용은 [사용자 정의 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)을 참조하십시오.

## Workfront 허용 목록에 추가하다 이메일 구성

허용 목록에 추가하다 이제 데이터 보안을 강화하기 위해 이메일 도메인을 사용하여 다음을 수행할 수 있습니다.

* Workfront에 저장된 보고서나 문서가 포함된 Workfront 이메일의 이동 경로 제어
* 제어 이메일 도메인은 사용자가 사용자 프로필에 지정할 수 있는 이메일 주소에 있을 수 있습니다

허용 목록에 추가하다 예를 들어, 위험 상태의 고객을 나열하는 보고서와 같은 중요한 데이터를 보호하려는 경우 이메일 도메인에 내부 이메일 또는 도메인만 포함할 수 있습니다. 이러한 방식으로 사용자는 해당 보고서(또는 다른 Workfront 보고서)를 외부 이메일 주소로 보낼 수 없습니다.

허용 목록에 추가하다 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) 문서 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 섹션을 참조하십시오.

## 하위 그룹에 그룹 관리자 할당

조직 수준이 독립적으로 더 쉽게 운영될 수 있도록 하위 그룹에 그룹 관리자를 할당하는 기능을 추가했습니다. 이제 하위 그룹 관리를 적합한 사람에게 위임할 수 있습니다.

이전에는 최상위 그룹만 그룹 관리자를 가질 수 있었으며, 이러한 관리자는 최상위 그룹 아래의 모든 하위 그룹을 관리했습니다.

자세한 내용은 문서 [하위 그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)의 [하위 그룹의 그룹 관리자](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) 섹션을 참조하십시오.

이제 이 기능은 새 Workfront 환경의 [관리자 기본 사항, Workfront One의 1부: 사용자 조직](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) 학습 경로에 포함되어 있습니다.

## 그룹에 대한 이벤트 알림 구성

>[!NOTE]
>
>그룹에 대한 프로젝트 환경 설정을 잠금 해제할 수 있는 고객에게만 단계별 롤아웃의 일부로 제공됩니다. 여기에는 클러스터 4와 6의 모든 고객과 다른 클러스터의 일부 고객이 포함됩니다. 이 참고 사항은 더 많은 클러스터에서 기능을 사용할 수 있게 됨에 따라 업데이트됩니다.

이제 Workfront 관리자는 그룹 관리자가 최상위 그룹에 대한 이벤트 알림을 구성할 수 있도록 하여 그룹 관리자에게 보다 많은 자율성을 부여할 수 있습니다. 하위 그룹은 최상위 그룹에서 이벤트 알림 구성을 상속합니다.

이전에는 이벤트 알림이 시스템 수준에서 Workfront 관리자만 구성할 수 있었습니다. 즉, 모든 그룹이 동일한 이벤트 알림 세트를 사용해야 했습니다.

자세한 내용은 다음 문서를 참조하십시오.

* [모든 그룹에 대한 이벤트 알림의 구성 잠금 해제 또는 잠금](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [그룹에 대한 이벤트 알림 보기 및 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

이제 이 기능은 새 Workfront 환경의 [관리자 기본 사항, Workfront One의 1부: 사용자 조직](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) 학습 경로에 포함되어 있습니다.

이 기능은 이제 Workfront One의 새 Workfront 경험에서 [전자 메일 및 인앱 알림](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) 학습 경로에 포함되어 있습니다.

## 그룹 영역에서 그룹 프로젝트 및 승인 진행을 사용하여 작업

그룹 관리자인 경우 그룹의 프로젝트 및 승인 프로세스가 그룹 영역에 나열되므로 이를 쉽게 보고 작업할 수 있습니다. 그룹의 기본 페이지에서 다음 작업을 수행할 수 있습니다.

* 왼쪽 메뉴에서 프로젝트 를 클릭하여 그룹의 프로젝트를 확인하고 그룹에 대한 새 프로젝트를 만듭니다. 선택한 프로젝트가 공유된 경우 도구 모음의 단추를 사용하여 프로젝트를 편집, 내보내기, 복사 또는 삭제할 수 있습니다.

  자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)을 참조하세요.

* 그룹과 관련된 모든 승인 프로세스를 보고 관리하려면 왼쪽 메뉴에서 승인 을 클릭합니다.

  자세한 내용은 [그룹 수준 승인 프로세스](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)를 참조하십시오.

이 기능은 Workfront 관리자도 사용할 수 있습니다.

## 그룹에서 사용 및 할당된 라이선스 수 보기

이제 라이선스가 얼마나 잘 배포되는지 확인하기 위해 그룹 및 그 아래에 있는 모든 하위 그룹에서 사용되는 라이선스 수를 볼 수 있습니다.

최상위 그룹을 관리하는 경우 그룹(및 해당 하위 그룹)에서 사용되는 라이선스 수와 그룹에 할당된 최대 라이선스 수를 모두 볼 수 있습니다.

자세한 내용은 [새 Adobe Workfront 환경에서 그룹에 할당되어 사용되는 라이선스 수 보기](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)를 참조하십시오.

