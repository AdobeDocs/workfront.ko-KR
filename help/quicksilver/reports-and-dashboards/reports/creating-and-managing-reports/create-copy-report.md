---
product-area: reporting;user-management
keywords: 저장,신규,보고서,복사
navigation-topic: create-and-manage-reports
title: 보고서 사본 만들기
description: 액세스 권한이 있는 모든 보고서의 사본을 만들 수 있습니다. 사용자 지정 보고서의 정확한 사본을 만들거나 기본 보고서의 새 버전을 저장할 수 있습니다. 보고서를 복사하면 복사된 보고서의 소유자가 되며 내 보고서 섹션에 표시됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 보고서 사본 만들기

액세스 권한이 있는 모든 보고서의 사본을 만들 수 있습니다. 사용자 지정 보고서의 정확한 사본을 만들거나 기본 보고서의 새 버전을 저장할 수 있습니다. 보고서를 복사하면 복사된 보고서의 소유자가 되며 내 보고서 섹션에 표시됩니다.

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
   <td> <p>보고서에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 보고서의 정확한 사본 만들기

소유자인 보고서 사본을 만들려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **보고서**, 그런 다음&#x200B;**모든 보고서**.
1. 보고서를 엽니다.
1. 클릭 **보고서 작업**, 그런 다음 **복사**.

   >[!TIP]
   >
   >보고서가 기본 보고서이면 복사 옵션이 보고서 작업 메뉴에 나타나지 않습니다.\
   >기본 보고서의 사본을 만드는 방법에 대한 자세한 내용은 [보고서의 새 버전 만들기](#create-a-new-version-of-a-report).

   ![보고서 복사](assets/nwe-fulllistofreportactions-2022.png)

   원래 보고서의 사본은 기본 이름인 *의 사본 [원래 보고서의 이름]*. 예를 들어 &quot;Q4 Completed Tasks&quot; 보고서에는 &quot;Copy of Q4 Completed Tasks&quot; 가 이름으로 표시됩니다.

1. (선택 사항) 보고서 이름을 변경하려면 새 이름을 입력합니다.

   >[!TIP]
   >
   >새 이름을 입력하기 전에 제목을 선택 취소한 경우 보고서 제목을 선택하고 이름을 삭제한 다음 새 이름을 입력합니다.

1. (선택 사항) 다른 사용자와 보고서의 새 버전을 공유하려면 **보고서 작업**, 그런 다음 **공유**.

   >[!NOTE]
   >
   >공유 정보는 원본 버전에서 복사된 보고서에 전송되지 않습니다.\
   >이전 보고서를 공유한 사용자를 확인하는 방법에 대한 자세한 내용은 [보고 활동에 대한 보고서 만들기](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. (선택 사항) 원래 보고서에 대한 관리 권한이 있고 원래 보고서가 더 이상 필요하지 않으면 삭제하여 Workfront에서 불필요한 중복 보고서를 제거할 수 있습니다.

   원래 보고서를 삭제하려면 다음을 수행합니다.

   1. 보고서로 이동합니다.
   1. 클릭 **보고서 작업**, 그런 다음 **삭제**.

   1. 클릭 **예, 삭제합니다.** 를 클릭하여 보고서를 삭제할 것인지 확인합니다.

## 보고서의 새 버전 만들기 {#create-a-new-version-of-a-report}

기본 보고서의 사본을 만들려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **보고서**, 그런 다음&#x200B;**모든 보고서**.
1. 기본 보고서의 이름을 클릭하여 엽니다.
1. 클릭 **보고서 작업**, 그런 다음 **편집**.

   ![보고서 편집](assets/nwe-reportactionsfordefaultreport-2022.png)

1. 보고서의 다음 탭에서 수정해야 합니다.

   * **열(보기)**: 보기 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **그룹화**: 그룹화 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **필터**: 필터 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **차트**: 보고서 차트 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 오른쪽 위 모서리에서 을(를) 클릭합니다. **보고서 설정**.
1. 에서 **보고서 제목** 필드에서 보고서에 새 이름을 지정합니다.
1. 클릭 **완료**.
1. 클릭 **새 보고서로 저장**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (선택 사항) 다른 사용자와 보고서의 새 버전을 공유하려면 **보고서 작업**, 그런 다음 **공유**.
