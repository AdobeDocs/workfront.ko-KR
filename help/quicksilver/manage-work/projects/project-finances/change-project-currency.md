---
product-area: projects
navigation-topic: financials
title: 프로젝트 통화 변경
description: 프로젝트 관리자는 Adobe Workfront 시스템에 대한 기본 통화 이외의 통화를 사용하도록 프로젝트를 구성할 수 있습니다. 이를 통해 인건비 및 수익을 계산할 때 프로젝트에 대한 재무 정보를 원하는 통화로 표시할 수 있습니다.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 프로젝트 통화 변경

프로젝트 관리자는 Adobe Workfront 시스템에 대한 기본 통화 이외의 통화를 사용하도록 프로젝트를 구성할 수 있습니다. 이를 통해 인건비 및 수익을 계산할 때 프로젝트에 대한 재무 정보를 원하는 통화로 표시할 수 있습니다.

이 섹션에 설명된 대로 대체 통화를 사용하려면 먼저 Workfront 관리자가 문서에 설명된 대로 여러 통화를 활성화하고 구성해야 합니다 [환율 설정](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## Workfront에서 프로젝트 통화를 변경할 때의 고려 사항

* 프로젝트에 재무 정보가 있는 경우 프로젝트의 통화를 변경할 수 없습니다.
* 이자율은 인건비 비용으로 사용됩니다. 매출 계산 및 은 향후에 보고 목적으로 사용됩니다.
* 프로젝트에 대해 다른 통화를 지정하지 않는 경우 Workfront에서는 프로젝트의 통화가 시스템의 기본 통화라고 가정합니다. 시스템 수준 기본 통화에 대한 자세한 내용은 [환율 설정](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* 기본적으로 모든 전체 라이센스 사용자는 통화와 환율을 볼 수 있습니다. Workfront 관리자는 **환율** 사용자가 프로젝트에 대해 특정 비율을 설정할 수 있도록 하는 것입니다.
* Workfront의 환율은 동적이지 않습니다. 이 값은 관리자가 설정하며 환율 변경이 발생할 때 업데이트해야 합니다.
* 프로젝트에 통화를 반영하도록 보고서를 만들 때 기본적으로 모든 보고서는 프로젝트의 기본 통화로 그룹화됩니다. 환율이 다른 여러 프로젝트의 보고서를 만들 경우 프로젝트에 적용된 모든 그룹화는 시스템 수준에서 기본 환율을 반영합니다. 자세한 내용은 문서를 참조하십시오 [고유한 환율을 사용하여 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## 프로젝트에 대한 통화 구성

1. 기본 통화를 변경할 프로젝트로 이동합니다.

   >[!TIP]
   >
   >프로젝트에 재무 정보가 아직 없는지 확인합니다. 예를 들어, 프로젝트와 연관된 계획 또는 실제 비용이 없는지 확인합니다.

1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에서 **재무** 영역.
1. 클릭 **추가** 에서 **통화** 필드를 선택하고 프로젝트의 기본 통화로 사용할 통화를 선택합니다. Workfront 관리자가 Workfront 인스턴스에 대해 설정한 모든 통화가 표시됩니다.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (조건부) Workfront 시스템에 대해 설정된 기본 통화 이외의 통화를 선택하는 경우, 시스템에서 기본 통화로 설정된 통화와 관련된 선택한 통화에 대한 환율을 지정합니다.
1. 클릭 **변경 내용 저장**.
