---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 타임시트 정보 편집
description: 타임시트에 대한 관리 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 타임시트에 대한 정보를 편집할 수 있습니다. 예를 들어 타임시트의 소유자, 승인자 또는 시간대를 편집할 수 있습니다.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
source-wordcount: '739'
ht-degree: 5%
---
# 타임시트 정보 편집

타임시트에 대한 관리 액세스 권한이 있는 사용자는 Adobe Workfront에서 기존 타임시트에 대한 정보를 편집할 수 있습니다. 예를 들어 타임시트의 소유자, 승인자 또는 시간대를 편집할 수 있습니다.

단일 타임시트의 정보를 편집하거나 여러 타임시트를 일괄적으로 편집할 수 있습니다.

>[!IMPORTANT]
>
>사용자가 타임시트 프로필과 연결되어 있고 타임시트가 자동으로 생성되는 경우, 기존 타임시트에 대한 변경 사항은 이후 날짜에 대해 생성될 타임시트에 반영되지 않습니다. 자동으로 생성된 모든 타임시트에는 타임시트 프로필에 설정된 설정이 있습니다. 자세한 내용은 [타임시트 프로필 만들기](../create-and-manage-timesheets/create-timesheet-profiles.md)를 참조하세요.

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

## 타임시트 편집

{{step1-to-timesheets}}

보기 액세스 권한이 있는 모든 타임시트가 기본적으로 표시됩니다.

![타임시트 목록](assets/list-of-all-timesheets.png)

1. (선택 사항) **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하고 키워드를 입력하여 특정 타임시트를 검색합니다. 예를 들어 타임시트 시간대 또는 소유자 이름을 검색할 수 있습니다.

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

     또는

     내 타임시트만 보려면 **내 타임시트**&#x200B;를 선택하십시오.

     **내 타임시트 승인** 또는 **내 타임시트** 필터를 타임시트 목록에 적용합니다.

   * 필터를 적용하거나 새 필터를 만들려면 **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭하십시오. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 이러한 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

1. (선택 사항) 보기 또는 그룹화를 적용하거나 새 보기를 만들려면 **보기** ![보기 아이콘](assets/view-icon.png) 또는 **그룹화** ![그룹화 아이콘](assets/grouping.png) 아이콘을 클릭합니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 하나 이상의 타임시트를 선택한 다음 타임시트 목록 맨 위에 있는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. 다음 정보를 보거나 입력합니다.

   | 필드 이름 | 설명 |
   | --------- | ---------- |
   | 소유자 | <p>타임시트가 생성된 사용자의 이름입니다. 이 필드는 편집할 수 없습니다.</p><p>이 필드는 여러 타임시트를 선택할 때 표시되지 않습니다.</p> |
   | 시작 일자 | 타임시트의 시작 날짜입니다. |
   | 종료일 | 타임시트의 종료 날짜입니다. |
   | 상태 | <p>타임시트의 상태입니다. 다음은 가능한 타임시트 상태 옵션입니다.</p><ul><li>**열기**: 타임시트가 열려 있으며 시간 항목을 편집할 수 있습니다.</li><li>**제출됨**: 지정된 승인자에게 승인을 위해 타임시트가 제출됩니다.</li><li>**거부됨**: 타임시트가 승인자에 의해 승인되지 않았으므로 사용자가 시간 항목을 편집할 수 있도록 다시 사용할 수 있습니다.</li><li>**닫힘**: 타임시트가 사용자에 의해 닫히거나 승인자에 의해 승인되어 현재 닫힙니다. 종료된 타임시트에 시간을 추가할 수 없습니다.</li></ul> |
   | 승인자 | <p>승인자는 타임시트와 연계된 사용자에 대해 타임시트를 승인하는 사용자입니다. 타임시트 관리 권한이 있는 사용자만 승인자로 설정할 수 있습니다. 타임시트 관리 권한에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.</p> <p>타임시트 승인자의 이름을 입력하기 시작하고 목록에 표시될 때 선택합니다.</p> <p>타임시트에 여러 승인자가 있을 수 있습니다. 이 경우 승인자 중 한 명이 타임시트를 승인하면 타임시트가 **마감됨**(으)로 표시되고 나머지 모든 승인자의 타임시트 승인 목록에서 사라집니다.</p> |
   | 시간을 편집할 수 있음 | <p>승인자가 타임시트의 시간을 편집할 수 있도록 하려면 이 옵션을 선택합니다.</p><p>여러 타임시트를 선택하는 경우에는 이 옵션을 사용할 수 없습니다.</p> |
   | 초과 작업 | <p>타임시트에서 초과 작업 시간 상자를 숨기도록 선택할 수 있습니다.</p><p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> |

1. **저장**&#x200B;을 클릭합니다.
