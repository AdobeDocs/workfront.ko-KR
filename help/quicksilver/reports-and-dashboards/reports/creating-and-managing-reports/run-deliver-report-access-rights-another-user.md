---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 다른 사용자의 액세스 권한으로 보고서 실행 및 전달
description: 기본적으로 사용자는 보기 권한이 있는 보고서 내의 개체만 볼 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# 다른 사용자의 액세스 권한으로 보고서 실행 및 전달

기본적으로 사용자는 보기 권한이 있는 보고서 내의 개체만 볼 수 있습니다.

모든 사용자가 보고서 내의 객체에 대한 액세스 수준이나 권한 수준에 관계없이 다른 사용자와 동일한 결과를 보고서에서 볼 수 있도록 할 수 있습니다.

더 높은 액세스 권한을 가진 다른 사용자의 액세스 권한(예: Adobe Workfront 관리자의 액세스 권한)으로 보고서를 실행하는 경우 보고서를 볼 수 있는 권한이 있는 모든 사용자는 Report Builder에서 지정한 사용자로 보고서의 정보를 볼 수 있습니다. 사용자가 Workfront 인터페이스에서 찾는 두 보고서 또는 전자 메일에 대한 첨부 파일로 사용자에게 전달되는 보고서에 대해 이 설정을 설정할 수 있습니다.

>[!TIP]
>
>다음을 교체해야 합니다. **다음의 액세스 권한으로 이 보고서 실행:** 해당 사용자의 액세스 권한으로 보고서를 표시하려는 경우에만 활성 사용자가 있는 필드입니다. 예를 들어, 보고서가 플래너 또는 시스템 관리자의 액세스 권한과 함께 표시되지 않는 한, 작업 라이선스 사용자는 플랜 라이선스 사용자 또는 시스템 관리자가 작성한 보고서의 모든 항목을 볼 수 있는 권한이 없을 수 있습니다.\
보고서가 다음에 지정된 사용자와 유사한 액세스 권한을 가진 사용자와 공유되는 경우 **다음의 액세스 권한으로 이 보고서 실행:** 필드에서는 이 필드를 비워 둘 수 있습니다.

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
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 보기 (게재된 보고서를 보기 위해)</p> <p>보고서에 대한 권한 관리(보고서 실행)</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 다른 사용자의 액세스 권한이 있는 보고서 표시

채우기 **다음의 액세스 권한으로 이 보고서 실행:** 필드는 보고서에 액세스하는 사용자에 관계없이 보고서에 동일한 데이터가 포함되어 있도록 합니다. 보고서는 지정된 사용자의 경우와 같이 표시됩니다.

보고서에 액세스하는 사용자에게 보고서에 대한 보기 권한이 적어도 있어야 보고서를 볼 수 있습니다. 사용자가 다음에 나열된 경우 **다음의 액세스 권한으로 이 보고서 실행:** 필드가 비활성화되면 보고서가 공유된 다른 사용자에 대해 보고서가 더 이상 표시되지 않습니다.

다른 사용자의 액세스 권한으로 보고서를 실행하려면

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **보고서**.

1. 다른 사용자의 액세스 권한으로 표시할 보고서를 선택합니다.
1. 클릭 **보고서 작업**&#x200B;을 클릭한 다음 을 클릭합니다 **편집**.

1. 클릭 **보고서 설정**.

1. 다음에서 **다음의 액세스 권한으로 이 보고서 실행:** 필드에서는 보고서를 표시할 사용자 이름을 입력한 다음 목록에 표시될 때 선택합니다.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   >
   보고서를 작성할 수 있는 액세스 수준이 낮은 사용자는에 대해 자신 이외의 사용자를 선택할 수 없습니다. **다음의 액세스 권한으로 이 보고서 실행:** 필드.

1. 클릭 **완료**.
1. 클릭 **저장 + 닫기**.\
   이제 보고서가 다음에 지정된 사용자가 본 것처럼 공유된 모든 사용자에 대해 보고서가 표시됩니다. **다음의 액세스 권한으로 이 보고서 실행:** 필드.

