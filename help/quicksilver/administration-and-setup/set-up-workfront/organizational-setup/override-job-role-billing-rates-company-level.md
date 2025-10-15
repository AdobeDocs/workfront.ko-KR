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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 회사 수준에서 작업 역할 청구 요금 재정의

작업 역할이 생성되면 해당 역할에 대한 시간당 청구 요금을 선택할 수 있습니다. 한 회사에만 해당되는 여러 개의 시간별 청구 요금을 생성할 수 있습니다. 각 청구 요금은 특정 날짜 범위에 유효합니다.

프로젝트 수준에서 회사 수준의 청구 요금이 프로젝트 수준의 요금을 재정의할 수 있도록 하는 옵션을 활성화할 수 있습니다. 자세한 내용은 [회사 수준의 청구 요율로 프로젝트 수준의 청구 요율 재정의](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>임의</p></td> 
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
1. **[!UICONTROL 청구 요금 추가] > [!UICONTROL 새 청구 요금]**&#x200B;을 클릭하거나 편집할 기존 요금을 선택하십시오.
1. [!UICONTROL 새 청구 요금] 대화 상자에서 [!UICONTROL **작업 역할**]&#x200B;을(를) 선택하여 청구 요금을 정의합니다.

   [!UICONTROL **기본 청구 요금**]&#x200B;은(는) 이 작업 역할에 대한 시스템 수준 요금을 표시합니다.

   ![새 청구 요금 대화 상자](assets/date-effective-billing-rates-for-company.png)

1. [!DNL **청구 요금 1**] 필드에 청구 요금을 입력합니다. 그런 다음 [!UICONTROL **저장**]&#x200B;을 클릭하여 청구 요금을 한 번 재정의합니다.

   또는

   유효 일자가 있는 청구 요금을 추가하려면 [!UICONTROL **요금 추가**]&#x200B;를 클릭하십시오.

1. (조건부) 두 개 이상의 청구 요율을 추가하는 경우 다음 정보를 입력합니다.

   * **[!UICONTROL 청구 요금 1], 2 등**: 해당 기간의 청구 요금 값입니다.
   * **[!UICONTROL 시작 날짜]**: 요금이 적용되는 날짜입니다.
   * **[!UICONTROL 종료 날짜]**: 요금이 종료되는 날짜입니다.

     청구 요금 1에는 시작 일자가 없으며 마지막 청구 요금에 종료 일자가 없습니다. 일부 날짜는 자동으로 추가됩니다. 예를 들어, 청구 요금 1에 종료 일자가 없고 시작 일자가 2023년 5월 1일인 청구 요금 2를 추가하는 경우, 2023년 4월 30일인 종료 일자가 청구 요금 1에 추가되므로 간격이 없습니다.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다. 회사 수준에서 변경된 요금은 모든 프로젝트에 영향을 줍니다. 자세한 내용은 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.
