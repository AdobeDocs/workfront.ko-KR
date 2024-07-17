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
source-wordcount: '528'
ht-degree: 0%

---


# 보고서 실행

보기에 액세스할 수 있는 모든 보고서를 실행할 수 있습니다.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 보고서 실행

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서**&#x200B;를 클릭합니다.

1. 다음 옵션 중에서 선택합니다.

   * **내 보고서:**&#x200B;개 보고서를 만들었습니다.
   * **나와 공유:** 다른 사용자가 귀하와 공유한 보고서입니다.
   * **모든 보고서:** 액세스 권한이 있는 시스템의 모든 보고서입니다.

1. 실행할 보고서의 이름을 클릭합니다.\
   또는\
   프롬프트를 사용하여 보고서를 만든 경우 드롭다운 메뉴에서 적절한 정보를 선택한 다음 **보고서 실행**&#x200B;을 클릭합니다.\
   프롬프트에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)를 참조하십시오.\
   보고서의 콘텐츠는 보고서를 실행한 사용자의 컨텍스트에서 보고서를 실행한 날짜, 시간 및 시간대를 포함하는 타임스탬프와 함께 보고서의 오른쪽 위 모서리에 표시됩니다.

1. (선택 사항) 보고서가 잠시 브라우저에 표시된 경우 **다시 로드 아이콘** ![](assets/qs-report-refresh-icon.png)을 클릭하여 보고서에서 결과를 새로 고칩니다.

1. (조건부) 보고서에서 필터 또는 프롬프트를 사용하는 경우 **필터 및 프롬프트 표시**&#x200B;를 클릭하여 보고 있는 보고서에서 사용 중인 필터 및 프롬프트 목록을 표시합니다. 보고서에 필터만 있거나 프롬프트가 있는 경우 **필터 표시** 또는 **프롬프트 표시**&#x200B;가 대신 나타납니다.

   ![필터 및 프롬프트 표시](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   페이지 왼쪽의 보고서 이름 아래에 정보가 표시됩니다. 프롬프트의 경우 4단계에 설명된 대로 보고서 실행 시 수행한 프롬프트 선택 사항에 대한 정보입니다.

1. 사용자 지정 프롬프트를 사용하는 경우 프롬프트가 표시되지 않습니다. 시스템 프롬프트만 표시됩니다. 사용자 지정 필터는 항상 표시됩니다.

## 캐시된 보고서 보기

보고서가 잠시 동안 브라우저에 표시되면 캐시될 수 있습니다. 다음 작업을 수행하면 캐시된 보고서가 다시 로드됩니다.

* 보고서 설정을 편집하고 보고서를 저장합니다.
* 보기, 그룹 또는 필터를 변경합니다.
* **다시 로드 아이콘**을 클릭합니다.
이 옵션은 보고서가 저장된 시간을 나타내는 메시지 상자 내의 페이지 오른쪽 상단 모서리에서 사용하거나 보고서가 배치된 대시보드의 오른쪽 상단 모서리에서 사용할 수 있습니다. 대시보드를 다시 로드하는 방법에 대한 자세한 내용은 문서 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)에서 &quot;대시보드 표시&quot; 섹션을 참조하십시오.

* 요약, 매트릭스 또는 차트 탭으로 이동하여 첫 번째 페이지 이외의 보고서 페이지에 액세스합니다.
