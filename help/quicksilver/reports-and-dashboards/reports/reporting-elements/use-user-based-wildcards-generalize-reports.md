---
product-area: reporting
navigation-topic: reporting-elements
title: 사용자 기반 와일드카드를 사용하여 보고서를 일반화합니다
description: 특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 사용자 기반 와일드카드를 사용하여 보고서를 일반화합니다

특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다. 예를 들어, 특정 사용자에게 할당된 작업을 표시하는 보고서를 만들려면 필터의 지정 대상 필드에서 사용자 이름을 사용할 수 있습니다. 그러나 로그인한 사용자에게 할당된 작업을 표시하는 보고서를 생성하려는 경우 해당 사용자가 누구인지에 관계없이 사용자가 보고서를 볼 때 해당 사용자와 관련된 정보만 표시된다는 와일드카드 를 사용할 수 있습니다. 이 방법으로 보고서를 한 번 작성할 수 있지만, 필터에서 와일드카드를 사용하면 다른 사람이 읽을 때마다 다른 결과가 생성됩니다.

다음 보고 요소를 작성할 때 사용자 기반 와일드카드를 사용할 수 있습니다.

* 필터
* 사용자 정의 프롬프트
* 열에 대한 규칙을 추가할 때 보기

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 보고 요소를 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 보고 요소를 편집합니다</p> <p>보기 또는 필터에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

와일드카드 변수를 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 지침은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 방법 단계

보고서에 사용자 기반 와일드카드를 삽입하려면

1. 사용자 기반 와일드카드를 삽입할 보고서로 이동합니다.
1. 클릭 **보고서 작업**, 그런 다음 **편집**.

1. 을(를) 클릭합니다. **필터** 탭.
1. 클릭 **필터 규칙 추가**.
1. 필터링할 필드의 이름을 입력하기 시작합니다.\
   사용자 개체를 참조하는 필드나 사용자 정보를 입력해야 합니다.
1. 선택 **Equal** 를 클릭합니다.

   >[!TIP]
   >
   >항상 을(를) 선택해야 합니다 **Equal** Adobe Workfront에서 와일드카드를 사용할 때 변수를 필터링합니다.

1. 에서 **이름 입력 시작..** 상자, 유형: `$$USER.ID` 또는 `$$USER.name` 사용자 이름에 따라 로그인한 사용자에 대한 정보를 보고서에 표시하도록 하려는 경우. 로그인한 사용자의 그룹, 팀, 회사 또는 기타 정보를 참조하는 다른 와일드카드를 삽입할 수 있습니다.

   사용자 기반 와일드카드의 전체 목록은 다음을 참조하십시오 [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 클릭 **저장 + 닫기**.

## 추가 정보

다음을 참조하십시오.

* [기본 보고서 생성 프로그램](https://one.workfront.com/s/basic-report-creation-program)
* [와일드카드 필터 변수](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
