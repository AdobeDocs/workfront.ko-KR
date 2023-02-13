---
product-area: projects
navigation-topic: financials
title: 프로젝트 레벨에서 작업 역할 청구 비율 대체
description: 프로젝트 관리자는 특정 프로젝트에서 작업 역할에 대한 청구 비율을 지정할 수 있습니다. 이 프로젝트 레벨 청구 비율은 이 작업 역할에 대한 시스템 레벨에서 청구 비율을 대체합니다. Workfront은 시스템 수준 청구 비율을 사용하는 대신 작업 역할의 프로젝트 수준 청구 비율을 사용하여 수익을 계산합니다.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 프로젝트 레벨에서 작업 역할 청구 비율 대체

프로젝트 관리자는 특정 프로젝트에서 작업 역할에 대한 청구 비율을 지정할 수 있습니다. 이 프로젝트 레벨 청구 비율은 이 작업 역할에 대한 시스템 레벨에서 청구 비율을 대체합니다. Workfront은 시스템 수준 청구 비율을 사용하는 대신 작업 역할의 프로젝트 수준 청구 비율을 사용하여 수익을 계산합니다.

이 문서에서는 프로젝트에 대한 시스템 작업 역할 청구 비율을 대체할 수 있는 방법에 대해 설명합니다.

프로젝트에 대한 작업 역할 청구 비율 대체 및 프로젝트 수익 계산에 대한 일반적인 정보는 [Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

프로젝트에서 수익을 계산하는 데 사용되는 Job 역할에 대한 자세한 내용은 문서의 &quot;사용자 및 역할 지정을 기반으로 태스크에 대한 수익 계산 이해&quot; 섹션을 참조하십시오 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>실제 수익의 경우, 청구됨으로 표시된 청구 레코드에 추가된 시간에 적용되는 청구 비율은 청구 레코드가 청구된 후 발생하는 청구 비율 대체의 영향을 받지 않습니다.

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
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>작업 역할에 대한 관리자 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 데이터 편집을 포함하는 프로젝트에 대한 권한 관리 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 레벨에서 작업 역할 청구 비율 대체

다음 방법으로 프로젝트에서 작업 역할의 청구 비율을 재정의할 수 있습니다.

* 한 번, 작업 역할에 대한 새 비율을 선택합니다.\
   새 비율은 프로젝트 전체 기간에 대해 사용하여 수익을 계산합니다.

* 특정 날짜 범위에 대해 여러 개의 새 비율을 선택하여 여러 번 수행합니다.\
   지정된 각 날짜 범위 동안 다른 비율을 사용할 수 있습니다.

>[!TIP]
>
>프로젝트에 대한 사용자 청구 비율은 대체할 수 없습니다.

프로젝트에 대한 청구 비율을 대체하려면

1. 청구 요금을 대체할 프로젝트로 이동합니다.
1. 클릭 **청구 비율** 왼쪽 패널에 표시됩니다. 먼저 **자세히 표시**.
1. 클릭 **청구 비율 추가** > **신규 청구 비율**.

   신규 청구 비율 상자가 열립니다.

1. 에서 **작업 역할** 필드에서 청구 비율을 변경할 작업 역할을 선택합니다.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   다음 **기본 청구 비율** 필드는 이 작업 역할에 대한 시스템 레벨 비율을 표시합니다.

1. 에서 **청구 비율 1** 필드를 입력하고 1회 청구 비율 대체를 입력한 다음 **저장** 청구율을 한 번 무시하려면

   또는

   클릭 **비율 추가** 청구 비율 대체를 더 추가하려면

1. (조건부) 두 개 이상의 청구 비율 대체를 추가하는 경우 다음 정보를 지정합니다.

   * **청구 비율 1**: 프로젝트 시작 일자부터 첫 번째 대체 일자까지의 청구 비율 값. 일반적으로 이 양은 **기본 비율**.
   * **시작 날짜**: 기본 비율이 끝나는 날짜입니다.
   * **종료 날짜**: 신규 청구 비율 대체 종료 일자.

   ![new_billing_rate_with_adjustment_date.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. 선택한 날짜에 대한 시간대가 새 청구 비율 상자 하단에 표시됩니다. 설정 의 고객 정보 영역에 표시된 대로 Workfront 인스턴스와 연결된 시간대입니다. 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront에서는 프로젝트에서 수익을 계산할 때 지정된 기간 동안 발생하는 시간에 무시 작업 역할율을 적용합니다.
1. 두 재정의 속도의 시간 프레임 간에 간격이 없어야 합니다. 다음 **시작 날짜** 재지정 비율은 다음 날짜여야 합니다. **종료 날짜** 이전 대체 날짜의 값.

1. 첫 번째 대체 비율에 대한 시작 일자를 지정하거나 마지막 대체 비율에 대한 종료 일자를 지정할 수 없습니다.\
   첫 번째 대체 비율에 기본값 을 사용하는 것이 좋습니다.\
   Workfront에서는 첫 번째 재정의 종료 날짜보다 오래된 날짜가 있는 모든 시간에 대해 첫 번째 재정의 비율이 적용되며, 마지막 재정의 시작 날짜보다 최신 날짜가 있는 모든 시간에 대해 마지막 재정의 비율이 적용된다고 가정합니다.\
   프로젝트의 계획 시작 일자 전에 한 시간이 기록되면 가장 첫 번째 청구 비율이 사용됩니다.\
   프로젝트의 계획 완료 일자 이후에 시간이 기록되면 가장 마지막 청구 비율이 사용됩니다.

1. **저장**&#x200B;을 클릭합니다.
