---
product-area: projects
navigation-topic: financials
title: 프로젝트 수준에서 작업 역할 청구 요금 재정의
description: 프로젝트 관리자는 특정 프로젝트의 작업 역할에 대한 청구 요금을 지정할 수 있습니다. 이 프로젝트 수준의 청구 요율은 이 작업 역할에 대한 시스템 수준의 청구 요율을 무시합니다. Workfront은 시스템 수준 청구 요금을 사용하는 대신 작업 역할의 프로젝트 수준 청구 요금을 사용하여 수익을 계산합니다.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: 1992e1c07e5e530a2e627ef5d2059b2384b31000
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# 프로젝트 수준에서 작업 역할 청구 요금 재정의

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

프로젝트 관리자는 특정 프로젝트의 작업 역할에 대한 청구 요금을 지정할 수 있습니다. 이 프로젝트 수준의 청구 요율은 이 작업 역할에 대한 시스템 수준의 청구 요율을 무시합니다. Workfront은 시스템 수준 청구 요금을 사용하는 대신 작업 역할의 프로젝트 수준 청구 요금을 사용하여 수익을 계산합니다.

이 문서에서는 프로젝트에 대한 시스템 작업 역할 청구 요율을 대체할 수 있는 방법에 대해 설명합니다.

프로젝트의 작업 역할 청구 요율 재정의 및 프로젝트 수익 계산에 대한 일반 정보는 [프로젝트의 작업 역할 청구 요율 재정의 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)를 참조하십시오.

프로젝트의 수익을 계산하는 데 사용되는 작업 역할에 대한 자세한 내용은 [청구 및 수익 개요](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) 문서의 &quot;사용자 및 역할 할당에 따른 작업에 대한 수익 계산 이해&quot; 섹션을 참조하십시오.

>[!NOTE]
>
>실제 매출의 경우, 청구됨으로 표시된 청구 기록에 추가된 시간에 적용되는 청구 요금은 청구 기록이 청구된 후에 발생하는 청구 요금 무시의 영향을 받지 않아야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>작업 역할에 대한 관리 액세스</p></td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>재무 데이터 편집이 포함된 프로젝트에 대한 권한 관리 </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 수준에서 작업 역할 청구 요금 재정의

다음과 같은 방법으로 프로젝트에 대한 작업 역할의 청구 요율을 대체할 수 있습니다.

* 작업 역할에 대한 새 비율을 선택하여 한 번.\
  새 비율은 프로젝트의 전체 기간에 대해 수익을 계산하는 데 사용됩니다.

* 특정 날짜 범위에 대해 몇 가지 새로운 요금을 선택하여 여러 번 호출합니다.\
  지정된 각 날짜 범위 동안 다른 비율을 사용할 수 있습니다.

* 프로젝트 템플릿에 새 청구 요금을 추가할 수 있으며, 이 요금은 해당 템플릿에서 프로젝트를 만들 때 프로젝트 청구 요금이 됩니다. 템플릿 편집에 대한 자세한 내용은 [프로젝트 템플릿 편집](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

>[!TIP]
>
>프로젝트에 대한 사용자 청구 요율을 재정의할 수 없습니다.

프로젝트에 대한 청구 요율을 대체하려면

1. 청구 요율을 재정의할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **청구 요금**&#x200B;을 클릭합니다.
1. **청구 요금 추가** > **새 청구 요금**&#x200B;을 클릭합니다.

   새 청구 요금 상자가 열립니다.

1. **작업 역할** 필드에서 청구 요금을 변경할 작업 역할을 선택합니다.

   **기본 청구 요금** 필드에 이 작업 역할에 대한 시스템 수준 요금이 표시됩니다.

1. **청구 요금 1** 필드에 일회성 청구 요금 재정의를 입력한 다음 **저장**&#x200B;을 클릭하여 청구 요금을 한 번 재정의합니다

   또는

   청구 요금 재정의를 추가하려면 **요금 추가**&#x200B;를 클릭하십시오.

1. (조건부) 두 개 이상의 청구 요금 재정의를 추가하는 경우 다음 정보를 지정합니다.

   * **청구 요금 1**: 프로젝트 시작부터 첫 번째 재정의 첫 번째 날짜까지의 청구 요금 값. 일반적으로 **기본 속도**&#x200B;와 같은 양입니다.
   * **시작 날짜**: 기본 요금이 끝나는 날짜입니다.
   * **종료 날짜**: 새 청구 요금 재정의가 종료되는 날짜입니다.

   <!--<span class="preview">Sample image in the Preview environment:</span>-->
   ![재정의 날짜가 포함된 청구 요금](assets/billing-rates-093025.png)

   <!--Sample image in the Production environment:
   ![Billing rates with override dates](assets/new-billing-rate-with-adjustment-dates-350x266.png)-->

1. 선택한 날짜에 대한 시간대가 새 청구 요금 상자 하단에 표시됩니다. 설정의 고객 정보 영역에 표시된 대로 Workfront 인스턴스와 연결된 시간대입니다. 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.
1. Workfront은 프로젝트의 매출을 계산할 때 지정된 기간 동안 발생하는 시간에 재정의 작업 역할 비율을 적용합니다.
1. 두 재정의 비율의 시간대 사이에 간격이 없어야 합니다. 재정의 비율의 **시작 날짜**&#x200B;는 이전 재정의 날짜의 **종료 날짜** 바로 다음 날이어야 합니다.

1. 첫 번째 대체 비율에 시작 일자를 지정하거나 마지막 대체 비율에 종료 일자를 지정할 수 없습니다.\
   첫 번째 재정의 비율에 기본 비율을 사용하는 것이 좋습니다.\
   Workfront에서는 첫 번째 재정의의 종료 날짜보다 오래된 날짜가 있는 모든 시간에 대해 첫 번째 재정의 비율이 적용되고, 마지막 재정의 시작 날짜보다 오래된 날짜가 있는 모든 시간에 대해 마지막 재정의 비율이 적용된다고 가정합니다.\
   프로젝트의 계획된 시작 일자 전에 시간이 기록되는 경우 첫 번째 청구 요금이 사용됩니다.\
   프로젝트의 계획된 완료 일자 이후 시간이 기록되는 경우 가장 마지막 청구 요금이 사용됩니다.

1. **저장**&#x200B;을 클릭합니다.
