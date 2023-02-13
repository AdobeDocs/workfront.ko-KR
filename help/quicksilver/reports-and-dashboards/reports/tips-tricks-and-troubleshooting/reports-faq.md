---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 보고서 FAQ
description: 보고서 FAQ
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# 보고서 FAQ

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

보고서에 대한 FAQ는 다음과 같습니다.

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
   <td> <p>계획, 작업</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 한 시간 차이에 대한 사용자 지정 계산에 열에 올바른 결과가 표시되지 않는 이유는 무엇입니까?

프로젝트 보고서의 경우 계획 시간(4)에서 실제 시간(2)을 빼는 계산이 있습니다. 제가 받는 결과는 120이 2가 될 겁니다\
내 계산은 다음과 같습니다.
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### 답변

Workfront에서 시간을 사용하는 필드는 분 단위로 저장됩니다. 계산에서 필드를 사용하면 결과가 분 단위로 표시됩니다. 결과를 시간 단위로 가져오려면 계산 결과를 60으로 나누어야 합니다.

정확한 계산은 다음과 같습니다.

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## 보고서에 있는 각 차트 요소의 값이 차트에 표시되지 않는 이유는 무엇입니까?

### 답변

보고서 차트에 50개가 넘는 차트 요소가 있는 경우 각 요소의 값이 차트에 표시되지 않습니다.

차트에 50개 미만의 요소가 있는 경우 각 요소의 값이 차트에 표시됩니다. 필터를 추가하거나 보고서의 그룹화를 수정하여 차트의 각 요소에 표시되는 항목의 양을 제한하는 것이 좋습니다.

## 보고서가 너무 많은 결과를 반환하여 차트를 표시하는 이유는 무엇입니까?

차트가 있는 보고서를 실행하면 &quot;와... 이 보고서는 차트를 읽을 수 없도록 하는 많은 데이터를 반환했습니다. 필터를 추가하거나 차트의 그룹을 변경하여 결과 범위를 좁히는 것이 좋습니다.&quot;

### 답변

이 오류는 차트에 최대 618개의 개별 결과가 포함되어 있음을 의미합니다. 예를 들어 막대 차트에 618개 이상의 막대가 포함되어 있습니다. 표시 문제를 해결하려면 현재 필터를 수정하고 선택 항목을 그룹화하여 결과를 세분화해야 합니다.

필터 및 그룹화 수정에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 및 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## 동료와 동일한 보고서(또는 달력)에 액세스하여 대신 해당 작업을 볼 때 작업(또는 문제)이 표시되는 이유는 무엇입니까?

### 답변

보고서나 달력에 로그인한 사용자를 가리키는 와일드카드 필터 변수가 있을 수 있습니다. 이 경우 보고서는 로그인한 사용자를 기반으로 정보를 보여줍니다. 로그인한 사용자를 가리키는 와일드카드를 제거하도록 필터를 조정합니다.\
![](assets/qs--user.id-filter-variable-350x79.png)

사용자 기반 와일드카드 필터 변수의 전체 목록은 다음을 참조하십시오 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 내 보고서의 데이터가 완료되지 않은 이유는 무엇입니까?

### 답변

대부분의 경우 시스템에 있는 항목을 볼 수 없는 제한된 액세스 권한이 있을 경우 이러한 문제가 발생할 수 있습니다. 또한 보려는 항목은 사용자와 공유되지 않습니다.

보고서 작성자는 보고서를 편집하여 시스템 관리자의 액세스 권한 또는 데이터를 볼 수 있는 액세스 권한이 있는 모든 계획 사용자와 보고서를 실행할 수 있습니다.

