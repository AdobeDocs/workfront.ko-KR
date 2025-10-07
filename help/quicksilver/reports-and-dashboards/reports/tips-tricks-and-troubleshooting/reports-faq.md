---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 보고서 FAQ
description: 보고서 FAQ
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 보고서 FAQ

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

다음은 보고서에 대한 FAQ입니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p> 
   <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 한 시간 차이에 대한 사용자 정의 계산이 열에 올바른 결과를 표시하지 않는 이유는 무엇입니까?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

프로젝트 보고서에 계획된 시간에서 실제 시간을 빼는 계산이 있습니다.

내가 받는 결과가 올바르지 않습니다.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

내 계산은 다음과 같습니다.

`valueexpression=SUB(workRequired,actualWorkRequired)`

### 답변

Workfront에서 시간을 사용하는 대부분의 필드는 분 단위로 저장됩니다. 계산에 이러한 필드를 사용할 때 결과는 대부분 분 단위입니다. 시간 단위로 결과를 얻으려면 계산 결과나 참조하는 필드를 60으로 나누어야 합니다.

계획된 시간은 분 단위로 저장됩니다.

계산에 사용할 실제 시간 필드에 따라 올바른 공식은 다음과 같습니다.

* 분 단위로 저장된 이전 실제 시간:

  `valueexpression=SUB(workRequired,actualWorkRequired)/60`

