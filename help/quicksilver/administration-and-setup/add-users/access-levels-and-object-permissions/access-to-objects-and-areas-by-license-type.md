---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 라이선스 유형별 개체 및 영역에 대한 액세스
description: 아래 표는 각 Adobe Workfront 라이센스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 액세스 수준(편집 또는 보기)을 알려줍니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 19%

---

# 라이선스 유형별 개체 및 영역에 대한 액세스

아래 표는 각 Adobe Workfront 라이센스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 액세스 수준(편집 또는 보기)을 알려줍니다.

* **보기**: 사용자는 항목을 검토하고 공유할 수 있습니다.
* **편집**: 사용자는 항목을 생성, 편집, 삭제 및 공유할 수 있습니다.

   >[!NOTE]
   >
   >다른 사용자가 개체를 공유할 때 공유자는 개체를 편집하는 능력을 제한하는 권한을 지정할 수 있습니다. 자세한 내용은 [개체에 대한 권한 공유 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | 플랜 | 작업 | 검토 | 요청 | 외부 |
|---|---|---|---|---|---|
| 프로젝트 | 편집 | 편집(만들기 권한 없음) | 보기 | 보기(세부 사항 페이지만) | 액세스 권한 없음 |
| 작업 | 편집 | 편집 | 보기 | 보기 | 보기 |
| 문제 | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |
| 포트폴리오 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 프로그램 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 보고서, 대시보드 및 달력 | 편집 | 보기 | 보기 | &#42; 보기 | 보기(달력에 대해서만, 공유 권한 없음) |
| 필터, 보기 및 그룹화 | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |
| 문서 | 편집 | 편집 | 편집 | 편집 | 보기(공유 권한 없음) |
| 사용자 | 편집 | 보기 | 보기 | 보기 | 보기 |
| 팀 | 편집 | 편집 | 보기 | 보기 | 액세스 권한 없음 |
| 템플릿 | 편집 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 |
| 재무 데이터 | 편집 | 뷰(프로젝트 상세내역의 재무 영역만) | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 리소스 관리 | 편집 | 보기 | 보기 | 액세스 권한 없음 | 액세스 권한 없음 |
| 시나리오 플래너 | 편집 | 편집 | 편집 | 액세스 권한 없음 | 액세스 권한 없음 |
| Workfront 목표 | 편집 | 편집 | 편집 | 편집 | 액세스 권한 없음 |

&#42; 요청 라이센스가 있는 사용자는 공유된 보고서, 대시보드 및 달력만 볼 수 있습니다.

>[!NOTE]
>
>검토 라이선스 또는 요청 라이선스를 가진 사용자에게 공유 기능이 제한됩니다. 자세한 내용은 [Adobe Workfront 라이선스 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>외부 사용자는 Workfront에서 항목을 검색할 수 없습니다. 이 사용자는 특별히 공유된 문서와 달력을 볼 수 있습니다. 또한 사용자와 항목을 공유하는 사용자를 볼 수 있습니다.

다음 문서에서 각 개체 및 영역에 대해 액세스 수준이 허용하는 사항에 대한 자세한 정보를 찾을 수 있습니다.

* [프로젝트에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [문서에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [포트폴리오 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [프로그램에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [팀에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [템플릿에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [시나리오 플래너에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Adobe Workfront 목표에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
