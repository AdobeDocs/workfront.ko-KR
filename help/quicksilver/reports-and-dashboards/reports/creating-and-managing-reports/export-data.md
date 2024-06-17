---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 데이터 내보내기
description: 다양한 목록, 보고서, 대시보드 및 검색에서 Adobe Workfront 데이터를 내보낼 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2164'
ht-degree: 0%

---

# 데이터 내보내기

<!-- Audited: 12/2023 -->

다양한 목록, 보고서, 대시보드 및 검색에서 Adobe Workfront 데이터를 내보낼 수 있습니다.

데이터를 내보내는 이유 중 일부는 다음과 같습니다.

* Workfront 외부의 사용자에게 데이터의 하드 복사본을 제공하려고 합니다.
* 보고서 결과를 외부 사용자에게 첨부 파일로 보내려고 합니다.
* Workfront 데이터의 외부 백업을 만들려고 합니다.
* Workfront 웹 애플리케이션 내의 한 페이지에 2,000개의 결과만 표시하는 데는 제한이 있습니다. 보고서가 2,000개를 초과하는 경우 보고서를 사용 가능한 형식 중 하나로 내보내고 보고서의 모든 결과를 하나의 목록으로 볼 수 있습니다.

Workfront 인터페이스에서 보고서를 수동으로 내보내거나 보고서 게재를 예약할 수 있으며 해당 보고서는 나중에 전송됩니다. 게재된 보고서 예약에 대한 자세한 내용은 [보고서 게재 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

이 문서의 정보는 다음 내보내기에는 적용되지 않습니다.

* 차트 보고서에서 정보를 내보내는 중입니다.

  차트 보고서 내보내기에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 간트 차트에서 정보 내보내기

  간트 차트 내보내기에 대한 자세한 내용은 [간트 차트를 PDF으로 내보내기](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* 리소스 플래너에서 정보 내보내기.

  리소스 플래너에서 정보를 내보내는 방법에 대한 자세한 내용은 의 &quot;내보내기 옵션&quot;을 참조하십시오 [리소스 플래너 탐색 개요](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
    <p>새로운 기능: 밝게 또는 높음</p>
    <p>또는</p>
    <p>현재: 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드 및 달력에 대한 보기 이상의 액세스 권한을 사용하여 보고서 내보내기</p> <p>목록을 내보내려면 목록에서 보는 객체에 대한 이상의 액세스 권한</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서 또는 대시보드를 내보낼 보고서 또는 대시보드에 대한 이상의 권한 보기</p> <p>목록을 내보내려면 목록에서 보는 객체에 대한 이상의 권한을 봅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 전제 조건

데이터를 내보내려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 또는 [보고서 사본 만들기](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## 내보내기 형식 및 제한

### 내보내기 형식 {#export-formats}

정보는 다음 형식으로 내보낼 수 있습니다.

* PDF(Letter Landscape 또는 Portrait, 법률, 원장 및 A4)
* Excel (.xls)
* Excel (.xlsx)
* 탭으로 구분됨

>[!NOTE]
>
>대시보드는 인쇄하거나 .pdf 파일로만 내보낼 수 있습니다.

### 내보내기 제한 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Workfront에 보고서가 표시되는 방식과 수동 내보내기, 배달된 보고서 또는 API를 통해 내보내는 방식에 따라 몇 가지 제한 사항이 있습니다.

* **50,000개 셀:** Excel 파일에 대한 보고서 내보내기에 허용되는 최대 셀 수입니다.
* **50,000행:** .pdf 및 탭으로 구분된 파일에 대한 보고서 내보내기에 허용되는 데이터 행 수입니다.

   * Excel .xls 파일의 경우 이 제한은 **65,000행**.
   * Excel .xlsx 파일의 경우 이 제한은 다음과 같습니다 **100,000행**.
   * 이러한 제한은 열 머리글과 보고서에서 그룹화를 위한 행을 제외합니다. 예를 들어 보고서에 6개의 그룹화가 있고 50,000개의 데이터 행이 있는 경우 내보낸 파일의 행은 50,000개가 됩니다.

  >[!IMPORTANT]
  >
  >열 내에 컬렉션 참조가 포함된 보고서를 내보내면 나열된 내보내기 제한 내에 보고서가 있더라도 오류가 발생할 수 있습니다. 참조된 컬렉션이 너무 크면 내보내기 프로세스가 시간 초과되어 오류가 발생합니다.
  >
  >이 오류를 방지하려면 내보내기 전에 큰 컬렉션을 참조하는 열을 제외하거나 참조된 컬렉션의 크기를 줄이십시오.
  >

  보고서에 이러한 제한보다 많은 항목이 있는 경우 내보내기가 실패했다는 오류가 표시됩니다. 결과를 내보낼 수 있도록 화면에 표시되는 항목 수를 이러한 제한보다 작거나 같은 수로 줄입니다.

  보고서에 50,000/ 65,000/ 100,000개 이상의 행이 있고 모든 데이터를 내보내려는 경우 필터 또는 프롬프트를 사용하여 데이터 로드를 줄이고 여러 내보내기를 수행하는 것이 좋습니다.

  필터 사용에 대한 자세한 내용은 [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  프롬프트 사용에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* 이러한 제한은 다음 경우에 적용됩니다.

   * 보고서의 수동 내보내기.
   * 예약된 보고서.
   * API 통합을 통한 내보내기.
   * 킥스타트를 통해 내보낸 데이터.

     킥스타트를 통해 데이터를 내보내는 방법에 대한 자세한 내용은 [킥스타트를 통해 Adobe Workfront에서 데이터 내보내기](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Excel 형식 파일로만 데이터를 내보낼 수 있지만 킥스타트 파일에서 50,000개의 행을 내보낼 수 있습니다.

   * 프로젝트에 대한 활용성 정보를 내보내는 중입니다.

     프로젝트의 활용성 정보 내보내기에 대한 자세한 내용은 [자원 가동률 보고서 개요](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB 파일 크기:** 내보내기로 예약된 보고서의 파일 크기 제한. 이메일에 첨부된 내보낸 파일이 5MB보다 큰 경우 첨부된 내보낸 보고서 대신 파일을 다운로드할 수 있는 링크가 이메일로 전송됩니다.
* **65,530개의 하이퍼링크:** Excel에서 65,530개 이상의 하이퍼링크가 포함된 문서에 적용하는 제한입니다. 이러한 문서는 수동으로 내보내거나 게재된 보고서에서 전송할 때 열 수 없습니다. Excel 문서에는 200개의 데이터 행만 있을 수 있지만 문서 내에 65,530개가 넘는 링크가 있으면 문서가 열리지 않습니다. 이 제한은 지원되는 다른 형식이 아닌 Excel 파일에만 적용됩니다. 
* **256열**: 열이 256개를 초과하는 문서에 대해 Excel에서 지정한 제한입니다. 이러한 문서는 수동으로 내보내거나 게재된 보고서에서 전송할 수 없습니다. 이 제한은 지원되는 다른 형식이 아닌 Excel 파일에만 적용됩니다.

한도를 초과하여 데이터를 내보내려고 하면 내보내기에서 예상되는 모든 데이터를 받지 못할 수 있습니다. 대신 수정된 보고서가 한도 내에서 생성됩니다.

또한 실행하는 데 60분 이상 걸리는 보고서가 중단됩니다.

제한과 관련하여 우려 사항이나 문제가 있는 경우 Workfront 기술 지원에 문의하십시오.

## 데이터 내보내기

### 보고서 또는 목록에서 데이터 내보내기 {#export-data-from-a-report-or-list}

1. 내보낼 보고서 또는 목록으로 이동합니다.
1. 내보낼 항목을 선택합니다. 개별 항목을 선택하면 선택한 항목만 내보내집니다.

   예를 들어, 프로젝트에서 내보낼 작업을 선택합니다.

   또는

   전체 목록을 내보내려면 모든 항목을 선택 해제한 상태로 둡니다.

1. 클릭 **내보내기**&#x200B;을 클릭한 다음 형식을 선택합니다.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   또는

   다음을 클릭합니다. **내보내기** 아이콘 ![내보내기 아이콘](assets/export-icon-nwe.png)을 클릭한 다음 형식을 선택합니다.

   PDF 내보내기에 사용할 수 있는 옵션은 Workfront 사용자 설정의 로케일 설정에 따라 다릅니다.

   * 북미 - 편지(기본값), 법적, 원장, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * 북미 이외의 모든 위치 - A3, A4(기본값), 편지, 법적, 원장

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (조건부) 사용하는 운영 체제에 따라 파일을 열거나 저장하는 옵션이 있을 수 있습니다. 연결된 응용 프로그램과 함께 파일을 열거나 하드 드라이브에 저장하십시오.
1. 계속 [내보낸 문서 사용](#use-the-exported-document).

### 대시보드에서 데이터 내보내기 {#export-data-from-a-dashboard}

대시보드에서 정보를 인쇄하거나 .pdf 파일로 내보낼 수 있습니다.

대시보드에서 데이터를 내보내는 방법에 대한 자세한 내용은 [대시보드 내보내기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## 내보낸 문서 사용 {#use-the-exported-document}

* [파일 이름](#file-names)
* [제목](#titles)
* [타임스탬프](#timestamps)
* [서식](#formatting)
* [링크](#links)
* [브랜딩](#branding)

### 파일 이름 {#file-names}

객체 목록을 내보내든 보고서를 내보내든 내보낸 파일에는 파일 이름과 제목이 있습니다. 파일 이름을 참조하여 컴퓨터에서 내보낸 파일을 찾을 수 있습니다. 보고서의 제목은 내보낸 파일을 사용자와 공유할 때 사용자가 나타내는 내용을 보여줍니다.

#### 내보낸 목록의 파일 이름 {#file-names-for-exported-lists}

객체 목록을 내보내면 객체 유형이 내보낸 파일에 파일 이름과 목록 제목으로 표시됩니다.

작업 또는 문제 목록을 내보낼 때 **파일 이름** 은 다음 중 하나일 수 있습니다.

* 프로젝트에서 작업 및 문제 목록을 내보낼 때:

   * *The_project_name_Exported_Tasks*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
   * *The_project_name_Exported_Issues*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

* 작업(하위 작업)에서 작업 및 문제 목록을 내보낼 때:

   * **_project_name_the_task_name_Exported_Tasks**(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
   * **The_project_name_the_task_name_Exported_Issues**(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

프로젝트의 다른 객체 목록을 PDF 파일로 내보낼 때 내보낸 문서의 파일 이름은 내보낸 객체의 유형을 나타냅니다.\
예를 들어 파일 이름은 다음과 같을 수 있습니다.

* *내보낸 사용자*&#x200B;프로젝트에서 사람 탭을 내보낼 때(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
* *Exported_Risk*&#x200B;프로젝트에서 위험 목록을 내보낼 때(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

#### 내보낸 보고서의 파일 이름 {#file-names-for-exported-reports}

보고서를 내보낼 때 내보낸 보고서의 파일 이름은 다음과 같습니다.

*The_report_name*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

### 제목 {#titles}

개체 목록을 내보내면 PDF 형식의 파일에만 제목이 지정됩니다. 목록이나 보고서를 Excel, Excel(.xlsx) 또는 탭으로 구분된 형식으로 내보내는 경우 파일에 제목이 없습니다.

#### 내보낸 목록의 제목 {#titles-for-exported-lists}

프로젝트의 작업 및 문제 목록을 PDF 파일로 내보낼 때 내보낸 문서의 제목은 다음 중 하나입니다.

* *프로젝트 이름 - 내보낸 작업*
* *프로젝트 이름 - 내보낸 문제*

작업의 작업 및 문제 목록을 PDF 파일로 내보낼 때 내보낸 문서의 타일은 다음 중 하나입니다.

* *프로젝트 이름 - 작업 이름 - 내보낸 작업*
* *프로젝트 이름 - 작업 이름 - 내보낸 문제*

프로젝트의 다른 객체 목록을 PDF 파일로 내보낼 때 내보낸 문서의 제목은 내보낸 객체의 유형을 나타냅니다.\
예를 들어 제목은 다음과 같을 수 있습니다.

* *내보낸 사용자*&#x200B;프로젝트에서 사람 탭을 내보낼 때 다음을 수행하십시오.
* *내보낸 위험*&#x200B;프로젝트에서 위험 목록을 내보낼 경우

#### 내보낸 보고서 제목 {#titles-for-exported-reports}

PDF 파일로 내보낸 보고서에는 제목이 있습니다.

보고서를 Excel, Excel(.xlsx) 또는 탭으로 구분된 형식으로 내보낼 경우 내보낸 보고서에 제목이 없습니다. 내보낸 파일의 제목은 Workfront 웹 애플리케이션에 나타나는 보고서 이름입니다.

보고서에 설명이 있으면 내보낸 파일에 포함됩니다.

### 타임스탬프 {#timestamps}

항목을 내보낸 사용자의 컨텍스트에서 내보낸 문서에 타임스탬프가 표시됩니다.

타임스탬프에는 다음이 포함됩니다.

* 일자
* 시간
* 항목을 내보낼 시간대

내보내는 문서 유형에 따라 다양한 위치에 타임스탬프가 표시됩니다.

* **PDF:** 타임스탬프는 각 페이지의 바닥글과 파일 이름에 표시됩니다.
* **Excel:** 타임스탬프는 파일 이름에 표시됩니다.

### 서식 {#formatting}

프로젝트를 .pdf로 내보내면 하위 작업이 상위 작업에 들여쓰기로 표시됩니다. 내보낸 목록은 상위 작업을 축소하지 않습니다.

보고서에 특수 보기가 없는 경우 보고서를 보내거나 배달 예약하면 항상 보고서의 기본 탭을 받게 됩니다.

웹 응용 프로그램에서 보고서에 특수 서식이 있는 경우 세부 정보 및 매트릭스 탭이 표시될 때 .pdf 및 Excel 파일에만 특수 서식으로 보고서가 전달되어야 합니다.

>[!NOTE]
>
>내보내려는 데이터에 공유 열이 포함되어 있고 Excel 또는 탭으로 구분된 형식으로 내보내는 경우 이러한 열은 내보낸 파일로 구분됩니다.

보고서에서 서식을 사용자 지정하는 방법에 대한 자세한 내용은 [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### 링크 {#links}

링크는 연결을 지원하는 Workfront의 모든 개체를 가리킬 수 있습니다. Workfront의 목록을 .pdf로 내보낼 때 원본 문서에 있는 지원되는 모든 링크는 내보낸 문서에 있는 라이브 상태로 유지됩니다.

>[!TIP]
>
>줄이 있는 경우 `valueformat=HTML` 사용자 정의 필드 열의 텍스트 모드에 나타나며 링크 값이 내보낸 .pdf 파일에 표시되지 않습니다. 텍스트 모드에서 열에 추가 코드 행을 입력해야 합니다.
>
>예를 들어 링크가 포함된 Q1 프로젝트 열기 라는 사용자 정의 필드가 있는 경우 다음 코드를 추가합니다.
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Excel 형식으로 내보낼 때 Workfront 내의 오브젝트에 대한 링크만 내보낸 파일에 포함되며 보고서 게재와 같이 내보낸 Excel 문서에서 링크를 허용하도록 선택할 수 있는 위치에서만 지원됩니다.

## 브랜딩 {#branding}

>[!IMPORTANT]
>
>브랜딩은 아직 Adobe Experience Cloud에 온보딩되지 않은 조직에만 적용됩니다.
>
>조직이 Adobe Experience Cloud에 온보딩된 경우 브랜딩을 사용할 수 없습니다.

Workfront 관리자가 전역 탐색 막대에 대한 Workfront 인스턴스에 사용자 지정된 브랜딩을 추가한 경우 내보낸 .pdf 파일에 개인화된 로고도 포함됩니다.

다른 형식으로 내보낸 데이터는 로고로 개인화할 수 없습니다.

Workfront 인스턴스 및 전역 탐색 막대 브랜딩에 대한 자세한 내용은 [Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
