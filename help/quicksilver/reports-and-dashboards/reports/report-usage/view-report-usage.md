---
product-area: reporting
navigation-topic: report-usage
title: 보고서 사용량 보기
description: 보고서 사용량 보기
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# 보고서 사용량 보기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

시스템에서 얼마나 많은 보고서가 사용되는지를 이해하기 위해 보고서 목록에서 다음 정보를 볼 수 있습니다.

* 보고서를 본 마지막 10명의 사용자
* 지정된 기간 내의 보기 횟수

   >[!NOTE]
   >
   >Adobe Workfront은 사용자당 하루에 한 개의 보기를 계산합니다. 하루에 여러 번 동일한 보고서에 액세스하는 경우 Workfront에서는 이 보고서를 해당 보고서에 대한 한 개의 보기로 계산합니다. 같은 날 다른 사용자가 동일한 보고서에 액세스하면 Workfront에서는 이를 두 번째 사용자에 대한 새 보기로 계산합니다.

* 마지막으로 조회한 일자
* 사용자가 마지막으로 본 날짜
* 보고서가 들어 있는 대시보드 목록입니다\
   보고서 목록에 추가할 수 있는 대시보드의 이름을 표시하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [대시보드에서 보고서를 구성하는 방법을 이해합니다](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

이 정보를 표시할 수 있는 보고서 목록에 대한 보기를 작성할 수 있습니다.\
이러한 필드 중 일부별로 보고서 목록을 필터링할 수 있습니다.\
보고서를 필터링할 수 있는 필드에 대한 자세한 내용은 문서를 참조하십시오 [사용 정보별로 보고서 목록 필터링](#filter-a-report-list-by-usage-information).

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

## 보고서 목록 보기에 보고서 사용 정보 표시

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.

1. 보고서 목록에서 **보기** 드롭다운 메뉴
1. (선택 사항) **보고서 사용량** 가장 일반적인 보고서 사용 정보를 표시하는 보기.\
   또는

1. 클릭 **새 보기** 사용자 지정 보기를 만들려면
1. 클릭 **열 추가**.
1. 다음 필드 중 하나를 입력하고 목록 아래에 이 필드가 나타나면 선택합니다 **보고서** 새 열에 추가할 객체입니다.

   * **최근 10명의 사용자**: 보고서를 본 마지막 10명의 사용자의 이름을 표시합니다.
   * **보기 횟수**: 다음 기간 내의 보기 수를 표시합니다.

      * **이번 달, 분기, 연도**
      * **지난달, 분기, 년**
      * **모든 보기**: 보고서의 모든 보기에 대한 전체 개수를 표시합니다
   * **마지막으로 본 사람**: 보고서를 마지막으로 본 사용자에 대한 정보를 표시합니다
   * **마지막으로 본 날짜**: 보고서를 마지막으로 본 날짜를 표시합니다


1. 클릭 **보기 저장**.\
   보고서에 대한 사용량 정보는 보기에 추가한 열에 표시됩니다.\
   보고서 객체에 대한 보고서를 작성하고 이 보기를 보고서에서 사용할 수도 있습니다.\
   보고서 작성에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   보고서를 만들려면 액세스 수준의 보고서에 대한 편집 액세스 권한이 있어야 합니다.\
   보고서 액세스에 대한 자세한 내용은 문서를 참조하십시오 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 사용 정보별로 보고서 목록 필터링 {#filter-a-report-list-by-usage-information}

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 보고서 목록에서 **필터** 드롭다운 메뉴
1. 클릭 **새 필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**.
1. 다음 필드 중 하나를 입력하고 목록 아래에 이 필드가 나타나면 선택합니다 **보고서** 새 필터 규칙으로 추가할 개체:

   * **보기 횟수**: 다음 기간 내의 보기 수를 표시합니다.

      * **이번 달, 분기, 연도**
      * **지난달, 분기, 년**
      * **모두 보기**
   * **마지막으로 본 사람**: 보고서를 마지막으로 본 사용자에 대한 정보를 표시합니다
   * **마지막으로 본 날짜**: 보고서를 마지막으로 본 날짜를 표시합니다


1. 필드에 대한 수정자를 선택한 다음, 메시지가 표시되면 값을 지정합니다.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. 클릭 **필터 저장**.\
   정의한 사용 정보를 충족하는 보고서 목록이 표시됩니다.\
   보고서 개체에 대한 보고서를 작성하고 이 필터를 보고서에서 사용할 수도 있습니다.\
   보고서 작성에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 보고서를 만들려면 액세스 수준의 보고서에 대한 편집 액세스 권한이 있어야 합니다.\
   보고서 액세스에 대한 자세한 내용은 문서를 참조하십시오 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 보고서 사용량 정보를 볼 때 예외

>[!IMPORTANT]
>
>보고서 사용 정보는 2018년 3월부터 수집되었습니다. 이 날짜 이전의 정보는 사용할 수 없습니다.

다음은 보고서 사용 정보 작업 시 알아야 할 몇 가지 예외입니다.

* 보고서가 대시보드 또는 사용자 지정 탭에 표시될 때마다 하나의 보기로 계산됩니다. 대시보드에 해당 보고서를 표시하는 사용자가 마지막 보기 기준: 사용자 이름을 지정하고 대시보드가 표시된 날짜가 마지막으로 본 날짜로 표시됩니다.
* Workfront은 기본 제공 보고서에 대한 사용 정보를 수집하지 않습니다.\
   Workfront 기본 제공 보고서에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront 기본 제공 보고서 사용](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront은 배달된 보고서에 대한 사용 정보를 수집하지 않습니다. 배달된 보고서는 한 개의 보기로 계산되지 않습니다.\
   배달된 보고서에 대한 자세한 내용은 문서를 참조하십시오 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* 시스템 또는 그룹 관리자가 다른 사용자로 로그인하면 해당 보기가 시스템 또는 그룹 관리자에 대해 계산되고 연결됩니다.
* Workfront은 사용자 지정 분기별로 보고서에 대한 사용 정보를 수집하지 않습니다. 표준 기본 제공 분기만 보고서 사용 필드에서 참조됩니다.
* Workfront은 공유되고 공개적으로 표시되는 보고서에 대한 사용 정보를 수집하지 않습니다. Workfront에 로그인하지 않은 사용자가 공개 보고서를 보면 보고서 보기가 카운트되지 않습니다.\
   보고서 공유에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront에서 보고서 공유](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
