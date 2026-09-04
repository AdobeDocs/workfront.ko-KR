---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 회사 수준에서 작업 역할 청구 요금 재정의
description: 작업 역할이 생성되면 해당 역할에 대한 시간당 청구 요금을 선택할 수 있습니다. 회사별로 고유한 시간당 청구 요금을 생성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
TQID: https://experienceleague.adobe.com/EbnybXqWehstH2ziLqNZfMHtarMvUiugvWioYv9wLds
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c08e110aeccdf6d6416fd1070fbcbd40fd46983
workflow-type: tm+mt
source-wordcount: 857
ht-degree: 2%

---

# 회사 수준에서 작업 역할 청구 요금 재정의

{{preview-fast-release-general}}

작업 역할이 생성되면 해당 역할에 대한 시간당 청구 요금을 선택할 수 있습니다. 한 회사에만 해당되는 여러 개의 시간별 청구 요금을 생성할 수 있습니다. 각 청구 요금은 특정 날짜 범위에 유효합니다.

프로젝트 수준에서 회사 수준의 청구 요금이 프로젝트 수준의 요금을 재정의할 수 있도록 하는 옵션을 활성화할 수 있습니다. 자세한 내용은 [회사 수준의 청구 요율로 프로젝트 수준의 청구 요율 재정의](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>회사 수준 청구 요금에 요금 속성을 추가하려면: Workflow Ultimate</p>
       <p>회사 수준의 청구 요금을 만들고 다른 모든 요금 설정을 편집하려면: 모든 Workfront 또는 워크플로 패키지</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL 계획]</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 관리자가 아닌 경우 회사에 대한 관리 액세스</p>
   <p>재무 데이터에 대한 액세스 편집</p> </td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 특정 작업 역할에 사용된 기존 청구 요금 재정의 또는 변경

{{step-1-to-setup}}

1. **[!UICONTROL 회사]**&#x200B;를 클릭합니다.
1. 작업 역할이 할당된 회사를 찾습니다.
1. 목록에서 회사 이름을 클릭합니다.
1. 왼쪽 패널에서 **[!UICONTROL 청구 요금]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 청구 요금 추가] > [!UICONTROL 새 청구 요금]** 또는 <span class="preview">**청구 요금 추가**</span>&#x200B;를 클릭합니다.
1. [!UICONTROL 새 청구 요금] 대화 상자에서 [!UICONTROL **작업 역할**]&#x200B;을(를) 선택하여 청구 요금을 정의합니다.

### 프로덕션 환경에서:

[!UICONTROL **기본 청구 요금**]&#x200B;은(는) 이 작업 역할에 대한 시스템 수준 요금을 표시합니다.

![새 청구 요금 대화 상자](assets/date-effective-billing-rates-for-company.png)

1. [!DNL **청구 요금 1**] 필드에 청구 요금을 입력합니다. 그런 다음 [!UICONTROL **저장**]&#x200B;을 클릭하여 청구 요금을 한 번 재정의합니다.

   또는

   유효 일자가 있는 청구 요금을 추가하려면 [!UICONTROL **요금 추가**]&#x200B;를 클릭하십시오.

1. (조건부) 두 개 이상의 청구 요율을 추가하는 경우 다음 정보를 입력합니다.

   * **[!UICONTROL 청구 요금 1], 2 등**: 해당 기간의 청구 요금 값.
   * **[!UICONTROL 시작 날짜]**: 요금이 적용되는 날짜입니다.
   * **[!UICONTROL 종료 날짜]**: 요금이 종료되는 날짜입니다.

     청구 요금 1에는 시작 일자가 없으며 마지막 청구 요금에 종료 일자가 없습니다. 일부 날짜는 자동으로 추가됩니다. 예를 들어, 청구 요금 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 청구 요금 2를 추가하는 경우, 2023년 4월 30일인 종료 일자가 청구 요금 1에 추가되므로 간격이 없습니다.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다. 회사 수준에서 변경된 요금은 모든 프로젝트에 영향을 줍니다. 자세한 내용은 [청구 요금 오버라이드 및 프로젝트 수익 계산 개요](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)를 참조하십시오.

<div class="preview">

### 미리보기 환경에서:

1. 대행업체, 위치 또는 비용 부서와 같은 비율 속성을 선택합니다.

   이러한 속성은 별도로 정의되며 매출 및 비용 계산에 영향을 줄 수 있습니다. 자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.

   ![새 청구 요금 대화 상자](assets/company-billing-rates-090326.png)

1. 환율에 대한 **통화**&#x200B;을(를) 선택하십시오. Workfront 관리자가 설정 영역에 기본 통화 를 추가합니다. 선택 항목을 사용 가능한 다른 통화로 변경하고 유효 일자 시간 범위의 통화를 변경할 수 있습니다.

   >[!TIP]
   >
   >시스템의 환율 영역에서 사용할 수 있는 통화만 이 필드에서 사용할 수 있습니다. 하나의 통화만 설정된 경우 해당 통화만 사용할 수 있습니다.

   Workfront에서 기본 통화 설정에 대한 자세한 내용은 [환율 설정](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하십시오.

   프로젝트 통화 변경에 대한 자세한 내용은 [프로젝트 통화 변경](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)을 참조하십시오.

1. [!DNL **청구 요금**] 필드에 작업 역할에 대한 청구 요금을 입력합니다.

   작업 역할의 시간당 청구 요금입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 수익과 궁극적으로 프로젝트의 계획 및 실제 수익을 계산합니다. 선택한 통화를 사용하여 환율을 입력합니다.

   속성을 사용하는 경우 속성과 작업 역할이 결합되어 고유 비율을 정의합니다. 예를 들어, 에이전시 A에 대한 뉴욕의 Designer 역할은 에이전시 B에 대한 파리의 Designer 역할과 별도의 요금이 있을 수 있습니다.

   날짜 유효 청구 요금이 필요하면 **날짜 유효 요금 추가**&#x200B;를 클릭하십시오. 해당 기간의 시간별 청구 요금을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 첫 번째 청구 요금에 시작 일자가 없고 마지막 청구 요금에 종료 일자가 없습니다.

   Workfront을 사용하면 날짜 범위 간 간격을 유지할 수 있지만, 의도적인 작업인지 확인하는 경고가 표시됩니다.

   Workfront이 매출을 계산하는 방법에 대한 자세한 내용은 [청구 및 매출 개요](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

   >[!TIP]
   >
   >기존 비율을 편집할 때 목록을 정렬하여 비율 목록의 맨 위에 가장 최근 시작 날짜를 표시할 수 있습니다.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다. 회사 수준에서 변경된 요금은 회사가 할당한 모든 프로젝트에 영향을 줍니다. 자세한 내용은 [청구 요금 오버라이드 및 프로젝트 수익 계산 개요](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)를 참조하십시오.

</div>

