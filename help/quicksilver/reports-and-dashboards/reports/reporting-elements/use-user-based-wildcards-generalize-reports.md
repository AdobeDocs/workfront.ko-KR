---
product-area: reporting
navigation-topic: reporting-elements
title: 사용자 기반 와일드카드를 사용하여 보고서 일반화
description: 특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# 사용자 기반 와일드카드를 사용하여 보고서 일반화

특정 보고 요소를 작성할 때 특정 정보 대신 와일드카드를 사용하여 보고서를 일반화할 수 있습니다. 예를 들어 특정 사용자에게 할당된 작업을 표시하는 보고서를 만들려는 경우 필터의 할당 대상 필드에서 사용자 이름을 사용할 수 있습니다. 그러나 로그인한 사용자에게 할당된 작업을 표시하는 보고서를 만들려는 경우 해당 사용자가 누구인지에 관계없이, 누군가가 보고서를 볼 때 자신에게만 관련된 정보를 표시함을 나타내는 와일드카드를 사용할 수 있습니다. 이렇게 하면 보고서를 한 번 빌드하지만 필터에서 와일드카드를 사용하기 때문에 다른 사람이 읽을 때마다 다른 결과를 생성합니다.

다음 보고 요소를 작성할 때 사용자 기반 와일드카드를 사용할 수 있습니다.

* 필터
* 사용자 정의 프롬프트
* 열에 대한 규칙을 추가할 때 보기

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서의 보고 요소를 편집합니다.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서에서 보고 요소 편집</p> <p>보기 또는 필터에 대한 권한을 관리하여 편집합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

와일드카드 변수를 추가하려면 먼저 보고서를 만들어야 합니다.

보고서 만들기에 대한 지침은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 방법 단계

보고서에 사용자 기반 와일드카드를 삽입하려면 다음을 수행합니다.

1. 사용자 기반 와일드카드를 삽입할 보고서로 이동합니다.
1. 클릭 **보고서 작업**, 그런 다음 **편집**.

1. 다음을 클릭합니다. **필터** 탭.
1. 클릭 **필터 규칙 추가**.
1. 필터링 기준으로 사용할 필드의 이름을 입력하십시오.\
   사용자 개체 또는 사용자에 대한 정보를 참조하는 필드를 입력해야 합니다.
1. 선택 **같음** 필터 변수에 대한 드롭다운 메뉴에서 을(를) 선택합니다.

   >[!TIP]
   >
   >항상 다음 항목을 선택해야 합니다. **같음** Adobe Workfront에서 와일드카드로 작업할 때 변수를 필터링합니다.

1. 다음에서 **이름을 입력하세요...** box, type: `$$USER.ID` 또는 `$$USER.name` 보고서에 이름을 기반으로 로그인하는 사용자에 대한 정보를 표시하려는 경우. 로그인한 사용자의 그룹, 팀, 회사 또는 기타 정보를 참조하는 다른 와일드카드를 삽입할 수 있습니다.

   사용자 기반 와일드카드의 전체 목록에 대해서는 [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. **저장 및 닫기**&#x200B;를 클릭합니다.

## 추가 정보

다음도 참조하십시오.

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [와일드카드 필터 변수 개요](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfront에서 필터 만들기 또는 편집](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [보기에서 조건부 서식 사용](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
