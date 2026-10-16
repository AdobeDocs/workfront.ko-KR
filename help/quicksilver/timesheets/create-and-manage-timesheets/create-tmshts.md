---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 일회용 타임시트 만들기
description: 반복되지 않는 타임시트를 원하는 경우 일회용 타임시트를 수동으로 만들 수 있습니다. 타임시트의 종료 날짜에 도달하여 더 많은 타임시트가 필요한 경우 새 타임시트를 만들어야 합니다.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 3%
---
# 일회용 타임시트 만들기

<!--Audited: 6/2025-->

반복되지 않는 타임시트를 원하는 경우 일회용 타임시트를 수동으로 만들 수 있습니다. 타임시트의 종료 날짜에 도달하여 더 많은 타임시트가 필요한 경우 새 타임시트를 만들어야 합니다.

사용자의 추가 개입 없이 사용자의 반복 타임시트를 생성하는 타임시트 프로필 만들기에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하십시오.

타임시트 프로필과 연결된 시스템의 모든 사용자에 대해 타임시트를 수동으로 생성하는 방법에 대한 자세한 내용은 [타임시트 수동으로 생성](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)을 참조하십시오.

>[!NOTE]
>
>* 그룹에 대해 일회용 타임시트를 만들 수 없습니다.
>* 일회용 타임시트를 만드는 경우 타임시트에 포함할 특정 일반 시간 유형을 선택할 수 없습니다. 시스템에서 활성화된 모든 일반 시간 유형이 수동으로 생성된 타임시트에 표시됩니다.
>
>타임시트에 표시할 특정 일반 시간 유형만 선택하려면 타임시트 프로필을 사용하십시오. 타임시트 프로필에 대한 자세한 내용은 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)을 참조하세요.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>타임시트에 대한 관리 액세스</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 일회용 타임시트 만들기

{{step1-to-timesheets}}

보기 액세스 권한이 있는 모든 타임시트가 기본적으로 표시됩니다.

![타임시트 목록](assets/list-of-all-timesheets.png)

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

     또는

     내 타임시트만 보려면 **내 타임시트**&#x200B;를 선택하십시오.

     **내 타임시트 승인** 또는 **내 타임시트** 필터를 타임시트 목록에 적용합니다.

   * 필터를 적용하거나 새 필터를 만들려면 **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭하십시오. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

1. (선택 사항) **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하여 키워드를 입력하고 특정 타임시트를 검색합니다. 예를 들어 소유자 이름의 타임시트 시간대를 검색할 수 있습니다.

1. (선택 사항) 보기 또는 그룹화를 적용하거나 새 보기를 만들려면 **보기** ![보기 아이콘](assets/view-icon.png) 또는 **그룹화** ![그룹화 아이콘](assets/grouping.png) 아이콘을 클릭합니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 타임시트 목록 맨 위에 있는 **새 타임시트**&#x200B;를 클릭합니다.

   다음 정보를 입력합니다.

   | 필드 이름 | 설명 |
   | --------- | ---------- |
   | 다음에 대한 타임시트 만들기: | 타임시트를 만들 사용자, 작업 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 클릭합니다. |
   | 시작 일자 | 타임시트의 시작 날짜입니다. |
   | 종료일 | 타임시트의 종료 날짜입니다. |
   | 승인자 | <p>승인자는 타임시트와 연계된 사용자에 대해 타임시트를 승인하는 사용자입니다. 타임시트 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 타임시트 관리 권한에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.</p> <p>타임시트 승인자의 이름을 입력하기 시작하고 목록에 표시될 때 선택합니다.</p> <p>타임시트에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 타임시트를 승인하면 타임시트가 **마감됨**(으)로 표시되고 나머지 모든 승인자의 타임시트 승인 목록에서 사라집니다.</p> |
   | 시간을 편집할 수 있음 | <p>승인자가 타임시트의 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p><p>이 옵션은 설정 > 타임시트 및 시간 > 환경 설정 영역에서 **타임시트 편집을 소유자 및 관리자로 제한** 설정과 함께 작동합니다. 자세한 내용은 [타임시트 및 시간 환경 설정 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.</p><p>다음과 같은 시나리오가 있습니다.</p><p>**타임시트 편집을 소유자 및 관리자로 제한** 옵션이 활성화된 경우:</p><ul><li>승인자는 **시간 편집 가능**&#x200B;의 사용 여부와 상관없이 타임시트만 승인하고 거부할 수 있습니다.</li><li>타임시트 소유자의 관리자는 부하 직원의 타임시트만 볼 수 있습니다.</li></ul><p>**타임시트 편집을 소유자 및 관리자로 제한** 옵션이 비활성화된 경우:</p><ul><li>**시간을 편집할 수 있음**&#x200B;이 활성화되면 승인자는 타임시트를 제출하거나 다시 열거나 닫을 수 있고 시간을 편집할 수 있습니다.</li><li>**시간을 편집할 수 있음**&#x200B;이 비활성화되면 승인자는 타임시트를 제출하거나 다시 열거나 닫을 수 없으며 시간을 편집할 수 없습니다. 승인자는 타임시트만 승인하거나 거부할 수 있습니다.</li><li>타임시트 소유자의 관리자는 부하 직원의 타임시트를 제출, 회수, 다시 열고 편집할 수 있습니다.</li></ul><p>**참고**</br>&#x200B;승인을 위해 타임시트를 제출하면 더 이상 시간을 편집할 수 없습니다. 제출된 타임시트를 편집 가능한 상태로 되돌리려면 타임시트를 불러오거나 승인자가 타임시트를 거부하도록 하십시오. 자세한 내용은 [승인을 위한 타임시트 제출](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) 및 [타임시트 승인](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)을 참조하세요. |
   | 초과 작업 | 타임시트에서 **초과 근무** 상자를 숨기도록 선택할 수 있습니다. 이 옵션은 기본적으로 비활성화되어 있습니다. |

1. **타임시트 만들기**&#x200B;를 클릭합니다.

## 사용자의 타임시트에 작업 및 문제가 표시되는 경우

사용자에게 할당된 작업 또는 문제가 다음 기준을 충족하면 사용자의 타임시트에 자동으로 표시됩니다.

* 사용자가 작업 또는 문제에 시간을 기록했습니다.
* 작업 또는 문제의 계획된 일자가 타임시트의 일자 내에 있습니다.
* 작업 또는 문제의 실제 시작 일자(작업 또는 문제 상태가 진행 중)가 있습니다.
* 작업 또는 문제가 타임시트에 고정됨
* 계획된 완료 일자가 타임시트의 일자 범위에 속하며 상태는 진행 중입니다.

**타임시트를 ...** 환경 설정(타임시트 및 시간 환경 설정에 있음)을 선택 취소한 경우 타임시트에 진행 중 상태의 문제와 작업이 표시됩니다. 타임시트 및 시간 환경 설정에 대한 자세한 내용은 [타임시트 및 시간 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)을 참조하십시오.