>[!IMPORTANT]
>
에 로그인한 사용자 이외의 사용자 입력 **다음의 액세스 권한으로 이 보고서 실행:** 필드는 보고서에 로그인한 사용자를 참조하는 와일드카드를 사용하는 필터가 포함된 경우 보고서에 표시되는 정보에 영향을 줍니다. 보고서는 다음에 지정된 값에 따라 표시됩니다 **다음의 액세스 권한으로 이 보고서 실행:** 와일드카드 필터에 정의된 필드 대신 를 사용하십시오.
>
사용자 필드의 와일드카드에 대한 자세한 내용은 의 &quot;사용자 기반 변수&quot; 섹션을 참조하십시오 [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 다른 사용자의 액세스 권한이 있는 보고서 게재

이메일에 첨부 파일로 게재되는 보고서를 설정할 수 있습니다. 모든 사용자가 배달된 보고서에서 동일한 정보를 볼 수 있도록 액세스 수준이 더 높은 사용자에게 표시될 때 이러한 배달된 보고서가 표시되도록 설정할 수 있습니다. 이메일에 게재된 보고서를 볼 사용자는 보고서 게재 내의 수신자 보내기 목록에 추가되어야 합니다. 보고서 배달 설정에 대한 자세한 내용은 문서 를 참조하십시오 [보고서 게재 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

다른 사용자의 액세스 권한이 있는 보고서를 게재하려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **보고서**.

1. 다른 사용자의 액세스 권한과 함께 제공할 보고서를 선택합니다.
1. 보고서 이름을 클릭하여 선택합니다.
1. 클릭 **보고서 작업**.
1. 클릭 **보고서 보내기**.

1. 다음에서 **다음의 액세스 권한으로 이 보고서 게재:** 필드에 이메일에 배달될 때처럼 보고서를 표시할 사용자의 이름을 입력한 다음 목록에 표시될 때 선택합니다. 기본값은 보고서를 작성하는 사용자의 이름입니다.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   >
   보고서를 작성할 수 있는 액세스 수준이 낮은 사용자는에 대해 자신 이외의 사용자를 선택할 수 없습니다. **다음의 액세스 권한으로 이 보고서 게재:** 필드.

1. 다음 항목 선택 **형식** 보고서를 전자 메일에 표시하려는 경우:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. 클릭 **지금 보내기** 즉시 보내게\
   또는\
   클릭 **반복 게재** 보고서에 대한 반복 게재를 예약합니다.\
   보고서 게재에 대한 자세한 내용은 이 문서 를 참조하십시오 [보고서 게재 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 소스 열이 있는 보고서의 제한 사항

다음 보고서에는 상위 객체에 대한 정보를 볼 수 있는 소스 열이 표시됩니다.

* 문제 보고서
* 시간 보고서
* 문서 보고서

사용자에게 문제, 시간 또는 문서의 상위 오브젝트에 대한 권한이 없는 경우 보고서가 표시되도록 구성되었거나 다른 사용자의 액세스 권한과 함께 제공되도록 구성된 경우에도 보고서의 소스 열이 비어 있습니다.

보고서에 상위 객체에 대한 정보를 표시하려면 상위 객체에 대한 열을 추가하여 상위 객체의 이름을 표시할 수 있습니다.

예를 들어 소스 열이 있는 보고서에 다음 중 하나를 추가할 수 있습니다.

* 문서 또는 시간 보고서에 대한 프로젝트 이름, 작업 이름 또는 문제 이름 열입니다.
* 문제 보고서에 대한 프로젝트 이름 또는 작업 이름 열입니다.
* 세 개체를 모두 참조하는 텍스트 모드 표현식을 사용하는 열입니다. 다음은 시간 보고서의 예입니다.

  `displayname=Custom Source`

  `linkedname=opTask`

  `namekey=view.relatedcolumn`

  `namekeyargkey.0=opTask`

  `namekeyargkey.1=name`

  `textmode=true`

  `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

  `valueformat=HTML`

  텍스트 모드 보기에 대한 자세한 내용은 [텍스트 모드를 사용하여 보기 편집](../text-mode/edit-text-mode-in-view.md).