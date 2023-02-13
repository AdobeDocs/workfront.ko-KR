---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 데이터 내보내기
description: 데이터를 내보내는 몇 가지 이유는 EDIT ME입니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2116'
ht-degree: 0%

---

# 데이터 내보내기

다양한 목록, 보고서, 대시보드 및 검색에서 Adobe Workfront 데이터를 내보낼 수 있습니다.
다음 내보내기에는 이 문서의 정보가 적용되지 않습니다.

* 차트 보고서에서 정보 내보내기.

   차트 보고서 내보내기에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 간트 차트에서 정보 내보내기.

   간트 차트 내보내기에 대한 자세한 내용은 [간트 차트를 PDF으로 내보내기](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* 리소스 계획자에서 정보 내보내기.

   리소스 계획자에서 정보를 내보내는 방법에 대한 자세한 내용은 [리소스 플래너 탐색 개요](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

데이터를 내보내는 몇 가지 이유는 다음과 같습니다.

* Workfront 외부의 사용자에게 데이터의 하드 사본을 제공하려고 합니다.
* 보고서 결과를 외부 사용자에게 첨부 파일로 전송하려고 합니다.
* Workfront 데이터의 외부 백업을 만들려고 합니다.
* Workfront 웹 애플리케이션 내의 한 페이지에는 결과를 2,000개만 표시하는 제한이 있습니다. 보고서에서 2,000개 이상을 생성하는 경우 보고서를 아래에서 설명하는 형식으로 내보내고 하나의 목록에 있는 보고서의 모든 결과를 볼 수 있습니다.

Workfront 인터페이스에서 보고서를 수동으로 내보내거나 보고서에 대한 게재를 예약하면 나중에 해당 보고서가 사용자에게 전송됩니다. 배달된 보고서 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서를 내보낼 보고서, 대시보드, 달력에 대한 보기 또는 위의 액세스 권한</p> <p>목록에서 보는 객체에 대한 보기 또는 더 높은 액세스를 통해 목록을 내보냅니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서나 대시보드를 내보내려면 보고서나 대시보드에 대한 보기 이상의 권한</p> <p>목록에서 보는 객체에 대한 보기 또는 더 높은 권한을 사용하여 목록을 내보냅니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

데이터를 내보내려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 내보내기 형식 및 제한

* [내보내기 형식](#export-formats)
* [내보내기 제한](#export-limits)

### 내보내기 형식 {#export-formats}

정보는 다음 형식으로 내보낼 수 있습니다.

* PDF(편지 가로 또는 세로, 법률, 원장 및 A4)
* Excel (.xls)
* Excel (.xlsx)
* 탭으로 구분됨

>[!NOTE]
>
>대시보드를 인쇄하거나 .pdf 파일만 내보낼 수 있습니다.

### 내보내기 제한 {#export-limits}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

보고서가 Workfront에 표시되는 방식과 수동 내보내기, 배달된 보고서 또는 API를 통해 내보내는 방식 간에는 몇 가지 제한 사항이 있습니다.

* **50,000개 행:** .pdf 및 탭으로 구분된 파일에 대해 보고서 내보내기에서 허용되는 데이터 행 수입니다.

   * Excel.xls 파일의 경우 이 제한은 다음과 같습니다 **65,000개 행**.
   * Excel .xlsx 파일의 경우 이 제한은 다음과 같습니다 **100,000개 행**.
   * 이러한 제한은 열 제목과 보고서 그룹의 행을 제외합니다. 예를 들어 보고서에 6개의 그룹화가 있고 50,000개의 행 또는 데이터가 있는 경우 내보낸 파일에 50,000개의 행이 있습니다.

   >[!NOTE]
   >
   >보고서에 이러한 제한보다 많은 항목이 있는 경우 내보내기가 실패했다는 오류가 표시됩니다. 화면에서 표시되는 항목 수를 이러한 제한보다 작거나 같은 수로 줄여 결과를 내보낼 수 있습니다.

   보고서에 50,000/ 65,000/ 100,000개 이상의 행이 있고 모든 데이터를 내보내려면 필터 또는 프롬프트를 사용하여 더 작은 데이터 로드를 가져오고 여러 내보내기를 수행하는 것이 좋습니다.

   필터 사용에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   프롬프트 사용에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* 이러한 제한은 다음과 같은 경우에 적용됩니다.

   * 보고서의 수동 내보내기.
   * 예약된 보고서입니다.
   * API 통합을 통한 내보내기.
   * 킥시작을 통해 데이터를 내보냅니다.

      kick-starts를 통해 데이터 내보내기에 대한 자세한 내용은 [킥스타트를 통해 Adobe Workfront에서 데이터 내보내기](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

      >[!NOTE]
      >
      >데이터를 Excel 형식 파일만 내보낼 수 있지만, 킥시작 파일에 50,000개의 행을 내보낼 수 있습니다. 

   * 프로젝트에 대한 활용률 정보 내보내기

      프로젝트에 대한 활용률 정보 내보내기에 대한 자세한 내용은 [자원 가동률 보고서 개요](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB 파일 크기:** 배달하도록 예약된 내보낸 보고서의 파일 크기 제한. 전자 메일에 첨부된 내보낸 파일이 5MB보다 큰 경우 첨부된 내보낸 보고서 대신 파일을 다운로드할 수 있는 링크가 이메일로 전송됩니다.
* **65,530개의 하이퍼링크:** 이는 65,530개 이상의 하이퍼링크가 포함된 문서에 대해 Excel에서 적용하는 제한입니다. 이러한 문서를 수동으로 내보내거나 전달된 보고서에서 전송할 때는 열 수 없습니다. Excel 문서에는 200개의 데이터 행만 있을 수 있지만 문서 내에 65,530개가 넘는 링크가 있는 경우 문서가 열리지 않습니다. 이 제한은 Excel 파일에만 있고, 지원되는 다른 형식에는 없습니다. 
* **256열**: 이는 256개 이상의 열이 포함된 문서에 대해 Excel에서 적용하는 제한입니다. 이러한 문서를 수동으로 내보내거나 전달된 보고서에서 전송할 수 없습니다. 이 제한은 Excel 파일에만 있고, 지원되는 다른 형식에는 없습니다.

제한 이상으로 데이터를 내보내려고 하면 내보내기에서 예상 데이터를 모두 받지 못할 수 있습니다. 대신, 수정된 보고서가 제한 내에 생성됩니다.

또한 실행하는 데 60분 이상 걸리는 보고서가 중지됩니다.

제한 사항에 대한 우려나 문제가 있는 경우 Workfront 기술 지원에 문의하십시오.

## 데이터 내보내기

* [보고서 또는 목록에서 데이터 내보내기](#export-data-from-a-report-or-list)
* [대시보드에서 데이터 내보내기](#export-data-from-a-dashboard)

### 보고서 또는 목록에서 데이터 내보내기 {#export-data-from-a-report-or-list}

1. 내보낼 보고서 또는 목록으로 이동합니다.
1. 내보낼 항목을 선택합니다. 개별 항목을 선택하면 선택한 항목만 내보내집니다.

   예를 들어 프로젝트에서 내보낼 작업을 선택합니다.

   또는

   전체 목록을 내보내려면 모든 항목을 선택 취소합니다.

1. 클릭 **내보내기**&#x200B;를 선택한 다음 형식을 선택합니다.

   >[!NOTE]
   대시보드 보고서를 내보내려면 계획 라이센스가 있어야 합니다.\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   또는

   을(를) 클릭합니다. **내보내기** 아이콘 ![](assets/export-icon-nwe.png)를 선택한 다음 형식을 선택합니다.

   PDF 내보내기에 사용할 수 있는 옵션은 Workfront 사용자 설정의 로케일 설정에 따라 다릅니다.

   * 북미 - 편지(기본값), 법률, 원장, A4

      <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * 북미 이외의 모든 위치 - A3, A4(기본값), 편지, 법률, 원장

      <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (조건부) 사용하는 운영 체제에 따라 파일을 열거나 저장하는 옵션이 있을 수 있습니다. 연결된 응용 프로그램이 있는 파일을 열거나 하드 드라이브에 저장합니다.
1. 계속 [내보낸 문서 사용](#use-the-exported-document).

### 대시보드에서 데이터 내보내기 {#export-data-from-a-dashboard}

대시보드에서 정보를 인쇄하거나 .pdf 파일로 내보낼 수 있습니다.

대시보드에서 데이터 내보내기에 대한 자세한 내용은 [대시보드 내보내기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## 내보낸 문서 사용 {#use-the-exported-document}

* [파일 이름](#file-names)
* [제목](#titles)
* [타임스탬프](#timestamps)
* [서식](#formatting)
* [링크](#links)
* [브랜딩](#branding)

### 파일 이름 {#file-names}

객체 목록이나 보고서를 내보내더라도 내보낸 파일의 파일 이름은 파일 이름과 제목을 가집니다. 파일 이름을 참조하여 내보낸 파일을 컴퓨터에서 찾을 수 있습니다. 보고서 제목에는 내보낸 파일을 사용자와 공유할 때 나타내는 표시가 있습니다.

* [내보낸 목록의 파일 이름](#file-names-for-exported-lists)
* [내보낸 보고서의 파일 이름](#file-names-for-exported-reports)

#### 내보낸 목록의 파일 이름 {#file-names-for-exported-lists}

객체 목록을 내보내면 객체 유형이 내보낸 파일에 파일 이름과 목록의 제목에 표시됩니다.

작업 또는 문제 목록을 내보낼 때 **파일 이름** 다음 중 하나일 수 있습니다.

* 프로젝트에서 작업 및 문제 목록을 내보내는 경우:

   * *The_project_name_Exported_Tasks*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
   * *The_project_name_Exported_Issues*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

* 작업(하위 작업)에서 작업 및 문제 목록을 내보낼 때

   * **The_project_name_the_task_name_Exported_Tasks**(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
   * **The_project_name_the_task_name_Exported_Issues**(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

프로젝트에서 PDF 파일로 다른 객체의 목록을 내보낼 때 내보낸 문서의 파일 이름은 내보낸 객체의 유형을 나타냅니다.\
예를 들어 파일 이름은 다음과 같습니다.

* *Exported_Users*&#x200B;프로젝트에서 사람 탭을 내보낼 때(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*
* *Exported_Risks*&#x200B;프로젝트에서 위험 목록을 내보낼 때(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

#### 내보낸 보고서의 파일 이름 {#file-names-for-exported-reports}

보고서를 내보낼 때 내보낸 보고서의 파일 이름은 다음과 같습니다.

*The_report_name*(*PDF, Excel, Excel(.xlsx) 또는 탭으로 구분된 형식)*

### 제목 {#titles}

객체 목록을 내보내면 PDF 형식의 파일만 제목을 갖게 됩니다. 목록이나 보고서를 Excel, Excel(.xlsx) 또는 탭으로 구분된 형식으로 내보낼 경우, 파일에 제목이 없습니다.

* [내보낸 목록의 제목](#titles-for-exported-lists)
* [내보낸 보고서의 제목](#titles-for-exported-reports)

#### 내보낸 목록의 제목 {#titles-for-exported-lists}

프로젝트의 작업 및 문제 목록을 PDF 파일로 내보낼 때 내보낸 문서의 제목은 다음 중 하나입니다.

* *프로젝트 이름 - 내보낸 작업*
* *프로젝트 이름 - 내보낸 문제*

작업 및 문제 목록을 PDF 파일로 내보낼 때 내보낸 문서의 타일은 다음 중 하나입니다.

* *프로젝트 이름 - 작업 이름 - 내보낸 작업*
* *프로젝트 이름 - 작업 이름 - 내보낸 문제*

프로젝트에서 PDF 파일로 다른 객체의 목록을 내보낼 때 내보낸 문서의 제목은 내보낸 객체의 유형을 나타냅니다.\
예를 들어, 제목은 다음과 같습니다.

* *내보낸 사용자*&#x200B;를 눌러 프로젝트의 사람 탭을 내보낼 때
* *내보낸 위험*: 프로젝트에서 위험 목록을 내보낼 때

#### 내보낸 보고서의 제목 {#titles-for-exported-reports}

PDF 파일로 내보낸 보고서에는 제목이 있습니다.

보고서를 Excel, Excel(.xlsx) 또는 탭으로 구분된 형식으로 내보낼 경우, 내보낸 보고서에 제목이 없습니다. 내보낸 파일의 제목은 Workfront 웹 애플리케이션에 표시되는 보고서의 이름입니다.

보고서에 설명이 있으면 내보낸 파일에 포함됩니다.

### 타임스탬프 {#timestamps}

항목을 내보낸 사용자의 컨텍스트에서 내보낸 문서에 타임스탬프가 표시됩니다.

타임스탬프는 다음과 같습니다.

* 일자
* 시간
* 항목을 내보낸 시간대

내보내는 문서의 유형에 따라 타임스탬프가 다양한 위치에 표시됩니다.

* **PDF:** 타임스탬프는 각 페이지의 바닥글과 파일 이름에 표시됩니다.
* **Excel:** 타임스탬프는 파일 이름에 표시됩니다.

### 서식 {#formatting}

프로젝트를 .pdf로 내보내면 하위 작업이 상위 작업에 들여쓰기로 표시됩니다. 내보낸 목록은 상위 작업을 축소하지 않습니다.

보고서에 특별한 보기가 없는 한 보고서 전송 또는 배달 예약 시 보고서의 기본 탭을 항상 받습니다.

웹 응용 프로그램에서 보고서에 특수 서식이 있는 경우 .pdf 및 Excel 파일에 대해서만 세부 정보 및 매트릭스 탭이 전달되는 경우 보고서에 특수 서식이 지정되어 있어야 합니다.

>[!NOTE]
내보내는 데이터에 공유 열이 포함되어 있고 Excel 또는 탭으로 구분된 형식으로 내보낼 경우 이러한 열은 내보낸 파일에서 분리됩니다.

보고서에서 서식을 사용자 지정하는 방법에 대한 자세한 내용은 [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### 링크 {#links}

링크는 연결을 지원하는 Workfront의 모든 개체를 가리킬 수 있습니다. Workfront의 목록을 .pdf로 내보내면 원본 문서에 있는 지원되는 모든 링크는 내보낸 문서에서 그대로 유지됩니다.

>[!TIP]
만약 `valueformat=HTML` 사용자 지정 필드 열에 대한 텍스트 모드에 나타나며, 링크 값이 내보낸 .pdf 파일에 표시되지 않으므로 텍스트 모드에서 열에 추가 코드 행을 입력해야 합니다.
예를 들어 링크가 포함된 Q1 프로젝트 열기라는 사용자 지정 필드가 있는 경우 다음 코드를 추가합니다.

```
link.url=customDataLabelsAsString(Open Q1 Projects)
linkedname=direct
```

Excel 형식으로 내보낼 때 Workfront 내의 개체에 대한 링크만 내보낸 파일에 포함되며, 보고서 배달과 같이 내보낸 Excel 문서에 링크를 허용하도록 선택할 수 있는 위치에서만 지원됩니다.

## 브랜딩 {#branding}

Workfront 관리자가 전역 탐색 모음에 대해 Workfront 인스턴스에 사용자 지정된 브랜딩을 추가한 경우 내보낸 .pdf 파일에 개인화된 로고도 포함됩니다.

다른 형식으로 내보낸 데이터는 로고로 개인화할 수 없습니다.

Workfront 인스턴스 및 전역 탐색 모음에 브랜딩하는 방법에 대한 자세한 내용은 [Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
