---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 만들기 및 관리
description: ' [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: d8a01839b8f1332741f87be766f3ccb7d08cef96
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# 작업 역할 만들기 및 관리

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>25.11 릴리스에서는 작업 역할에 대한 통화 재정의가 프로덕션에서 더 이상 사용되지 않습니다. (사용 중단 은 미리보기 환경에서 10월 30일에 수행되었습니다.) 이제 기본 통화와 대체 통화가 아닌 작업 역할에 하나의 통화를 사용할 수 있으며 해당 통화를 사용하여 비용 및 청구 요금이 정의됩니다.

[!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 편집 액세스 권한이 있는 표준 사용자로서 사용자에게 할당할 수 있는 작업 역할을 만들고 조직과 관련이 없는 기본 작업 역할을 삭제할 수 있습니다. [!DNL Workfront]의 관리 액세스에 대한 자세한 내용은 [특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

>[!TIP]
>
>작업 역할은 리소스 관리의 필수적인 부분입니다. 자원 계획 도구를 사용하려면 작업 역할에 연관된 비용 및 청구 요금이 필요합니다. 자세한 내용은 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)을 참조하세요.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>작업 역할을 만들거나 편집하려면: 모든 Workfront 또는 워크플로 패키지</p>
   <p>비율 속성을 적용하고 사용자 정의 양식을 작업 역할에 추가하려면: Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL 계획]</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>작업 역할에 대한 액세스 편집</td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 역할 만들기

작업 역할을 생성하려면 다음을 수행합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 작업 역할]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 새 작업 역할] > 새 작업 역할 만들기**&#x200B;를 클릭합니다.
1. 다음 필드에 정보를 입력합니다.

   * **이름**: 작업 역할의 이름을 나타냅니다. Workfront에서 작업 역할 필드가 표시되는 모든 위치에 표시되는 이름입니다.

     >[!TIP]
     >
     >작업 역할의 이름은 최대 255자를 포함할 수 있습니다. 그러나 Workfront의 특정 영역에서 더 긴 이름이 잘릴 수 있습니다.

   * **설명**: 역할에 대한 고유한 설명을 입력하십시오.
   * **활성 상태**: 역할을 활성화하여 Workfront의 모든 곳에서 사용자, 작업 항목 등과 연결할 수 있도록 하려면 **예**&#x200B;를 선택합니다. 역할을 비활성화하고 사용자, 작업 항목 등에 할당할 수 없도록 하려면 **아니요**&#x200B;를 선택하십시오.

     작업 역할 비활성화에 대한 자세한 내용은 [작업 역할 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)를 참조하십시오.

1. **[!UICONTROL 작업 역할 만들기]**&#x200B;를 클릭합니다. 이제 작업 역할을 작업, 문제, 승인에 할당하거나 레이아웃 템플릿 또는 다른 개체를 공유할 수 있습니다. [!DNL Workfront]의 모든 작업 역할 사용에 대한 자세한 내용은 [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)를 참조하십시오. 작업 역할 삭제에 대한 자세한 내용은 [작업 역할 삭제](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)를 참조하십시오.

## 작업 역할에 비율 및 속성 추가

작업 역할에 대한 청구 및 비용 요금은 재무 계산에 사용됩니다.

비율 속성은 작업 역할 및 사용자와 같이 비율이 존재하는 Workfront 영역에서 지원됩니다. 작업 역할에 속성이 적용되면 해당 할당이 자동으로 올바른 비율로 확인됩니다.

자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 작업 역할]**&#x200B;을 클릭합니다.
1. 기존 작업 역할의 이름을 클릭하여 편집합니다.
1. 작업 역할 세부 정보를 업데이트하려면 왼쪽 패널에서 **세부 정보**&#x200B;를 클릭하십시오.
1. (선택 사항) 사용자 정의 양식을 작업 역할에 첨부하려면 세부 정보 페이지의 오른쪽 위 모서리에 있는 **사용자 정의 양식 추가** 필드를 클릭하고 표시되는 목록에서 사용자 정의 양식을 선택합니다.

   사용자 정의 양식을 첨부하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

1. 왼쪽 패널에서 [!UICONTROL **속도**]&#x200B;를 클릭합니다.
1. 요금 유형을 선택하려면 [!UICONTROL **청구**] 또는 [!UICONTROL **비용**]&#x200B;을 클릭하세요.
1. 새 요금을 추가하려면 [!UICONTROL **요금 추가**]&#x200B;를 클릭하세요.

   또는

   기존 비율을 선택하고 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 업데이트합니다.

   >[!NOTE]
   >
   >각 비율은 역할 및 속성의 조합과 연결되어 고유 비율을 만들기 때문에 비율을 편집할 때 속성을 변경할 수 없습니다.

