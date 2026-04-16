---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 등급 카드 관리
description: 요금 카드는 작업을 완료할 작업 역할에 대해 시간당 요금이 정의된 고객과의 계약 계약을 나타냅니다. 요금 카드에서 속성을 기준으로 작업 역할당 여러 청구 요금을 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 1%

---

# 등급 카드 관리

요금 카드는 작업을 완료할 작업 역할에 대해 시간당 요금이 정의된 고객과의 계약 계약을 나타냅니다. 요금 카드에서 에이전시, 위치 또는 비용 부서와 같은 속성을 기준으로 작업 역할당 여러 청구 요금을 정의할 수 있습니다. 고유 비율 속성은 설정 영역에서 구성됩니다. 자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.

예를 들어, 각각 청구 요금이 다른 에이전시에 할당되지 않은 Designer(파리 기반, 에이전시 A), 다른 Designer(파리 기반, 에이전시 B), 세 번째 Designer(뉴욕 기반)의 작업 역할이 있을 수 있습니다. 하지만 비율 카드의 작업 역할에는 속성이 필요하지 않습니다. 속성은 보다 세부적인 비율을 설정하는 도구 역할을 합니다. 요금 카드의 청구 요금도 날짜 유효일 수 있으므로 지정된 날짜에 요금이 시작되고 종료됩니다.

또한 비율 카드에 대한 비율을 잠가서 프로젝트 또는 작업 수준에서 재정의되지 않도록 할 수 있습니다. 잠긴 요금은 프로젝트의 보존된 요금을 제외하고 청구 요금 계층에서 가장 높습니다. 자세한 내용은 [수익 및 비용 계층 구조 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td>워크플로 얼티밋</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 등급 카드]에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>공유된 요금 카드를 편집하려면 요금 카드에 대한 관리 권한이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요금 카드 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**]&#x200B;를 클릭합니다.
1. [!UICONTROL **새 요금 카드**]&#x200B;를 클릭한 다음 [!UICONTROL **새 요금 카드 만들기**]&#x200B;를 클릭합니다.
1. [!UICONTROL **새 요금 카드**] 상자에 요금 카드의 이름과 설명을 입력하십시오.

   이름은 고유해야 합니다.

   ![새 요금 카드 대화 상자](assets/new-rate-card-dialog.png)

1. (선택 사항) 요금 카드로 [!UICONTROL **그룹**]&#x200B;을 선택합니다. 이것이 요금 카드를 정의하는 에이전시입니다.
1. (선택 사항) 요금 카드로 [!UICONTROL **회사**]&#x200B;를 선택합니다. 이 고객이 요금을 계약한 고객입니다.

   >[!NOTE]
   >
   >그룹 및 회사는 요금 카드 세부 사항뿐만 아니라 프로젝트에 요금 카드를 첨부할 때 필터로도 사용됩니다.

1. Click **Create**.

   비율 카드 > 작업 역할 및 비율 화면이 나타납니다.

1. [!UICONTROL **작업 역할 추가**]&#x200B;를 클릭합니다.
1. [!UICONTROL **새 청구 요금**] 상자에서 [!UICONTROL **작업 역할**]&#x200B;을(를) 선택하여 청구 요금을 정의합니다.

   ![새 청구 요금 대화 상자](assets/new-job-role-rate-on-rate-card.png)

1. (선택사항) 청구 요금에 대한 속성(예: 대리, 위치 또는 비용 부서)을 선택합니다.

   >[!NOTE]
   >
   >이러한 속성은 별도로 정의되며 매출 및 비용 계산에 영향을 줄 수 있습니다. 자세한 내용은 [비율 특성 정의](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)를 참조하십시오.

1. 청구 요금에 대해 [!UICONTROL **통화**]&#x200B;를 선택하세요.
1. (선택 사항) 작업 역할에 대해 [!UICONTROL **작업 역할 별칭**]&#x200B;을 입력합니다.

   입력한 별칭 이름이 없는 경우 추가할 수 있습니다.

   비율 카드가 프로젝트에 첨부된 경우 내부 작업 역할 이름 대신 자리 표시자 할당, 경비 및 보고서와 같은 정보에 별칭이 표시됩니다.

   >[!NOTE]
   >
   >* 단일 속도 카드 내에서 각 작업 역할 및 속성 조합에 대해 하나의 별칭만 존재할 수 있습니다.
   >* 요율 카드에서 별칭을 업데이트해야 하며 프로젝트에서 편집할 수 없습니다.

1. [!UICONTROL **청구 요금**] 필드에 이 작업 역할과 해당 특성에 대한 청구 요금을 입력합니다.
1. (선택 사항) [!UICONTROL **속도 잠금**]&#x200B;을 선택하여 이 속도를 잠그고 프로젝트 또는 작업 수준에서 변경할 수 없도록 합니다. 필요한 경우 나중에 잠금을 해제할 수 있습니다.
1. (선택 사항) 청구 요금에 유효 날짜를 적용하려면 [!UICONTROL **날짜 유효 요율 추가**]&#x200B;를 클릭합니다.
1. (선택 사항) 이 작업 역할 및 해당 특성에 대한 유효 날짜가 포함된 청구 요금을 추가하려면 [!UICONTROL **날짜 유효 비율 추가**]&#x200B;를 다시 클릭합니다.
1. (조건부) 이 작업 역할에 대해 두 개 이상의 청구 요율을 추가하는 경우 다음 정보를 입력합니다.

   * [!UICONTROL **청구 요금**]: 해당 기간의 청구 요금 값입니다.
   * [!UICONTROL **시작 날짜**]: 요금이 시작되는 날짜입니다.
   * [!UICONTROL **종료 날짜**]: 요금이 종료되는 날짜입니다.

     첫 번째 청구 요금에 시작 일자가 있을 필요는 없으며, 마지막 청구 요금에 종료 일자가 있을 필요는 없습니다. 요금 일자 사이에는 간격이 허용되지만, 겹치는 일자는 허용되지 않습니다. 간격 동안 청구 요금 계층의 다른 영역은 작업의 수익 유형에 따라 청구 요금을 결정하는 데 사용됩니다. 자세한 내용은 [수익 및 비용 계층 구조 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)를 참조하십시오.

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.
1. (선택 사항) 특성이 다른 동일한 작업 역할이나 별도의 작업 역할에 대해 다른 청구 요금을 추가하려면 [!UICONTROL **작업 역할 추가**]&#x200B;를 클릭하십시오.

   각 역할에 대한 요금은 만들 때 요금 카드에 추가됩니다. 날짜를 기준으로 현재 유효율은 ![현재 환율 아이콘](assets/current-rate-icon.png) 아이콘으로 표시됩니다.

   ![요금이 표시된 등급 카드](assets/rates-on-rate-card.png)

