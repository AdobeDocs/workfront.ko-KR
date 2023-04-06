---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: 대시보드에서 보고서를 구성하는 방법을 이해합니다
description: Adobe Workfront에서 보고서가 대시보드에 추가되었는지 확인할 수 있습니다. 이 기능은 유지할 수 있는 보고서와 시스템에서 삭제할 수 있는 보고서를 결정할 때 유용합니다. 보고서가 대시보드에 있는 경우 사용자가 보고서에 의존할 수 있습니다. 사용자가 사용 중인 대시보드에 나열된 보고서를 삭제하지 않는 것이 좋습니다. 대시보드에 보고서를 추가하는 방법에 대한 자세한 내용은 대시보드에 보고서 추가 문서를 참조하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 대시보드에서 보고서를 구성하는 방법을 이해합니다

## 보고서 목록에서 대시보드 정보에 액세스

Adobe Workfront에서 보고서가 대시보드에 추가되었는지 확인할 수 있습니다. 이 기능은 유지할 수 있는 보고서와 시스템에서 삭제할 수 있는 보고서를 결정할 때 유용합니다. 보고서가 대시보드에 있는 경우 사용자가 보고서에 의존할 수 있습니다. 사용자가 사용 중인 대시보드에 나열된 보고서를 삭제하지 않는 것이 좋습니다.\
대시보드에 보고서 추가에 대한 자세한 내용은 문서를 참조하십시오 [대시보드에 보고서 추가](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

다음 중 하나를 수행하여 보고서가 대시보드에 추가되는지 여부를 확인할 수 있습니다.

* 보고서 목록에 대한 보기 작성 및 열에 대시보드 정보 포함
* 사용 중인 하나 또는 여러 개의 특정 대시보드별로 보고서 목록 필터링
* 보고서 객체에 대한 보고서 작성 및 대시보드 정보가 포함된 보기 또는 필터 사용

누구나 보기 또는 필터를 작성할 수 있지만 보고서를 만들려면 액세스 수준의 보고서에 대한 편집 액세스 권한이 있어야 합니다.\
보고서 액세스에 대한 자세한 내용은 문서를 참조하십시오 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
보고서 작성에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## 보고서 목록 보기에 대시보드 정보 표시

>[!WARNING]
>
>보고서 목록에 대시보드 열을 포함하면 특히 긴 보고서 목록의 경우 로드 시간이 크게 늘어날 수 있습니다.

보고서 목록에 대한 대시보드 정보가 있는 보기를 만들려면,

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 보고서 목록에서 **보기** 드롭다운 메뉴
1. 클릭 **새 보기**.
1. 클릭 **열 추가**.
1. 에 &quot;대시보드&quot;를 입력합니다. **필드 이름 입력 시작** 필드.
1. 아래에 **보고서** 개체, 선택 **대시보드**.

1. 클릭 **보기 저장**.\
   보고서가 표시되는 대시보드는 보고서 목록의 대시보드 열에 표시됩니다.\
   ![](assets/qs-dashboards-in-report-view.png)

## 대시보드 정보별로 보고서 목록 필터링

보고서 목록을 대시보드 정보별로 필터링하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.

1. 보고서 목록에서 **필터** 드롭다운 메뉴
1. 클릭 **새 필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**.

1. 에 &quot;대시보드&quot;를 입력합니다. **필드 이름 입력 시작** 필드.

1. 아래에 **대시보드** 개체, 선택 **이름**.

1. 선택 **Equal** 수정자 드롭다운 메뉴에서 필터링할 대시보드의 이름을 입력을 시작합니다. 필터에 대한 여러 대시보드를 선택할 수 있습니다.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. 클릭 **저장 + 닫기**.\
   지정된 대시보드에만 나열되는 보고서 목록을 표시합니다.\
   보고서 개체에 대한 보고서를 작성하고 이 필터를 보고서에서 사용할 수도 있습니다.