1. **새 요금** 상자에서 요금 특성을 선택합니다(예: 에이전시, 위치 또는 비용 센터).

   >[!NOTE]
   >
   >이러한 속성은 별도로 정의되며 매출 및 비용 계산에 영향을 줄 수 있습니다. 자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.

1. 환율에 대한 **통화**&#x200B;을(를) 선택하십시오. Workfront 관리자가 설정 영역에 기본 통화 를 추가합니다. 선택 항목을 사용 가능한 다른 통화로 변경하고 유효 일자 시간 범위의 통화를 변경할 수 있습니다.

   >[!TIP]
   >
   >시스템의 환율 영역에서 사용할 수 있는 통화만 이 필드에서 사용할 수 있습니다. 하나의 통화만 설정된 경우 해당 통화만 사용할 수 있습니다.

   Workfront에서 기본 통화 설정에 대한 자세한 내용은 [환율 설정](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하십시오.

   프로젝트 통화 변경에 대한 자세한 내용은 [프로젝트 통화 변경](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)을 참조하십시오.

1. (조건부) 청구 요금의 경우 이 작업 역할의 **청구 요율**&#x200B;을 입력하십시오.

   작업 역할의 시간당 청구 요금입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 수익과 궁극적으로 프로젝트의 계획 및 실제 수익을 계산합니다. 선택한 통화를 사용하여 환율을 입력합니다.

   속성을 사용하는 경우 속성과 작업 역할이 결합되어 고유 비율을 정의합니다. 예를 들어, 에이전시 A에 대한 뉴욕의 Designer 역할은 에이전시 B에 대한 파리의 Designer 역할과 별도의 요금이 있을 수 있습니다.

   날짜 유효 청구 요금을 보려면 **요금 추가**&#x200B;를 클릭하십시오. 기간에 대한 청구/시간의 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 첫 번째 청구 요금에 시작 일자가 없고 마지막 청구 요금에 종료 일자가 없습니다.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   Workfront을 사용하면 날짜 범위 간 간격을 유지할 수 있지만, 의도적인 작업인지 확인하는 경고가 표시됩니다.

   Workfront이 매출을 계산하는 방법에 대한 자세한 내용은 [청구 및 매출 개요](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)를 참조하십시오.

   >[!TIP]
   >
   >기존 작업 역할을 편집할 때 요율 목록의 맨 위에서 가장 최근 시작 일자를 표시하도록 목록을 정렬할 수 있습니다.

1. (조건부) 비용 비율의 경우 이 작업 역할의 **비용 비율**&#x200B;을 입력합니다.

   작업 역할의 시간당 비용입니다. 이 값은 역할과 관련된 작업 및 문제의 계획 및 실제 비용과 궁극적으로 프로젝트의 계획 및 실제 비용을 계산합니다. 선택한 통화를 사용하여 환율을 입력합니다.

   속성을 사용하는 경우 속성과 작업 역할이 결합되어 고유 비율을 정의합니다. 예를 들어, 에이전시 A에 대한 뉴욕의 Designer 역할은 에이전시 B에 대한 파리의 Designer 역할과 별도의 요금이 있을 수 있습니다.

   날짜 유효 비용 요율을 보려면 **요율 추가**&#x200B;를 클릭하십시오. 기간에 대한 비용/시간 값을 입력하고 필요에 따라 시작 일자와 종료 일자를 지정합니다. 첫 번째 원가에는 시작 일자가 없고 마지막 원가에는 종료 일자가 없습니다.

   일부 날짜는 자동으로 추가됩니다. 예를 들어, 첫 번째 원가율에 종료 일자가 없고 시작 일자가 5월 1일인 두 번째 원가율을 추가하는 경우, 간격이 없도록 시작 일자가 4월 30일인 종료 일자가 첫 번째 원가율에 추가됩니다.

   Workfront에서 비용을 계산하는 방법에 대한 자세한 내용은 [비용 추적](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)을 참조하십시오.

   >[!TIP]
   >
   >기존 작업 역할을 편집할 때 요율 목록의 맨 위에서 가장 최근 시작 일자를 표시하도록 목록을 정렬할 수 있습니다.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