## 요금 카드 세부 정보 및 요금 편집

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**]&#x200B;를 클릭합니다.
1. 기존 요금 카드를 편집하려면 요금 카드 목록에서 요금 카드 이름을 클릭합니다.
1. 요금 카드 세부 정보를 업데이트하려면 왼쪽 패널에서 [!UICONTROL **세부 정보**]&#x200B;를 클릭하십시오.
1. (선택 사항) 사용자 정의 양식을 요율 카드에 첨부하려면 세부 정보 페이지의 오른쪽 상단에 있는 [!UICONTROL **사용자 정의 양식 추가**] 필드를 클릭하고 표시되는 목록에서 사용자 정의 양식을 선택합니다.

   사용자 정의 양식을 첨부하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

1. 요금 카드 세부 정보를 편집한 후 [!UICONTROL **변경 내용 저장**]&#x200B;을 클릭합니다.
1. 청구 요금을 편집하려면 왼쪽 패널의 [!UICONTROL **작업 역할 및 요금**]&#x200B;을 클릭하세요.
1. 비율을 편집하려면 비율 옆에 있는 확인란을 선택하고 화면 하단의 작업 표시줄에서 [!UICONTROL **편집**]&#x200B;을 클릭합니다.

   작업 표시줄에 대한 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

   >[!NOTE]
   >
   >각 비율은 역할 및 속성의 조합과 연결되어 고유 비율을 만들기 때문에 비율을 편집할 때 역할 및 속성을 변경할 수 없습니다.

1. 요금 카드에서 청구 요금을 삭제하려면 요금 옆에 있는 확인란을 선택하고 작업 표시줄에서 [!UICONTROL **삭제**]&#x200B;를 클릭합니다.
1. 비율을 잠그려면 비율 옆에 있는 확인란을 선택하고 작업 표시줄에서 [!UICONTROL **잠금**]&#x200B;을 클릭합니다.

   잠긴 비율은 프로젝트 또는 작업 수준에서 변경할 수 없습니다. 목록의 잠긴 비율 옆에 잠금 아이콘이 나타납니다.

   작업 표시줄에서 잠긴 비율의 잠금을 해제할 수도 있습니다.

1. 백분율로 비율을 조정하려면 다음 단계를 수행합니다.

   1. 비율 카드 > 작업 역할 및 비율 화면에서 조정할 모든 비율을 선택합니다.

      한 개의 환율을 선택하거나 여러 개의 환율을 선택할 수 있습니다. 모두 동일한 비율로 조정됩니다.

   1. 작업 표시줄에서 [!UICONTROL **비율 조정**]&#x200B;을 클릭합니다.
   1. [!UICONTROL **작업 역할 비율 조정**] 상자에서 선택한 기간(기존 유효 날짜) 동안 비율을 조정할지, 사용자가 정의하는 사용자 지정 날짜 범위 동안 비율을 조정할지 선택합니다.

      ![작업 역할 비율 조정](assets/adjust-job-role-rates-dialog.png)

   1. 비율의 조정 값을 입력합니다.

      이 값은 백분율로 적용됩니다. 예를 들어 10을 입력하면 선택한 요금이 10% 증가합니다.

   1. [!UICONTROL **속도 업데이트**]&#x200B;를 클릭합니다.
   1. 확인 메시지에서 [!UICONTROL **업데이트**]&#x200B;를 클릭합니다.

      선택한 비율이 백분율만큼 증가합니다.

## 요금 카드 가져오기

[템플릿에서 비율 카드 가져오기](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md) 문서를 참조하십시오.

## 요금 카드 복사

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**]&#x200B;를 클릭합니다.
1. 목록의 요금 카드 옆에 있는 확인란을 선택하고 **복사** 아이콘 ![복사 아이콘](assets/copy-icon.png)을 클릭합니다.
1. [!UICONTROL **요금 카드 복사**] 상자에 새 요금 카드의 이름을 입력하십시오. 그런 다음 [!UICONTROL **만들기**]&#x200B;를 클릭합니다.

   새 요금 카드가 저장되었습니다. 필요에 따라 비율 카드 세부 정보, 작업 역할 및 비율을 편집합니다.

## 전체 요금 카드 삭제

{{step-1-to-setup}}

1. 왼쪽 패널에서 [!UICONTROL **카드 평가**]&#x200B;를 클릭합니다.
1. 목록의 요금 카드 옆에 있는 확인란을 선택하고 **삭제** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.

   >[!NOTE]
   >
   >프로젝트에 첨부된 요금 카드가 프로젝트에서 삭제됩니다.

