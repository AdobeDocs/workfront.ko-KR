---
product-area: reporting
navigation-topic: report-usage
title: 보고서 사용 보기
description: 보고서 사용 보기
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---

# 보고서 사용 보기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

시스템에서 보고서가 얼마나 광범위하게 사용되는지 이해하기 위해 보고서 목록에서 다음 정보를 볼 수 있습니다.

* 보고서를 열람한 마지막 10명의 사용자
* 지정된 시간대 내의 카운트 보기

  >[!NOTE]
  >
  >Adobe Workfront은 하루에 사용자당 하나의 보기를 계산합니다. 하루에 여러 번 동일한 보고서에 액세스하는 경우 Workfront은 이 보고서를 해당 보고서에 대한 하나의 보기로 계산합니다. 같은 날 다른 사용자가 동일한 보고서에 액세스하면 Workfront에서는 이 보고서를 두 번째 사용자에 대한 새 보기로 계산합니다.

* 마지막으로 조회한 일자
* 사용자가 마지막으로 본 항목
* 보고서가 포함된 대시보드 목록\
  보고서 목록에 보고서가 추가될 수 있는 대시보드 이름을 표시하는 방법에 대한 자세한 내용은 문서 [대시보드에서 보고서를 구성하는 방법 이해](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md)를 참조하십시오.

이 정보를 표시할 수 있는 보고서 목록에 대한 보기를 만들 수 있습니다.\
이러한 필드 중 일부로 보고서 목록을 필터링할 수 있습니다.\
보고서를 필터링할 수 있는 필드에 대한 자세한 내용은 [사용 정보별로 보고서 목록 필터링](#filter-a-report-list-by-usage-information) 문서를 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 보고서 목록 보기에 보고서 사용 정보 표시

1. Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서**&#x200B;를 클릭합니다.

1. 보고서 목록에서 **보기** 드롭다운 메뉴를 클릭합니다.
1. (선택 사항) 가장 일반적인 보고서 사용 정보를 표시하려면 **보고서 사용** 보기를 선택하십시오.\
   또는

1. 사용자 지정 보기를 만들려면 **새 보기**&#x200B;를 클릭합니다.
1. **열 추가**&#x200B;를 클릭합니다.
1. 다음 필드 입력을 시작하고 **보고서** 개체 아래의 목록에 표시될 때 해당 필드를 선택하여 새 열에 추가하십시오.

   * **최근 10명의 사용자**: 보고서를 열람한 최근 10명의 사용자 이름을 표시합니다.
   * **보기**: 다음 시간대 내의 보기 수를 표시합니다.

      * **이번 달, 분기, 연도**
      * **지난 달, 분기, 연도**
      * **모든 보기**: 보고서에 있는 모든 보기의 전체 개수를 표시합니다

   * **마지막으로 본 사람**: 보고서를 마지막으로 본 사용자에 대한 정보를 표시합니다
   * **마지막으로 본 날짜**: 보고서를 마지막으로 본 날짜를 표시합니다

1. **보기 저장**&#x200B;을 클릭합니다.\
   보고서에 대한 사용 정보는 보기에 추가한 열에 표시됩니다.\
   보고서 개체에 대한 보고서를 작성하고 보고서에서 이 보기를 사용할 수도 있습니다.\
   보고서 작성에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.\
   보고서를 작성하려면 액세스 수준의 보고서에 대한 편집 액세스 권한이 있어야 합니다.\
   보고서 액세스에 대한 자세한 내용은 문서 [보고서, 대시보드 및 일정에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

## 사용 정보로 보고서 목록 필터링 {#filter-a-report-list-by-usage-information}

1. Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서**&#x200B;를 클릭합니다.
1. 보고서 목록에서 **필터** 드롭다운 메뉴를 클릭합니다.
1. **새 필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**&#x200B;를 클릭합니다.
1. 다음 필드 입력을 시작하고 **보고서** 개체 아래의 목록에 표시될 때 해당 필드를 선택하여 새 필터 규칙으로 추가하십시오.

   * **보기**: 다음 시간대 내의 보기 수를 표시합니다.

      * **이번 달, 분기, 연도**
      * **지난 달, 분기, 연도**
      * **모든 보기**

   * **마지막으로 본 사람**: 보고서를 마지막으로 본 사용자에 대한 정보를 표시합니다
   * **마지막으로 본 날짜**: 보고서를 마지막으로 본 날짜를 표시합니다

1. 필드에 대한 수정자를 선택한 다음 메시지가 표시되면 값을 지정합니다.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. **필터 저장**&#x200B;을 클릭합니다.\
   정의한 사용 정보를 충족하는 보고서 목록이 표시됩니다.\
   보고서 개체에 대한 보고서를 작성하고 보고서에서 이 필터를 사용할 수도 있습니다.\
   보고서 작성에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요. 보고서를 작성하려면 액세스 수준의 보고서에 대한 편집 액세스 권한이 있어야 합니다.\
   보고서 액세스에 대한 자세한 내용은 문서 [보고서, 대시보드 및 일정에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

## 보고서 사용 정보를 볼 때 예외 발생

>[!IMPORTANT]
>
>보고서 사용 정보는 2018년 3월부터 수집되었습니다. 이 날짜 이전의 모든 정보는 사용할 수 없습니다.

다음은 보고서 사용 정보로 작업할 때 알아 두어야 할 몇 가지 예외입니다.

* 보고서가 대시보드 또는 사용자 지정 탭에 표시될 때마다 하나의 보기로 계산됩니다. 대시보드에 해당 보고서를 표시하는 사용자는 마지막 조회 기준: 이름 사용자로 표시되며, 대시보드가 표시된 일자는 마지막 조회 기준 일자로 표시됩니다.
* Workfront은 기본 제공 보고서에 대한 사용 정보를 수집하지 않습니다.\
  Workfront 기본 제공 보고서에 대한 자세한 내용은 문서 [Adobe Workfront 기본 제공 보고서 사용](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)을 참조하십시오.

* Workfront은 게재된 보고서에 대한 사용 정보를 수집하지 않습니다. 게재된 보고서는 하나의 보기로 계산되지 않습니다.\
  배달된 보고서에 대한 자세한 내용은 문서 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

* 시스템 또는 그룹 관리자가 다른 사용자로 로그인하면 시스템 또는 그룹 관리자에 대해 보기가 계산되고 연결됩니다.
* Workfront은 사용자 정의 분기별로 보고서에 대한 사용 정보를 수집하지 않습니다. 보고서 사용 현황 필드에는 표준 기본 제공 분기만 참조됩니다.
* Workfront은 공개적으로 공유 및 열람되는 보고서에 대한 사용 정보를 수집하지 않습니다. Workfront에 로그인하지 않은 사용자가 공개 보고서를 볼 경우 보고서 보기는 계산되지 않습니다.\
  보고서 공유에 대한 자세한 내용은 문서 [Adobe Workfront에서 보고서 공유](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)를 참조하십시오.