* 시간 단위로 저장된 실제 시간의 경우:

  `valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

자세한 내용은 [실제 근로시간 보기](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)를 참조하십시오.

## 보고서에 있는 각 차트 요소의 값이 차트에 표시되지 않는 이유는 무엇입니까?

### 답변

보고서 차트에 50개가 넘는 차트 요소가 있는 경우 각 요소의 값이 차트에 표시되지 않습니다.

차트에 50개 미만의 요소가 있는 경우 각 요소의 값이 차트에 표시됩니다. 차트의 각 요소에 표시되는 항목의 양을 제한하려면 보고서에서 필터를 추가하거나 그룹화를 수정하는 것이 좋습니다.

## 보고서가 차트를 표시하기 위해 너무 많은 결과를 반환하는 이유는 무엇입니까?

차트가 있는 보고서를 실행하면 오류 메시지가 표시됩니다. &quot;우와... 이 보고서는 차트를 읽을 수 없게 하는 많은 데이터를 반환했습니다. 필터를 추가하거나 차트에서 그룹화를 변경하여 결과 범위를 좁히는 것이 좋습니다.&quot;

### 답변

이 오류는 차트에 최대 618개의 개별 결과(예: 막대 차트에 618개 이상의 막대)가 포함되어 있음을 의미합니다. 표시 문제를 해결하려면 현재 필터를 수정하고 선택 항목을 그룹화하여 결과를 세분화해야 합니다.

필터 및 그룹화 수정에 대한 자세한 내용은 문서 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 및 [그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.

## 동료와 동일한 보고서(또는 달력)에 액세스하면 대신 내 작업이 표시되는 이유는 무엇입니까?

### 답변

보고서 또는 달력에는 로그인한 사용자를 가리키는 와일드카드 필터 변수가 있을 수 있습니다. 이 경우 보고서는 로그인한 사용자를 기반으로 한 정보를 표시합니다. 로그인한 사용자를 가리키는 와일드카드를 제거하려면 필터를 조정합니다.\
![사용자 ID 필터 변수](assets/qs--user.id-filter-variable-350x79.png)

사용자 기반 와일드카드 필터 변수의 전체 목록을 보려면 [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)를 참조하십시오.

## 내 보고서의 데이터가 불완전한 이유는 무엇입니까?

### 답변

이 문제는 대부분의 경우 시스템에서 항목을 볼 수 없도록 제한된 액세스 권한이 있는 경우에 발생할 수 있습니다. 또한 보려는 항목이 사용자와 공유되지 않습니다.

보고서 작성자는 시스템 관리자 또는 데이터를 볼 수 있는 액세스 권한이 있는 모든 계획 사용자의 액세스 권한으로 보고서를 실행하도록 편집할 수 있습니다.

자세한 내용은 [다른 사용자의 액세스 권한으로 보고서 실행 및 배달](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)을 참조하십시오.

## 내가 담당자인지 여부에 관계없이 나에게 할당된 작업(또는 문제)에 대해 어떻게 보고합니까?

### 답변

소유자(또는 기본 담당자)인지 여부에 관계없이 사용자에게 할당된 모든 작업 또는 문제를 보려면 작업 또는 문제 보고서에서 다음 필터를 사용하십시오.

1. 작업 또는 문제 보고서에 액세스합니다.
1. **필터** 탭에서 **필터 규칙 추가**&#x200B;를 클릭합니다.

1. **필드 이름 입력 시작...** 필드에 **할당 사용자 이름**&#x200B;을 입력한 다음 목록에 나타나면 선택하십시오.

   >[!NOTE]
   >
   >**할당 대상 이름** 필드는 기본 담당자 또는 소유자인 작업 및 문제에만 사용할 수 있으므로 사용하지 마십시오.

1. **Equal** 한정자를 선택하십시오.
1. 텍스트 상자에 *$$USER.ID*&#x200B;을(를) 입력하고 표시되는 드롭다운 목록에서 선택하십시오.\
   이렇게 하면 로그인한 사용자에게 할당된 모든 작업 및 문제가 표시됩니다. 와일드카드를 특정 사용자 이름으로 바꿀 수 있습니다.\
   ![나에게 할당된 작업](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 프로젝트의 내 문제 및 작업 목록 하단에 문제 추가/작업 추가 링크가 표시되지 않는 이유는 무엇입니까?

### 답변

먼저, 프로젝트에 문제 및 작업을 추가할 수 있는 올바른 액세스 및 권한이 있는지 확인하십시오. 이 경우 **문제** 및 **작업** 목록 맨 아래에 **문제 추가** 및 **작업 추가** 링크가 표시됩니다.

그러나 이러한 링크가 표시되지 않을 수 있는 몇 가지 사항이 있습니다.

* 이러한 목록에 빠른 필터가 적용된 경우 링크가 표시되지 않습니다. 빠른 필터를 제거하면 프로젝트에 문제와 작업을 추가할 수 있는 링크가 표시됩니다.\
  빠른 필터에 대한 자세한 내용은 [Adobe Workfront 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)을 참조하십시오.

* 이 목록에 **그룹화**&#x200B;이 적용되어 있으면 링크가 표시되지 않습니다. **그룹화**&#x200B;을(를) 제거하면 프로젝트에 문제와 작업을 추가할 수 있는 링크가 표시됩니다.\
  그룹화 만들기에 대한 자세한 내용은 Adobe Workfront의 [그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.

* 프로젝트의 기본 통화 이외의 통화가 선택된 이러한 목록에 **보기**&#x200B;가 적용된 경우 링크가 표시되지 않습니다. **보기**&#x200B;를 **프로젝트의 원래 통화**(으)로 변경하면 프로젝트에 문제와 작업을 추가할 수 있도록 링크가 표시됩니다.\
  보기에서 통화 변경에 대한 자세한 내용은 [환율이 고유한 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)를 참조하십시오.

![프로젝트 통화](assets/nwe-project-original-currency-350x229.png)

## 보고서나 대시보드의 정보가 자동으로 새로 고쳐집니까?

### 답변

보고서 또는 대시보드의 정보가 자동으로 새로 고쳐지지 않습니다.

캐시된 보고서에서 정보를 수동으로 새로 고칠 수 있습니다.\
캐시된 보고서를 새로 고치는 방법에 대한 자세한 내용은 [보고서 실행](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md)을 참조하세요.

캐시된 대시보드에서 정보를 수동으로 새로 고칠 수 있습니다.\
캐시된 대시보드를 새로 고치는 방법에 대한 자세한 내용은 문서 [대시보드 시작](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards)에서 [대시보드 표시](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md) 섹션을 참조하십시오.

## 보고서 소유자를 변경할 수 있습니까?

### 답변

보고서 소유자는 변경할 수 없습니다. 하지만 보고서를 만든 사용자는 다른 사용자가 보고서를 편집할 수 있도록 허용할 수 있습니다. 사용자가 보고서를 편집할 수 있도록 허용하는 방법은 현재 사용자 유형에 따라 다릅니다.

* 시스템 관리자는 보고서 행에서 편집 옵션을 구성하여 보고서 작성에 대한 액세스 권한을 포함하여 플랜 라이선스가 있는 사용자가 보고서를 편집할 수 있도록 허용할 수 있습니다.\
  자세한 내용은 [보고서, 대시보드 및 일정에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)를 참조하십시오.

* 보고서를 만들고 공유할 수 있는 액세스 권한이 있는 모든 최종 사용자는 보고서를 공유하고 다른 사용자에게 보고서 관리 권한을 부여하여 다른 사용자가 개별 보고서를 편집할 수 있도록 허용할 수 있습니다.\
  자세한 내용은 [Adobe Workfront에서 보고서 공유](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)를 참조하십시오.

보고서를 보거나 관리할 수 있는 권한이 있는 경우 보고서 사본을 만들 수도 있으며, 이 복사본은 기본적으로 소유자가 됩니다. 보고서 복사에 대한 자세한 내용은 [보고서 복사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)를 참조하세요.

## 비활성화된 사용자가 소유한 보고서에 액세스할 수 없는 이유는 무엇입니까?

### 답변

보고서의 소유자는 **보고서의 액세스 권한** 필드에서 이 보고서 실행에 지정된 사용자이기도 합니다. **다음 사용자의 액세스 권한으로 이 보고서 실행:** 사용자가 비활성화된 경우 보고서를 공유한 사용자에게 보고서가 더 이상 표시되지 않습니다. 이 경우 **액세스 권한이 있는 이 보고서 실행:**&#x200B;을 비워 두거나 필드에 활성 사용자를 입력하여 보고서에 다시 액세스할 수 있습니다.

**다음 액세스 권한으로 이 보고서 실행:** 필드에 대한 자세한 내용은 [다른 사용자의 액세스 권한으로 보고서 실행 및 전달](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)을 참조하세요. 비활성화된 사용자가 소유한 모든 보고서를 식별하는 방법에 대한 자세한 내용은 [보고 활동에 대한 보고서 만들기](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md)를 참조하십시오.

## 삭제된 사용자가 소유한 보고서가 포함된 대시보드에 액세스하려면 어떻게 합니까?

### 답변

사용자를 삭제하면 사용자가 만든 모든 보고서에 계속 액세스할 수 있지만, 보고서를 포함한 모든 대시보드도 삭제됩니다. 즉, 다음에 더 이상 액세스할 수 없습니다.

* 오브젝트의 왼쪽 패널에 있는 대시보드를 포함하여 보고서가 포함된 대시보드

사용자 삭제의 의미에 대한 자세한 내용은 [사용자 삭제](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)를 참조하세요.

보고서에 대한 보기 액세스 권한이 있는 경우 다음을 수행할 수 있습니다.

1. 보고서 사본을 만듭니다.\
   보고서 복사본을 만드는 방법은 [보고서 복사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)를 참조하세요.

1. 복사된 보고서를 포함하도록 대시보드를 업데이트합니다.\
   대시보드를 편집하는 방법에 대해 알아보려면 [대시보드 편집](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md)을 참조하세요.
