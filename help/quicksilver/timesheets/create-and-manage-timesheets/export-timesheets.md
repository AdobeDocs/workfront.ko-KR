---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 타임시트 목록 내보내기
description: 직원 관리자 또는 타임시트 승인자는 담당 직원의 타임시트에 대한 정보를 빠르게 보려면 타임시트 목록을 다운로드해야 할 수 있습니다. 타임시트 목록을 내보내면 됩니다.
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 2%

---

# 타임시트 목록 내보내기

<!--Audited: 8/2024-->

직원 관리자 또는 타임시트 승인자는 담당 직원의 타임시트에 대한 정보를 빠르게 보려면 타임시트 목록을 다운로드해야 할 수 있습니다. 타임시트 목록을 내보내면 됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 밝게 또는 높음 </p>
   <p>현재: 검토 이상 </p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 문제에 대한 보기 또는 상위 액세스 권한 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>타임시트에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to Tasks and Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the timesheets</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan or license type you have, contact your Workfront administrator.-->

## 타임시트 목록 내보내기

{{step1-to-timesheets}}

**타임시트** 영역이 열립니다.


![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png)을(를) 클릭하고 키워드를 입력한 다음 특정 타임시트를 검색합니다. 예를 들어 일정 기간 또는 소유자 이름을 검색할 수 있습니다.

1. (선택 사항) 다음 중 하나를 수행하여 타임시트 목록의 필터를 업데이트합니다.

   * 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

     또는

     내 타임시트만 보려면 **내 타임시트**&#x200B;를 선택하십시오.

     내 타임시트 승인 또는 내 타임시트 필터가 타임시트 목록에 적용됩니다.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 필터 아이콘 ![](assets/filter-nwepng.png)을(를) 클릭하여 다른 필터를 적용하거나 새 필터를 만듭니다. 필터 만들기 또는 업데이트에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 및 내 타임시트 필터를 제거한 경우 내 타임시트 승인 및 내 타임시트 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   >
   >   
   >   
   >   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (선택 사항) **보기** ![](assets/view-icon.png) 또는 **그룹화** ![](assets/grouping.png) 아이콘을 클릭하여 다른 보기 또는 그룹화를 적용하거나 새 보기 또는 그룹화를 만듭니다.

   필터, 보기 또는 그룹화 만들기에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 필터 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront에서 보기 만들기 또는 편집](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront에서 그룹화 만들기](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 내보낼 타임시트를 선택한 다음 **내보내기** ![](assets/export-38x15.png) 아이콘을 클릭합니다.

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. 다음 옵션 중에서 타임시트 목록을 내보낼 파일 유형을 선택합니다.

   * PDF 랜드스케이프
   * PDF 세로
   * PDF 기타 크기
   * Excel
   * Excel(xlsx)
   * 탭으로 구분됨

   타임시트 목록은 선택한 형식으로 컴퓨터에 다운로드되며 다음 타임시트 정보를 포함합니다.

   * 날짜 범위
   * 소유자 이름
   * 총 시간
   * 초과 근무 금액
   * 승인자 이름
   * 상태
