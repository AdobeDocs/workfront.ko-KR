---
title: 보고서, 대시보드 및 캘린더 공유
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 보고서, 대시보드 및 달력을 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 보고서, 대시보드 및 캘린더에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 보고서, 대시보드 및 캘린더 공유

Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 보고서, 대시보드 및 달력을 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 보고서, 대시보드 및 캘린더에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유 액세스 권한이 있는 특정 보고서, 대시보드 또는 달력을 보거나 관리할 수 있는 권한을 부여할 수도 있습니다. 개체에 대한 공유 권한을 사용자에게 부여하는 방법에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

각 액세스 수준의 사용자가 문제에 대해 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)의 [보고서](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) 섹션을 참조하십시오.

## 보고서, 대시보드 또는 캘린더 공유에 대한 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

* 보고서, 대시보드 또는 캘린더의 작성자에게는 기본적으로 관리 권한이 있습니다.
* 보고서, 대시보드 및 달력을 공유하는 것은 Workfront의 다른 개체를 공유하는 것과 유사합니다.

  Workfront에서 개체를 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

  보고서, 대시보드 및 달력을 공유하는 방법에 대해 알아보려면 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 보고서 공유](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [대시보드 공유](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [캘린더 보고서 공유](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* 보고서와 대시보드를 개별적으로 공유하거나 일괄적으로 공유할 수 있습니다.

  캘린더는 개별적으로 공유할 수 있습니다. 일괄적으로 공유할 수 없습니다.

* 기본 제공 시스템 보고서는 공유할 수 없습니다. 사용자 지정 보고서만 공유할 수 있습니다.

  시스템 보고서를 새 사용자 지정 보고서로 저장하는 방법에 대한 자세한 내용은 [보고서 복사본 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)를 참조하십시오.

* 보고서, 대시보드 및 달력에 다음 권한을 부여할 수 있습니다.

   * 보기
   * 관리

* 대시보드를 공유할 때 대시보드의 모든 보고서, 달력 및 외부 페이지에 대한 보기 권한은 기본적으로 사용자에게 있습니다.
* 요청 라이선스가 있는 사용자는 시스템 전체 보고서를 볼 수 없습니다. 보고서를 조회해야 하는 경우 요청자와 개별적으로 공유해야 합니다.
* 보고서에 프롬프트가 있고 공개적으로 공유하는 경우 보고서에 액세스하는 사용자가 Workfront에 로그인해야 프롬프트를 사용하여 보고서를 실행할 수 있습니다. Workfront에 로그인할 수 없는 경우 보고서에 적용하라는 메시지가 표시되지 않습니다.\
  프롬프트와 보고서를 공유하는 제한 사항에 대한 자세한 내용은 문서 [보고서에 프롬프트 추가](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)의 [프롬프트 보고서 공유 제한](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) 섹션을 참조하십시오.

* 보고서 또는 달력에서 상속된 권한을 제거할 수 있습니다.

  개체에서 상속된 사용 권한을 제거하는 방법에 대한 자세한 내용은 [개체에서 사용 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)를 참조하십시오.

* 보고서 또는 달력을 공개적으로 또는 시스템 전체에서 공유할 수도 있습니다.

  대시보드를 공개적으로 공유할 수는 없지만 시스템 전반에서 공유할 수는 있습니다.

  >[!CAUTION]
  >
  >외부 사용자와 기밀 정보가 포함된 오브젝트를 공유할 때는 주의하는 것이 좋습니다. 이를 통해 Workfront 사용자 또는 조직의 일부가 아니더라도 정보를 볼 수 있습니다.