자세한 내용은 [다른 사용자의 액세스 권한이 있는 보고서를 실행하고 전달합니다](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## 제가 지정되는 작업(또는 문제)에 대해 보고하려면 어떻게 해야 합니까?

### 답변

소유자(또는 주 담당자)인지 여부에 관계없이 자신에게 할당된 모든 작업 또는 문제를 보려면 작업이나 문제 보고서에서 다음 필터를 사용하십시오.

1. 작업 또는 문제 보고서에 액세스합니다.
1. 설정 **필터** 탭, **필터 규칙 추가**.

1. 에서 **필드 이름 입력 시작..** 필드, 입력 시작 **배정 사용자 이름**&#x200B;그런 다음 목록에 나타나면 선택합니다.

   >[!NOTE]
   >
   >를 사용하지 마십시오 **지정 대상 이름** 필드. 기본 할당자 또는 소유자인 작업 및 문제에 대해서만 필터링됩니다.

1. 을(를) 선택합니다 **Equal** 수정자.
1. 입력 시작 *$$USER.ID* 텍스트 상자에 있는 드롭다운 목록에서 해당 텍스트 상자를 선택합니다.\
   이렇게 하면 로그인한 사용자에게 할당된 모든 작업 및 문제가 표시됩니다. 와일드카드를 특정 사용자 이름으로 바꿀 수 있습니다.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. 클릭 **저장 + 닫기**.

## 프로젝트에 있는 문제 및 작업 목록 맨 아래에 문제 추가/작업 추가 링크가 표시되지 않는 이유는 무엇입니까?

### 답변

먼저 프로젝트에 문제와 작업을 추가할 수 있는 올바른 액세스 및 권한이 있는지 확인합니다. 이 경우 **문제 추가** 및 **작업 추가** 의 맨 아래에 있는 링크 **문제** 및 **작업** 목록.

그러나 이러한 링크가 표시되지 않도록 하는 몇 가지 사항이 있습니다.

* 이러한 목록에 빠른 필터가 적용되어 있으면 링크가 표시되지 않습니다. 프로젝트에 문제와 작업을 추가할 수 있도록 빠른 필터를 제거하면 링크가 표시되어야 합니다.\
   빠른 필터에 대한 자세한 내용은 [Adobe Workfront에서 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* 만약 **그룹화** 이러한 목록에 적용되면 링크가 표시되지 않습니다. 제거 **그룹화** 프로젝트에 문제와 작업을 추가할 수 있도록 및 링크가 표시되어야 합니다.\
   그룹화 만들기에 대한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* 만약 **보기** 프로젝트에 대한 기본 통화 이외의 통화를 선택한 통화가 있는 목록에 적용되면 링크가 표시되지 않습니다. 변경 **보기** to **프로젝트의 원래 통화** 프로젝트에 문제와 작업을 추가할 수 있도록 및 링크가 표시되어야 합니다.\
   보기에서 통화 변경에 대한 자세한 내용은 [고유한 환율을 사용하여 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## 내 보고서나 대시보드의 정보가 자동으로 새로 고침됩니까?

### 답변

보고서 또는 대시보드의 정보는 자동으로 새로 고쳐지지 않습니다.

캐시된 보고서에서 정보를 수동으로 새로 고칠 수 있습니다.\
캐시된 보고서를 새로 고치는 방법에 대한 자세한 내용은 [보고서 실행](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

캐시된 대시보드에서 정보를 수동으로 새로 고칠 수 있습니다.\
캐시된 대시보드를 새로 고치는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [대시보드 표시](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) 기사 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 보고서 소유자를 바꿀 수 있습니까?

### 답변

보고서 소유자를 변경할 수 없습니다. 하지만 보고서를 만든 사용자는 다른 사용자가 보고서를 편집할 수 있도록 허용할 수 있습니다. 사용자가 보고서를 편집할 수 있도록 허용하는 방법은 사용자의 유형에 따라 다릅니다.

* 시스템 관리자는 보고서 행에 있는 편집 옵션을 구성하여 계획 라이센스가 있는 사용자가 보고서 작성에 대한 액세스 권한을 포함하도록 보고서를 편집할 수 있도록 할 수 있습니다.\
   자세한 내용은 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* 보고서를 만들고 공유할 수 있는 액세스 권한이 있는 모든 최종 사용자는 다른 사용자가 보고서를 공유하고 다른 사용자에게 보고서 관리 권한을 부여하여 개별 보고서를 편집할 수 있습니다.\
   자세한 내용은 [Adobe Workfront에서 보고서 공유](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

보고서를 보거나 관리할 수 있는 권한이 있는 경우 보고서의 사본을 만들 수도 있습니다. 그렇게 되면 기본적으로 보고서의 소유자가 됩니다. 보고서 복사에 대한 자세한 내용은 [보고서 사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## 비활성화된 사용자가 소유한 보고서에 액세스할 수 없는 이유는 무엇입니까?

### 답변

경우에 따라 보고서 소유자는 **다음 액세스 권한으로 이 보고서를 실행합니다.** 보고서의 필드. 만약 **다음 액세스 권한으로 이 보고서를 실행합니다.** 사용자가 비활성화되면, 사용자와 공유된 보고서가 있는 사용자에 대해 더 이상 보고서가 표시되지 않습니다. 이런 경우, **다음 액세스 권한으로 이 보고서를 실행합니다.** 비워 두거나 필드에 활성 사용자를 입력합니다.

에 대해 자세히 알아보려면 **다음 액세스 권한으로 이 보고서를 실행합니다.** 필드 [다른 사용자의 액세스 권한이 있는 보고서를 실행하고 전달합니다](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). 비활성화된 사용자가 소유한 모든 보고서를 식별하는 방법에 대한 자세한 내용은 [보고 활동에 대한 보고서 만들기](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## 삭제된 사용자가 소유한 보고서가 포함된 대시보드에 액세스하려면 어떻게 합니까?

### 답변

사용자를 삭제해도 사용자가 만든 모든 보고서에 액세스할 수 있지만 보고서를 포함한 모든 대시보드도 삭제됩니다. 즉, 더 이상 다음 항목에 액세스할 수 없습니다.

* 보고서가 포함된 대시보드
* 보고서의 대시보드를 포함하는 사용자 지정 섹션

사용자 삭제에 대한 의미에 대한 자세한 내용은 [사용자 삭제](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

보고서에 대한 보기 액세스 권한이 있는 경우 다음을 수행할 수 있습니다.

1. 보고서 사본을 만듭니다.\
   보고서 사본을 만드는 방법에 대해 알아보려면 [보고서 사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. 복사된 보고서를 포함하도록 대시보드를 업데이트합니다.\
   대시보드를 편집하는 방법에 대해 알아보려면 [대시보드 편집](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
