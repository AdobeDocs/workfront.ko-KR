---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 보고서 실행
description: 보기에 액세스할 수 있는 모든 보고서를 실행할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# 보고서 실행

보기에 액세스할 수 있는 모든 보고서를 실행할 수 있습니다.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 보고서 실행

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.

1. 다음 옵션 중에서 선택합니다.

   * **내 보고서:** 생성한 보고서입니다.
   * **나와 공유:** 다른 사용자가 사용자와 공유한 보고서입니다.
   * **모든 보고서:** 액세스할 수 있는 시스템의 모든 보고서입니다.

1. 실행할 보고서의 이름을 클릭합니다.\
   또는\
   프롬프트를 사용하여 보고서가 생성된 경우 드롭다운 메뉴에서 적절한 정보를 선택한 다음 을 클릭합니다 **보고서 실행**.\
   프롬프트에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   보고서 컨텐츠는 보고서를 실행한 사용자의 컨텍스트에서 보고서를 실행한 날짜, 시간 및 시간대를 포함하는 보고서 오른쪽 위의 타임스탬프와 함께 표시됩니다.

1. (선택 사항) **다시 로드 아이콘** ![](assets/qs-report-refresh-icon.png) 을 눌러 보고서가 한동안 브라우저에 표시된 경우 보고서의 결과를 새로 고칩니다.

1. (조건부) 보고서에서 필터나 프롬프트를 사용하는 경우 을 클릭합니다. **필터 및 프롬프트 표시** 보고 있는 보고서에서 사용 중인 필터 및 프롬프트 목록을 표시합니다. 보고서에 필터만 포함되거나 프롬프트만 포함된 경우 **필터 표시** 또는 **프롬프트 표시** 이 대신 나타납니다.

   ![필터 및 프롬프트 표시](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   페이지 왼쪽에 있는 보고서 이름 아래에 정보가 표시됩니다. 프롬프트의 경우 4단계에서 설명한 대로 보고서 실행 시 선택한 프롬프트 항목에 대한 정보입니다.

1. 사용자 정의 프롬프트를 사용하는 경우에는 표시되지 않습니다. 시스템 프롬프트가 표시됩니다. 사용자 지정 필터는 항상 표시됩니다.

## 캐시된 보고서 보기

한동안 브라우저에 표시된 경우 보고서가 캐시될 수 있습니다. 다음 작업을 수행할 때 캐시된 보고서가 다시 로드되도록 할 수 있습니다.

* 보고서 설정을 편집하고 보고서를 저장합니다.
* 보기, 그룹 또는 필터를 변경합니다.
* 을(를) 클릭합니다. **다시 로드 아이콘**
이 옵션은 메시지 상자 내의 페이지 오른쪽 위 모서리에서 보고서를 저장한 시간을 나타내거나 보고서가 배치된 대시보드의 오른쪽 위 모서리에서 사용할 수 있습니다. 대시보드 다시 로드에 대한 자세한 내용은 문서의 &quot;대시보드 표시&quot; 섹션을 참조하십시오 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* 요약, 매트릭스 또는 차트 탭으로 이동하여 첫 번째 페이지 이외의 보고서의 페이지에 액세스합니다.
