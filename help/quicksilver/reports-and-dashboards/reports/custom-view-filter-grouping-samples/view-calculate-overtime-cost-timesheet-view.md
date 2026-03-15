---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업표 보기에서 초과 작업 비용 계산'
description: Adobe Workfront에서는 기본적으로 초과 시간이 계산되지 않지만 초과 시간을 계산하는 작업표 보고서를 만들 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 5%

---

# 보기: 작업표 보기에서 초과 작업 비용 계산

<!--Audited: 11/2024-->

Adobe Workfront에서는 기본적으로 초과 시간이 계산되지 않지만 초과 시간을 계산하는 작업표 보고서를 만들 수 있습니다.

사용자가 프로필의 시간당 비용 비율과 연관되어 있으면 해당 사용자의 초과 작업 시간에 대한 비용을 계산할 수도 있습니다.\
사용자를 시간당 비용과 연결하는 방법에 대한 자세한 내용은 [내 설정 구성](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) 문서를 참조하십시오.

>[!NOTE]
>
>목록이나 보고서의 작업표 보기에 추가할 수 있는 초과 작업 시간 필드에는 작업표의 초과 작업 시간 필드에 있는 정보가 표시됩니다. 작업표를 수정할 수 있는 액세스 권한이 있는 사용자가 이 정보를 수동으로 업데이트합니다. 작업표의 초과 작업 시간 필드에 대한 자세한 내용은 [작업표 레이아웃 개요](../../../timesheets/timesheets/timesheet-layout.md) 문서를 참조하십시오.

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>참여자 또는 필터 수정 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 레벨 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹에 대한 액세스를 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 작업표 보기에서 초과 작업 비용 계산

작업표 보기에 계산된 초과 작업 시간 열을 추가하려면 다음을 수행하십시오.

1. 작업표 목록으로 이동합니다.

1. **보기** 드롭다운 메뉴를 클릭한 다음 **새 보기**&#x200B;를 클릭합니다.

1. **열 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 상자에 있는 텍스트를 제거한 다음 다음 다음 텍스트 모드 코드를 복사하여 붙여넣습니다.

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >이 계산에서는 사용자가 일반적으로 주 40시간 근무한다고 가정합니다.

1. **완료**&#x200B;를 클릭한 다음 새 보기의 이름을 지정하고 작업표 목록에서 **보기 저장**&#x200B;을 클릭합니다.

   각 사용자의 초과 작업 비용은 **계산된 초과 작업 비용** 열에 표시됩니다.


