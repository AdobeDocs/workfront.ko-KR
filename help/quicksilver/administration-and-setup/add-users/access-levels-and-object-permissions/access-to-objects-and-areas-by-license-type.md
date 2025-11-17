---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 라이선스 유형별 오브젝트 및 영역에 대한 액세스
description: 아래 표는 각 Adobe Workfront 라이선스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 수준의 액세스(편집 또는 보기)를 보여 줍니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 24%

---

# 라이선스 유형별 오브젝트 및 영역에 대한 액세스

<!-- Audited: 11/2025 -->

아래 표는 각 Adobe Workfront 라이선스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 수준의 액세스(편집 또는 보기)를 보여 줍니다.

* 보기: 사용자가 항목을 검토하고 공유할 수 있습니다.
* 편집: 사용자가 항목을 만들고, 편집하고, 삭제하고, 공유할 수 있습니다.

  >[!NOTE]
  >
  >다른 사용자가 오브젝트를 공유할 때 공유자는 오브젝트를 편집하는 기능을 제한하는 권한을 지정할 수 있습니다. 새 라이선스 유형에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

  >[!NOTE]
  >
  >이 문서에는 기존 라이선스 유형의 개체 액세스에 대한 정보가 포함되어 있습니다. 새 라이선스 유형에 대한 자세한 내용은 [새 액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) 및 [새 라이선스 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)를 참조하십시오.

|   | 플랜 | 작업 | 검토 | 요청 | 외부 |
|---|---|---|---|---|---|
| 프로젝트 | 편집 | 편집(만들기 권한 없음) | 보기 | 보기(세부 정보 페이지만) | 액세스 권한 없음 |
| 작업 | 편집 | 편집 | 보기 | 보기 | 액세스 권한 없음 |
| 문제 | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |
| 포트폴리오 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 프로그램 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 보고서, 대시보드 및 캘린더 | 편집 | 보기 | 보기 | 보기&#42; | 보기(캘린더에만 해당되며 공유 권한 없음) |
| 필터, 보기 및 그룹화 | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |
| 문서 | 편집 | 편집 | 편집 | 편집 | 보기(공유 권한 없음) |
| 사용자 | 편집 | 보기 | 보기 | 보기 | 보기 |
| 팀 | 편집 | 편집 | 보기 | 보기 | 액세스 권한 없음 |
| 템플릿 | 편집 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 |
| 재무 데이터 | 편집 | 보기(프로젝트 세부 정보의 재무 영역만) | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 리소스 관리 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 시나리오 플래너 | 편집 | 편집 | 편집 | 액세스 권한 없음 | 액세스 권한 없음 |
| Workfront Goals | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |

요청 라이선스가 있는 &#42;명의 사용자는 공유된 보고서, 대시보드 및 캘린더만 볼 수 있습니다.

>[!NOTE]
>
>검토 라이선스 또는 요청 라이선스가 있는 사용자의 공유 기능은 제한됩니다. 자세한 내용은 [라이선스 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)를 참조하십시오.
>
>외부 사용자가 Workfront에서 항목을 검색할 수 없습니다. 문서 및 캘린더와 특별히 공유되는 문서를 볼 수 있습니다. 또한 사용자와 항목을 공유하는 사용자를 볼 수 있습니다.

다음 문서에서 액세스 수준이 각 개체 및 영역에 허용하는 내용에 대한 자세한 정보를 찾을 수 있습니다.

* [프로젝트에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [문서에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [포트폴리오에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [프로그램에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [보고서, 대시보드 및 일정에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [팀에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [템플릿에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [시나리오 플래너에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Adobe Workfront 목표에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
