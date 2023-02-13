---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업표 보기에서 초과 작업 비용 계산'
description: Adobe Workfront에서는 기본적으로 초과 근무가 계산되지 않지만 초과 근무를 계산하는 작업표 보고서를 만들 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 보기: 작업표 보기에서 초과 작업 비용 계산

Adobe Workfront에서는 기본적으로 초과 근무가 계산되지 않지만 초과 근무를 계산하는 작업표 보고서를 만들 수 있습니다.

사용자가 프로필에서 시간당 비용 비율과 연관되어 있으면 해당 사용자의 시간외 근무 비용을 계산할 수도 있습니다.\
사용자를 시간당 비용과 연결하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [내 설정 구성](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>목록의 작업표 보기에 추가할 수 있는 초과 작업 필드나 보고서에는 작업표의 초과 작업 시간 필드에 있는 정보가 표시됩니다. 작업표를 수정할 수 있는 액세스 권한이 있는 사용자가 이 정보를 수동으로 업데이트합니다. 작업표의 초과 작업 필드에 대한 자세한 내용은 문서를 참조하십시오 [작업표 레이아웃 이해](../../../timesheets/timesheets/timesheet-layout.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업표 보기에서 초과 작업 시간 비용 계산

작업표 보기에 계산된 기간 열을 추가하려면 다음을 수행합니다.

1. 작업표 목록으로 이동하거나 작업표 보고서를 만듭니다.

   보고서 만들기에 대한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 클릭 **보기 사용자 지정** 작업표 목록

   또는

   을(를) 선택합니다 **열(보기)** 작업표 보고서의 탭입니다.

1. 클릭 **열 추가**.
1. 클릭 **텍스트 모드로 전환**.
1. 에서 **이 열에 표시** 영역을 클릭합니다. **텍스트를 편집하려면 클릭하십시오.**.
1. 다음 텍스트 모드 코드를 복사하여 **텍스트 모드** 대화 상자
   <pre>displayname=계산된 초과 작업 비용<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >이 계산에서는 사용자가 일반적으로 주 40시간을 작업한다고 가정합니다.

1. 클릭 **저장**&#x200B;를 클릭한 다음 새 보기의 이름을 지정하고 **보기 저장** 작업표 목록

   또는

   클릭 **저장 + 닫기** 작업표 보고서에서 사용됩니다.

1. (선택 사항 및 조건부) 작업표 보고서를 작성하는 경우 보고서 이름을 지정한 다음 **보고서 저장**.

   각 사용자의 시간외 근무 비용은 **계산된 초과 근무 비용** 열.

   ![calculated_overlaunch_cost_in_timeset_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
