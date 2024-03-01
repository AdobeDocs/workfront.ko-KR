---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 새 라이센스로 오브젝트 및 영역에 액세스
description: 아래 표는 각 Adobe Workfront 라이선스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 수준의 액세스(편집 또는 보기)를 보여 줍니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 18%

---

# 새 라이센스로 오브젝트 및 영역에 액세스

<!-- Audited: 2/2024 -->

아래 표는 각 Adobe Workfront 라이선스에서 Workfront의 개체 및 영역에 대해 허용하는 가장 높은 수준의 액세스(편집 또는 보기)를 보여 줍니다.

* **보기**: 사용자가 항목을 검토하고 공유할 수 있습니다.
* **편집**: 사용자가 항목을 만들고, 편집하고, 삭제하고, 공유할 수 있습니다.

  >[!NOTE]
  >
  >다른 사용자가 오브젝트를 공유할 때 공유자는 오브젝트를 편집하는 기능을 제한하는 권한을 지정할 수 있습니다. 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>표준</td>
        <td>라이트</td>
        <td>기여자</td>
        <td>외부</td>
    </tr>
    <tr>
        <td>프로젝트</td>
        <td>편집</td>
        <td>보기</td>
        <td>보기(세부 정보 페이지만)</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>작업</td>
        <td>편집</td>
        <td>보기</td>
        <td>보기</td>
        <td>보기</td>
    </tr>
    <tr>
        <td>문제</td>
        <td>편집</td>
        <td>편집</td>
        <td>편집</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>포트폴리오</td>
        <td>편집</td>
        <td>보기</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>프로그램</td>
        <td>편집</td>
        <td>보기</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>보고서, 대시보드 및 캘린더</td>
        <td>편집</td>
        <td>보기</td>
        <td>보기*</td>
        <td>보기(캘린더에만 해당되며 공유 권한 없음)</td>
    </tr>
    <tr>
        <td>필터, 보기 및 그룹화</td>
        <td>편집</td>
        <td>편집</td>
        <td>편집</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>문서</td>
        <td>편집</td>
        <td>편집</td>
        <td>편집</td>
        <td>보기(공유 권한 없음)</td>
    </tr>
    <tr>
        <td>사용자</td>
        <td>편집</td>
        <td>보기</td>
        <td>보기</td>
        <td>보기</td>
    </tr>
    <tr>
        <td>팀</td>
        <td>편집</td>
        <td>보기</td>
        <td>보기</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>템플릿</td>
        <td>편집</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>재무 데이터</td>
        <td>편집</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>리소스 관리</td>
        <td>편집</td>
        <td>보기</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>시나리오 플래너</td>
        <td>편집</td>
        <td>보기</td>
        <td>액세스 권한 없음</td>
        <td>액세스 권한 없음</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>편집</td>
        <td>편집</td>
        <td>편집</td>
        <td>액세스 권한 없음</td>
    </tr>
</table>

&#42; 기여자 라이선스가 있는 사용자는 공유된 보고서, 대시보드 및 캘린더만 볼 수 있습니다.

>[!NOTE]
>
>Light 라이선스나 기여자 라이선스가 있는 사용자는 공유 기능이 제한됩니다. 자세한 내용은 [라이선스 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>외부 사용자가 Workfront에서 항목을 검색할 수 없습니다. 문서 및 캘린더와 특별히 공유되는 문서를 볼 수 있습니다. 또한 사용자와 항목을 공유하는 사용자를 볼 수 있습니다.

다음 문서에서 액세스 수준이 각 개체 및 영역에 허용하는 내용에 대한 자세한 정보를 찾을 수 있습니다.

* [프로젝트에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [문서에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [포트폴리오 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [프로그램에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [팀에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [템플릿에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [시나리오 플래너에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Adobe Workfront 목표에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
